# Comparing `tmp/sdqrcode-0.3.1.tar.gz` & `tmp/sdqrcode-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.1.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.2.tar", max compression
```

## Comparing `sdqrcode-0.3.1.tar` & `sdqrcode-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-06-25 10:02:14.561147 sdqrcode-0.3.1/LICENSE
--rw-r--r--   0        0        0     5343 2023-06-25 10:02:14.561147 sdqrcode-0.3.1/README.md
--rw-r--r--   0        0        0      474 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2410 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     1749 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      616 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      696 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0     8892 2023-06-25 10:02:14.585148 sdqrcode-0.3.1/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 sdqrcode-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-26 19:56:24.268532 sdqrcode-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9268 2023-06-26 19:56:24.268532 sdqrcode-0.3.2/README.md
+-rw-r--r--   0        0        0      495 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     7900 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      426 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      721 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      779 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    12834 2023-06-26 19:56:24.316533 sdqrcode-0.3.2/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    10101 1970-01-01 00:00:00.000000 sdqrcode-0.3.2/PKG-INFO
```

### Comparing `sdqrcode-0.3.1/LICENSE` & `sdqrcode-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.1/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.2/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.1/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.2/src/sdqrcode/configs/default_auto.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 global:
-  prompt: "a beautiful minecraft landscape, lights and shadows"
-  model_name_or_path: "6ce0161689"
+  mode: txt2img
+  prompt: a beautiful dalmatian portrait, front shot
+  negative_prompt: ugly
+  model_name_or_path: 6ce0161689
   steps: 20
-  sampler_name: Euler a
+  scheduler_name: DPM++ 2M Karras
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
+  batch_size: 1
 
 controlnet_units:
   brightness:
     model: control_v1p_sd15_brightness [5f6aa6ed]
+    cn_input_image: qrcode
     module: none
     weight: 0.35
     start: 0.0
     end: 1.0
 
   tile:
     model: control_v11f1e_sd15_tile [a371b31b]
+    cn_input_image: qrcode
     module: none
     weight: 0.5
     start: 0.35
     end: 0.70
 
 qrcode:
-  text: "https://koll.ai"
+  text: https://koll.ai
   error_correction: high # [low, medium, quart, high]
   box_size: 10
   border: 4
   fill_color: black
   back_color: white
```

### Comparing `sdqrcode-0.3.1/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.2/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 global:
-  prompt: "a beautiful minecraft landscape, lights and shadows"
-  model_name_or_path: "SG161222/Realistic_Vision_V2.0"
+  mode: txt2img
+  prompt: a beautiful dalmatian portrait, front shot
+  negative_prompt: ugly
+  model_name_or_path: SG161222/Realistic_Vision_V2.0
   steps: 20
-  # sampler_name: Euler a not implemented yet
+  scheduler_name: DPM++ 2M Karras
   cfg_scale: 7
   width: 768
   height: 768
   seed: -1
+  batch_size: 1
 
 controlnet_units:
   brightness:
     model: ioclab/control_v1p_sd15_brightness
-    #module: none not implemented yet
+    cn_input_image: qrcode
+    module: none #not implemented yet
     weight: 0.35
     start: 0.0
     end: 1.0
 
   tile:
     model: lllyasviel/control_v11f1e_sd15_tile
-    #module: none not implemented yet
+    module: none #not implemented yet
+    cn_input_image: qrcode
     weight: 0.5
     start: 0.35
     end: 0.70
 
 qrcode:
-  text: "https://koll.ai"
+  text: https://koll.ai
   error_correction: high # [low, medium, quart, high]
   box_size: 10
   border: 4
   fill_color: black
   back_color: white
```

