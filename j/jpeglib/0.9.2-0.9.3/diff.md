# Comparing `tmp/jpeglib-0.9.2.tar.gz` & `tmp/jpeglib-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpeglib-0.9.2.tar", last modified: Wed Mar 16 08:51:54 2022, max compression
+gzip compressed data, was "jpeglib-0.9.3.tar", last modified: Fri Mar 25 12:47:25 2022, max compression
```

## Comparing `jpeglib-0.9.2.tar` & `jpeglib-0.9.3.tar`

### file list

```diff
@@ -1,342 +1,1060 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.590182 jpeglib-0.9.2/
--rw-r--r--   0 martin     (501) staff       (20)      107 2022-01-18 11:52:57.000000 jpeglib-0.9.2/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)     4444 2022-03-16 08:51:54.590037 jpeglib-0.9.2/PKG-INFO
--rwxr-xr-x   0 martin     (501) staff       (20)     2843 2022-03-16 08:49:45.000000 jpeglib-0.9.2/README.md
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.552329 jpeglib-0.9.2/jpeglib/
--rw-r--r--   0 martin     (501) staff       (20)      460 2022-01-25 12:19:27.000000 jpeglib-0.9.2/jpeglib/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     5007 2022-03-16 08:49:49.000000 jpeglib-0.9.2/jpeglib/_bind.py
--rw-r--r--   0 martin     (501) staff       (20)      478 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/_timer.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.553110 jpeglib-0.9.2/jpeglib/cjpeglib/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.560303 jpeglib-0.9.2/jpeglib/cjpeglib/6b/
--rw-r--r--   0 martin     (501) staff       (20)     5249 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/cderror.h
--rw-r--r--   0 martin     (501) staff       (20)     6123 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/cdjpeg.h
--rw-r--r--   0 martin     (501) staff       (20)     9121 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcapimin.c
--rw-r--r--   0 martin     (501) staff       (20)     5881 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcapistd.c
--rw-r--r--   0 martin     (501) staff       (20)    16400 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jccoefct.c
--rw-r--r--   0 martin     (501) staff       (20)    14848 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jccolor.c
--rw-r--r--   0 martin     (501) staff       (20)    12469 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcdctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    28222 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jchuff.c
--rw-r--r--   0 martin     (501) staff       (20)     1575 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jchuff.h
--rw-r--r--   0 martin     (501) staff       (20)     2349 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcinit.c
--rw-r--r--   0 martin     (501) staff       (20)     9168 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmainct.c
--rw-r--r--   0 martin     (501) staff       (20)    17245 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    19889 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmaster.c
--rw-r--r--   0 martin     (501) staff       (20)     3110 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcomapi.c
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jconfig.h
--rw-r--r--   0 martin     (501) staff       (20)    21275 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcparam.c
--rw-r--r--   0 martin     (501) staff       (20)    25115 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcphuff.c
--rw-r--r--   0 martin     (501) staff       (20)    12073 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcprepct.c
--rw-r--r--   0 martin     (501) staff       (20)    18859 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcsample.c
--rw-r--r--   0 martin     (501) staff       (20)    13977 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jctrans.c
--rw-r--r--   0 martin     (501) staff       (20)    12637 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdapimin.c
--rw-r--r--   0 martin     (501) staff       (20)     9348 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdapistd.c
--rw-r--r--   0 martin     (501) staff       (20)     5119 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdatadst.c
--rw-r--r--   0 martin     (501) staff       (20)     7604 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdatasrc.c
--rw-r--r--   0 martin     (501) staff       (20)    25155 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdcoefct.c
--rw-r--r--   0 martin     (501) staff       (20)    12962 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdcolor.c
--rw-r--r--   0 martin     (501) staff       (20)     7041 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdct.h
--rw-r--r--   0 martin     (501) staff       (20)     8293 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jddctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    20866 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdhuff.c
--rw-r--r--   0 martin     (501) staff       (20)     8138 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdhuff.h
--rw-r--r--   0 martin     (501) staff       (20)    13500 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdinput.c
--rw-r--r--   0 martin     (501) staff       (20)    20366 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmainct.c
--rw-r--r--   0 martin     (501) staff       (20)    41118 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    19710 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmaster.c
--rw-r--r--   0 martin     (501) staff       (20)    13916 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmerge.c
--rw-r--r--   0 martin     (501) staff       (20)    20559 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdphuff.c
--rw-r--r--   0 martin     (501) staff       (20)     9723 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdpostct.c
--rw-r--r--   0 martin     (501) staff       (20)    16381 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdsample.c
--rw-r--r--   0 martin     (501) staff       (20)     5090 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdtrans.c
--rw-r--r--   0 martin     (501) staff       (20)     7801 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jerror.c
--rw-r--r--   0 martin     (501) staff       (20)    13936 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jerror.h
--rw-r--r--   0 martin     (501) staff       (20)     5486 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctflt.c
--rw-r--r--   0 martin     (501) staff       (20)     7578 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctfst.c
--rw-r--r--   0 martin     (501) staff       (20)    11066 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctint.c
--rw-r--r--   0 martin     (501) staff       (20)     8451 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctflt.c
--rw-r--r--   0 martin     (501) staff       (20)    13170 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctfst.c
--rw-r--r--   0 martin     (501) staff       (20)    14815 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctint.c
--rw-r--r--   0 martin     (501) staff       (20)    13528 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctred.c
--rw-r--r--   0 martin     (501) staff       (20)     3250 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jinclude.h
--rw-r--r--   0 martin     (501) staff       (20)    40988 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemmgr.c
--rw-r--r--   0 martin     (501) staff       (20)     2772 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemnobs.c
--rw-r--r--   0 martin     (501) staff       (20)     8230 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemsys.h
--rw-r--r--   0 martin     (501) staff       (20)    12458 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmorecfg.h
--rw-r--r--   0 martin     (501) staff       (20)    15712 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jpegint.h
--rw-r--r--   0 martin     (501) staff       (20)    46205 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jpeglib.h
--rw-r--r--   0 martin     (501) staff       (20)    31294 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jquant1.c
--rw-r--r--   0 martin     (501) staff       (20)    48429 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jquant2.c
--rw-r--r--   0 martin     (501) staff       (20)     5240 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jutils.c
--rw-r--r--   0 martin     (501) staff       (20)      360 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/jversion.h
--rw-r--r--   0 martin     (501) staff       (20)    32630 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/transupp.c
--rw-r--r--   0 martin     (501) staff       (20)     5761 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/transupp.h
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/6b/vjpeglib.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.567711 jpeglib-0.9.2/jpeglib/cjpeglib/8d/
--rw-r--r--   0 martin     (501) staff       (20)     5465 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/cderror.h
--rw-r--r--   0 martin     (501) staff       (20)     6443 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/cdjpeg.h
--rw-r--r--   0 martin     (501) staff       (20)     5235 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jaricom.c
--rw-r--r--   0 martin     (501) staff       (20)     9672 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcapimin.c
--rw-r--r--   0 martin     (501) staff       (20)     6042 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcapistd.c
--rw-r--r--   0 martin     (501) staff       (20)    29126 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcarith.c
--rw-r--r--   0 martin     (501) staff       (20)    17104 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jccoefct.c
--rw-r--r--   0 martin     (501) staff       (20)    16124 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jccolor.c
--rw-r--r--   0 martin     (501) staff       (20)    16255 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcdctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    49777 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jchuff.c
--rw-r--r--   0 martin     (501) staff       (20)     2239 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcinit.c
--rw-r--r--   0 martin     (501) staff       (20)     9626 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmainct.c
--rw-r--r--   0 martin     (501) staff       (20)    18408 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    32422 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmaster.c
--rw-r--r--   0 martin     (501) staff       (20)     3216 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcomapi.c
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jconfig.h
--rw-r--r--   0 martin     (501) staff       (20)    22641 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcparam.c
--rw-r--r--   0 martin     (501) staff       (20)    12574 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcprepct.c
--rw-r--r--   0 martin     (501) staff       (20)    20468 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcsample.c
--rw-r--r--   0 martin     (501) staff       (20)    14283 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jctrans.c
--rw-r--r--   0 martin     (501) staff       (20)    13103 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdapimin.c
--rw-r--r--   0 martin     (501) staff       (20)     9625 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdapistd.c
--rw-r--r--   0 martin     (501) staff       (20)    24718 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdarith.c
--rw-r--r--   0 martin     (501) staff       (20)     8804 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdatadst.c
--rw-r--r--   0 martin     (501) staff       (20)     9636 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdatasrc.c
--rw-r--r--   0 martin     (501) staff       (20)    26169 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdcoefct.c
--rw-r--r--   0 martin     (501) staff       (20)    16768 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdcolor.c
--rw-r--r--   0 martin     (501) staff       (20)    17538 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdct.h
--rw-r--r--   0 martin     (501) staff       (20)    12786 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jddctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    49915 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdhuff.c
--rw-r--r--   0 martin     (501) staff       (20)    25699 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdinput.c
--rw-r--r--   0 martin     (501) staff       (20)    20920 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmainct.c
--rw-r--r--   0 martin     (501) staff       (20)    43998 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    19567 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmaster.c
--rw-r--r--   0 martin     (501) staff       (20)    14316 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmerge.c
--rw-r--r--   0 martin     (501) staff       (20)    10013 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdpostct.c
--rw-r--r--   0 martin     (501) staff       (20)    12329 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdsample.c
--rw-r--r--   0 martin     (501) staff       (20)     5193 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdtrans.c
--rw-r--r--   0 martin     (501) staff       (20)     8053 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jerror.c
--rw-r--r--   0 martin     (501) staff       (20)    14885 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jerror.h
--rw-r--r--   0 martin     (501) staff       (20)     6182 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctflt.c
--rw-r--r--   0 martin     (501) staff       (20)     8210 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctfst.c
--rw-r--r--   0 martin     (501) staff       (20)   163026 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctint.c
--rw-r--r--   0 martin     (501) staff       (20)     8554 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctflt.c
--rw-r--r--   0 martin     (501) staff       (20)    13538 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctfst.c
--rw-r--r--   0 martin     (501) staff       (20)   187037 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctint.c
--rw-r--r--   0 martin     (501) staff       (20)     3341 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jinclude.h
--rw-r--r--   0 martin     (501) staff       (20)    42642 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemmgr.c
--rw-r--r--   0 martin     (501) staff       (20)     2881 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemnobs.c
--rw-r--r--   0 martin     (501) staff       (20)     8428 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemsys.h
--rw-r--r--   0 martin     (501) staff       (20)    12927 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmorecfg.h
--rw-r--r--   0 martin     (501) staff       (20)    17658 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jpegint.h
--rw-r--r--   0 martin     (501) staff       (20)    49733 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jpeglib.h
--rw-r--r--   0 martin     (501) staff       (20)    32184 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jquant1.c
--rw-r--r--   0 martin     (501) staff       (20)    49782 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jquant2.c
--rw-r--r--   0 martin     (501) staff       (20)     6962 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jutils.c
--rw-r--r--   0 martin     (501) staff       (20)      410 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/jversion.h
--rw-r--r--   0 martin     (501) staff       (20)    58860 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/transupp.c
--rw-r--r--   0 martin     (501) staff       (20)     9482 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/transupp.h
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/8d/vjpeglib.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.574554 jpeglib-0.9.2/jpeglib/cjpeglib/9d/
--rwxr-xr-x   0 martin     (501) staff       (20)     5577 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/cderror.h
--rwxr-xr-x   0 martin     (501) staff       (20)     6508 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/cdjpeg.h
--rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jaricom.c
--rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcapimin.c
--rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcapistd.c
--rwxr-xr-x   0 martin     (501) staff       (20)    29200 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcarith.c
--rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jccoefct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    20059 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jccolor.c
--rwxr-xr-x   0 martin     (501) staff       (20)    16027 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcdctmgr.c
--rwxr-xr-x   0 martin     (501) staff       (20)    51922 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jchuff.c
--rwxr-xr-x   0 martin     (501) staff       (20)    10912 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcinit.c
--rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmainct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    19631 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmarker.c
--rwxr-xr-x   0 martin     (501) staff       (20)    23827 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmaster.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8358 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcomapi.c
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jconfig.h
--rwxr-xr-x   0 martin     (501) staff       (20)    20421 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcparam.c
--rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcprepct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcsample.c
--rwxr-xr-x   0 martin     (501) staff       (20)    15030 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jctrans.c
--rwxr-xr-x   0 martin     (501) staff       (20)    13241 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdapimin.c
--rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdapistd.c
--rwxr-xr-x   0 martin     (501) staff       (20)    25068 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdarith.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8947 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdatadst.c
--rwxr-xr-x   0 martin     (501) staff       (20)     9619 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdatasrc.c
--rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdcoefct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    23804 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdcolor.c
--rwxr-xr-x   0 martin     (501) staff       (20)    18028 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdct.h
--rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jddctmgr.c
--rwxr-xr-x   0 martin     (501) staff       (20)    50320 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdhuff.c
--rwxr-xr-x   0 martin     (501) staff       (20)    25749 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdinput.c
--rwxr-xr-x   0 martin     (501) staff       (20)    20877 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmainct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    47329 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmarker.c
--rwxr-xr-x   0 martin     (501) staff       (20)    19631 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmaster.c
--rwxr-xr-x   0 martin     (501) staff       (20)    16070 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmerge.c
--rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdpostct.c
--rwxr-xr-x   0 martin     (501) staff       (20)    12290 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdsample.c
--rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdtrans.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8103 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jerror.c
--rwxr-xr-x   0 martin     (501) staff       (20)    14892 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jerror.h
--rwxr-xr-x   0 martin     (501) staff       (20)     6225 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctflt.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8253 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctfst.c
--rwxr-xr-x   0 martin     (501) staff       (20)   163428 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctint.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8600 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctflt.c
--rwxr-xr-x   0 martin     (501) staff       (20)    13069 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctfst.c
--rwxr-xr-x   0 martin     (501) staff       (20)   190040 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctint.c
--rwxr-xr-x   0 martin     (501) staff       (20)     3596 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jinclude.h
--rwxr-xr-x   0 martin     (501) staff       (20)    42144 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemmgr.c
--rwxr-xr-x   0 martin     (501) staff       (20)     3023 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemnobs.c
--rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemsys.h
--rwxr-xr-x   0 martin     (501) staff       (20)    15375 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmorecfg.h
--rwxr-xr-x   0 martin     (501) staff       (20)    18471 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jpegint.h
--rwxr-xr-x   0 martin     (501) staff       (20)    50595 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jpeglib.h
--rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jquant1.c
--rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jquant2.c
--rwxr-xr-x   0 martin     (501) staff       (20)     6969 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jutils.c
--rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/jversion.h
--rwxr-xr-x   0 martin     (501) staff       (20)    90648 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/transupp.c
--rwxr-xr-x   0 martin     (501) staff       (20)    10313 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/transupp.h
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/9d/vjpeglib.h
--rw-r--r--   0 martin     (501) staff       (20)    27286 2022-03-16 08:49:45.000000 jpeglib-0.9.2/jpeglib/cjpeglib/cjpeglib.c
--rw-r--r--   0 martin     (501) staff       (20)     1261 2022-03-11 13:25:31.000000 jpeglib-0.9.2/jpeglib/cjpeglib/cjpeglib.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.588188 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/
--rw-r--r--   0 martin     (501) staff       (20)     4708 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cderror.h
--rw-r--r--   0 martin     (501) staff       (20)     4369 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cdjpeg.c
--rw-r--r--   0 martin     (501) staff       (20)     5929 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cdjpeg.h
--rw-r--r--   0 martin     (501) staff       (20)    24736 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cjpeg.c
--rw-r--r--   0 martin     (501) staff       (20)     1598 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cmyk.h
--rw-r--r--   0 martin     (501) staff       (20)    29742 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/djpeg.c
--rw-r--r--   0 martin     (501) staff       (20)     5132 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jaricom.c
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.588670 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/
--rw-r--r--   0 martin     (501) staff       (20)     5804 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJ.h
--rw-r--r--   0 martin     (501) staff       (20)     3521 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJCompressor.h
--rw-r--r--   0 martin     (501) staff       (20)     3479 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJDecompressor.h
--rw-r--r--   0 martin     (501) staff       (20)      838 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJTransformer.h
--rw-r--r--   0 martin     (501) staff       (20)     9684 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcapimin.c
--rw-r--r--   0 martin     (501) staff       (20)     5903 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcapistd.c
--rw-r--r--   0 martin     (501) staff       (20)    29654 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcarith.c
--rw-r--r--   0 martin     (501) staff       (20)    17271 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccoefct.c
--rw-r--r--   0 martin     (501) staff       (20)     4521 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccolext.c
--rw-r--r--   0 martin     (501) staff       (20)    23593 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccolor.c
--rw-r--r--   0 martin     (501) staff       (20)    22364 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcdctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    36597 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jchuff.c
--rw-r--r--   0 martin     (501) staff       (20)     1514 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jchuff.h
--rw-r--r--   0 martin     (501) staff       (20)     4072 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcicc.c
--rw-r--r--   0 martin     (501) staff       (20)     2565 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcinit.c
--rw-r--r--   0 martin     (501) staff       (20)     5221 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmainct.c
--rw-r--r--   0 martin     (501) staff       (20)    17532 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    21955 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmaster.c
--rw-r--r--   0 martin     (501) staff       (20)     3239 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcomapi.c
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jconfig.h
--rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jconfigint.h
--rw-r--r--   0 martin     (501) staff       (20)    18203 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcparam.c
--rw-r--r--   0 martin     (501) staff       (20)    33518 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcphuff.c
--rw-r--r--   0 martin     (501) staff       (20)    12994 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcprepct.c
--rw-r--r--   0 martin     (501) staff       (20)    19156 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcsample.c
--rw-r--r--   0 martin     (501) staff       (20)     3851 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcstest.c
--rw-r--r--   0 martin     (501) staff       (20)    14936 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jctrans.c
--rw-r--r--   0 martin     (501) staff       (20)    13202 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdapimin.c
--rw-r--r--   0 martin     (501) staff       (20)    24975 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdapistd.c
--rw-r--r--   0 martin     (501) staff       (20)    25523 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdarith.c
--rw-r--r--   0 martin     (501) staff       (20)     6828 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatadst-tj.c
--rw-r--r--   0 martin     (501) staff       (20)     9699 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatadst.c
--rw-r--r--   0 martin     (501) staff       (20)     6969 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatasrc-tj.c
--rw-r--r--   0 martin     (501) staff       (20)    10280 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatasrc.c
--rw-r--r--   0 martin     (501) staff       (20)    34027 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcoefct.c
--rw-r--r--   0 martin     (501) staff       (20)     2704 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcoefct.h
--rw-r--r--   0 martin     (501) staff       (20)    11665 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcol565.c
--rw-r--r--   0 martin     (501) staff       (20)     4355 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcolext.c
--rw-r--r--   0 martin     (501) staff       (20)    28549 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcolor.c
--rw-r--r--   0 martin     (501) staff       (20)     9708 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdct.h
--rw-r--r--   0 martin     (501) staff       (20)    11415 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jddctmgr.c
--rw-r--r--   0 martin     (501) staff       (20)    26269 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdhuff.c
--rw-r--r--   0 martin     (501) staff       (20)     9795 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdhuff.h
--rw-r--r--   0 martin     (501) staff       (20)     5524 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdicc.c
--rw-r--r--   0 martin     (501) staff       (20)    14580 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdinput.c
--rw-r--r--   0 martin     (501) staff       (20)    19741 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmainct.c
--rw-r--r--   0 martin     (501) staff       (20)     2448 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmainct.h
--rw-r--r--   0 martin     (501) staff       (20)    42210 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmarker.c
--rw-r--r--   0 martin     (501) staff       (20)    27453 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmaster.c
--rw-r--r--   0 martin     (501) staff       (20)      788 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmaster.h
--rw-r--r--   0 martin     (501) staff       (20)    19804 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmerge.c
--rw-r--r--   0 martin     (501) staff       (20)     1630 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmerge.h
--rw-r--r--   0 martin     (501) staff       (20)    11030 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmrg565.c
--rw-r--r--   0 martin     (501) staff       (20)     5787 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmrgext.c
--rw-r--r--   0 martin     (501) staff       (20)    22145 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdphuff.c
--rw-r--r--   0 martin     (501) staff       (20)    10948 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdpostct.c
--rw-r--r--   0 martin     (501) staff       (20)    18058 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdsample.c
--rw-r--r--   0 martin     (501) staff       (20)     1725 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdsample.h
--rw-r--r--   0 martin     (501) staff       (20)     5461 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdtrans.c
--rw-r--r--   0 martin     (501) staff       (20)     7916 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jerror.c
--rw-r--r--   0 martin     (501) staff       (20)    15715 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jerror.h
--rw-r--r--   0 martin     (501) staff       (20)     5588 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctflt.c
--rw-r--r--   0 martin     (501) staff       (20)     7792 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctfst.c
--rw-r--r--   0 martin     (501) staff       (20)    11508 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctint.c
--rw-r--r--   0 martin     (501) staff       (20)     8729 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctflt.c
--rw-r--r--   0 martin     (501) staff       (20)    13554 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctfst.c
--rw-r--r--   0 martin     (501) staff       (20)   106254 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctint.c
--rw-r--r--   0 martin     (501) staff       (20)    14528 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctred.c
--rw-r--r--   0 martin     (501) staff       (20)     2958 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jinclude.h
--rw-r--r--   0 martin     (501) staff       (20)    44779 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemmgr.c
--rw-r--r--   0 martin     (501) staff       (20)     2825 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemnobs.c
--rw-r--r--   0 martin     (501) staff       (20)     7788 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemsys.h
--rw-r--r--   0 martin     (501) staff       (20)    14317 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmorecfg.h
--rw-r--r--   0 martin     (501) staff       (20)   270393 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpeg_nbits_table.h
--rw-r--r--   0 martin     (501) staff       (20)     1130 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegcomp.h
--rw-r--r--   0 martin     (501) staff       (20)    15619 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegint.h
--rw-r--r--   0 martin     (501) staff       (20)    50281 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpeglib.h
--rw-r--r--   0 martin     (501) staff       (20)    24913 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegtran.c
--rw-r--r--   0 martin     (501) staff       (20)    32176 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jquant1.c
--rw-r--r--   0 martin     (501) staff       (20)    48710 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jquant2.c
--rw-r--r--   0 martin     (501) staff       (20)     5853 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimd.h
--rw-r--r--   0 martin     (501) staff       (20)     8036 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimd_none.c
--rw-r--r--   0 martin     (501) staff       (20)     3085 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimddct.h
--rw-r--r--   0 martin     (501) staff       (20)     5306 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jstdhuff.c
--rw-r--r--   0 martin     (501) staff       (20)     3791 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jutils.c
--rw-r--r--   0 martin     (501) staff       (20)     1754 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jversion.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.588770 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/md5/
--rw-r--r--   0 martin     (501) staff       (20)     2371 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/md5/md5.h
--rw-r--r--   0 martin     (501) staff       (20)    23029 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdbmp.c
--rw-r--r--   0 martin     (501) staff       (20)     7001 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdcolmap.c
--rw-r--r--   0 martin     (501) staff       (20)    23805 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdgif.c
--rw-r--r--   0 martin     (501) staff       (20)    14989 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdjpgcom.c
--rw-r--r--   0 martin     (501) staff       (20)    25423 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdppm.c
--rw-r--r--   0 martin     (501) staff       (20)    13133 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdswitch.c
--rw-r--r--   0 martin     (501) staff       (20)    15480 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdtarga.c
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.588873 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.589141 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/arm/
--rw-r--r--   0 martin     (501) staff       (20)     1221 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/arm/align.h
--rw-r--r--   0 martin     (501) staff       (20)     3595 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/arm/jchuff.h
--rw-r--r--   0 martin     (501) staff       (20)    56939 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/jsimd.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.589247 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips/
--rw-r--r--   0 martin     (501) staff       (20)     8032 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips/jsimd_dspr2_asm.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.589546 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/
--rw-r--r--   0 martin     (501) staff       (20)      701 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/jcsample.h
--rw-r--r--   0 martin     (501) staff       (20)     2458 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/jsimd_mmi.h
--rw-r--r--   0 martin     (501) staff       (20)    23014 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/loongson-mmintrin.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.589666 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/nasm/
--rw-r--r--   0 martin     (501) staff       (20)     4768 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/nasm/jsimdcfg.inc.h
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.589862 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/powerpc/
--rw-r--r--   0 martin     (501) staff       (20)      701 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/powerpc/jcsample.h
--rw-r--r--   0 martin     (501) staff       (20)     4269 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/powerpc/jsimd_altivec.h
--rw-r--r--   0 martin     (501) staff       (20)    39357 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjbench.c
--rw-r--r--   0 martin     (501) staff       (20)    15178 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjexample.c
--rw-r--r--   0 martin     (501) staff       (20)    30208 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjunittest.c
--rw-r--r--   0 martin     (501) staff       (20)     2259 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjutil.c
--rw-r--r--   0 martin     (501) staff       (20)     1956 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjutil.h
--rw-r--r--   0 martin     (501) staff       (20)    92968 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/transupp.c
--rw-r--r--   0 martin     (501) staff       (20)    11134 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/transupp.h
--rw-r--r--   0 martin     (501) staff       (20)    47012 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg-jni.c
--rw-r--r--   0 martin     (501) staff       (20)    75349 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg.c
--rw-r--r--   0 martin     (501) staff       (20)    74651 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg.h
--rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/vjpeglib.h
--rw-r--r--   0 martin     (501) staff       (20)    18019 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrbmp.c
--rw-r--r--   0 martin     (501) staff       (20)    18631 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrgif.c
--rw-r--r--   0 martin     (501) staff       (20)    17895 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrjpgcom.c
--rw-r--r--   0 martin     (501) staff       (20)    10859 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrppm.c
--rw-r--r--   0 martin     (501) staff       (20)     7486 2022-01-25 12:07:11.000000 jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrtarga.c
--rw-r--r--   0 martin     (501) staff       (20)    22679 2022-03-16 08:49:45.000000 jpeglib-0.9.2/jpeglib/jpeg.py
--rw-r--r--   0 martin     (501) staff       (20)     2820 2022-03-16 08:49:45.000000 jpeglib-0.9.2/jpeglib/version.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-16 08:51:54.552880 jpeglib-0.9.2/jpeglib.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     4444 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)    10763 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)        6 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)      130 2022-03-16 08:51:54.000000 jpeglib-0.9.2/jpeglib.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)       38 2022-03-16 08:51:54.590228 jpeglib-0.9.2/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)     6425 2022-03-16 08:50:19.000000 jpeglib-0.9.2/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.826054 jpeglib-0.9.3/
+-rw-r--r--   0 martin     (501) staff       (20)      107 2022-01-18 11:52:57.000000 jpeglib-0.9.3/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     4444 2022-03-25 12:47:25.825895 jpeglib-0.9.3/PKG-INFO
+-rwxr-xr-x   0 martin     (501) staff       (20)     2843 2022-03-18 18:13:53.000000 jpeglib-0.9.3/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.546032 jpeglib-0.9.3/jpeglib/
+-rw-r--r--   0 martin     (501) staff       (20)      460 2022-03-25 12:45:13.000000 jpeglib-0.9.3/jpeglib/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     5007 2022-03-25 12:45:13.000000 jpeglib-0.9.3/jpeglib/_bind.py
+-rw-r--r--   0 martin     (501) staff       (20)      478 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/_timer.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.547422 jpeglib-0.9.3/jpeglib/cjpeglib/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.566768 jpeglib-0.9.3/jpeglib/cjpeglib/6b/
+-rw-r--r--   0 martin     (501) staff       (20)     5249 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/cderror.h
+-rw-r--r--   0 martin     (501) staff       (20)     6123 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/cdjpeg.h
+-rw-r--r--   0 martin     (501) staff       (20)     9121 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)     5881 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)    16400 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jccoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)    14848 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jccolor.c
+-rw-r--r--   0 martin     (501) staff       (20)    12469 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcdctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    28222 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jchuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     1575 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jchuff.h
+-rw-r--r--   0 martin     (501) staff       (20)     2349 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcinit.c
+-rw-r--r--   0 martin     (501) staff       (20)     9168 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)    17245 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    19889 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)     3110 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jconfig.h
+-rw-r--r--   0 martin     (501) staff       (20)    21275 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcparam.c
+-rw-r--r--   0 martin     (501) staff       (20)    25115 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcphuff.c
+-rw-r--r--   0 martin     (501) staff       (20)    12073 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcprepct.c
+-rw-r--r--   0 martin     (501) staff       (20)    18859 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcsample.c
+-rw-r--r--   0 martin     (501) staff       (20)    13977 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jctrans.c
+-rw-r--r--   0 martin     (501) staff       (20)    12637 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)     9348 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)     5119 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdatadst.c
+-rw-r--r--   0 martin     (501) staff       (20)     7604 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdatasrc.c
+-rw-r--r--   0 martin     (501) staff       (20)    25155 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdcoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)    12962 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdcolor.c
+-rw-r--r--   0 martin     (501) staff       (20)     7041 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdct.h
+-rw-r--r--   0 martin     (501) staff       (20)     8293 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jddctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    20866 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdhuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     8138 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdhuff.h
+-rw-r--r--   0 martin     (501) staff       (20)    13500 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdinput.c
+-rw-r--r--   0 martin     (501) staff       (20)    20366 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)    41118 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    19710 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)    13916 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmerge.c
+-rw-r--r--   0 martin     (501) staff       (20)    20559 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdphuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     9723 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdpostct.c
+-rw-r--r--   0 martin     (501) staff       (20)    16381 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdsample.c
+-rw-r--r--   0 martin     (501) staff       (20)     5090 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdtrans.c
+-rw-r--r--   0 martin     (501) staff       (20)     7801 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jerror.c
+-rw-r--r--   0 martin     (501) staff       (20)    13936 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jerror.h
+-rw-r--r--   0 martin     (501) staff       (20)     5486 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)     7578 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)    11066 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctint.c
+-rw-r--r--   0 martin     (501) staff       (20)     8451 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)    13170 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)    14815 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctint.c
+-rw-r--r--   0 martin     (501) staff       (20)    13528 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctred.c
+-rw-r--r--   0 martin     (501) staff       (20)     3250 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jinclude.h
+-rw-r--r--   0 martin     (501) staff       (20)    40988 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)     2772 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemnobs.c
+-rw-r--r--   0 martin     (501) staff       (20)     8230 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemsys.h
+-rw-r--r--   0 martin     (501) staff       (20)    12458 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmorecfg.h
+-rw-r--r--   0 martin     (501) staff       (20)    15712 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jpegint.h
+-rw-r--r--   0 martin     (501) staff       (20)    46205 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jpeglib.h
+-rw-r--r--   0 martin     (501) staff       (20)    31294 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jquant1.c
+-rw-r--r--   0 martin     (501) staff       (20)    48429 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jquant2.c
+-rw-r--r--   0 martin     (501) staff       (20)     5240 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jutils.c
+-rw-r--r--   0 martin     (501) staff       (20)      360 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/jversion.h
+-rw-r--r--   0 martin     (501) staff       (20)    32630 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/transupp.c
+-rw-r--r--   0 martin     (501) staff       (20)     5761 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/6b/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.581106 jpeglib-0.9.3/jpeglib/cjpeglib/7/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5381 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5485 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9445 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29029 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17060 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    51428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9626 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18031 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    28263 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22641 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14183 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13083 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24557 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5270 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7816 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25905 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12689 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    43646 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14019 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20920 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    42478 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25784 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5047 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14885 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8693 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13022 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    16215 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    48609 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32150 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5419 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      409 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    56730 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8956 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/7/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.597655 jpeglib-0.9.3/jpeglib/cjpeglib/8/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5219 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9445 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29108 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17060 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49777 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9626 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18402 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    30661 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22641 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14274 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24662 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8770 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9629 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25905 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12689 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49915 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25699 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20920 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    43998 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19632 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14885 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8693 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13085 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    16877 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    49633 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32150 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7004 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      409 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    58413 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9283 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.614907 jpeglib-0.9.3/jpeglib/cjpeglib/8a/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5219 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29108 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17060 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49777 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9626 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18402 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    30550 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22641 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14274 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24662 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8770 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9629 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25905 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12786 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49915 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25699 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20920 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    43998 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19632 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14885 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13085 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    16877 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    49633 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32150 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7004 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    58413 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9283 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8a/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.631653 jpeglib-0.9.3/jpeglib/cjpeglib/8b/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5219 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29108 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17060 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49777 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9626 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18402 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    30550 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22641 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14274 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24662 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8770 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9643 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25905 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12786 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49915 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25699 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20920 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    43998 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19632 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14885 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13085 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    16877 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    49633 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32150 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7004 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    58413 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9283 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8b/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.648238 jpeglib-0.9.3/jpeglib/cjpeglib/8c/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5219 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29108 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17060 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49777 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9626 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18408 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    32234 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22641 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14274 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24662 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8770 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9643 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25905 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12786 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49915 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25699 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20920 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    43998 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19632 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14885 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13085 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    16877 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    49724 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32150 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7004 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    58413 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9283 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8c/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.662705 jpeglib-0.9.3/jpeglib/cjpeglib/8d/
+-rw-r--r--   0 martin     (501) staff       (20)     5465 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/cderror.h
+-rw-r--r--   0 martin     (501) staff       (20)     6443 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/cdjpeg.h
+-rw-r--r--   0 martin     (501) staff       (20)     5235 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jaricom.c
+-rw-r--r--   0 martin     (501) staff       (20)     9672 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)     6042 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)    29126 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcarith.c
+-rw-r--r--   0 martin     (501) staff       (20)    17104 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jccoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)    16124 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jccolor.c
+-rw-r--r--   0 martin     (501) staff       (20)    16255 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcdctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    49777 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jchuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     2239 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcinit.c
+-rw-r--r--   0 martin     (501) staff       (20)     9626 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)    18408 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    32422 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)     3216 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jconfig.h
+-rw-r--r--   0 martin     (501) staff       (20)    22641 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcparam.c
+-rw-r--r--   0 martin     (501) staff       (20)    12574 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcprepct.c
+-rw-r--r--   0 martin     (501) staff       (20)    20468 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcsample.c
+-rw-r--r--   0 martin     (501) staff       (20)    14283 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jctrans.c
+-rw-r--r--   0 martin     (501) staff       (20)    13103 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)     9625 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)    24718 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdarith.c
+-rw-r--r--   0 martin     (501) staff       (20)     8804 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdatadst.c
+-rw-r--r--   0 martin     (501) staff       (20)     9636 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdatasrc.c
+-rw-r--r--   0 martin     (501) staff       (20)    26169 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdcoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)    16768 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdcolor.c
+-rw-r--r--   0 martin     (501) staff       (20)    17538 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdct.h
+-rw-r--r--   0 martin     (501) staff       (20)    12786 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jddctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    49915 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdhuff.c
+-rw-r--r--   0 martin     (501) staff       (20)    25699 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdinput.c
+-rw-r--r--   0 martin     (501) staff       (20)    20920 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)    43998 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    19567 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)    14316 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdmerge.c
+-rw-r--r--   0 martin     (501) staff       (20)    10013 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdpostct.c
+-rw-r--r--   0 martin     (501) staff       (20)    12329 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdsample.c
+-rw-r--r--   0 martin     (501) staff       (20)     5193 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdtrans.c
+-rw-r--r--   0 martin     (501) staff       (20)     8053 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jerror.c
+-rw-r--r--   0 martin     (501) staff       (20)    14885 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jerror.h
+-rw-r--r--   0 martin     (501) staff       (20)     6182 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jfdctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)     8210 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jfdctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)   163026 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jfdctint.c
+-rw-r--r--   0 martin     (501) staff       (20)     8554 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jidctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)    13538 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jidctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)   187037 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jidctint.c
+-rw-r--r--   0 martin     (501) staff       (20)     3341 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jinclude.h
+-rw-r--r--   0 martin     (501) staff       (20)    42642 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmemmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)     2881 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmemnobs.c
+-rw-r--r--   0 martin     (501) staff       (20)     8428 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmemsys.h
+-rw-r--r--   0 martin     (501) staff       (20)    12927 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmorecfg.h
+-rw-r--r--   0 martin     (501) staff       (20)    17658 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jpegint.h
+-rw-r--r--   0 martin     (501) staff       (20)    49733 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jpeglib.h
+-rw-r--r--   0 martin     (501) staff       (20)    32184 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jquant1.c
+-rw-r--r--   0 martin     (501) staff       (20)    49782 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jquant2.c
+-rw-r--r--   0 martin     (501) staff       (20)     6962 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jutils.c
+-rw-r--r--   0 martin     (501) staff       (20)      410 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/jversion.h
+-rw-r--r--   0 martin     (501) staff       (20)    58860 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/transupp.c
+-rw-r--r--   0 martin     (501) staff       (20)     9482 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/8d/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.676751 jpeglib-0.9.3/jpeglib/cjpeglib/9/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29095 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17729 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16255 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49777 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    32234 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22812 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14395 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9625 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24723 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8982 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9636 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19847 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12786 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49863 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25699 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    21030 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47115 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19567 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8098 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14884 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163026 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187037 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42154 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    13695 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    17658 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50083 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6962 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      409 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    58859 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9482 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.690950 jpeglib-0.9.3/jpeglib/cjpeglib/9a/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29171 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19989 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16027 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49544 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2989 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    32053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    24486 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14355 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13241 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25042 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8982 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9636 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24481 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    50103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25749 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    21030 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47450 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19980 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14363 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8098 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14884 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6182 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8210 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163307 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13538 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   187211 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42154 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15371 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    17710 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50461 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6962 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    65483 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9784 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9a/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.705383 jpeglib-0.9.3/jpeglib/cjpeglib/9b/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5465 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29171 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19989 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16027 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49544 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2989 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    32053 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    24486 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14355 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13241 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25041 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8982 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23506 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18349 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    50103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25749 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    21030 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47450 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19589 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16076 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12290 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14884 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6219 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8247 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163272 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8594 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13058 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   189981 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3341 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42154 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15371 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    17710 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50467 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6962 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    65483 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9784 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9b/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.718665 jpeglib-0.9.3/jpeglib/cjpeglib/9c/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5577 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6443 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29171 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19989 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16027 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49544 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10912 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23761 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3216 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    24486 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15030 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13241 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25041 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8984 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23630 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18292 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    50107 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25749 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20877 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47450 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19598 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16200 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12290 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14884 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6225 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8253 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163272 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8600 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13069 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   190063 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3596 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42154 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2881 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15371 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    18202 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50461 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6962 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    67627 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9784 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9c/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.732088 jpeglib-0.9.3/jpeglib/cjpeglib/9d/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5577 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6508 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29200 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    17104 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20059 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16027 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    51922 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10912 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19631 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23827 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8358 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    20421 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12574 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20468 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15030 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13241 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25068 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8947 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9619 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26169 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23804 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18028 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    50320 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25749 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20877 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47329 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19631 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16070 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12290 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8103 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14892 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6225 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8253 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163428 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8600 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13069 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   190040 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3596 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42144 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3023 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15375 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    18471 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50595 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32184 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49782 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6969 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    90648 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10313 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9d/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.749081 jpeglib-0.9.3/jpeglib/cjpeglib/9e/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5650 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6508 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5235 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jaricom.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9672 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6102 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    29205 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16800 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20059 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15771 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    51928 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10912 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19631 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23685 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8358 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jconfig.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    20715 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12591 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20479 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14864 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13966 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9669 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25073 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8947 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9619 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25945 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25850 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18028 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    12764 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    50326 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25580 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    21284 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    47329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19548 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    16064 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10013 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    11935 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5193 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8103 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14892 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6225 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8253 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   163428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8600 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13069 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   190040 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3596 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42144 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3023 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8428 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15371 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    18417 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    50591 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32133 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    49773 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6901 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      410 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/jversion.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    90648 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10313 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/9e/vjpeglib.h
+-rw-r--r--   0 martin     (501) staff       (20)    27647 2022-03-25 12:45:13.000000 jpeglib-0.9.3/jpeglib/cjpeglib/cjpeglib.c
+-rw-r--r--   0 martin     (501) staff       (20)     1261 2022-03-25 12:45:13.000000 jpeglib-0.9.3/jpeglib/cjpeglib/cjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.783212 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/
+-rwxr-xr-x   0 martin     (501) staff       (20)     5752 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/cderror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6048 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/cdjpeg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     1598 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/cmyk.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5132 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jaricom.c
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.784965 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/
+-rwxr-xr-x   0 martin     (501) staff       (20)     4731 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJ.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     3521 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJCompressor.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     3479 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJDecompressor.h
+-rwxr-xr-x   0 martin     (501) staff       (20)      838 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJTransformer.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    10131 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6192 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    31106 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23862 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jccoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    23735 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jccolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    55695 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcdctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5391 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcext.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    34512 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jchuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     1868 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jchuff.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     4072 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcicc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2673 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcinit.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5221 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    21971 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    35137 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2275 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcmaster.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     3239 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jconfig.h
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jconfigint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    34019 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcparam.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    33767 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcphuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    12994 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcprepct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    20209 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15230 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jctrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13239 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdapimin.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    24632 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdapistd.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25157 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdarith.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6828 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatadst-tj.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10110 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatadst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     6969 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatasrc-tj.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10280 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatasrc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    25505 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdcoefct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2668 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdcoefct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    28655 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdcolor.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9708 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    11899 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jddctmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    26299 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdhuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     9503 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdhuff.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5700 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdicc.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14580 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdinput.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    19741 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmainct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2448 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmainct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    42686 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmarker.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    27953 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmaster.c
+-rwxr-xr-x   0 martin     (501) staff       (20)      894 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmaster.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    19804 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmerge.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     1630 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmerge.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22291 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdphuff.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10948 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdpostct.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    18121 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdsample.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     1725 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdsample.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5461 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdtrans.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7916 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jerror.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    15329 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jerror.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     5588 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7792 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    11508 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     8729 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctflt.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    13554 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctfst.c
+-rwxr-xr-x   0 martin     (501) staff       (20)   106238 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctint.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    14528 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctred.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2958 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jinclude.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    44779 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemmgr.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     2825 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemnobs.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     7788 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemsys.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    15139 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmorecfg.h
+-rwxr-xr-x   0 martin     (501) staff       (20)   270393 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpeg_nbits_table.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     1130 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpegcomp.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    18739 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpegint.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    54316 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpeglib.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    32422 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jquant1.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    48978 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jquant2.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     5505 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jsimd.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     7759 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jsimd_none.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     3085 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jsimddct.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     3791 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jutils.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     1812 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jversion.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.785111 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/md5/
+-rwxr-xr-x   0 martin     (501) staff       (20)     2371 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/md5/md5.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     6870 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/rdpng.c
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.785256 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/
+-rwxr-xr-x   0 martin     (501) staff       (20)    48969 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/jsimd.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.786293 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/loongson/
+-rwxr-xr-x   0 martin     (501) staff       (20)      744 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/loongson/jcsample.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     2114 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/loongson/jsimd_mmi.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    22837 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/loongson/loongson-mmintrin.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.787409 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/mips/
+-rwxr-xr-x   0 martin     (501) staff       (20)     8032 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/mips/jsimd_dspr2_asm.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.787983 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/nasm/
+-rwxr-xr-x   0 martin     (501) staff       (20)     4768 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/nasm/jsimdcfg.inc.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.788609 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/powerpc/
+-rwxr-xr-x   0 martin     (501) staff       (20)      744 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/powerpc/jcsample.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     4269 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/powerpc/jsimd_altivec.h
+-rwxr-xr-x   0 martin     (501) staff       (20)     2259 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/tjutil.c
+-rwxr-xr-x   0 martin     (501) staff       (20)     1954 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/tjutil.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    62694 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/transupp.c
+-rwxr-xr-x   0 martin     (501) staff       (20)    10148 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/transupp.h
+-rwxr-xr-x   0 martin     (501) staff       (20)    74006 2022-03-18 18:01:48.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/turbojpeg.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/vjpeglib.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.821800 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/
+-rw-r--r--   0 martin     (501) staff       (20)     4708 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cderror.h
+-rw-r--r--   0 martin     (501) staff       (20)     4369 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cdjpeg.c
+-rw-r--r--   0 martin     (501) staff       (20)     5929 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cdjpeg.h
+-rw-r--r--   0 martin     (501) staff       (20)    24736 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cjpeg.c
+-rw-r--r--   0 martin     (501) staff       (20)     1598 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cmyk.h
+-rw-r--r--   0 martin     (501) staff       (20)    29742 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/djpeg.c
+-rw-r--r--   0 martin     (501) staff       (20)     5132 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jaricom.c
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.822652 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/
+-rw-r--r--   0 martin     (501) staff       (20)     5804 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJ.h
+-rw-r--r--   0 martin     (501) staff       (20)     3521 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJCompressor.h
+-rw-r--r--   0 martin     (501) staff       (20)     3479 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJDecompressor.h
+-rw-r--r--   0 martin     (501) staff       (20)      838 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJTransformer.h
+-rw-r--r--   0 martin     (501) staff       (20)     9684 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)     5903 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)    29654 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcarith.c
+-rw-r--r--   0 martin     (501) staff       (20)    17271 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)     4521 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccolext.c
+-rw-r--r--   0 martin     (501) staff       (20)    23593 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccolor.c
+-rw-r--r--   0 martin     (501) staff       (20)    22364 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcdctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    36597 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jchuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     1514 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jchuff.h
+-rw-r--r--   0 martin     (501) staff       (20)     4072 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcicc.c
+-rw-r--r--   0 martin     (501) staff       (20)     2565 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcinit.c
+-rw-r--r--   0 martin     (501) staff       (20)     5221 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)    17532 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    21955 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)     3239 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcomapi.c
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jconfig.h
+-rw-r--r--   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jconfigint.h
+-rw-r--r--   0 martin     (501) staff       (20)    18203 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcparam.c
+-rw-r--r--   0 martin     (501) staff       (20)    33518 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcphuff.c
+-rw-r--r--   0 martin     (501) staff       (20)    12994 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcprepct.c
+-rw-r--r--   0 martin     (501) staff       (20)    19156 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcsample.c
+-rw-r--r--   0 martin     (501) staff       (20)     3851 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcstest.c
+-rw-r--r--   0 martin     (501) staff       (20)    14936 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jctrans.c
+-rw-r--r--   0 martin     (501) staff       (20)    13202 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdapimin.c
+-rw-r--r--   0 martin     (501) staff       (20)    24975 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdapistd.c
+-rw-r--r--   0 martin     (501) staff       (20)    25523 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdarith.c
+-rw-r--r--   0 martin     (501) staff       (20)     6828 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdatadst-tj.c
+-rw-r--r--   0 martin     (501) staff       (20)     9699 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdatadst.c
+-rw-r--r--   0 martin     (501) staff       (20)     6969 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdatasrc-tj.c
+-rw-r--r--   0 martin     (501) staff       (20)    10280 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdatasrc.c
+-rw-r--r--   0 martin     (501) staff       (20)    34027 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcoefct.c
+-rw-r--r--   0 martin     (501) staff       (20)     2704 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcoefct.h
+-rw-r--r--   0 martin     (501) staff       (20)    11665 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcol565.c
+-rw-r--r--   0 martin     (501) staff       (20)     4355 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcolext.c
+-rw-r--r--   0 martin     (501) staff       (20)    28549 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcolor.c
+-rw-r--r--   0 martin     (501) staff       (20)     9708 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdct.h
+-rw-r--r--   0 martin     (501) staff       (20)    11415 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jddctmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)    26269 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdhuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     9795 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdhuff.h
+-rw-r--r--   0 martin     (501) staff       (20)     5524 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdicc.c
+-rw-r--r--   0 martin     (501) staff       (20)    14580 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdinput.c
+-rw-r--r--   0 martin     (501) staff       (20)    19741 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmainct.c
+-rw-r--r--   0 martin     (501) staff       (20)     2448 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmainct.h
+-rw-r--r--   0 martin     (501) staff       (20)    42210 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmarker.c
+-rw-r--r--   0 martin     (501) staff       (20)    27453 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmaster.c
+-rw-r--r--   0 martin     (501) staff       (20)      788 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmaster.h
+-rw-r--r--   0 martin     (501) staff       (20)    19804 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmerge.c
+-rw-r--r--   0 martin     (501) staff       (20)     1630 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmerge.h
+-rw-r--r--   0 martin     (501) staff       (20)    11030 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmrg565.c
+-rw-r--r--   0 martin     (501) staff       (20)     5787 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmrgext.c
+-rw-r--r--   0 martin     (501) staff       (20)    22145 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdphuff.c
+-rw-r--r--   0 martin     (501) staff       (20)    10948 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdpostct.c
+-rw-r--r--   0 martin     (501) staff       (20)    18058 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdsample.c
+-rw-r--r--   0 martin     (501) staff       (20)     1725 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdsample.h
+-rw-r--r--   0 martin     (501) staff       (20)     5461 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdtrans.c
+-rw-r--r--   0 martin     (501) staff       (20)     7916 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jerror.c
+-rw-r--r--   0 martin     (501) staff       (20)    15715 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jerror.h
+-rw-r--r--   0 martin     (501) staff       (20)     5588 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jfdctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)     7792 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jfdctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)    11508 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jfdctint.c
+-rw-r--r--   0 martin     (501) staff       (20)     8729 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jidctflt.c
+-rw-r--r--   0 martin     (501) staff       (20)    13554 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jidctfst.c
+-rw-r--r--   0 martin     (501) staff       (20)   106254 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jidctint.c
+-rw-r--r--   0 martin     (501) staff       (20)    14528 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jidctred.c
+-rw-r--r--   0 martin     (501) staff       (20)     2958 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jinclude.h
+-rw-r--r--   0 martin     (501) staff       (20)    44779 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jmemmgr.c
+-rw-r--r--   0 martin     (501) staff       (20)     2825 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jmemnobs.c
+-rw-r--r--   0 martin     (501) staff       (20)     7788 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jmemsys.h
+-rw-r--r--   0 martin     (501) staff       (20)    14317 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jmorecfg.h
+-rw-r--r--   0 martin     (501) staff       (20)   270393 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpeg_nbits_table.h
+-rw-r--r--   0 martin     (501) staff       (20)     1130 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpegcomp.h
+-rw-r--r--   0 martin     (501) staff       (20)    15619 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpegint.h
+-rw-r--r--   0 martin     (501) staff       (20)    50281 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpeglib.h
+-rw-r--r--   0 martin     (501) staff       (20)    24913 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpegtran.c
+-rw-r--r--   0 martin     (501) staff       (20)    32176 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jquant1.c
+-rw-r--r--   0 martin     (501) staff       (20)    48710 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jquant2.c
+-rw-r--r--   0 martin     (501) staff       (20)     5853 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jsimd.h
+-rw-r--r--   0 martin     (501) staff       (20)     8036 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jsimd_none.c
+-rw-r--r--   0 martin     (501) staff       (20)     3085 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jsimddct.h
+-rw-r--r--   0 martin     (501) staff       (20)     5306 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jstdhuff.c
+-rw-r--r--   0 martin     (501) staff       (20)     3791 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jutils.c
+-rw-r--r--   0 martin     (501) staff       (20)     1754 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jversion.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.822793 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/md5/
+-rw-r--r--   0 martin     (501) staff       (20)     2371 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/md5/md5.h
+-rw-r--r--   0 martin     (501) staff       (20)    23029 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdbmp.c
+-rw-r--r--   0 martin     (501) staff       (20)     7001 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdcolmap.c
+-rw-r--r--   0 martin     (501) staff       (20)    23805 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdgif.c
+-rw-r--r--   0 martin     (501) staff       (20)    14989 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdjpgcom.c
+-rw-r--r--   0 martin     (501) staff       (20)    25423 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdppm.c
+-rw-r--r--   0 martin     (501) staff       (20)    13133 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdswitch.c
+-rw-r--r--   0 martin     (501) staff       (20)    15480 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdtarga.c
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.822930 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.823819 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/arm/
+-rw-r--r--   0 martin     (501) staff       (20)     1221 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/arm/align.h
+-rw-r--r--   0 martin     (501) staff       (20)     3595 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/arm/jchuff.h
+-rw-r--r--   0 martin     (501) staff       (20)    56939 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/jsimd.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.824040 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips/
+-rw-r--r--   0 martin     (501) staff       (20)     8032 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips/jsimd_dspr2_asm.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.824749 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/
+-rw-r--r--   0 martin     (501) staff       (20)      701 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/jcsample.h
+-rw-r--r--   0 martin     (501) staff       (20)     2458 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/jsimd_mmi.h
+-rw-r--r--   0 martin     (501) staff       (20)    23014 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/loongson-mmintrin.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.825102 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/nasm/
+-rw-r--r--   0 martin     (501) staff       (20)     4768 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/nasm/jsimdcfg.inc.h
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.825579 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/powerpc/
+-rw-r--r--   0 martin     (501) staff       (20)      701 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/powerpc/jcsample.h
+-rw-r--r--   0 martin     (501) staff       (20)     4269 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/powerpc/jsimd_altivec.h
+-rw-r--r--   0 martin     (501) staff       (20)    39357 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjbench.c
+-rw-r--r--   0 martin     (501) staff       (20)    15178 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjexample.c
+-rw-r--r--   0 martin     (501) staff       (20)    30208 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjunittest.c
+-rw-r--r--   0 martin     (501) staff       (20)     2259 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjutil.c
+-rw-r--r--   0 martin     (501) staff       (20)     1956 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjutil.h
+-rw-r--r--   0 martin     (501) staff       (20)    92968 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/transupp.c
+-rw-r--r--   0 martin     (501) staff       (20)    11134 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/transupp.h
+-rw-r--r--   0 martin     (501) staff       (20)    47012 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg-jni.c
+-rw-r--r--   0 martin     (501) staff       (20)    75349 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg.c
+-rw-r--r--   0 martin     (501) staff       (20)    74651 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg.h
+-rw-r--r--   0 martin     (501) staff       (20)       20 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/vjpeglib.h
+-rw-r--r--   0 martin     (501) staff       (20)    18019 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrbmp.c
+-rw-r--r--   0 martin     (501) staff       (20)    18631 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrgif.c
+-rw-r--r--   0 martin     (501) staff       (20)    17895 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrjpgcom.c
+-rw-r--r--   0 martin     (501) staff       (20)    10859 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrppm.c
+-rw-r--r--   0 martin     (501) staff       (20)     7486 2022-01-25 12:07:11.000000 jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrtarga.c
+-rw-r--r--   0 martin     (501) staff       (20)    22685 2022-03-25 12:45:13.000000 jpeglib-0.9.3/jpeglib/jpeg.py
+-rw-r--r--   0 martin     (501) staff       (20)     2927 2022-03-18 18:13:53.000000 jpeglib-0.9.3/jpeglib/version.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-25 12:47:25.547157 jpeglib-0.9.3/jpeglib.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     4444 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)    32917 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        6 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)      454 2022-03-25 12:47:25.000000 jpeglib-0.9.3/jpeglib.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)       38 2022-03-25 12:47:25.826103 jpeglib-0.9.3/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)     6798 2022-03-23 12:43:18.000000 jpeglib-0.9.3/setup.py
```

### Comparing `jpeglib-0.9.2/PKG-INFO` & `jpeglib-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpeglib
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python envelope for the popular C library libjpeg for handling JPEG files.
 Home-page: https://jpeglib.readthedocs.io/en/latest/
 Author: Martin Beneš
 Author-email: martinbenes1996@gmail.com
 License: MPL
 Keywords: jpeglib,jpeg,jpg,libjpeg,compression,decompression,dct-coefficients,dct
 Platform: UNKNOWN
```

### Comparing `jpeglib-0.9.2/README.md` & `jpeglib-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/_bind.py` & `jpeglib-0.9.3/jpeglib/_bind.py`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/cderror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/cderror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/cdjpeg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/cdjpeg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jccoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jccoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jccolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jccolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcdctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jchuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jchuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jchuff.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jchuff.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcinit.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcinit.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcomapi.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcomapi.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcparam.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcparam.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcphuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcphuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcprepct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcprepct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jcsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jcsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jctrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jctrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdatadst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdatadst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdatasrc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdcoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdcolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdcolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jddctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdhuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdhuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdhuff.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdhuff.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdinput.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdinput.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdmerge.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdmerge.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdphuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdphuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdpostct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdpostct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jdtrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jdtrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jerror.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jerror.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jerror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jerror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jfdctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jfdctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jidctred.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jidctred.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jinclude.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jinclude.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemnobs.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmemsys.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmemsys.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jmorecfg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jpegint.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jpegint.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jpeglib.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jpeglib.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jquant1.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jquant1.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jquant2.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jquant2.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/jutils.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/jutils.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/transupp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/transupp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/6b/transupp.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/6b/transupp.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/cderror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/cderror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/cdjpeg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/cdjpeg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jaricom.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jaricom.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8a/jcapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jccoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jccoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jccolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jccolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcdctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jchuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jchuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcinit.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcinit.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8c/jcmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jcmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcomapi.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcomapi.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcparam.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcparam.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcprepct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcprepct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jcsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jcsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jctrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jctrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdatadst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdatadst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdatasrc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdcoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdcolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdcolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jddctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8a/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdhuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdhuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdinput.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdinput.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jdmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdmerge.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdmerge.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdpostct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdpostct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jdsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jdtrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdtrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jerror.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jerror.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jerror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jerror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jfdctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jfdctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8a/jidctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jidctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jidctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jidctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jinclude.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jinclude.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemnobs.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmemsys.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/7/jmemsys.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jmorecfg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jpegint.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jpegint.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jpeglib.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jpeglib.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jquant1.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jquant1.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jquant2.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jquant2.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/jutils.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/jutils.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/transupp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/transupp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/8d/transupp.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8d/transupp.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/cderror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/cderror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/cdjpeg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/cdjpeg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jaricom.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jaricom.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8b/jcapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jccoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jccoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jccolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jccolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcdctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jchuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jchuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcinit.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jcinit.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jcmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcomapi.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcomapi.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcparam.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jcparam.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcprepct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jcprepct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jcsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jcsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jctrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jctrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdatadst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdatadst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdatasrc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdcoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdcolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdcolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jddctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdhuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdhuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdinput.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9a/jdinput.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jdmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdmerge.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jdmerge.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdpostct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jdpostct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9b/jdsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jdtrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/8a/jdtrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jerror.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9b/jerror.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jerror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jerror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jfdctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jfdctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jidctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jidctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jidctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jidctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jinclude.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9c/jinclude.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemnobs.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmemsys.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/8/jmemsys.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jmorecfg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jpegint.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jpegint.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jpeglib.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jpeglib.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jquant1.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jquant1.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jquant2.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9/jquant2.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/jutils.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/jutils.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/transupp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/transupp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/9d/transupp.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/9d/transupp.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/cjpeglib.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/cjpeglib.c`

 * *Files 1% similar despite different names*

```diff
@@ -450,18 +450,18 @@
 
   if (overwrite_flag(flags, QUANTIZE_COLORS) && flag_is_set(flags, QUANTIZE_COLORS)) {
     cinfo.actual_number_of_colors = 256; // TODO: parametrized
     cinfo.desired_number_of_colors = 256;
     if(in_colormap != NULL) cinfo.colormap = (char**)cmap;
   }
   
-  // fprintf(stderr, "PROGRESSIVE_MODE: owrt %d set %d\n", 
-  //   overwrite_flag(flags, PROGRESSIVE_MODE),
-  //   flag_is_set(flags, PROGRESSIVE_MODE)
-  // );fprintf(stderr, "ARITH_CODE: owrt %d set %d\n", 
+  //fprintf(stderr, "read PROGRESSIVE_MODE: owrt %d set %d\n", 
+  //  overwrite_flag(flags, PROGRESSIVE_MODE),
+  //  flag_is_set(flags, PROGRESSIVE_MODE)
+  //);fprintf(stderr, "ARITH_CODE: owrt %d set %d\n", 
   //   overwrite_flag(flags, ARITH_CODE),
   //   flag_is_set(flags, ARITH_CODE)
   // );fprintf(stderr, "CCIR601_SAMPLING: owrt %d set %d\n", 
   //   overwrite_flag(flags, CCIR601_SAMPLING),
   //   flag_is_set(flags, CCIR601_SAMPLING)
   // );fprintf(stderr, "TWO_PASS_QUANTIZE: owrt %d set %d\n", 
   //   overwrite_flag(flags, TWO_PASS_QUANTIZE),
@@ -491,15 +491,17 @@
   if (overwrite_flag(flags, ENABLE_2PASS_QUANT))
     cinfo.enable_2pass_quant    = flag_is_set(flags, ENABLE_2PASS_QUANT);
 
   // decompress
   (void)jpeg_start_decompress(&cinfo);
   // read pixels
   unsigned char *rowptr = rgb;
-  unsigned short stride = (flag_is_set(flags, QUANTIZE_COLORS)) ? 1 : cinfo.out_color_components;
+  unsigned short stride = (overwrite_flag(flags, QUANTIZE_COLORS) && flag_is_set(flags, QUANTIZE_COLORS)) ?
+    1 : cinfo.out_color_components;
+  
   while(cinfo.output_scanline < cinfo.output_height) {
     jpeg_read_scanlines(&cinfo, &rowptr, 1);
     rowptr += cinfo.output_width * stride;
   }
   // read quantization colormap
   if(overwrite_flag(flags, QUANTIZE_COLORS) && flag_is_set(flags, QUANTIZE_COLORS)) {
     int N = cinfo.out_color_components;
@@ -584,14 +586,15 @@
     // read file
     if((fp_in = _read_jpeg(srcfile, &cinfo_in, &jerr_in)) == NULL) return 0;
     // decompress
     (void)jpeg_start_decompress(&cinfo_in);
     jpeg_copy_critical_parameters((j_decompress_ptr)&cinfo_in, (j_compress_ptr)&cinfo);
   }
 
+  //fprintf(stderr, "quality %d\n", quality);
   if(qt != NULL) {
     unsigned qt_u[64];
     // component 0
     for(int i = 0; i < 64; i++) qt_u[i] = qt[i]; // (i&7)*8+(i>>3)
     jpeg_add_quant_table(&cinfo, 0, qt_u, 100, FALSE);
     cinfo.comp_info[0].component_id = 0;
     cinfo.comp_info[0].quant_tbl_no = 0;
@@ -610,16 +613,19 @@
   if(in_color_space >= 0)
     cinfo.in_color_space = in_color_space;
 
   #if JPEG_LIB_VERSION >= 70
   if (overwrite_flag(flags, DO_FANCY_UPSAMPLING))
     cinfo.do_fancy_downsampling = flag_is_set(flags, DO_FANCY_UPSAMPLING);
   #endif
+  //fprintf(stderr, "write PROGRESSIVE_MODE owr %d set %d\n", overwrite_flag(flags, PROGRESSIVE_MODE), flag_is_set(flags, OPTIMIZE_CODING));
   if (overwrite_flag(flags, PROGRESSIVE_MODE))
     cinfo.progressive_mode   = flag_is_set(flags, PROGRESSIVE_MODE);
+  if (overwrite_flag(flags, PROGRESSIVE_MODE) && flag_is_set(flags, PROGRESSIVE_MODE))
+    jpeg_simple_progression(&cinfo);
   if (overwrite_flag(flags, OPTIMIZE_CODING))
     cinfo.optimize_coding    = flag_is_set(flags, OPTIMIZE_CODING);
   if (overwrite_flag(flags, ARITH_CODE))
     cinfo.arith_code         = flag_is_set(flags, ARITH_CODE);
   if (overwrite_flag(flags, WRITE_JFIF_HEADER))
     cinfo.write_JFIF_header  = flag_is_set(flags, WRITE_JFIF_HEADER);
   if (overwrite_flag(flags, WRITE_ADOBE_MARKER))
```

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/cjpeglib.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/cjpeglib.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cderror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cderror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cdjpeg.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cdjpeg.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cdjpeg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cdjpeg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cjpeg.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/cjpeg.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/cmyk.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/cmyk.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/djpeg.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/djpeg.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jaricom.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jaricom.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJ.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJ.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJCompressor.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJCompressor.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJDecompressor.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJDecompressor.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/java/org_libjpegturbo_turbojpeg_TJTransformer.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/java/org_libjpegturbo_turbojpeg_TJTransformer.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccolext.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccolext.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jccolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jccolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcdctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcdctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jchuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jchuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jchuff.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jchuff.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcicc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcicc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcinit.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcinit.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcomapi.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcomapi.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcparam.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcparam.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcphuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcphuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcprepct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jcprepct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jcstest.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jcstest.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jctrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jctrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdapimin.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdapimin.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdapistd.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdapistd.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdarith.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdarith.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatadst-tj.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatadst-tj.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatadst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdatadst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatasrc-tj.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatasrc-tj.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdatasrc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdatasrc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcoefct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcoefct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcoefct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcoefct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcol565.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcol565.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcolext.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcolext.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdcolor.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdcolor.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jddctmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jddctmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdhuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdhuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdhuff.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdhuff.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdicc.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdicc.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdinput.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdinput.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmainct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmainct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmainct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmainct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmarker.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmarker.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmaster.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmaster.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmaster.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmaster.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmerge.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmerge.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmerge.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdmerge.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmrg565.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmrg565.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdmrgext.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdmrgext.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdphuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdphuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdpostct.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdpostct.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdsample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jdsample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdsample.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdsample.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jdtrans.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jdtrans.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jerror.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jerror.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jerror.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jerror.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jfdctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jfdctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctflt.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctflt.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctfst.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctfst.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctint.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jidctint.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jidctred.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jidctred.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jinclude.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jinclude.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemmgr.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemmgr.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemnobs.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemnobs.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmemsys.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jmemsys.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jmorecfg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jmorecfg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpeg_nbits_table.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpeg_nbits_table.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegcomp.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jpegcomp.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegint.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpegint.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpeglib.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpeglib.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jpegtran.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jpegtran.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jquant1.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jquant1.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jquant2.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jquant2.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimd.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jsimd.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimd_none.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jsimd_none.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jsimddct.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jsimddct.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jstdhuff.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jstdhuff.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jutils.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/jutils.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/jversion.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/jversion.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/md5/md5.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/md5/md5.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdbmp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdbmp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdcolmap.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdcolmap.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdgif.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdgif.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdjpgcom.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdjpgcom.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdppm.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdppm.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdswitch.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdswitch.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/rdtarga.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/rdtarga.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/arm/align.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/arm/align.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/arm/jchuff.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/arm/jchuff.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/jsimd.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/jsimd.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips/jsimd_dspr2_asm.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/mips/jsimd_dspr2_asm.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/jcsample.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/jcsample.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/jsimd_mmi.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/jsimd_mmi.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/mips64/loongson-mmintrin.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/mips64/loongson-mmintrin.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/nasm/jsimdcfg.inc.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/nasm/jsimdcfg.inc.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/powerpc/jcsample.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/simd/powerpc/jcsample.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/simd/powerpc/jsimd_altivec.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/simd/powerpc/jsimd_altivec.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjbench.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjbench.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjexample.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjexample.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjunittest.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjunittest.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjutil.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/mozjpeg403/tjutil.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/tjutil.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/tjutil.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/transupp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/transupp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/transupp.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/transupp.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg-jni.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg-jni.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/turbojpeg.h` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/turbojpeg.h`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrbmp.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrbmp.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrgif.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrgif.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrjpgcom.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrjpgcom.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrppm.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrppm.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/cjpeglib/turbo210/wrtarga.c` & `jpeglib-0.9.3/jpeglib/cjpeglib/turbo210/wrtarga.c`

 * *Files identical despite different names*

### Comparing `jpeglib-0.9.2/jpeglib/jpeg.py` & `jpeglib-0.9.3/jpeglib/jpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,28 +171,28 @@
         # execute
         spatial = self._read_spatial(self.srcfile, out_color_space, dither_mode, dct_method, colormap, flags)
         self._im_dct = None # free DCT buffer
         # result
         return spatial
 
     def write_spatial(self, dstfile, data=None, in_color_space=None, dct_method="JDCT_ISLOW",
-                      samp_factor=None, qt=75, smoothing_factor=None, flags=[]):
+                      samp_factor=None, qt=-1, smoothing_factor=None, flags=[]):
         """Writes spatial image representation (i.e. RGB) to a file.
         
         :param dstfile: Destination file name.
         :type dstfile: str
         :param data: Numpy array with spatial data.
         :type data: numpy.ndarray, optional
         :param in_color_space: Input color space. Must be key of :class:`jpeg.JPEG.J_COLOR_SPACE`. According to source by default.
         :type in_color_space: str, optional
         :param dct_method: DCT method. Must be key of :class:`jpeg.JPEG.J_DCT_METHOD`. Using default from libjpeg by default.
         :type dct_method: str, optional
         :param samp_factor: Sampling factor. None, or list of 3 tuples of 2 ints. According to source by default. Read more at `glossary <https://jpeglib.readthedocs.io/en/latest/glossary.html#jpeg-sampling-factor>`_.
         :type samp_factor: list, optional
-        :param qt: Compression quality, between 0 and 100 or a tensor with quantization tables. Defaultly 100 (full quality).
+        :param qt: Compression quality, between 0 and 100 or a tensor with quantization tables. Defaultly -1 (default factor kept).
         :type qt: int | numpy.ndarray, optional
         :param smoothing_factor: Smoothing factor, between 0 and 100. Using default from libjpeg by default.
         :type smoothing_factor: int, optional
         :param flags: Bool decompression parameters as str to set to be true. Using default from libjpeg by default.
         :type flags: list, optional
 
         :Example:
```

### Comparing `jpeglib-0.9.2/jpeglib/version.py` & `jpeglib-0.9.3/jpeglib/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         :Example:
 
         >>> import jpeglib
         >>> jpeglib.version.set('8d')
         """
         if version in {'6','6b'}:
             CJpegLib.set_version(version='6b')
-        elif version in {'8','8d'}:
-            CJpegLib.set_version(version='8d')
-        elif version in {'9','9d'}:
-            CJpegLib.set_version(version='9d')
-        elif version in {'turbo2.1.0','turbo2.1','turbo210','turbo21'}:
+        elif version in {'7','8','8a','8b','8c','8d','9','9a','9b','9c','9d','9e'}:
+            CJpegLib.set_version(version=version)
+        elif version in {'turbo','turbo2.1.0','turbo2.1','turbo210','turbo21'}:
             CJpegLib.set_version(version='turbo210')
+        elif version in {'mozjpeg4.0.3','mozjpeg4','mozjpeg403','mozjpeg'}:
+            CJpegLib.set_version(version='mozjpeg403')
         else:
             raise NotImplementedError(f'Unsupported libjpeg version')
     @staticmethod
     def get():
         """Gets the currently used version of libjpeg. 
         
         :return: libjpeg version or None if not been loaded yet.
```

### Comparing `jpeglib-0.9.2/jpeglib.egg-info/PKG-INFO` & `jpeglib-0.9.3/jpeglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpeglib
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python envelope for the popular C library libjpeg for handling JPEG files.
 Home-page: https://jpeglib.readthedocs.io/en/latest/
 Author: Martin Beneš
 Author-email: martinbenes1996@gmail.com
 License: MPL
 Keywords: jpeglib,jpeg,jpg,libjpeg,compression,decompression,dct-coefficients,dct
 Platform: UNKNOWN
```

### Comparing `jpeglib-0.9.2/setup.py` & `jpeglib-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 
 # versions
 import os
-__version__ = os.environ.get('VERSION_NEW', '0.9.2')
+__version__ = os.environ.get('VERSION_NEW', '0.9.3')
 libjpeg_versions = {
   '6b': (None,60),
+  '7': (None,70),
+  '8': (None,80),
+  '8a': (None,80),
+  '8b': (None,80),
+  '8c': (None,80),
   '8d': (None,80),
+  '9': (None,90),
+  '9a': (None,90),
+  '9b': (None,90),
+  '9c': (None,90),
   '9d': (None,90),
-  'turbo210': ('2.1.0',210)
+  '9e': (None,90),
+  'turbo210': ('2.1.0',210),
+  'mozjpeg403': ('4.0.3',403)
 }
 
 # requirements
 try:
   with open('requirements.txt') as f:
     reqs = f.read().splitlines()
 except:
@@ -25,15 +36,17 @@
 import ctypes
 from pathlib import Path
 import re
 cfiles = {}
 hfiles = {}
 cjpeglib = {}
 for v in libjpeg_versions:
-  is_turbo = v[:5] == "turbo"
+  is_moz = v[:3] == "moz"
+  is_turbo = v[:5] == "turbo" or is_moz
+  
   clib = f'jpeglib/cjpeglib/{v}'
   
   # create missing
   package_name = 'libjpeg'
   (Path(clib) / 'jconfig.h').touch()
   (Path(clib) / 'vjpeglib.h').touch()
   if is_turbo:
@@ -41,49 +54,55 @@
     (Path(clib) / 'jconfigint.h').touch()
 
   files = [f'{clib}/{f}' for f in os.listdir(clib) if re.fullmatch(f'.*\.(c|h)', f)]
   for excluded_module in ['jmemdos','jmemmac','jmemansi','ansi2knr','ckconfig','jmemname', # platform dependents
                           'djpeg','cjpeg','rdjpgcom','wrjpgcom','cdjpeg','jpegtran', # executables
                           'rdbmp','wrbmp','rdcolmap','rdppm','wrppm','rdtarga','wrtarga','rdrle','wrrle','rdgif','wrgif','rdswitch', # others
                           'example', # example
+                          'cjpegalt','djpegalt',
                           #'jerror',
                           # turbo
                           'jccolext','jdcolext','jdcol565','jstdhuff',
                           'jdmrg565','jdmrgext',"jcstest","tjunittest","tjbench",
                           'turbojpeg-jni','turbojpeg']: 
     lim = -2 - len(excluded_module)
     files = [f for f in files if f[lim:-2] != excluded_module]
   #
   cfiles[v] = [f for f in files if f[-2:] == '.c']
   hfiles[v] = [f for f in files if f[-2:] == '.h']
   sources = ['jpeglib/cjpeglib/cjpeglib.c',*cfiles[v]]
   
-  turbo_macros = [
-    ("JPEG_LIB_VERSION",70),
-    ("INLINE","__inline__"),
-    ("PACKAGE_NAME",f"\"{package_name}\""),
-    ("BUILD",f"\"unknown\""),
-    ("VERSION",f"\"{libjpeg_versions[v][0]}\""),
-    ("SIZEOF_SIZE_T",int(ctypes.sizeof(ctypes.c_size_t))),
-    ("THREAD_LOCAL", "__thread")
-  ] if is_turbo else []
+  macros = [
+    ("BITS_IN_JSAMPLE",8),
+    ("HAVE_STDLIB_H",1),
+    ("LIBVERSION",libjpeg_versions[v][1]),
+    ("HAVE_PROTOTYPES",1),
+  ]
+  if is_turbo:
+    macros += [
+      ("JPEG_LIB_VERSION",80),#70),
+      ("INLINE","__inline__"),
+      ("PACKAGE_NAME",f"\"{package_name}\""),
+      ("BUILD",f"\"unknown\""),
+      ("VERSION",f"\"{libjpeg_versions[v][0]}\""),
+      ("SIZEOF_SIZE_T",int(ctypes.sizeof(ctypes.c_size_t))),
+      ("THREAD_LOCAL", "__thread")
+    ]
+  if is_moz:
+    macros += [
+      ('C_ARITH_CODING_SUPPORTED',1)
+    ]
 
   cjpeglib[v] = setuptools.Extension(
     name = f"jpeglib/cjpeglib/cjpeglib_{v}",
     library_dirs=['./jpeglib/cjpeglib',f'./{clib}'],#[f'./{clib}'],
     include_dirs=['./jpeglib/cjpeglib',f'./{clib}'],#[f'./{clib}'],
     sources = sources,
     headers = hfiles[v],
-    define_macros = [
-      ("BITS_IN_JSAMPLE",8),
-      ("HAVE_STDLIB_H",1),
-      ("LIBVERSION",libjpeg_versions[v][1]),
-      ("HAVE_PROTOTYPES",1),
-      *turbo_macros
-    ],
+    define_macros = macros,
     extra_compile_args=["-fPIC","-g"],
     language="c",
   )
 
 from setuptools.command.build_ext import build_ext
 class custom_build_ext(build_ext):
     def build_extensions(self):
@@ -100,15 +119,14 @@
         # 'object_filenames', 'objects', 'output_dir', 'preprocess', 'preprocessor', 'ranlib', 'runtime_library_dir_option',
         # 'runtime_library_dirs', 'set_executable', 'set_executables', 'set_include_dirs', 'set_libraries', 'set_library_dirs',
         # 'set_link_objects', 'set_runtime_library_dirs', 'shared_lib_extension', 'shared_lib_format', 'shared_object_filename',
         # 'spawn', 'src_extensions', 'static_lib_extension', 'static_lib_format', 'undefine_macro', 'verbose', 'warn',
         # 'xcode_stub_lib_extension', 'xcode_stub_lib_format'
         #print("==========", self.compiler.library_dirs)
         build_ext.build_extensions(self)
-        
 
 setuptools.setup(
   name = 'jpeglib',
   version = __version__,
   author = u'Martin Beneš',
   author_email = 'martinbenes1996@gmail.com',
   description = 'Python envelope for the popular C library libjpeg for handling JPEG files.',
@@ -149,7 +167,10 @@
     'Topic :: Scientific/Engineering :: Information Analysis',
     'Topic :: Security',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Utilities'
   ],
 )
+
+
+
```

