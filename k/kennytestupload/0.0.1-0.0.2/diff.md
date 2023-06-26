# Comparing `tmp/kennytestupload-0.0.1.macosx-10.9-x86_64.tar.gz` & `tmp/kennytestupload-0.0.2.macosx-10.9-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kenny/Desktop/GitHub/PythonClassContent/Pygame/dist/kennytestupload-0.0.1.macosx-10.9-x86_64.tar", last modified: Mon Jun 26 20:13:56 2023, max compression
+gzip compressed data, was "/Users/kenny/Desktop/GitHub/PythonClassContent/Pygame/dist/kennytestupload-0.0.2.macosx-10.9-x86_64.tar", last modified: Mon Jun 26 20:25:10 2023, max compression
```

## Comparing `kennytestupload-0.0.1.macosx-10.9-x86_64.tar` & `kennytestupload-0.0.2.macosx-10.9-x86_64.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.450896 ./
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.450959 ./Users/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451014 ./Users/kenny/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451072 ./Users/kenny/Desktop/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451130 ./Users/kenny/Desktop/GitHub/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451185 ./Users/kenny/Desktop/GitHub/PythonClassContent/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451289 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451353 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451412 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.451473 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.452059 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.493968 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.496187 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/
--rw-r--r--   0 kenny      (501) staff       (20)      416 2023-06-26 20:13:56.490932 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)      393 2023-06-26 20:13:56.493776 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 20:13:56.491149 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 kenny      (501) staff       (20)       12 2023-06-26 20:13:56.491442 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/requires.txt
--rw-r--r--   0 kenny      (501) staff       (20)       11 2023-06-26 20:13:56.492138 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.1-py3.8.egg-info/top_level.txt
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.454910 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854665 ./
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854722 ./Users/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854780 ./Users/kenny/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854842 ./Users/kenny/Desktop/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854899 ./Users/kenny/Desktop/GitHub/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.854952 ./Users/kenny/Desktop/GitHub/PythonClassContent/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.855007 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.855063 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.855118 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.855180 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.855238 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.891850 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.892868 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/
+-rw-r--r--   0 kenny      (501) staff       (20)      416 2023-06-26 20:25:10.888967 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)      393 2023-06-26 20:25:10.891681 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 20:25:10.889419 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        7 2023-06-26 20:25:10.889756 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/requires.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       11 2023-06-26 20:25:10.890197 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.2-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.858214 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/
 -rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/BasicDemo.py
 -rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/ClassUsage.py
 -rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Collision.py
 -rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Features.py
 -rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Main.py
 -rw-r--r--   0 kenny      (501) staff       (20)     3008 2023-06-26 19:40:48.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/SpaceInvader.py
 -rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Tets.py
 -rw-r--r--   0 kenny      (501) staff       (20)      126 2023-06-26 19:40:13.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__init__.py
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:13:56.463248 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/
--rw-r--r--   0 kenny      (501) staff       (20)      634 2023-06-26 20:13:56.455440 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/BasicDemo.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1770 2023-06-26 20:13:56.456868 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/ClassUsage.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1939 2023-06-26 20:13:56.458085 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Collision.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      213 2023-06-26 20:13:56.457442 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Features.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     9394 2023-06-26 20:13:56.463113 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Main.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     2930 2023-06-26 20:13:56.456312 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/SpaceInvader.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1640 2023-06-26 20:13:56.458859 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Tets.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      297 2023-06-26 20:13:56.457179 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:25:10.864916 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/
+-rw-r--r--   0 kenny      (501) staff       (20)      634 2023-06-26 20:25:10.858755 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/BasicDemo.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)     1770 2023-06-26 20:25:10.860191 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/ClassUsage.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)     1939 2023-06-26 20:25:10.861299 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Collision.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)      213 2023-06-26 20:25:10.860776 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Features.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)     9394 2023-06-26 20:25:10.864823 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Main.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)     2930 2023-06-26 20:25:10.859590 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/SpaceInvader.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)     1640 2023-06-26 20:25:10.861757 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Tets.cpython-38.pyc
+-rw-r--r--   0 kenny      (501) staff       (20)      297 2023-06-26 20:25:10.860519 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/__init__.cpython-38.pyc
```

### ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/BasicDemo.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 12 20:55:20 2023 UTC, .py size: 582 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -10,27 +10,27 @@
 00000090: a012 a100 0100 6513 8300 0100 7150 6509  ......e.....qPe.
 000000a0: 7280 6504 a014 650d 6406 a102 0100 6500  r.e...e.d.....e.
 000000b0: 6a02 a015 a100 0100 6508 a016 6407 a101  j.......e...d...
 000000c0: 0100 7146 6401 5300 2908 e900 0000 004e  ..qFd.S.)......N
 000000d0: 2902 6920 0300 00e9 9001 0000 5a04 4465  ).i ........Z.De
 000000e0: 6d6f 547a 0f64 6174 612f 616c 6965 6e33  moTz.data/alien3
 000000f0: 2e70 6e67 2902 7202 0000 00e9 c800 0000  .png).r.........
-00000100: e93c 0000 0029 175a 0670 7967 616d 65da  .<...).Z.pygame.
+00000100: e93c 0000 0029 17da 0670 7967 616d 65da  .<...)...pygame.
 00000110: 0469 6e69 745a 0764 6973 706c 6179 5a08  .initZ.displayZ.
 00000120: 7365 745f 6d6f 6465 5a06 7363 7265 656e  set_modeZ.screen
 00000130: 5a0b 7365 745f 6361 7074 696f 6eda 0474  Z.set_caption..t
 00000140: 696d 655a 0543 6c6f 636b 5a05 636c 6f63  imeZ.ClockZ.cloc
 00000150: 6b5a 0b67 616d 655f 6163 7469 7665 da05  kZ.game_active..
 00000160: 696d 6167 65da 046c 6f61 645a 0d63 6f6e  image..loadZ.con
 00000170: 7665 7274 5f61 6c70 6861 5a0e 706c 6179  vert_alphaZ.play
 00000180: 6572 5f73 7572 6661 6365 da05 6576 656e  er_surface..even
 00000190: 74da 0367 6574 da04 7479 7065 5a04 5155  t..get..typeZ.QU
 000001a0: 4954 da04 7175 6974 da04 6578 6974 5a04  IT..quit..exitZ.
 000001b0: 626c 6974 da06 7570 6461 7465 5a04 7469  blit..updateZ.ti
-000001c0: 636b a900 720f 0000 0072 0f00 0000 fa7b  ck..r....r.....{
+000001c0: 636b a900 7210 0000 0072 1000 0000 fa7b  ck..r....r.....{
 000001d0: 2f55 7365 7273 2f6b 656e 6e79 2f44 6573  /Users/kenny/Des
 000001e0: 6b74 6f70 2f47 6974 4875 622f 5079 7468  ktop/GitHub/Pyth
 000001f0: 6f6e 436c 6173 7343 6f6e 7465 6e74 2f50  onClassContent/P
 00000200: 7974 686f 6e41 6c67 6f2f 5079 7468 6f6e  ythonAlgo/Python
 00000210: 4453 2f76 656e 762f 6c69 622f 7079 7468  DS/venv/lib/pyth
 00000220: 6f6e 332e 382f 7369 7465 2d70 6163 6b61  on3.8/site-packa
 00000230: 6765 732f 7465 7374 7570 6c6f 6164 2f42  ges/testupload/B
```

### ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Main.cpython-38.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:31:00 2023 UTC, .py size: 11451 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -564,15 +564,15 @@
 00002330: 0403 0c01 0a01 0a02 0a03 0c03 0803 1401  ................
 00002340: 0a01 0a01 1c01 0c01 0801 0801 0603 0601  ................
 00002350: 0a01 1201 0601 0403 1801 0a03 1401 0801  ................
 00002360: 0801 0801 0801 0801 0c03 1a01 0801 0801  ................
 00002370: 0801 0c03 1401 0801 0801 0801 0801 0c03  ................
 00002380: 0a01 0c03 0e02 0801 0e01 7278 0000 00da  ..........rx....
 00002390: 085f 5f6d 6169 6e5f 5f29 0172 0100 0000  .__main__).r....
-000023a0: 2920 723f 0000 0072 0700 0000 5a06 7079  ) r?...r....Z.py
+000023a0: 2920 723f 0000 0072 0700 0000 da06 7079  ) r?...r......py
 000023b0: 6761 6d65 720b 0000 0072 0c00 0000 5a0c  gamer....r....Z.
 000023c0: 6765 745f 6578 7465 6e64 6564 720f 0000  get_extendedr...
 000023d0: 0072 7000 0000 7272 0000 0072 7300 0000  .rp...rr...rs...
 000023e0: 7265 0000 005a 0452 6563 7472 2500 0000  re...Z.Rectr%...
 000023f0: 7258 0000 0072 0800 0000 da05 7370 6c69  rX...r......spli
 00002400: 74da 0761 6273 7061 7468 da08 5f5f 6669  t..abspath..__fi
 00002410: 6c65 5f5f 720a 0000 0072 1400 0000 7217  le__r....r....r.
```

