# Comparing `tmp/WIDscript-1.1.1.tar.gz` & `tmp/WIDscript-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WIDscript-1.1.1.tar", last modified: Sun Jun 25 11:31:37 2023, max compression
+gzip compressed data, was "WIDscript-1.1.2.tar", last modified: Sun Jun 25 22:29:11 2023, max compression
```

## Comparing `WIDscript-1.1.1.tar` & `WIDscript-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 11:31:37.108217 WIDscript-1.1.1/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      520 2023-06-25 11:31:37.109224 WIDscript-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.1.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      661 2023-06-25 11:31:37.110223 WIDscript-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 11:31:37.077659 WIDscript-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 11:31:37.089189 WIDscript-1.1.1/src/WIDscript/
--rw-rw-rw-   0        0        0    26578 2023-06-25 11:30:24.000000 WIDscript-1.1.1/src/WIDscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 11:31:37.107210 WIDscript-1.1.1/src/WIDscript.egg-info/
--rw-rw-rw-   0        0        0      520 2023-06-25 11:31:37.000000 WIDscript-1.1.1/src/WIDscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-25 11:31:37.000000 WIDscript-1.1.1/src/WIDscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 11:31:37.000000 WIDscript-1.1.1/src/WIDscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-25 11:31:37.000000 WIDscript-1.1.1/src/WIDscript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.666245 WIDscript-1.1.2/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-06-25 22:29:11.666245 WIDscript-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-21 01:38:12.000000 WIDscript-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      661 2023-06-25 22:29:11.668248 WIDscript-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.648248 WIDscript-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.653246 WIDscript-1.1.2/src/WIDscript/
+-rw-rw-rw-   0        0        0    26393 2023-06-25 22:28:10.000000 WIDscript-1.1.2/src/WIDscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 22:29:11.665243 WIDscript-1.1.2/src/WIDscript.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 22:29:11.000000 WIDscript-1.1.2/src/WIDscript.egg-info/top_level.txt
```

### Comparing `WIDscript-1.1.1/PKG-INFO` & `WIDscript-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.1.1
+Version: 1.1.2
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `WIDscript-1.1.1/setup.cfg` & `WIDscript-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 4944 7363 7269 7074 0d0a 7665   = WIDscript..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 310d 0a61  rsion = 1.1.1..a
+00000020: 7273 696f 6e20 3d20 312e 312e 320d 0a61  rsion = 1.1.2..a
 00000030: 7574 686f 7220 3d20 5749 444f 574e 0d0a  uthor = WIDOWN..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2077  author_email = w
 00000050: 6964 6f77 6e2e 6d61 4067 6d61 696c 2e63  idown.ma@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7072 6976 6174 6520 7772 6170  = A private wrap
 00000080: 7065 7220 6d61 6465 2066 6f72 2057 4944  per made for WID
 00000090: 4f57 4e20 7265 6c65 6173 6573 2e0d 0a6c  OWN releases...l
```

### Comparing `WIDscript-1.1.1/src/WIDscript/__init__.py` & `WIDscript-1.1.2/src/WIDscript/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,37 +106,31 @@
     slice = everything(source, **parameters_slice) if (useInOut == False) else initClip(inOutPath)
     clip  = core.std.Splice([clip[:start], slice, clip[end:]])
     
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
-def downscale(clip     : vs.VideoNode,
-              dsWidth  : int = 1920,
-              dsHeight : int = 1080) :
-
-    clip = format(clip)
-
-    # Downscaling using high quality algo.
-    clip = SSIM.scale(clip, dsWidth, dsHeight)
-
-    return clip
-
-############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
-
 def hdr2SDR(clip    : vs.VideoNode,
             dst_max : int   = 110,
             src_max : int   = 4000,
             src_min : float = 0.0050) :
     
     clip = format(clip)
-
-    # Tonemapping for HDR to SDR. Change src_max and src_min according to the source.
     clip = core.placebo.Tonemap(clip, src_csp=1, dst_csp=0, dst_prim=3, dynamic_peak_detection=1, dst_max=dst_max, src_max=src_max, src_min=src_min, tone_mapping_function=6, tone_mapping_mode=4, gamut_mode=0)
+    return clip
+
+############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
+
+def downscale(clip     : vs.VideoNode,
+              dsWidth  : int = 1920,
+              dsHeight : int = 1080) :
 
+    clip = format(clip)
+    clip = SSIM.scale(clip, dsWidth, dsHeight)
     return clip
 
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def mage(clip             : vs.VideoNode,
          thsxdxMultiplier : float = 0.65) :
 
@@ -225,20 +219,17 @@
             fsrcnnxPath   : str  = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1.glsl",
             fsrcnnxLaPath : str  = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1_LineArt.glsl",
             usWidth       : int  = 1920,
             usHeight      : int  = 1080) :
     
     # Verifying which upcaling model should be used depending on the content.
     fsrcnnxFinalPath = fsrcnnxLaPath if (isAnime == True) else fsrcnnxPath
-
+    
     clip = format(clip)
-
-    # Upscaling using high quality algo.
     clip = core.placebo.Shader(clip, fsrcnnxFinalPath,  usWidth, usHeight, filter="catmull_rom", antiring=0.7)
-    
     return clip
     
 ############################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################################
 
 def dehalo(clip : vs.VideoNode) :
     clip = format(clip)
     clip = DeHalo_alpha(clip, darkstr=0.4)
@@ -311,23 +302,23 @@
 
 def everything(clip                   : vs.VideoNode,
                #
                slice                  : bool  = False,
                start                  : int   = 0,
                end                    : int   = 0,
                #
-               useDownscaling         : bool  = False,
-               dsWidth                : int   = 1920,
-               dsHeight               : int   = 1080,
-               #
                useHDR2SDR             : bool  = False,
                dst_max                : int   = 110,
                src_max                : int   = 4000,
                src_min                : float = 0.0050,
                #
+               useDownscaling         : bool  = False,
+               dsWidth                : int   = 1920,
+               dsHeight               : int   = 1080,
+               #
                useMAGE                : bool  = False,
                thsxdxMultiplier       : float = 0.65,
                #
                useUpscaling           : bool  = False,
                isAnime                : bool  = True,
                fsrcnnxPath            : str   = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1.glsl",
                fsrcnnxLaPath          : str   = "C:/Softwares/AV1AN/FSRCNNX_x2_8-0-4-1_LineArt.glsl",
@@ -348,16 +339,16 @@
                #
                useDebanding           : bool  = False,
                dbRemBinarize          : int   = 1500,
                #
                useFinalizing          : bool  = True) :
     
     if (slice          == True) : clip = clip[start:end]
-    if (useDownscaling == True) : clip = downscale(clip, dsWidth, dsHeight)
     if (useHDR2SDR     == True) : clip = hdr2SDR(clip, dst_max, src_max, src_min)
+    if (useDownscaling == True) : clip = downscale(clip, dsWidth, dsHeight)
     if (useMAGE        == True) : clip = mage(clip, thsxdxMultiplier)
     if (useUpscaling   == True) : clip = upscale(clip, isAnime, fsrcnnxPath, fsrcnnxLaPath, usWidth, usHeight)
     if (useDehaloing   == True) : clip = dehalo(clip)
     if (useDeringing   == True) : clip = dering(clip)
     if (useAA          == True) : clip = aa(clip, useUsAA)
     if (useDPIR        == True) : clip = dpir(clip, dpirTileDenominator, dpirDeblocking, dpirDenoising, dpirDeblockingStrength, dpirDenoisingStrength)
     if (useDebanding   == True) : clip = deband(clip, dbRemBinarize)
```

### Comparing `WIDscript-1.1.1/src/WIDscript.egg-info/PKG-INFO` & `WIDscript-1.1.2/src/WIDscript.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WIDscript
-Version: 1.1.1
+Version: 1.1.2
 Summary: A private wrapper made for WIDOWN releases.
 Home-page: https://github.com/pypa/sampleproject
 Author: WIDOWN
 Author-email: widown.ma@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

