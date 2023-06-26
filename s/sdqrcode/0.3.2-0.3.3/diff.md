# Comparing `tmp/sdqrcode-0.3.2.tar.gz` & `tmp/sdqrcode-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.2.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.3.tar", max compression
```

## Comparing `sdqrcode-0.3.2.tar` & `sdqrcode-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-06-26 19:56:24.268532 sdqrcode-0.3.2/LICENSE
--rw-r--r--   0        0        0     9268 2023-06-26 19:56:24.268532 sdqrcode-0.3.2/README.md
--rw-r--r--   0        0        0      495 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     7900 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      721 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      779 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    12834 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    10101 1970-01-01 00:00:00.000000 sdqrcode-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-26 20:10:18.146164 sdqrcode-0.3.3/LICENSE
+-rw-r--r--   0        0        0     9268 2023-06-26 20:10:18.146164 sdqrcode-0.3.3/README.md
+-rw-r--r--   0        0        0      495 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     7900 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      719 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    12834 2023-06-26 20:10:18.190165 sdqrcode-0.3.3/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    10101 1970-01-01 00:00:00.000000 sdqrcode-0.3.3/PKG-INFO
```

### Comparing `sdqrcode-0.3.2/LICENSE` & `sdqrcode-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/README.md` & `sdqrcode-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.3/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.3/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.3/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.3/src/sdqrcode/configs/default_auto.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 global:
   mode: txt2img
   prompt: a beautiful dalmatian portrait, front shot
-  negative_prompt: ugly
+  negative_prompt: ""
   model_name_or_path: 6ce0161689
   steps: 20
   scheduler_name: DPM++ 2M Karras
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
```

### Comparing `sdqrcode-0.3.2/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.3/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 global:
   mode: txt2img
   prompt: a beautiful dalmatian portrait, front shot
-  negative_prompt: ugly
+  negative_prompt: ""
   model_name_or_path: SG161222/Realistic_Vision_V2.0
   steps: 20
   scheduler_name: DPM++ 2M Karras
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
```

### Comparing `sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_diffusers.yaml` & `sdqrcode-0.3.3/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.3/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.2/PKG-INFO` & `sdqrcode-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

