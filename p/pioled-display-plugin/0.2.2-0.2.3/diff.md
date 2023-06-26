# Comparing `tmp/pioled_display_plugin-0.2.2-py3-none-any.whl.zip` & `tmp/pioled_display_plugin-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4964 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5417 b- defN 23-Jun-12 16:01 pioled_display_plugin/__init__.py
+Zip file size: 5303 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5631 b- defN 23-Jun-26 15:35 pioled_display_plugin/__init__.py
 -rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/post_install.sh
 -rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/pre_uninstall.sh
--rw-r--r--  2.0 unx     1052 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      800 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/RECORD
-9 files, 8655 bytes uncompressed, 3468 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1313 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      846 b- defN 23-Jun-26 15:36 pioled_display_plugin-0.2.3.dist-info/RECORD
+9 files, 9383 bytes uncompressed, 3807 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pioled_display_plugin/post_install.sh
 Comment: 
 
 Filename: pioled_display_plugin/pre_uninstall.sh
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/LICENSE.txt
+Filename: pioled_display_plugin-0.2.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/METADATA
+Filename: pioled_display_plugin-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/WHEEL
+Filename: pioled_display_plugin-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/entry_points.txt
+Filename: pioled_display_plugin-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/top_level.txt
+Filename: pioled_display_plugin-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.2.dist-info/RECORD
+Filename: pioled_display_plugin-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioled_display_plugin/__init__.py

```diff
@@ -9,20 +9,25 @@
 from msgspec.json import decode
 from PIL import Image
 from PIL import ImageDraw
 from PIL import ImageFont
 from pioreactor import structs
 from pioreactor import types as pt
 from pioreactor.background_jobs.base import BackgroundJobContrib
+from pioreactor.cli.pio import JOBS_TO_SKIP_KILLING
 from pioreactor.hardware import SCL
 from pioreactor.hardware import SDA
 from pioreactor.utils.networking import get_ip
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import UNIVERSAL_EXPERIMENT
 
+# since this is a long-running job, we don't want it to be killed by pio kill --all-jobs.
+
+JOBS_TO_SKIP_KILLING.append("pioled_display")
+
 
 class PiOLEDDisplay(BackgroundJobContrib):
 
     job_name = "pioled_display"
 
     growth_rate: Optional[float] = None
     od: Optional[float] = None
@@ -33,15 +38,15 @@
 
         # Create the I2C interface.
         i2c = busio.I2C(SCL, SDA)
 
         try:
             self.disp = adafruit_ssd1306.SSD1306_I2C(128, 32, i2c)
         except Exception as e:
-            self.logger.error("Unable to find hardware")
+            self.logger.error("Unable to find PiOLED hardware. Is it attached?")
             self.clean_up()
             raise e
 
         # get ip for displaying
         self._ip = get_ip()
 
         # rotate the screen since we are flipping it
```

## Comparing `pioled_display_plugin-0.2.2.dist-info/LICENSE.txt` & `pioled_display_plugin-0.2.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioled_display_plugin-0.2.2.dist-info/METADATA` & `pioled_display_plugin-0.2.3.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioled-display-plugin
-Version: 0.2.2
+Version: 0.2.3
 Summary: Use an OLED display with your Pioreactor
 Home-page: https://github.com/Pioreactor/PiOLED-display-plugin
 Author: Cameron Davidson-Pilon
 Author-email: hello@pioreactor.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: adafruit-circuitpython-ssd1306
@@ -15,12 +15,20 @@
 
 
 ### Hardware required
 
  - [Adafruit PiOLED display](https://www.adafruit.com/product/3527)
  - [0.1" 2x20-pin Strip Right Angle Female Header](https://www.adafruit.com/product/2823)
 
+
 ### Installation
 
+Install from the UI, or run:
 ```
 pio install-plugin pioled-display-plugin
 ```
+
+### Hardware installation
+
+With the Pioreactor turned off, install the 2x20 right-angle header onto the the 2x20 header on the Pioreactor HAT. Attach the PiOLED display onto the right-hand side of the new header, with the orientation as shown in the image below:
+
+<img width="462" alt="Screenshot 2023-06-21 at 2 40 14 PM" alt="PiOLD attached to the right-angle headers." src="https://github.com/Pioreactor/PiOLED-display-plugin/assets/884032/3b3096d0-4cfa-4a74-8ff1-36cff2fb4d99">
```

## Comparing `pioled_display_plugin-0.2.2.dist-info/RECORD` & `pioled_display_plugin-0.2.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pioled_display_plugin/__init__.py,sha256=QvxiS-cgKzOS1K2pyuCEGZzuVf1MyV-Z_eORW8jXSaE,5417
+pioled_display_plugin/__init__.py,sha256=Mhh0xFsdkgfz4zz26Nezg0l7wkJDSNyzZtqmRstlt5A,5631
 pioled_display_plugin/post_install.sh,sha256=cV2Ft1Jq6uxbAgOxSfoqDRZSx0mlhKd0NlMZgcE809E,180
 pioled_display_plugin/pre_uninstall.sh,sha256=7Ya_m3QVPCIFz8_dR7ZgaO5jKuqSlaS2EwPryoSjd6g,180
-pioled_display_plugin-0.2.2.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
-pioled_display_plugin-0.2.2.dist-info/METADATA,sha256=YfcRwh0qRyXQusSNUdzNdW73mK73GSnR6kV3i0zRURQ,800
-pioled_display_plugin-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioled_display_plugin-0.2.2.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
-pioled_display_plugin-0.2.2.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
-pioled_display_plugin-0.2.2.dist-info/RECORD,,
+pioled_display_plugin-0.2.3.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
+pioled_display_plugin-0.2.3.dist-info/METADATA,sha256=C7nlSAx3RPLUgyQKzFRxrUprSR_XvwiHlNz1pAdfmUw,1313
+pioled_display_plugin-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioled_display_plugin-0.2.3.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
+pioled_display_plugin-0.2.3.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
+pioled_display_plugin-0.2.3.dist-info/RECORD,,
```

