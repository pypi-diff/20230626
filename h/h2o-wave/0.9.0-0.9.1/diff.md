# Comparing `tmp/h2o_wave-0.9.0-py3-none-any.whl.zip` & `tmp/h2o_wave-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 62284 bytes, number of entries: 16
+Zip file size: 62405 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      913 b- defN 20-Oct-26 21:42 h2o_wave/__init__.py
 -rw-rw-r--  2.0 unx       61 b- defN 20-Oct-28 03:28 h2o_wave/__main__.py
--rw-rw-r--  2.0 unx     1139 b- defN 20-Oct-28 09:42 h2o_wave/cli.py
+-rw-rw-r--  2.0 unx     1387 b- defN 20-Oct-29 06:19 h2o_wave/cli.py
 -rw-rw-r--  2.0 unx    21911 b- defN 20-Oct-28 04:12 h2o_wave/core.py
 -rw-rw-r--  2.0 unx     5877 b- defN 20-Oct-28 01:04 h2o_wave/db.py
 -rw-rw-r--  2.0 unx    25866 b- defN 20-Oct-20 00:19 h2o_wave/graphics.py
 -rw-rw-r--  2.0 unx    11127 b- defN 20-Oct-28 05:01 h2o_wave/server.py
 -rw-rw-r--  2.0 unx     2143 b- defN 20-Oct-20 20:31 h2o_wave/test.py
 -rw-rw-r--  2.0 unx   244709 b- defN 20-Oct-28 21:14 h2o_wave/types.py
 -rw-rw-r--  2.0 unx    95754 b- defN 20-Oct-28 21:14 h2o_wave/ui.py
--rw-rw-r--  2.0 unx       53 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2452 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1227 b- defN 20-Oct-29 04:35 h2o_wave-0.9.0.dist-info/RECORD
-16 files, 413377 bytes uncompressed, 60296 bytes compressed:  85.4%
+-rw-rw-r--  2.0 unx       53 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2452 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1227 b- defN 20-Oct-29 06:23 h2o_wave-0.9.1.dist-info/RECORD
+16 files, 413625 bytes uncompressed, 60417 bytes compressed:  85.4%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: h2o_wave/types.py
 Comment: 
 
 Filename: h2o_wave/ui.py
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/LICENSE
+Filename: h2o_wave-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/METADATA
+Filename: h2o_wave-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/WHEEL
+Filename: h2o_wave-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/entry_points.txt
+Filename: h2o_wave-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/top_level.txt
+Filename: h2o_wave-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_wave-0.9.0.dist-info/RECORD
+Filename: h2o_wave-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_wave/cli.py

```diff
@@ -1,7 +1,8 @@
+import sys
 import socket
 from contextlib import closing
 import uvicorn
 import click
 import os
 
 _localhost = '127.0.0.1'
@@ -40,8 +41,14 @@
     """
 
     port = _scan_free_port()
     addr = f'http://{_localhost}:{port}'
     os.environ['H2O_WAVE_INTERNAL_ADDRESS'] = addr  # TODO deprecated
     os.environ['H2O_WAVE_EXTERNAL_ADDRESS'] = addr  # TODO deprecated
     os.environ['H2O_WAVE_APP_ADDRESS'] = addr
+
+    # Make "python -m h2o_wave run" behave identical to "wave run":
+    # Insert cwd into path, otherwise uvicorn fails to locate the app module.
+    # uvicorn.main() does this before calling uvicorn.run().
+    sys.path.insert(0, '.')
+
     uvicorn.run(f'{app}:main', host=_localhost, port=port, reload=not no_reload)
```

## Comparing `h2o_wave-0.9.0.dist-info/METADATA` & `h2o_wave-0.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-wave
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python driver for H2O Wave Realtime Apps
 Home-page: https://h2o.ai/h2o-wave/
 Author: Prithvi Prabhu
 Author-email: prithvi@h2o.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `h2o_wave-0.9.0.dist-info/RECORD` & `h2o_wave-0.9.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 h2o_wave/__init__.py,sha256=CAHlJzPWGEV81bzT3FA8n5fd7o6G8VaX9T7TqWUvRVY,913
 h2o_wave/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
-h2o_wave/cli.py,sha256=80FxOYtvA9GY4s0MYygkxz1jc4C0N59P6AVTHL_DFJA,1139
+h2o_wave/cli.py,sha256=_AfmU0yGUnP3At4-EaJkbLbQRZgoPsdKXHZQcXKPqPM,1387
 h2o_wave/core.py,sha256=XzTfJvhZoA5cq02e1Z7ZGXx11LzbQ94c-u2XRNPcVNo,21911
 h2o_wave/db.py,sha256=igONeXg2PPSXlWPy44r6K2n6i6hX-zPGVsNO0szp4bM,5877
 h2o_wave/graphics.py,sha256=HLYrX-lwsMKbyLmy2ClG5L46DA2_hSCEPTsv0gPVoyg,25866
 h2o_wave/server.py,sha256=8W4k8D_Tag6JKPiSys-N9r_yZgqph7tKooKkTeGMrQQ,11127
 h2o_wave/test.py,sha256=dy4imDCKCajGshRmPXe1AB50_00DoqGS-7-ng5LoRME,2143
 h2o_wave/types.py,sha256=g55SQPUx_JJBkToHY1p6yDQsCZvypN6V_V-mEFUtBw0,244709
 h2o_wave/ui.py,sha256=O6nzZSswFGwO7jUAqQJUl1F6rwQZAgf0h4LiQDLhnE8,95754
-h2o_wave-0.9.0.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
-h2o_wave-0.9.0.dist-info/METADATA,sha256=4JtnEGqaR8c2-47568lF64Ssyvj_UKRTcxEhJmOyl6o,2452
-h2o_wave-0.9.0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-h2o_wave-0.9.0.dist-info/entry_points.txt,sha256=0JfvaphzVeSD5pkJTr6OKTLcROFnQ1cp31DI8M5frzY,44
-h2o_wave-0.9.0.dist-info/top_level.txt,sha256=jmpW_e6CkJf82dE4S7ofAe2ipbBd1YmrS-0MM-DN0lY,9
-h2o_wave-0.9.0.dist-info/RECORD,,
+h2o_wave-0.9.1.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
+h2o_wave-0.9.1.dist-info/METADATA,sha256=MRs11T1cFUonsRWLobUuGfCucaTV2aEteThBe9qR9Ss,2452
+h2o_wave-0.9.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+h2o_wave-0.9.1.dist-info/entry_points.txt,sha256=0JfvaphzVeSD5pkJTr6OKTLcROFnQ1cp31DI8M5frzY,44
+h2o_wave-0.9.1.dist-info/top_level.txt,sha256=jmpW_e6CkJf82dE4S7ofAe2ipbBd1YmrS-0MM-DN0lY,9
+h2o_wave-0.9.1.dist-info/RECORD,,
```

