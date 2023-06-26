# Comparing `tmp/trtpg-1.0.2-py3-none-any.whl.zip` & `tmp/trtpg-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,43 @@
-Zip file size: 17307 bytes, number of entries: 13
+Zip file size: 113905 bytes, number of entries: 41
 -rw-rw-r--  2.0 unx     1188 b- defN 23-Jun-26 03:16 trtpg/__init__.py
 -rw-rw-r--  2.0 unx     4262 b- defN 23-Jun-26 04:28 trtpg/__main__.py
 -rw-rw-r--  2.0 unx     4088 b- defN 23-Jun-26 03:16 trtpg/config.py
 -rw-rw-r--  2.0 unx     8237 b- defN 23-Jun-26 04:24 trtpg/extract_unsupported_operators.py
 -rw-rw-r--  2.0 unx    25575 b- defN 23-Jun-26 04:24 trtpg/generate.py
 -rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-26 03:16 trtpg/log.py
 -rw-rw-r--  2.0 unx     2646 b- defN 23-Jun-26 04:24 trtpg/yaml_parser.py
--rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1006 b- defN 23-Jun-26 04:36 trtpg-1.0.2.dist-info/RECORD
-13 files, 49975 bytes uncompressed, 15645 bytes compressed:  68.7%
+-rw-rw-r--  2.0 unx    49231 b- defN 23-Jun-26 03:16 trtpg/doc/config.png
+-rw-rw-r--  2.0 unx     4373 b- defN 23-Jun-26 03:16 trtpg/doc/edit_yaml_config.md
+-rw-rw-r--  2.0 unx    19016 b- defN 23-Jun-26 03:16 trtpg/doc/onnx.png
+-rw-rw-r--  2.0 unx     9401 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.cpp
+-rw-rw-r--  2.0 unx     4895 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.h
+-rw-rw-r--  2.0 unx     8977 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.cpp
+-rw-rw-r--  2.0 unx     4706 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.h
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/license.template
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/makefile
+-rw-rw-r--  2.0 unx     1976 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/supported_operator_trt84.txt
+-rw-rw-r--  2.0 unx     1532 b- defN 23-Jun-26 03:16 trtpg/samples/readme.md
+-rw-rw-r--  2.0 unx     8606 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/README.md
+-rw-rw-r--  2.0 unx      749 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/efficientdet.yml
+-rw-rw-r--  2.0 unx     1528 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/modify_onnx.py
+-rw-rw-r--  2.0 unx     7574 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/README.md
+-rw-rw-r--  2.0 unx     1618 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/modify_onnx.py
+-rw-rw-r--  2.0 unx      423 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet.yml
+-rw-rw-r--  2.0 unx      439 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet_modified.yml
+-rw-rw-r--  2.0 unx     5322 b- defN 23-Jun-26 03:16 trtpg/samples/pointpillar/README.md
+-rw-rw-r--  2.0 unx      632 b- defN 23-Jun-26 03:16 trtpg/samples/pointpillar/pointpillar.yml
+-rw-rw-r--  2.0 unx     6995 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/README.md
+-rw-rw-r--  2.0 unx     1537 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py
+-rw-rw-r--  2.0 unx      246 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/README.md
+-rw-rw-r--  2.0 unx     1553 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/modify_onnx.py
+-rw-rw-r--  2.0 unx      798 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/yolov4.yml
+-rw-rw-r--  2.0 unx     5860 b- defN 23-Jun-26 03:16 trtpg/tests/generate_fake_onnx_from_yml.py
+-rw-rw-r--  2.0 unx     3926 b- defN 23-Jun-26 03:16 trtpg/tests/test.yml
+-rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3681 b- defN 23-Jun-26 04:39 trtpg-1.0.3.dist-info/RECORD
+41 files, 213832 bytes uncompressed, 107949 bytes compressed:  49.5%
```

## zipnote {}

```diff
@@ -15,26 +15,110 @@
 
 Filename: trtpg/log.py
 Comment: 
 
 Filename: trtpg/yaml_parser.py
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/LICENSE.md
+Filename: trtpg/doc/config.png
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/METADATA
+Filename: trtpg/doc/edit_yaml_config.md
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/WHEEL
+Filename: trtpg/doc/onnx.png
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/entry_points.txt
+Filename: trtpg/plugin_templates/IPluginV2DynamicExt.cpp
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/top_level.txt
+Filename: trtpg/plugin_templates/IPluginV2DynamicExt.h
 Comment: 
 
-Filename: trtpg-1.0.2.dist-info/RECORD
+Filename: trtpg/plugin_templates/IPluginV2IOExt.cpp
+Comment: 
+
+Filename: trtpg/plugin_templates/IPluginV2IOExt.h
+Comment: 
+
+Filename: trtpg/plugin_templates/license.template
+Comment: 
+
+Filename: trtpg/plugin_templates/makefile
+Comment: 
+
+Filename: trtpg/plugin_templates/supported_operator_trt84.txt
+Comment: 
+
+Filename: trtpg/samples/readme.md
+Comment: 
+
+Filename: trtpg/samples/efficientdet/README.md
+Comment: 
+
+Filename: trtpg/samples/efficientdet/efficientdet.yml
+Comment: 
+
+Filename: trtpg/samples/efficientdet/modify_onnx.py
+Comment: 
+
+Filename: trtpg/samples/onnx_packnet/README.md
+Comment: 
+
+Filename: trtpg/samples/onnx_packnet/modify_onnx.py
+Comment: 
+
+Filename: trtpg/samples/onnx_packnet/onnx_packnet.yml
+Comment: 
+
+Filename: trtpg/samples/onnx_packnet/onnx_packnet_modified.yml
+Comment: 
+
+Filename: trtpg/samples/pointpillar/README.md
+Comment: 
+
+Filename: trtpg/samples/pointpillar/pointpillar.yml
+Comment: 
+
+Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/README.md
+Comment: 
+
+Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py
+Comment: 
+
+Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml
+Comment: 
+
+Filename: trtpg/samples/yolov4/README.md
+Comment: 
+
+Filename: trtpg/samples/yolov4/modify_onnx.py
+Comment: 
+
+Filename: trtpg/samples/yolov4/yolov4.yml
+Comment: 
+
+Filename: trtpg/tests/generate_fake_onnx_from_yml.py
+Comment: 
+
+Filename: trtpg/tests/test.yml
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/LICENSE.md
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/METADATA
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/entry_points.txt
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: trtpg-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trtpg-1.0.2.dist-info/LICENSE.md` & `trtpg-1.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

