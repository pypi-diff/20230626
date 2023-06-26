# Comparing `tmp/imaginepy-1.1.0.tar.gz` & `tmp/imaginepy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginepy-1.1.0.tar", last modified: Mon May 22 22:10:40 2023, max compression
+gzip compressed data, was "imaginepy-2.0.0.tar", last modified: Mon Jun 26 00:36:50 2023, max compression
```

## Comparing `imaginepy-1.1.0.tar` & `imaginepy-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.261387 imaginepy-1.1.0/
--rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5009 2023-05-22 22:10:40.260381 imaginepy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4338 2023-05-22 22:10:21.000000 imaginepy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.238769 imaginepy-1.1.0/imaginepy/
--rw-rw-rw-   0        0        0      127 2023-05-22 21:09:41.000000 imaginepy-1.1.0/imaginepy/__init__.py
--rw-rw-rw-   0        0        0     6522 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/async_imagine.py
--rw-rw-rw-   0        0        0    18638 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/constants.py
--rw-rw-rw-   0        0        0     6988 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/sync_imagine.py
-drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.259881 imaginepy-1.1.0/imaginepy.egg-info/
--rw-rw-rw-   0        0        0     5009 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 22:10:40.261387 imaginepy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-05-22 21:11:16.000000 imaginepy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.949813 imaginepy-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5376 2023-06-26 00:36:50.949313 imaginepy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4510 2023-06-26 00:35:21.000000 imaginepy-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.933788 imaginepy-2.0.0/imaginepy/
+-rw-rw-rw-   0        0        0      146 2023-06-25 23:44:15.000000 imaginepy-2.0.0/imaginepy/__init__.py
+-rw-rw-rw-   0        0        0    11029 2023-06-26 00:08:10.000000 imaginepy-2.0.0/imaginepy/async_imagine.py
+-rw-rw-rw-   0        0        0    44101 2023-06-25 23:52:33.000000 imaginepy-2.0.0/imaginepy/constants.py
+-rw-rw-rw-   0        0        0      326 2023-06-25 22:17:39.000000 imaginepy-2.0.0/imaginepy/exceptions.py
+-rw-rw-rw-   0        0        0    10572 2023-06-26 00:10:58.000000 imaginepy-2.0.0/imaginepy/sync_imagine.py
+-rw-rw-rw-   0        0        0     1615 2023-06-25 22:15:48.000000 imaginepy-2.0.0/imaginepy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.948313 imaginepy-2.0.0/imaginepy.egg-info/
+-rw-rw-rw-   0        0        0     5376 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 00:36:50.950314 imaginepy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-06-26 00:15:09.000000 imaginepy-2.0.0/setup.py
```

### Comparing `imaginepy-1.1.0/LICENSE` & `imaginepy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginepy-1.1.0/PKG-INFO` & `imaginepy-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: imaginepy
-Version: 1.1.0
-Summary: Python library to create Art with AI.
-Home-page: https://github.com/ItsCEED/imaginepy
-Author: CEED
-Author-email: 
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
-
+<b>>PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!</b>
+<br>
+  
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
 <br>
-<img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4"/>
+<a href="https://discord.gg/axfkjqWR5E" target="_blank">
+  <img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4">
+</a>
 <br>
 <img src="https://img.shields.io/badge/python-3.7+-informational?style=plastic" alt="Python version">
 <img src="https://img.shields.io/github/release-date/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Release">
 <img src="https://img.shields.io/github/release/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Version">
 
 </div>
 
@@ -86,15 +71,15 @@
 The following is a minimal example of using ImaginePy in a script. It gets the generated image
 from the text and increases the quality.
 
 ```python
 from imaginepy import Imagine, Style, Ratio
 
 def main():
-    imagine = Imagine()
+    imagine = Imagine(style=Style.ANIME_V2)
 
     img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
         style=Style.ANIME_V2,
         ratio=Ratio.RATIO_16X9
     )
 
@@ -122,15 +107,15 @@
 
 ```python
 import asyncio
 from imaginepy import AsyncImagine, Style, Ratio
 
 
 async def main():
-    imagine = AsyncImagine()
+    imagine = AsyncImagine(style=Style.ANIME_V2)
 
     img_data = await imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
         style=Style.ANIME_V2,
         ratio=Ratio.RATIO_16X9
     )
```

### Comparing `imaginepy-1.1.0/imaginepy.egg-info/PKG-INFO` & `imaginepy-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,314 +1,336 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2069 6d61  : 2.1..Name: ima
 00000020: 6769 6e65 7079 0d0a 5665 7273 696f 6e3a  ginepy..Version:
-00000030: 2031 2e31 2e30 0d0a 5375 6d6d 6172 793a   1.1.0..Summary:
+00000030: 2032 2e30 2e30 0d0a 5375 6d6d 6172 793a   2.0.0..Summary:
 00000040: 2050 7974 686f 6e20 6c69 6272 6172 7920   Python library 
 00000050: 746f 2063 7265 6174 6520 4172 7420 7769  to create Art wi
 00000060: 7468 2041 492e 0d0a 486f 6d65 2d70 6167  th AI...Home-pag
 00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000080: 622e 636f 6d2f 4974 7343 4545 442f 696d  b.com/ItsCEED/im
 00000090: 6167 696e 6570 790d 0a41 7574 686f 723a  aginepy..Author:
 000000a0: 2043 4545 440d 0a41 7574 686f 722d 656d   CEED..Author-em
-000000b0: 6169 6c3a 200d 0a43 6c61 7373 6966 6965  ail: ..Classifie
-000000c0: 723a 2045 6e76 6972 6f6e 6d65 6e74 203a  r: Environment :
-000000d0: 3a20 436f 6e73 6f6c 650d 0a43 6c61 7373  : Console..Class
-000000e0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-000000f0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000100: 3a20 474e 5520 4765 6e65 7261 6c20 5075  : GNU General Pu
-00000110: 626c 6963 204c 6963 656e 7365 2076 3320  blic License v3 
-00000120: 2847 504c 7633 290d 0a43 6c61 7373 6966  (GPLv3)..Classif
-00000130: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000140: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000150: 7065 6e64 656e 740d 0a43 6c61 7373 6966  pendent..Classif
-00000160: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000170: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000180: 686f 6e20 3a3a 2033 2e34 0d0a 436c 6173  hon :: 3.4..Clas
-00000190: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000001a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001b0: 5079 7468 6f6e 203a 3a20 332e 350d 0a43  Python :: 3.5..C
-000001c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e36  :: Python :: 3.6
-000001f0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 332e 370d 0a43 6c61 7373 6966 6965 723a  3.7..Classifier:
-00000230: 2054 6f70 6963 203a 3a20 5574 696c 6974   Topic :: Utilit
-00000240: 6965 730d 0a52 6571 7569 7265 732d 5079  ies..Requires-Py
-00000250: 7468 6f6e 3a20 3e3d 332e 370d 0a44 6573  thon: >=3.7..Des
-00000260: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000270: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000280: 646f 776e 0d0a 4c69 6365 6e73 652d 4669  down..License-Fi
-00000290: 6c65 3a20 4c49 4345 4e53 450d 0a0d 0a3c  le: LICENSE....<
-000002a0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-000002b0: 7222 3e0d 0a0d 0a3c 696d 6720 7372 633d  r">....<img src=
-000002c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002d0: 636f 6d2f 4974 7343 4545 442f 496d 6167  com/ItsCEED/Imag
-000002e0: 696e 6550 792d 4d69 646a 6f75 726e 6579  inePy-Midjourney
-000002f0: 2d46 7265 652d 416c 7465 726e 6174 6976  -Free-Alternativ
-00000300: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
-00000310: 2f69 6d61 6769 6e65 5f6c 6f67 6f2e 6769  /imagine_logo.gi
-00000320: 6622 2077 6964 7468 3d22 3130 2522 3e0d  f" width="10%">.
-00000330: 0a0d 0a2a 2a49 6d61 6769 6e65 5079 2a2a  ...**ImaginePy**
-00000340: 0d0a 3c62 723e 0d0a 3c69 6d67 2073 7263  ..<br>..<img src
-00000350: 3d22 6874 7470 733a 2f2f 6469 7363 6f72  ="https://discor
-00000360: 6461 7070 2e63 6f6d 2f61 7069 2f67 7569  dapp.com/api/gui
-00000370: 6c64 732f 3131 3130 3331 3439 3731 3031  lds/111031497101
-00000380: 3238 3038 3737 342f 7769 6467 6574 2e70  2808774/widget.p
-00000390: 6e67 3f73 7479 6c65 3d62 616e 6e65 7234  ng?style=banner4
-000003a0: 2220 616c 743d 2244 6973 636f 7264 2042  " alt="Discord B
-000003b0: 616e 6e65 7220 3422 2f3e 0d0a 3c62 723e  anner 4"/>..<br>
-000003c0: 0d0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
-000003d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000003e0: 696f 2f62 6164 6765 2f70 7974 686f 6e2d  io/badge/python-
-000003f0: 332e 372b 2d69 6e66 6f72 6d61 7469 6f6e  3.7+-information
-00000400: 616c 3f73 7479 6c65 3d70 6c61 7374 6963  al?style=plastic
-00000410: 2220 616c 743d 2250 7974 686f 6e20 7665  " alt="Python ve
-00000420: 7273 696f 6e22 3e0d 0a3c 696d 6720 7372  rsion">..<img sr
-00000430: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000440: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000450: 2f72 656c 6561 7365 2d64 6174 652f 4974  /release-date/It
-00000460: 7343 4545 442f 496d 6167 696e 6550 792d  sCEED/ImaginePy-
-00000470: 4d69 646a 6f75 726e 6579 2d46 7265 652d  Midjourney-Free-
-00000480: 416c 7465 726e 6174 6976 653f 7374 796c  Alternative?styl
-00000490: 653d 706c 6173 7469 6322 2061 6c74 3d22  e=plastic" alt="
-000004a0: 5265 6c65 6173 6522 3e0d 0a3c 696d 6720  Release">..<img 
-000004b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000004c0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000004d0: 7562 2f72 656c 6561 7365 2f49 7473 4345  ub/release/ItsCE
-000004e0: 4544 2f49 6d61 6769 6e65 5079 2d4d 6964  ED/ImaginePy-Mid
-000004f0: 6a6f 7572 6e65 792d 4672 6565 2d41 6c74  journey-Free-Alt
-00000500: 6572 6e61 7469 7665 3f73 7479 6c65 3d70  ernative?style=p
-00000510: 6c61 7374 6963 2220 616c 743d 2256 6572  lastic" alt="Ver
-00000520: 7369 6f6e 223e 0d0a 0d0a 3c2f 6469 763e  sion">....</div>
-00000530: 0d0a 0d0a 2323 2046 6561 7475 7265 730d  ....## Features.
-00000540: 0a0d 0a2d 20f0 9f8e a820 5475 726e 2077  ...- .... Turn w
-00000550: 6f72 6473 2069 6e74 6f20 6172 740d 0a2d  ords into art..-
-00000560: 20f0 9f91 9320 4368 6f6f 7365 2066 726f   .... Choose fro
-00000570: 6d20 616e 2061 7272 6179 206f 6620 6172  m an array of ar
-00000580: 7420 7374 796c 6573 0d0a 2d20 f09f 94a7  t styles..- ....
-00000590: 2041 646a 7573 7420 796f 7572 206d 6173   Adjust your mas
-000005a0: 7465 7270 6965 6365 2077 6974 6820 6372  terpiece with cr
-000005b0: 6561 7469 7665 2063 6f6e 7472 6f6c 7321  eative controls!
-000005c0: 0d0a 2d20 f09f 93a6 2053 7461 7920 6168  ..- .... Stay ah
-000005d0: 6561 6420 6f66 2074 6865 2067 616d 6520  ead of the game 
-000005e0: 7769 7468 2074 6865 2065 7665 722d 6772  with the ever-gr
-000005f0: 6f77 696e 6720 6172 7420 6c69 6272 6172  owing art librar
-00000600: 7921 0d0a 2d20 f09f 8c87 2047 656e 6572  y!..- .... Gener
-00000610: 6174 6520 7761 6c6c 7061 7065 7273 0d0a  ate wallpapers..
-00000620: 2d20 f09f 948e 2044 6973 636f 7665 7220  - .... Discover 
-00000630: 616e 6420 6578 706c 6f72 6520 7369 6d69  and explore simi
-00000640: 6c61 7220 6172 7469 7374 6963 2064 6573  lar artistic des
-00000650: 6967 6e73 0d0a 2d20 5468 6973 2069 7320  igns..- This is 
-00000660: 7265 6661 6374 6f72 6564 2061 6e64 2069  refactored and i
-00000670: 6d70 726f 7665 6420 7665 7273 696f 6e20  mproved version 
-00000680: 6f66 2074 6865 206f 7269 6769 6e61 6c20  of the original 
-00000690: 6672 6f6d 205b 6879 7567 6f67 6972 7562  from [hyugogirub
-000006a0: 6174 6f5d 0d0a 0d0a 2323 2049 6e73 7461  ato]....## Insta
-000006b0: 6c6c 6174 696f 6e0d 0a0d 0a5f 4e6f 7465  llation...._Note
-000006c0: 3a20 5265 7175 6972 6573 205b 5079 7468  : Requires [Pyth
-000006d0: 6f6e 5d20 332e 372e 3020 6f72 206e 6577  on] 3.7.0 or new
-000006e0: 6572 2077 6974 6820 5049 5020 696e 7374  er with PIP inst
-000006f0: 616c 6c65 642e 5f0d 0a0d 0a60 6060 7368  alled._....```sh
-00000700: 656c 6c0d 0a24 2070 7974 686f 6e20 7365  ell..$ python se
-00000710: 7475 702e 7079 2069 6e73 7461 6c6c 0d0a  tup.py install..
-00000720: 6060 600d 0a0d 0a59 6f75 206e 6f77 2068  ```....You now h
-00000730: 6176 6520 7468 6520 6069 6d61 6769 6e65  ave the `imagine
-00000740: 7079 6020 7061 636b 6167 6520 696e 7374  py` package inst
-00000750: 616c 6c65 642e 0d0a 0d0a 2323 2320 5079  alled.....### Py
-00000760: 5069 2049 6e73 7461 6c6c 6174 696f 6e0d  Pi Installation.
-00000770: 0a0d 0a60 6060 0d0a 7069 7020 696e 7374  ...```..pip inst
-00000780: 616c 6c20 696d 6167 696e 6570 790d 0a60  all imaginepy..`
-00000790: 6060 0d0a 0d0a 5b50 7974 686f 6e5d 3a20  ``....[Python]: 
-000007a0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6f  https://python.o
-000007b0: 7267 0d0a 5b56 656e 7627 735d 3a20 6874  rg..[Venv's]: ht
-000007c0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-000007d0: 6e2e 6f72 672f 332f 7475 746f 7269 616c  n.org/3/tutorial
-000007e0: 2f76 656e 762e 6874 6d6c 0d0a 5b56 656e  /venv.html..[Ven
-000007f0: 7627 7320 446f 6373 5d3a 2068 7474 7073  v's Docs]: https
-00000800: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00000810: 7267 2f33 2f6c 6962 7261 7279 2f76 656e  rg/3/library/ven
-00000820: 762e 6874 6d6c 0d0a 5b68 7975 676f 6769  v.html..[hyugogi
-00000830: 7275 6261 746f 5d3a 2068 7474 7073 3a2f  rubato]: https:/
-00000840: 2f67 6974 6875 622e 636f 6d2f 6879 7567  /github.com/hyug
-00000850: 6f67 6972 7562 6174 6f2f 7079 496d 6167  ogirubato/pyImag
-00000860: 696e 650d 0a0d 0a23 2323 2046 726f 6d20  ine....### From 
-00000870: 536f 7572 6365 2043 6f64 650d 0a0d 0a54  Source Code....T
-00000880: 6865 2066 6f6c 6c6f 7769 6e67 2073 7465  he following ste
-00000890: 7073 2061 7265 2069 6e73 7472 7563 7469  ps are instructi
-000008a0: 6f6e 7320 6f6e 2064 6f77 6e6c 6f61 642c  ons on download,
-000008b0: 2070 7265 7061 7269 6e67 2c20 616e 6420   preparing, and 
-000008c0: 7275 6e6e 696e 6720 7468 6520 636f 6465  running the code
-000008d0: 2075 6e64 6572 2061 2056 656e 7620 656e   under a Venv en
-000008e0: 7669 726f 6e6d 656e 742e 0d0a 596f 7520  vironment...You 
-000008f0: 6361 6e20 736b 6970 2073 7465 7073 2033  can skip steps 3
-00000900: 2d35 2077 6974 6820 6120 7369 6d70 6c65  -5 with a simple
-00000910: 2060 7079 7468 6f6e 2073 6574 7570 2e70   `python setup.p
-00000920: 7920 696e 7374 616c 6c60 2063 616c 6c20  y install` call 
-00000930: 696e 7374 6561 642c 2062 7574 2079 6f75  instead, but you
-00000940: 206d 6973 7320 6f75 7420 6f6e 2061 2077   miss out on a w
-00000950: 6964 6520 6172 7261 7920 6f66 2062 656e  ide array of ben
-00000960: 6566 6974 732e 0d0a 0d0a 312e 2060 6769  efits.....1. `gi
-00000970: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
-00000980: 6769 7468 7562 2e63 6f6d 2f49 7473 4345  github.com/ItsCE
-00000990: 4544 2f49 6d61 6769 6e65 7079 600d 0a32  ED/Imaginepy`..2
-000009a0: 2e20 6063 6420 496d 6167 696e 6570 7960  . `cd Imaginepy`
-000009b0: 0d0a 332e 2060 7079 7468 6f6e 202d 6d20  ..3. `python -m 
-000009c0: 7665 6e76 2065 6e76 600d 0a34 2e20 6073  venv env`..4. `s
-000009d0: 6f75 7263 6520 656e 762f 6269 6e2f 6163  ource env/bin/ac
-000009e0: 7469 7661 7465 600d 0a35 2e20 6070 7974  tivate`..5. `pyt
-000009f0: 686f 6e20 7365 7475 702e 7079 2069 6e73  hon setup.py ins
-00000a00: 7461 6c6c 600d 0a0d 0a41 7320 7365 656e  tall`....As seen
-00000a10: 2069 6e20 5374 6570 2035 2c20 7275 6e6e   in Step 5, runn
-00000a20: 696e 6720 7468 6520 6069 6d61 6769 6e65  ing the `imagine
-00000a30: 7079 6020 6578 6563 7574 6162 6c65 2069  py` executable i
-00000a40: 7320 736f 6d65 7768 6174 2064 6966 6665  s somewhat diffe
-00000a50: 7265 6e74 2074 6f20 6120 6e6f 726d 616c  rent to a normal
-00000a60: 2050 4950 2069 6e73 7461 6c6c 6174 696f   PIP installatio
-00000a70: 6e2e 0d0a 5365 6520 5b56 656e 7627 7320  n...See [Venv's 
-00000a80: 446f 6373 5d20 6f6e 2076 6172 696f 7573  Docs] on various
-00000a90: 2077 6179 7320 6f66 206d 616b 696e 6720   ways of making 
-00000aa0: 6361 6c6c 7320 756e 6465 7220 7468 6520  calls under the 
-00000ab0: 7669 7274 7561 6c2d 656e 7669 726f 6e6d  virtual-environm
-00000ac0: 656e 742e 0d0a 0d0a 5b50 7974 686f 6e5d  ent.....[Python]
-00000ad0: 3a20 6874 7470 733a 2f2f 7079 7468 6f6e  : https://python
-00000ae0: 2e6f 7267 0d0a 5b56 656e 7627 735d 3a20  .org..[Venv's]: 
-00000af0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00000b00: 686f 6e2e 6f72 672f 332f 7475 746f 7269  hon.org/3/tutori
-00000b10: 616c 2f76 656e 762e 6874 6d6c 0d0a 5b56  al/venv.html..[V
-00000b20: 656e 7627 7320 446f 6373 5d3a 2068 7474  env's Docs]: htt
-00000b30: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00000b40: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f76  .org/3/library/v
-00000b50: 656e 762e 6874 6d6c 0d0a 5b68 7975 676f  env.html..[hyugo
-00000b60: 6769 7275 6261 746f 5d3a 2068 7474 7073  girubato]: https
-00000b70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6879  ://github.com/hy
-00000b80: 7567 6f67 6972 7562 6174 6f2f 7079 496d  ugogirubato/pyIm
-00000b90: 6167 696e 650d 0a0d 0a23 2320 5573 6167  agine....## Usag
-00000ba0: 650d 0a0d 0a54 6865 2066 6f6c 6c6f 7769  e....The followi
-00000bb0: 6e67 2069 7320 6120 6d69 6e69 6d61 6c20  ng is a minimal 
-00000bc0: 6578 616d 706c 6520 6f66 2075 7369 6e67  example of using
-00000bd0: 2049 6d61 6769 6e65 5079 2069 6e20 6120   ImaginePy in a 
-00000be0: 7363 7269 7074 2e20 4974 2067 6574 7320  script. It gets 
-00000bf0: 7468 6520 6765 6e65 7261 7465 6420 696d  the generated im
-00000c00: 6167 650d 0a66 726f 6d20 7468 6520 7465  age..from the te
-00000c10: 7874 2061 6e64 2069 6e63 7265 6173 6573  xt and increases
-00000c20: 2074 6865 2071 7561 6c69 7479 2e0d 0a0d   the quality....
-00000c30: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00000c40: 2069 6d61 6769 6e65 7079 2069 6d70 6f72   imaginepy impor
-00000c50: 7420 496d 6167 696e 652c 2053 7479 6c65  t Imagine, Style
-00000c60: 2c20 5261 7469 6f0d 0a0d 0a64 6566 206d  , Ratio....def m
-00000c70: 6169 6e28 293a 0d0a 2020 2020 696d 6167  ain():..    imag
-00000c80: 696e 6520 3d20 496d 6167 696e 6528 290d  ine = Imagine().
-00000c90: 0a0d 0a20 2020 2069 6d67 5f64 6174 6120  ...    img_data 
-00000ca0: 3d20 696d 6167 696e 652e 7364 7072 656d  = imagine.sdprem
-00000cb0: 280d 0a20 2020 2020 2020 2070 726f 6d70  (..        promp
-00000cc0: 743d 2257 6f6d 616e 2073 6974 7469 6e67  t="Woman sitting
-00000cd0: 206f 6e20 6120 7461 626c 652c 206c 6f6f   on a table, loo
-00000ce0: 6b69 6e67 2061 7420 7468 6520 736b 792c  king at the sky,
-00000cf0: 2073 6565 6e20 6672 6f6d 2062 6568 696e   seen from behin
-00000d00: 6422 2c0d 0a20 2020 2020 2020 2073 7479  d",..        sty
-00000d10: 6c65 3d53 7479 6c65 2e41 4e49 4d45 5f56  le=Style.ANIME_V
-00000d20: 322c 0d0a 2020 2020 2020 2020 7261 7469  2,..        rati
-00000d30: 6f3d 5261 7469 6f2e 5241 5449 4f5f 3136  o=Ratio.RATIO_16
-00000d40: 5839 0d0a 2020 2020 290d 0a0d 0a20 2020  X9..    )....   
-00000d50: 2069 6620 696d 675f 6461 7461 2069 7320   if img_data is 
-00000d60: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2070  None:..        p
-00000d70: 7269 6e74 2822 416e 2065 7272 6f72 206f  rint("An error o
-00000d80: 6363 7572 7265 6420 7768 696c 6520 6765  ccurred while ge
-00000d90: 6e65 7261 7469 6e67 2074 6865 2069 6d61  nerating the ima
-00000da0: 6765 2e22 290d 0a20 2020 2020 2020 2072  ge.")..        r
-00000db0: 6574 7572 6e0d 0a0d 0a20 2020 2069 6d67  eturn....    img
-00000dc0: 5f64 6174 6120 3d20 696d 6167 696e 652e  _data = imagine.
-00000dd0: 7570 7363 616c 6528 696d 6167 653d 696d  upscale(image=im
-00000de0: 675f 6461 7461 290d 0a0d 0a20 2020 2069  g_data)....    i
-00000df0: 6620 696d 675f 6461 7461 2069 7320 4e6f  f img_data is No
-00000e00: 6e65 3a0d 0a20 2020 2020 2020 2070 7269  ne:..        pri
-00000e10: 6e74 2822 416e 2065 7272 6f72 206f 6363  nt("An error occ
-00000e20: 7572 7265 6420 7768 696c 6520 7570 7363  urred while upsc
-00000e30: 616c 696e 6720 7468 6520 696d 6167 652e  aling the image.
-00000e40: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00000e50: 726e 0d0a 0d0a 2020 2020 7472 793a 0d0a  rn....    try:..
-00000e60: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00000e70: 6e28 2265 7861 6d70 6c65 2e6a 7065 6722  n("example.jpeg"
-00000e80: 2c20 6d6f 6465 3d22 7762 2229 2061 7320  , mode="wb") as 
-00000e90: 696d 675f 6669 6c65 3a0d 0a20 2020 2020  img_file:..     
-00000ea0: 2020 2020 2020 2069 6d67 5f66 696c 652e         img_file.
-00000eb0: 7772 6974 6528 696d 675f 6461 7461 290d  write(img_data).
-00000ec0: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00000ed0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00000ee0: 2020 2020 2070 7269 6e74 2866 2241 6e20       print(f"An 
-00000ef0: 6572 726f 7220 6f63 6375 7272 6564 2077  error occurred w
-00000f00: 6869 6c65 2077 7269 7469 6e67 2074 6865  hile writing the
-00000f10: 2069 6d61 6765 2074 6f20 6669 6c65 3a20   image to file: 
-00000f20: 7b65 7d22 290d 0a0d 0a69 6620 5f5f 6e61  {e}")....if __na
-00000f30: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
-00000f40: 5f22 3a0d 0a20 2020 206d 6169 6e28 290d  _":..    main().
-00000f50: 0a60 6060 0d0a 0d0a 4173 796e 6320 7665  .```....Async ve
-00000f60: 7273 696f 6e0d 0a0d 0a60 6060 7079 7468  rsion....```pyth
-00000f70: 6f6e 0d0a 696d 706f 7274 2061 7379 6e63  on..import async
-00000f80: 696f 0d0a 6672 6f6d 2069 6d61 6769 6e65  io..from imagine
-00000f90: 7079 2069 6d70 6f72 7420 4173 796e 6349  py import AsyncI
-00000fa0: 6d61 6769 6e65 2c20 5374 796c 652c 2052  magine, Style, R
-00000fb0: 6174 696f 0d0a 0d0a 0d0a 6173 796e 6320  atio......async 
-00000fc0: 6465 6620 6d61 696e 2829 3a0d 0a20 2020  def main():..   
-00000fd0: 2069 6d61 6769 6e65 203d 2041 7379 6e63   imagine = Async
-00000fe0: 496d 6167 696e 6528 290d 0a0d 0a20 2020  Imagine()....   
-00000ff0: 2069 6d67 5f64 6174 6120 3d20 6177 6169   img_data = awai
-00001000: 7420 696d 6167 696e 652e 7364 7072 656d  t imagine.sdprem
-00001010: 280d 0a20 2020 2020 2020 2070 726f 6d70  (..        promp
-00001020: 743d 2257 6f6d 616e 2073 6974 7469 6e67  t="Woman sitting
-00001030: 206f 6e20 6120 7461 626c 652c 206c 6f6f   on a table, loo
-00001040: 6b69 6e67 2061 7420 7468 6520 736b 792c  king at the sky,
-00001050: 2073 6565 6e20 6672 6f6d 2062 6568 696e   seen from behin
-00001060: 6422 2c0d 0a20 2020 2020 2020 2073 7479  d",..        sty
-00001070: 6c65 3d53 7479 6c65 2e41 4e49 4d45 5f56  le=Style.ANIME_V
-00001080: 322c 0d0a 2020 2020 2020 2020 7261 7469  2,..        rati
-00001090: 6f3d 5261 7469 6f2e 5241 5449 4f5f 3136  o=Ratio.RATIO_16
-000010a0: 5839 0d0a 2020 2020 290d 0a0d 0a20 2020  X9..    )....   
-000010b0: 2069 6620 696d 675f 6461 7461 2069 7320   if img_data is 
-000010c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2070  None:..        p
-000010d0: 7269 6e74 2822 416e 2065 7272 6f72 206f  rint("An error o
-000010e0: 6363 7572 7265 6420 7768 696c 6520 6765  ccurred while ge
-000010f0: 6e65 7261 7469 6e67 2074 6865 2069 6d61  nerating the ima
-00001100: 6765 2e22 290d 0a20 2020 2020 2020 2072  ge.")..        r
-00001110: 6574 7572 6e0d 0a0d 0a20 2020 2069 6d67  eturn....    img
-00001120: 5f64 6174 6120 3d20 6177 6169 7420 696d  _data = await im
-00001130: 6167 696e 652e 7570 7363 616c 6528 696d  agine.upscale(im
-00001140: 6167 653d 696d 675f 6461 7461 290d 0a0d  age=img_data)...
-00001150: 0a20 2020 2069 6620 696d 675f 6461 7461  .    if img_data
-00001160: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00001170: 2020 2070 7269 6e74 2822 416e 2065 7272     print("An err
-00001180: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
-00001190: 6520 7570 7363 616c 696e 6720 7468 6520  e upscaling the 
-000011a0: 696d 6167 652e 2229 0d0a 2020 2020 2020  image.")..      
-000011b0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-000011c0: 6177 6169 7420 696d 6167 696e 652e 636c  await imagine.cl
-000011d0: 6f73 6528 290d 0a20 2020 2074 7279 3a0d  ose()..    try:.
-000011e0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-000011f0: 656e 2822 6578 616d 706c 652e 706e 6722  en("example.png"
-00001200: 2c20 6d6f 6465 3d22 7762 2229 2061 7320  , mode="wb") as 
-00001210: 696d 675f 6669 6c65 3a0d 0a20 2020 2020  img_file:..     
-00001220: 2020 2020 2020 2069 6d67 5f66 696c 652e         img_file.
-00001230: 7772 6974 6528 696d 675f 6461 7461 290d  write(img_data).
-00001240: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00001250: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00001260: 2020 2020 2070 7269 6e74 2866 2241 6e20       print(f"An 
-00001270: 6572 726f 7220 6f63 6375 7272 6564 2077  error occurred w
-00001280: 6869 6c65 2077 7269 7469 6e67 2074 6865  hile writing the
-00001290: 2069 6d61 6765 2074 6f20 6669 6c65 3a20   image to file: 
-000012a0: 7b65 7d22 290d 0a0d 0a0d 0a69 6620 5f5f  {e}")......if __
-000012b0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
-000012c0: 6e5f 5f22 3a0d 0a20 2020 2061 7379 6e63  n__":..    async
-000012d0: 696f 2e72 756e 286d 6169 6e28 2929 0d0a  io.run(main())..
-000012e0: 6060 600d 0a0d 0a23 2320 4372 6564 6974  ```....## Credit
-000012f0: 0d0a 0d0a 2d20 496d 6167 696e 6520 4963  ....- Imagine Ic
-00001300: 6f6e 2026 636f 7079 3b20 5679 726f 2041  on &copy; Vyro A
-00001310: 4920 2620 4150 490d 0a2d 204f 7269 6769  I & API..- Origi
-00001320: 6e61 6c20 7265 7665 7273 6520 616e 6420  nal reverse and 
-00001330: 7665 7273 696f 6e20 6279 3a20 5b68 7975  version by: [hyu
-00001340: 676f 6769 7275 6261 746f 5d0d 0a0d 0a23  gogirubato]....#
-00001350: 2320 4c69 6365 6e73 650d 0a0d 0a5b 474e  # License....[GN
-00001360: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00001370: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
-00001380: 6e20 332e 305d 284c 4943 454e 5345 290d  n 3.0](LICENSE).
-00001390: 0a                                       .
+000000b0: 6169 6c3a 200d 0a4c 6963 656e 7365 3a20  ail: ..License: 
+000000c0: 4750 4c2d 332e 302d 6f6e 6c79 0d0a 4b65  GPL-3.0-only..Ke
+000000d0: 7977 6f72 6473 3a20 6172 742c 696d 6167  ywords: art,imag
+000000e0: 652c 6169 2c73 7461 626c 652d 6469 6666  e,ai,stable-diff
+000000f0: 7573 696f 6e0d 0a43 6c61 7373 6966 6965  usion..Classifie
+00000100: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000110: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00000120: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
+00000130: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000140: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000150: 2044 6576 656c 6f70 6572 730d 0a43 6c61   Developers..Cla
+00000160: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000170: 6420 4175 6469 656e 6365 203a 3a20 456e  d Audience :: En
+00000180: 6420 5573 6572 732f 4465 736b 746f 700d  d Users/Desktop.
+00000190: 0a43 6c61 7373 6966 6965 723a 204e 6174  .Classifier: Nat
+000001a0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+000001b0: 2045 6e67 6c69 7368 0d0a 436c 6173 7369   English..Classi
+000001c0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+000001d0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001e0: 6570 656e 6465 6e74 0d0a 436c 6173 7369  ependent..Classi
+000001f0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000210: 7468 6f6e 203a 3a20 330d 0a43 6c61 7373  thon :: 3..Class
+00000220: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000240: 7974 686f 6e20 3a3a 2033 2e37 0d0a 436c  ython :: 3.7..Cl
+00000250: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000260: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000270: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+00000280: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000290: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002b0: 2e39 0d0a 436c 6173 7369 6669 6572 3a20  .9..Classifier: 
+000002c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002e0: 3a20 332e 3130 0d0a 436c 6173 7369 6669  : 3.10..Classifi
+000002f0: 6572 3a20 546f 7069 6320 3a3a 2055 7469  er: Topic :: Uti
+00000300: 6c69 7469 6573 0d0a 5265 7175 6972 6573  lities..Requires
+00000310: 2d50 7974 686f 6e3a 203e 3d33 2e37 0d0a  -Python: >=3.7..
+00000320: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000330: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000340: 6172 6b64 6f77 6e0d 0a4c 6963 656e 7365  arkdown..License
+00000350: 2d46 696c 653a 204c 4943 454e 5345 0d0a  -File: LICENSE..
+00000360: 0d0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000370: 6e74 6572 223e 0d0a 3c62 3e3e 5079 5069  nter">..<b>>PyPi
+00000380: 2049 5320 4e4f 5420 5550 4441 5445 2120   IS NOT UPDATE! 
+00000390: 504c 4541 5345 2049 4e53 5441 4c4c 2046  PLEASE INSTALL F
+000003a0: 524f 4d20 5448 4520 5245 504f 213c 2f62  ROM THE REPO!</b
+000003b0: 3e0d 0a3c 6272 3e0d 0a20 200d 0a3c 696d  >..<br>..  ..<im
+000003c0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+000003d0: 6974 6875 622e 636f 6d2f 4974 7343 4545  ithub.com/ItsCEE
+000003e0: 442f 496d 6167 696e 6550 792d 4d69 646a  D/ImaginePy-Midj
+000003f0: 6f75 726e 6579 2d46 7265 652d 416c 7465  ourney-Free-Alte
+00000400: 726e 6174 6976 652f 626c 6f62 2f6d 6169  rnative/blob/mai
+00000410: 6e2f 646f 6373 2f69 6d61 6769 6e65 5f6c  n/docs/imagine_l
+00000420: 6f67 6f2e 6769 6622 2077 6964 7468 3d22  ogo.gif" width="
+00000430: 3130 2522 3e0d 0a0d 0a2a 2a49 6d61 6769  10%">....**Imagi
+00000440: 6e65 5079 2a2a 0d0a 3c62 723e 0d0a 3c61  nePy**..<br>..<a
+00000450: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000460: 6973 636f 7264 2e67 672f 6178 666b 6a71  iscord.gg/axfkjq
+00000470: 5752 3545 2220 7461 7267 6574 3d22 5f62  WR5E" target="_b
+00000480: 6c61 6e6b 223e 0d0a 2020 3c69 6d67 2073  lank">..  <img s
+00000490: 7263 3d22 6874 7470 733a 2f2f 6469 7363  rc="https://disc
+000004a0: 6f72 6461 7070 2e63 6f6d 2f61 7069 2f67  ordapp.com/api/g
+000004b0: 7569 6c64 732f 3131 3130 3331 3439 3731  uilds/1110314971
+000004c0: 3031 3238 3038 3737 342f 7769 6467 6574  012808774/widget
+000004d0: 2e70 6e67 3f73 7479 6c65 3d62 616e 6e65  .png?style=banne
+000004e0: 7234 2220 616c 743d 2244 6973 636f 7264  r4" alt="Discord
+000004f0: 2042 616e 6e65 7220 3422 3e0d 0a3c 2f61   Banner 4">..</a
+00000500: 3e0d 0a3c 6272 3e0d 0a3c 696d 6720 7372  >..<br>..<img sr
+00000510: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000520: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000530: 7079 7468 6f6e 2d33 2e37 2b2d 696e 666f  python-3.7+-info
+00000540: 726d 6174 696f 6e61 6c3f 7374 796c 653d  rmational?style=
+00000550: 706c 6173 7469 6322 2061 6c74 3d22 5079  plastic" alt="Py
+00000560: 7468 6f6e 2076 6572 7369 6f6e 223e 0d0a  thon version">..
+00000570: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000580: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000590: 2f67 6974 6875 622f 7265 6c65 6173 652d  /github/release-
+000005a0: 6461 7465 2f49 7473 4345 4544 2f49 6d61  date/ItsCEED/Ima
+000005b0: 6769 6e65 5079 2d4d 6964 6a6f 7572 6e65  ginePy-Midjourne
+000005c0: 792d 4672 6565 2d41 6c74 6572 6e61 7469  y-Free-Alternati
+000005d0: 7665 3f73 7479 6c65 3d70 6c61 7374 6963  ve?style=plastic
+000005e0: 2220 616c 743d 2252 656c 6561 7365 223e  " alt="Release">
+000005f0: 0d0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+00000600: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000610: 696f 2f67 6974 6875 622f 7265 6c65 6173  io/github/releas
+00000620: 652f 4974 7343 4545 442f 496d 6167 696e  e/ItsCEED/Imagin
+00000630: 6550 792d 4d69 646a 6f75 726e 6579 2d46  ePy-Midjourney-F
+00000640: 7265 652d 416c 7465 726e 6174 6976 653f  ree-Alternative?
+00000650: 7374 796c 653d 706c 6173 7469 6322 2061  style=plastic" a
+00000660: 6c74 3d22 5665 7273 696f 6e22 3e0d 0a0d  lt="Version">...
+00000670: 0a3c 2f64 6976 3e0d 0a0d 0a23 2320 4665  .</div>....## Fe
+00000680: 6174 7572 6573 0d0a 0d0a 2d20 f09f 8ea8  atures....- ....
+00000690: 2054 7572 6e20 776f 7264 7320 696e 746f   Turn words into
+000006a0: 2061 7274 0d0a 2d20 f09f 9193 2043 686f   art..- .... Cho
+000006b0: 6f73 6520 6672 6f6d 2061 6e20 6172 7261  ose from an arra
+000006c0: 7920 6f66 2061 7274 2073 7479 6c65 730d  y of art styles.
+000006d0: 0a2d 20f0 9f94 a720 4164 6a75 7374 2079  .- .... Adjust y
+000006e0: 6f75 7220 6d61 7374 6572 7069 6563 6520  our masterpiece 
+000006f0: 7769 7468 2063 7265 6174 6976 6520 636f  with creative co
+00000700: 6e74 726f 6c73 210d 0a2d 20f0 9f93 a620  ntrols!..- .... 
+00000710: 5374 6179 2061 6865 6164 206f 6620 7468  Stay ahead of th
+00000720: 6520 6761 6d65 2077 6974 6820 7468 6520  e game with the 
+00000730: 6576 6572 2d67 726f 7769 6e67 2061 7274  ever-growing art
+00000740: 206c 6962 7261 7279 210d 0a2d 20f0 9f8c   library!..- ...
+00000750: 8720 4765 6e65 7261 7465 2077 616c 6c70  . Generate wallp
+00000760: 6170 6572 730d 0a2d 20f0 9f94 8e20 4469  apers..- .... Di
+00000770: 7363 6f76 6572 2061 6e64 2065 7870 6c6f  scover and explo
+00000780: 7265 2073 696d 696c 6172 2061 7274 6973  re similar artis
+00000790: 7469 6320 6465 7369 676e 730d 0a2d 2054  tic designs..- T
+000007a0: 6869 7320 6973 2072 6566 6163 746f 7265  his is refactore
+000007b0: 6420 616e 6420 696d 7072 6f76 6564 2076  d and improved v
+000007c0: 6572 7369 6f6e 206f 6620 7468 6520 6f72  ersion of the or
+000007d0: 6967 696e 616c 2066 726f 6d20 5b68 7975  iginal from [hyu
+000007e0: 676f 6769 7275 6261 746f 5d0d 0a0d 0a23  gogirubato]....#
+000007f0: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
+00000800: 0d0a 5f4e 6f74 653a 2052 6571 7569 7265  .._Note: Require
+00000810: 7320 5b50 7974 686f 6e5d 2033 2e37 2e30  s [Python] 3.7.0
+00000820: 206f 7220 6e65 7765 7220 7769 7468 2050   or newer with P
+00000830: 4950 2069 6e73 7461 6c6c 6564 2e5f 0d0a  IP installed._..
+00000840: 0d0a 6060 6073 6865 6c6c 0d0a 2420 7079  ..```shell..$ py
+00000850: 7468 6f6e 2073 6574 7570 2e70 7920 696e  thon setup.py in
+00000860: 7374 616c 6c0d 0a60 6060 0d0a 0d0a 596f  stall..```....Yo
+00000870: 7520 6e6f 7720 6861 7665 2074 6865 2060  u now have the `
+00000880: 696d 6167 696e 6570 7960 2070 6163 6b61  imaginepy` packa
+00000890: 6765 2069 6e73 7461 6c6c 6564 2e0d 0a0d  ge installed....
+000008a0: 0a23 2323 2050 7950 6920 496e 7374 616c  .### PyPi Instal
+000008b0: 6c61 7469 6f6e 0d0a 0d0a 6060 600d 0a70  lation....```..p
+000008c0: 6970 2069 6e73 7461 6c6c 2069 6d61 6769  ip install imagi
+000008d0: 6e65 7079 0d0a 6060 600d 0a0d 0a5b 5079  nepy..```....[Py
+000008e0: 7468 6f6e 5d3a 2068 7474 7073 3a2f 2f70  thon]: https://p
+000008f0: 7974 686f 6e2e 6f72 670d 0a5b 5665 6e76  ython.org..[Venv
+00000900: 2773 5d3a 2068 7474 7073 3a2f 2f64 6f63  's]: https://doc
+00000910: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f74  s.python.org/3/t
+00000920: 7574 6f72 6961 6c2f 7665 6e76 2e68 746d  utorial/venv.htm
+00000930: 6c0d 0a5b 5665 6e76 2773 2044 6f63 735d  l..[Venv's Docs]
+00000940: 3a20 6874 7470 733a 2f2f 646f 6373 2e70  : https://docs.p
+00000950: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+00000960: 6172 792f 7665 6e76 2e68 746d 6c0d 0a5b  ary/venv.html..[
+00000970: 6879 7567 6f67 6972 7562 6174 6f5d 3a20  hyugogirubato]: 
+00000980: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000990: 6f6d 2f68 7975 676f 6769 7275 6261 746f  om/hyugogirubato
+000009a0: 2f70 7949 6d61 6769 6e65 0d0a 0d0a 2323  /pyImagine....##
+000009b0: 2320 4672 6f6d 2053 6f75 7263 6520 436f  # From Source Co
+000009c0: 6465 0d0a 0d0a 5468 6520 666f 6c6c 6f77  de....The follow
+000009d0: 696e 6720 7374 6570 7320 6172 6520 696e  ing steps are in
+000009e0: 7374 7275 6374 696f 6e73 206f 6e20 646f  structions on do
+000009f0: 776e 6c6f 6164 2c20 7072 6570 6172 696e  wnload, preparin
+00000a00: 672c 2061 6e64 2072 756e 6e69 6e67 2074  g, and running t
+00000a10: 6865 2063 6f64 6520 756e 6465 7220 6120  he code under a 
+00000a20: 5665 6e76 2065 6e76 6972 6f6e 6d65 6e74  Venv environment
+00000a30: 2e0d 0a59 6f75 2063 616e 2073 6b69 7020  ...You can skip 
+00000a40: 7374 6570 7320 332d 3520 7769 7468 2061  steps 3-5 with a
+00000a50: 2073 696d 706c 6520 6070 7974 686f 6e20   simple `python 
+00000a60: 7365 7475 702e 7079 2069 6e73 7461 6c6c  setup.py install
+00000a70: 6020 6361 6c6c 2069 6e73 7465 6164 2c20  ` call instead, 
+00000a80: 6275 7420 796f 7520 6d69 7373 206f 7574  but you miss out
+00000a90: 206f 6e20 6120 7769 6465 2061 7272 6179   on a wide array
+00000aa0: 206f 6620 6265 6e65 6669 7473 2e0d 0a0d   of benefits....
+00000ab0: 0a31 2e20 6067 6974 2063 6c6f 6e65 2068  .1. `git clone h
+00000ac0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ad0: 6d2f 4974 7343 4545 442f 496d 6167 696e  m/ItsCEED/Imagin
+00000ae0: 6570 7960 0d0a 322e 2060 6364 2049 6d61  epy`..2. `cd Ima
+00000af0: 6769 6e65 7079 600d 0a33 2e20 6070 7974  ginepy`..3. `pyt
+00000b00: 686f 6e20 2d6d 2076 656e 7620 656e 7660  hon -m venv env`
+00000b10: 0d0a 342e 2060 736f 7572 6365 2065 6e76  ..4. `source env
+00000b20: 2f62 696e 2f61 6374 6976 6174 6560 0d0a  /bin/activate`..
+00000b30: 352e 2060 7079 7468 6f6e 2073 6574 7570  5. `python setup
+00000b40: 2e70 7920 696e 7374 616c 6c60 0d0a 0d0a  .py install`....
+00000b50: 4173 2073 6565 6e20 696e 2053 7465 7020  As seen in Step 
+00000b60: 352c 2072 756e 6e69 6e67 2074 6865 2060  5, running the `
+00000b70: 696d 6167 696e 6570 7960 2065 7865 6375  imaginepy` execu
+00000b80: 7461 626c 6520 6973 2073 6f6d 6577 6861  table is somewha
+00000b90: 7420 6469 6666 6572 656e 7420 746f 2061  t different to a
+00000ba0: 206e 6f72 6d61 6c20 5049 5020 696e 7374   normal PIP inst
+00000bb0: 616c 6c61 7469 6f6e 2e0d 0a53 6565 205b  allation...See [
+00000bc0: 5665 6e76 2773 2044 6f63 735d 206f 6e20  Venv's Docs] on 
+00000bd0: 7661 7269 6f75 7320 7761 7973 206f 6620  various ways of 
+00000be0: 6d61 6b69 6e67 2063 616c 6c73 2075 6e64  making calls und
+00000bf0: 6572 2074 6865 2076 6972 7475 616c 2d65  er the virtual-e
+00000c00: 6e76 6972 6f6e 6d65 6e74 2e0d 0a0d 0a5b  nvironment.....[
+00000c10: 5079 7468 6f6e 5d3a 2068 7474 7073 3a2f  Python]: https:/
+00000c20: 2f70 7974 686f 6e2e 6f72 670d 0a5b 5665  /python.org..[Ve
+00000c30: 6e76 2773 5d3a 2068 7474 7073 3a2f 2f64  nv's]: https://d
+00000c40: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00000c50: 2f74 7574 6f72 6961 6c2f 7665 6e76 2e68  /tutorial/venv.h
+00000c60: 746d 6c0d 0a5b 5665 6e76 2773 2044 6f63  tml..[Venv's Doc
+00000c70: 735d 3a20 6874 7470 733a 2f2f 646f 6373  s]: https://docs
+00000c80: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00000c90: 6272 6172 792f 7665 6e76 2e68 746d 6c0d  brary/venv.html.
+00000ca0: 0a5b 6879 7567 6f67 6972 7562 6174 6f5d  .[hyugogirubato]
+00000cb0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000cc0: 2e63 6f6d 2f68 7975 676f 6769 7275 6261  .com/hyugogiruba
+00000cd0: 746f 2f70 7949 6d61 6769 6e65 0d0a 0d0a  to/pyImagine....
+00000ce0: 2323 2055 7361 6765 0d0a 0d0a 5468 6520  ## Usage....The 
+00000cf0: 666f 6c6c 6f77 696e 6720 6973 2061 206d  following is a m
+00000d00: 696e 696d 616c 2065 7861 6d70 6c65 206f  inimal example o
+00000d10: 6620 7573 696e 6720 496d 6167 696e 6550  f using ImagineP
+00000d20: 7920 696e 2061 2073 6372 6970 742e 2049  y in a script. I
+00000d30: 7420 6765 7473 2074 6865 2067 656e 6572  t gets the gener
+00000d40: 6174 6564 2069 6d61 6765 0d0a 6672 6f6d  ated image..from
+00000d50: 2074 6865 2074 6578 7420 616e 6420 696e   the text and in
+00000d60: 6372 6561 7365 7320 7468 6520 7175 616c  creases the qual
+00000d70: 6974 792e 0d0a 0d0a 6060 6070 7974 686f  ity.....```pytho
+00000d80: 6e0d 0a66 726f 6d20 696d 6167 696e 6570  n..from imaginep
+00000d90: 7920 696d 706f 7274 2049 6d61 6769 6e65  y import Imagine
+00000da0: 2c20 5374 796c 652c 2052 6174 696f 0d0a  , Style, Ratio..
+00000db0: 0d0a 6465 6620 6d61 696e 2829 3a0d 0a20  ..def main():.. 
+00000dc0: 2020 2069 6d61 6769 6e65 203d 2049 6d61     imagine = Ima
+00000dd0: 6769 6e65 2873 7479 6c65 3d53 7479 6c65  gine(style=Style
+00000de0: 2e41 4e49 4d45 5f56 3229 0d0a 0d0a 2020  .ANIME_V2)....  
+00000df0: 2020 696d 675f 6461 7461 203d 2069 6d61    img_data = ima
+00000e00: 6769 6e65 2e73 6470 7265 6d28 0d0a 2020  gine.sdprem(..  
+00000e10: 2020 2020 2020 7072 6f6d 7074 3d22 576f        prompt="Wo
+00000e20: 6d61 6e20 7369 7474 696e 6720 6f6e 2061  man sitting on a
+00000e30: 2074 6162 6c65 2c20 6c6f 6f6b 696e 6720   table, looking 
+00000e40: 6174 2074 6865 2073 6b79 2c20 7365 656e  at the sky, seen
+00000e50: 2066 726f 6d20 6265 6869 6e64 222c 0d0a   from behind",..
+00000e60: 2020 2020 2020 2020 7374 796c 653d 5374          style=St
+00000e70: 796c 652e 414e 494d 455f 5632 2c0d 0a20  yle.ANIME_V2,.. 
+00000e80: 2020 2020 2020 2072 6174 696f 3d52 6174         ratio=Rat
+00000e90: 696f 2e52 4154 494f 5f31 3658 390d 0a20  io.RATIO_16X9.. 
+00000ea0: 2020 2029 0d0a 0d0a 2020 2020 6966 2069     )....    if i
+00000eb0: 6d67 5f64 6174 6120 6973 204e 6f6e 653a  mg_data is None:
+00000ec0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00000ed0: 2241 6e20 6572 726f 7220 6f63 6375 7272  "An error occurr
+00000ee0: 6564 2077 6869 6c65 2067 656e 6572 6174  ed while generat
+00000ef0: 696e 6720 7468 6520 696d 6167 652e 2229  ing the image.")
+00000f00: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000f10: 0d0a 0d0a 2020 2020 696d 675f 6461 7461  ....    img_data
+00000f20: 203d 2069 6d61 6769 6e65 2e75 7073 6361   = imagine.upsca
+00000f30: 6c65 2869 6d61 6765 3d69 6d67 5f64 6174  le(image=img_dat
+00000f40: 6129 0d0a 0d0a 2020 2020 6966 2069 6d67  a)....    if img
+00000f50: 5f64 6174 6120 6973 204e 6f6e 653a 0d0a  _data is None:..
+00000f60: 2020 2020 2020 2020 7072 696e 7428 2241          print("A
+00000f70: 6e20 6572 726f 7220 6f63 6375 7272 6564  n error occurred
+00000f80: 2077 6869 6c65 2075 7073 6361 6c69 6e67   while upscaling
+00000f90: 2074 6865 2069 6d61 6765 2e22 290d 0a20   the image.").. 
+00000fa0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00000fb0: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
+00000fc0: 2020 2077 6974 6820 6f70 656e 2822 6578     with open("ex
+00000fd0: 616d 706c 652e 6a70 6567 222c 206d 6f64  ample.jpeg", mod
+00000fe0: 653d 2277 6222 2920 6173 2069 6d67 5f66  e="wb") as img_f
+00000ff0: 696c 653a 0d0a 2020 2020 2020 2020 2020  ile:..          
+00001000: 2020 696d 675f 6669 6c65 2e77 7269 7465    img_file.write
+00001010: 2869 6d67 5f64 6174 6129 0d0a 2020 2020  (img_data)..    
+00001020: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00001030: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00001040: 7072 696e 7428 6622 416e 2065 7272 6f72  print(f"An error
+00001050: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
+00001060: 7772 6974 696e 6720 7468 6520 696d 6167  writing the imag
+00001070: 6520 746f 2066 696c 653a 207b 657d 2229  e to file: {e}")
+00001080: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
+00001090: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0d0a  == "__main__":..
+000010a0: 2020 2020 6d61 696e 2829 0d0a 6060 600d      main()..```.
+000010b0: 0a0d 0a41 7379 6e63 2076 6572 7369 6f6e  ...Async version
+000010c0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
+000010d0: 6d70 6f72 7420 6173 796e 6369 6f0d 0a66  mport asyncio..f
+000010e0: 726f 6d20 696d 6167 696e 6570 7920 696d  rom imaginepy im
+000010f0: 706f 7274 2041 7379 6e63 496d 6167 696e  port AsyncImagin
+00001100: 652c 2053 7479 6c65 2c20 5261 7469 6f0d  e, Style, Ratio.
+00001110: 0a0d 0a0d 0a61 7379 6e63 2064 6566 206d  .....async def m
+00001120: 6169 6e28 293a 0d0a 2020 2020 696d 6167  ain():..    imag
+00001130: 696e 6520 3d20 4173 796e 6349 6d61 6769  ine = AsyncImagi
+00001140: 6e65 2873 7479 6c65 3d53 7479 6c65 2e41  ne(style=Style.A
+00001150: 4e49 4d45 5f56 3229 0d0a 0d0a 2020 2020  NIME_V2)....    
+00001160: 696d 675f 6461 7461 203d 2061 7761 6974  img_data = await
+00001170: 2069 6d61 6769 6e65 2e73 6470 7265 6d28   imagine.sdprem(
+00001180: 0d0a 2020 2020 2020 2020 7072 6f6d 7074  ..        prompt
+00001190: 3d22 576f 6d61 6e20 7369 7474 696e 6720  ="Woman sitting 
+000011a0: 6f6e 2061 2074 6162 6c65 2c20 6c6f 6f6b  on a table, look
+000011b0: 696e 6720 6174 2074 6865 2073 6b79 2c20  ing at the sky, 
+000011c0: 7365 656e 2066 726f 6d20 6265 6869 6e64  seen from behind
+000011d0: 222c 0d0a 2020 2020 2020 2020 7374 796c  ",..        styl
+000011e0: 653d 5374 796c 652e 414e 494d 455f 5632  e=Style.ANIME_V2
+000011f0: 2c0d 0a20 2020 2020 2020 2072 6174 696f  ,..        ratio
+00001200: 3d52 6174 696f 2e52 4154 494f 5f31 3658  =Ratio.RATIO_16X
+00001210: 390d 0a20 2020 2029 0d0a 0d0a 2020 2020  9..    )....    
+00001220: 6966 2069 6d67 5f64 6174 6120 6973 204e  if img_data is N
+00001230: 6f6e 653a 0d0a 2020 2020 2020 2020 7072  one:..        pr
+00001240: 696e 7428 2241 6e20 6572 726f 7220 6f63  int("An error oc
+00001250: 6375 7272 6564 2077 6869 6c65 2067 656e  curred while gen
+00001260: 6572 6174 696e 6720 7468 6520 696d 6167  erating the imag
+00001270: 652e 2229 0d0a 2020 2020 2020 2020 7265  e.")..        re
+00001280: 7475 726e 0d0a 0d0a 2020 2020 696d 675f  turn....    img_
+00001290: 6461 7461 203d 2061 7761 6974 2069 6d61  data = await ima
+000012a0: 6769 6e65 2e75 7073 6361 6c65 2869 6d61  gine.upscale(ima
+000012b0: 6765 3d69 6d67 5f64 6174 6129 0d0a 0d0a  ge=img_data)....
+000012c0: 2020 2020 6966 2069 6d67 5f64 6174 6120      if img_data 
+000012d0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+000012e0: 2020 7072 696e 7428 2241 6e20 6572 726f    print("An erro
+000012f0: 7220 6f63 6375 7272 6564 2077 6869 6c65  r occurred while
+00001300: 2075 7073 6361 6c69 6e67 2074 6865 2069   upscaling the i
+00001310: 6d61 6765 2e22 290d 0a20 2020 2020 2020  mage.")..       
+00001320: 2072 6574 7572 6e0d 0a0d 0a20 2020 2061   return....    a
+00001330: 7761 6974 2069 6d61 6769 6e65 2e63 6c6f  wait imagine.clo
+00001340: 7365 2829 0d0a 2020 2020 7472 793a 0d0a  se()..    try:..
+00001350: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00001360: 6e28 2265 7861 6d70 6c65 2e70 6e67 222c  n("example.png",
+00001370: 206d 6f64 653d 2277 6222 2920 6173 2069   mode="wb") as i
+00001380: 6d67 5f66 696c 653a 0d0a 2020 2020 2020  mg_file:..      
+00001390: 2020 2020 2020 696d 675f 6669 6c65 2e77        img_file.w
+000013a0: 7269 7465 2869 6d67 5f64 6174 6129 0d0a  rite(img_data)..
+000013b0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+000013c0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+000013d0: 2020 2020 7072 696e 7428 6622 416e 2065      print(f"An e
+000013e0: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
+000013f0: 696c 6520 7772 6974 696e 6720 7468 6520  ile writing the 
+00001400: 696d 6167 6520 746f 2066 696c 653a 207b  image to file: {
+00001410: 657d 2229 0d0a 0d0a 0d0a 6966 205f 5f6e  e}")......if __n
+00001420: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00001430: 5f5f 223a 0d0a 2020 2020 6173 796e 6369  __":..    asynci
+00001440: 6f2e 7275 6e28 6d61 696e 2829 290d 0a60  o.run(main())..`
+00001450: 6060 0d0a 0d0a 2323 2043 7265 6469 740d  ``....## Credit.
+00001460: 0a0d 0a2d 2049 6d61 6769 6e65 2049 636f  ...- Imagine Ico
+00001470: 6e20 2663 6f70 793b 2056 7972 6f20 4149  n &copy; Vyro AI
+00001480: 2026 2041 5049 0d0a 2d20 4f72 6967 696e   & API..- Origin
+00001490: 616c 2072 6576 6572 7365 2061 6e64 2076  al reverse and v
+000014a0: 6572 7369 6f6e 2062 793a 205b 6879 7567  ersion by: [hyug
+000014b0: 6f67 6972 7562 6174 6f5d 0d0a 0d0a 2323  ogirubato]....##
+000014c0: 204c 6963 656e 7365 0d0a 0d0a 5b47 4e55   License....[GNU
+000014d0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000014e0: 4c69 6365 6e73 652c 2056 6572 7369 6f6e  License, Version
+000014f0: 2033 2e30 5d28 4c49 4345 4e53 4529 0d0a   3.0](LICENSE)..
```

