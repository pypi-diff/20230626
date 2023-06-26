# Comparing `tmp/trtpg-1.0.5-py3-none-any.whl.zip` & `tmp/trtpg-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 113940 bytes, number of entries: 41
+Zip file size: 115897 bytes, number of entries: 42
 -rw-rw-r--  2.0 unx     1188 b- defN 23-Jun-26 03:16 trtpg/__init__.py
 -rw-rw-r--  2.0 unx     4262 b- defN 23-Jun-26 04:28 trtpg/__main__.py
 -rw-rw-r--  2.0 unx     4088 b- defN 23-Jun-26 03:16 trtpg/config.py
 -rw-rw-r--  2.0 unx     8237 b- defN 23-Jun-26 04:24 trtpg/extract_unsupported_operators.py
--rw-rw-r--  2.0 unx    25729 b- defN 23-Jun-26 04:51 trtpg/generate.py
+-rw-rw-r--  2.0 unx    25740 b- defN 23-Jun-26 04:55 trtpg/generate.py
 -rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-26 03:16 trtpg/log.py
 -rw-rw-r--  2.0 unx     2646 b- defN 23-Jun-26 04:24 trtpg/yaml_parser.py
 -rw-rw-r--  2.0 unx    49231 b- defN 23-Jun-26 03:16 trtpg/doc/config.png
 -rw-rw-r--  2.0 unx     4373 b- defN 23-Jun-26 03:16 trtpg/doc/edit_yaml_config.md
 -rw-rw-r--  2.0 unx    19016 b- defN 23-Jun-26 03:16 trtpg/doc/onnx.png
 -rw-rw-r--  2.0 unx     9401 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.cpp
 -rw-rw-r--  2.0 unx     4895 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.h
 -rw-rw-r--  2.0 unx     8977 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.cpp
 -rw-rw-r--  2.0 unx     4706 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.h
 -rw-rw-r--  2.0 unx     1381 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/license.template
 -rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/makefile
 -rw-rw-r--  2.0 unx     1976 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/supported_operator_trt84.txt
 -rw-rw-r--  2.0 unx     1532 b- defN 23-Jun-26 03:16 trtpg/samples/readme.md
+-rw-rw-r--  2.0 unx     5750 b- defN 23-Jun-26 03:16 trtpg/samples/sample.yml
 -rw-rw-r--  2.0 unx     8606 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/README.md
 -rw-rw-r--  2.0 unx      749 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/efficientdet.yml
 -rw-rw-r--  2.0 unx     1528 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/modify_onnx.py
 -rw-rw-r--  2.0 unx     7574 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/README.md
 -rw-rw-r--  2.0 unx     1618 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/modify_onnx.py
 -rw-rw-r--  2.0 unx      423 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet.yml
 -rw-rw-r--  2.0 unx      439 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet_modified.yml
@@ -30,14 +31,14 @@
 -rw-rw-r--  2.0 unx     1537 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py
 -rw-rw-r--  2.0 unx      246 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml
 -rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/README.md
 -rw-rw-r--  2.0 unx     1553 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/modify_onnx.py
 -rw-rw-r--  2.0 unx      798 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/yolov4.yml
 -rw-rw-r--  2.0 unx     5860 b- defN 23-Jun-26 03:16 trtpg/tests/generate_fake_onnx_from_yml.py
 -rw-rw-r--  2.0 unx     3926 b- defN 23-Jun-26 03:16 trtpg/tests/test.yml
--rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3681 b- defN 23-Jun-26 04:52 trtpg-1.0.5.dist-info/RECORD
-41 files, 213986 bytes uncompressed, 107984 bytes compressed:  49.5%
+-rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3762 b- defN 23-Jun-26 04:55 trtpg-1.0.6.dist-info/RECORD
+42 files, 219828 bytes uncompressed, 109817 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -48,14 +48,17 @@
 
 Filename: trtpg/plugin_templates/supported_operator_trt84.txt
 Comment: 
 
 Filename: trtpg/samples/readme.md
 Comment: 
 
+Filename: trtpg/samples/sample.yml
+Comment: 
+
 Filename: trtpg/samples/efficientdet/README.md
 Comment: 
 
 Filename: trtpg/samples/efficientdet/efficientdet.yml
 Comment: 
 
 Filename: trtpg/samples/efficientdet/modify_onnx.py
@@ -99,26 +102,26 @@
 
 Filename: trtpg/tests/generate_fake_onnx_from_yml.py
 Comment: 
 
 Filename: trtpg/tests/test.yml
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/LICENSE.md
+Filename: trtpg-1.0.6.dist-info/LICENSE.md
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/METADATA
+Filename: trtpg-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/WHEEL
+Filename: trtpg-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/entry_points.txt
+Filename: trtpg-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/top_level.txt
+Filename: trtpg-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: trtpg-1.0.5.dist-info/RECORD
+Filename: trtpg-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trtpg/generate.py

```diff
@@ -596,15 +596,15 @@
         print(h)
         print(cpp)
         print(makefile)
 
 def generate(args):
     if not os.path.exists(args.yaml):
         if args.yaml == "@sample":
-            args.yaml = os.path.join(os.path.dirname(os.path.realpath(__file__)), "sample.yaml")
+            args.yaml = os.path.join(os.path.dirname(os.path.realpath(__file__)), "samples", "sample.yaml")
         else:
             print(f"Not exists file: {args.yaml}")
             return 1
     
     configs = read_yaml(args.yaml)
     for config in configs:
         codegen(config, args)
```

## Comparing `trtpg-1.0.5.dist-info/LICENSE.md` & `trtpg-1.0.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `trtpg-1.0.5.dist-info/RECORD` & `trtpg-1.0.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 trtpg/__init__.py,sha256=aUT9KqqX8pxwHpztw-xrAQ63TcsYUsoWVlp-nal1Flo,1188
 trtpg/__main__.py,sha256=0-yb4s6vYHKWCLxl0z2j7K30xMWHxZstKxP8WrqRapM,4262
 trtpg/config.py,sha256=dZn52Tf0QgOfmsOctmpQOfh0tZ82OHM-pIlPgzLEfgw,4088
 trtpg/extract_unsupported_operators.py,sha256=p37-AT5K60H-cuIu8lBbHKp0lN6lu96TUcoyRvx2UYw,8237
-trtpg/generate.py,sha256=E1aYRUtqtreRDvV9bkHtUylFVcaRMhD0dOdVN3nDzvs,25729
+trtpg/generate.py,sha256=h8kW-8E2IcKv_f26r1F3PrWSl4IZfc9meIk7THgv4T8,25740
 trtpg/log.py,sha256=4re8r5e3hgBhYCVBnf_Us5bbvIhBrryY_JRPK9DDjJk,1438
 trtpg/yaml_parser.py,sha256=N6WwCETg_ExA4GkJJcf895FaZBXoX7QCev9geLlB82g,2646
 trtpg/doc/config.png,sha256=P9NnmQFvE-KLbph-Z_GYn7zlAsjfnM-bPwxdJg305EI,49231
 trtpg/doc/edit_yaml_config.md,sha256=I7rGw2fj4AYviT8HbcGKipwaWLzzqoWiCrnQkkQaGlE,4373
 trtpg/doc/onnx.png,sha256=w800J6Xpi7rggaPipwi0QVml595urcLO8-gPqSAMuQM,19016
 trtpg/plugin_templates/IPluginV2DynamicExt.cpp,sha256=EpTOjNl93zJtpRfgyHV5jG67CzvccxmluafSViEYd8w,9401
 trtpg/plugin_templates/IPluginV2DynamicExt.h,sha256=Mdi2JWdKLNlO2AomKbTwTYQ99goxvEnPIqJgRYaQ1hM,4895
 trtpg/plugin_templates/IPluginV2IOExt.cpp,sha256=2-tJxkGgBulxQ2LJxQVNB3lOt-8sox9S6gFh1dvs3CM,8977
 trtpg/plugin_templates/IPluginV2IOExt.h,sha256=qHqifyPEFFmkn697Tj2AGXgr6_B9Y-sDH37mYYMxgdk,4706
 trtpg/plugin_templates/license.template,sha256=ScXqVT3Yys-KllzIrPx613rbWt5oruTq277K3hHDllU,1381
 trtpg/plugin_templates/makefile,sha256=3t4hIjFJD_wnHB1XhqvEdtSNqdWsZwc8thm_TupmZGc,1772
 trtpg/plugin_templates/supported_operator_trt84.txt,sha256=EOlrwRG0u2FVLfXgVoYMr0eqxhKorv21InYcVk1qYCM,1976
 trtpg/samples/readme.md,sha256=EBkC5EoU6b1csPDvpXSdEUEtKF9PD1REJglgL7VSoOM,1532
+trtpg/samples/sample.yml,sha256=jNC6iUMWORB_OqI4vqj0EdIEeL0Z34JOVTKdAVeJM1c,5750
 trtpg/samples/efficientdet/README.md,sha256=I2ddSQiOd6Zndu_9b-4PIA9kzmJwo5qhp3eeu895zDU,8606
 trtpg/samples/efficientdet/efficientdet.yml,sha256=5MmV3qtfC9581MrahXn59RAsSb7SyYYzdS80AEXaW_o,749
 trtpg/samples/efficientdet/modify_onnx.py,sha256=d9fBDDvW3LoUqRDDkxWqbivxl24Ug_QkMIjksQuJeKI,1528
 trtpg/samples/onnx_packnet/README.md,sha256=LXbBpHqITWDGdBU5EviKxVzkhAaKMoMdKnnXP5yxseU,7574
 trtpg/samples/onnx_packnet/modify_onnx.py,sha256=i7GyZ1ZbIEIaZHV7TiUeD7kLD1_GbY3AI8KGgxNXriw,1618
 trtpg/samples/onnx_packnet/onnx_packnet.yml,sha256=ZXRhkGbzX1Y83xs5lxue69izcXw7VWjn2mRLbRsdrx4,423
 trtpg/samples/onnx_packnet/onnx_packnet_modified.yml,sha256=s-Vslg2MsYHTVMqBqQNBjDvDFr1QricyFPOaJ08bFNc,439
@@ -29,13 +30,13 @@
 trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py,sha256=nhc0Xjht-jvfAzFrU1QZOscItuc6bB8pTmRrHdk16gM,1537
 trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml,sha256=FWTQ2A70wpBmcKISdVqXbNpF2d4qvZ0EyWwC8dbWzr0,246
 trtpg/samples/yolov4/README.md,sha256=9xnN7Ro9MTLTTNw0m1yY3pMiOyXkhmqffIySvMLkvF4,6116
 trtpg/samples/yolov4/modify_onnx.py,sha256=0EBLV6hxPJu9W0iPBuyPUJ1j4HYdyojHlncRUZLtYxY,1553
 trtpg/samples/yolov4/yolov4.yml,sha256=nsFqznjwpbNuYrr-XG_-sAK2FjGafCjeqzyBcfdmLqo,798
 trtpg/tests/generate_fake_onnx_from_yml.py,sha256=eThyvNyy91ZxPxpiWxD6uKIBcmYzAfWMBadG-GuqCLM,5860
 trtpg/tests/test.yml,sha256=extQuyrsCzSJ1TaDzWMS-h4YAaAcLAu7C8_-cpzw3JQ,3926
-trtpg-1.0.5.dist-info/LICENSE.md,sha256=59W3aI6gNG4CwIWjCSh4yXr937oWCIbPdtlrysRfckY,1084
-trtpg-1.0.5.dist-info/METADATA,sha256=TWQqnVXfscY0KUZXbUjXugYj6FTb0fqwwFQkRHHfOK4,307
-trtpg-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-trtpg-1.0.5.dist-info/entry_points.txt,sha256=8mOpiGKsxFGkK16wv4Sk95DhpTz7LCmJoji4Gf2xTJY,46
-trtpg-1.0.5.dist-info/top_level.txt,sha256=6e7w13oPzUS2M-HvpkmADRGL2c_XOkbyXJgNIHtnJuQ,6
-trtpg-1.0.5.dist-info/RECORD,,
+trtpg-1.0.6.dist-info/LICENSE.md,sha256=59W3aI6gNG4CwIWjCSh4yXr937oWCIbPdtlrysRfckY,1084
+trtpg-1.0.6.dist-info/METADATA,sha256=1ikvMVIWIeD_TS2rXBArBBnhFY2m7iVltgq7js-NTSo,307
+trtpg-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+trtpg-1.0.6.dist-info/entry_points.txt,sha256=8mOpiGKsxFGkK16wv4Sk95DhpTz7LCmJoji4Gf2xTJY,46
+trtpg-1.0.6.dist-info/top_level.txt,sha256=6e7w13oPzUS2M-HvpkmADRGL2c_XOkbyXJgNIHtnJuQ,6
+trtpg-1.0.6.dist-info/RECORD,,
```

