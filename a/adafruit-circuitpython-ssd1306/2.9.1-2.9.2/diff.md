# Comparing `tmp/adafruit-circuitpython-ssd1306-2.9.1.tar.gz` & `tmp/adafruit-circuitpython-ssd1306-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-ssd1306-2.9.1.tar", last modified: Mon Aug 31 20:35:00 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-ssd1306-2.9.2.tar", last modified: Mon Sep 14 17:08:51 2020, max compression
```

## Comparing `adafruit-circuitpython-ssd1306-2.9.1.tar` & `adafruit-circuitpython-ssd1306-2.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.106672 adafruit-circuitpython-ssd1306-2.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.098672 adafruit-circuitpython-ssd1306-2.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.102672 adafruit-circuitpython-ssd1306-2.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1855 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2598 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    16127 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     5991 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1082 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5506 2020-08-31 20:35:00.106672 adafruit-circuitpython-ssd1306-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3847 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.102672 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5506 2020-08-31 20:34:59.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1022 2020-08-31 20:34:59.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-31 20:34:59.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-08-31 20:34:59.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-08-31 20:34:59.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     9416 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/adafruit_ssd1306.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.102672 adafruit-circuitpython-ssd1306-2.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.102672 adafruit-circuitpython-ssd1306-2.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      266 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5214 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      188 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1095 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-31 20:35:00.102672 adafruit-circuitpython-ssd1306-2.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (116)    12341 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/happycat_oled_32.ppm
--rw-r--r--   0 runner    (1001) docker     (116)    24629 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/happycat_oled_64.ppm
--rw-r--r--   0 runner    (1001) docker     (116)     4653 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_bonnet_buttons.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_bouncing_ball.py
--rw-r--r--   0 runner    (1001) docker     (116)     2787 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_framebuftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     4099 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_animate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_clock.py
--rw-r--r--   0 runner    (1001) docker     (116)     1766 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (116)      976 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_image_display.py
--rw-r--r--   0 runner    (1001) docker     (116)     2321 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_images.py
--rw-r--r--   0 runner    (1001) docker     (116)     2113 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_ip.py
--rw-r--r--   0 runner    (1001) docker     (116)     3474 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_shapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1386 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_text.py
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)     3851 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_stats.py
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-31 20:35:00.106672 adafruit-circuitpython-ssd1306-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1907 2020-08-31 20:34:51.000000 adafruit-circuitpython-ssd1306-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.620272 adafruit-circuitpython-ssd1306-2.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.620272 adafruit-circuitpython-ssd1306-2.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1855 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2598 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)    16127 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     5991 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1082 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     5800 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4085 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5800 2020-09-14 17:08:51.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1022 2020-09-14 17:08:51.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-14 17:08:51.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-09-14 17:08:51.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2020-09-14 17:08:51.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     9416 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/adafruit_ssd1306.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     4414 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5214 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1095 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)    12341 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/happycat_oled_32.ppm
+-rw-r--r--   0 runner    (1001) docker     (116)    24629 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/happycat_oled_64.ppm
+-rw-r--r--   0 runner    (1001) docker     (116)     4653 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_bonnet_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2309 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_bouncing_ball.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2787 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_framebuftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4099 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_animate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1803 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_clock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1766 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (116)      976 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_image_display.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2321 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_images.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2113 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_ip.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3474 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1386 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_text.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1085 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3851 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_stats.py
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-14 17:08:51.624272 adafruit-circuitpython-ssd1306-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1907 2020-09-14 17:08:43.000000 adafruit-circuitpython-ssd1306-2.9.2/setup.py
```

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/.github/workflows/build.yml` & `adafruit-circuitpython-ssd1306-2.9.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/.github/workflows/release.yml` & `adafruit-circuitpython-ssd1306-2.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/.pylintrc` & `adafruit-circuitpython-ssd1306-2.9.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1306-2.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/LICENSE` & `adafruit-circuitpython-ssd1306-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/PKG-INFO` & `adafruit-circuitpython-ssd1306-2.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1306
-Version: 2.9.1
+Version: 2.9.2
 Summary: CircuitPython library for SSD1306 OLED displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1306
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
@@ -93,14 +93,21 @@
         
           # Clear the display.  Always call show after changing pixels to make the display
           # update visible!
           display.fill(0)
         
           display.show()
         
+          # Set a pixel in the origin 0,0 position.
+          display.pixel(0, 0, 1)
+          # Set a pixel in the middle 64, 16 position.
+          display.pixel(64, 16, 1)
+          # Set a pixel in the opposite 127, 31 position.
+          display.pixel(127, 31, 1)
+          display.show()
         
         More examples and details can be found in the `adafruit_framebuf docs <https://circuitpython.readthedocs.io/projects/framebuf/en/latest>`__.
         
         
         Contributing
         ============
```

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/README.rst` & `adafruit-circuitpython-ssd1306-2.9.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -85,14 +85,21 @@
 
   # Clear the display.  Always call show after changing pixels to make the display
   # update visible!
   display.fill(0)
 
   display.show()
 
+  # Set a pixel in the origin 0,0 position.
+  display.pixel(0, 0, 1)
+  # Set a pixel in the middle 64, 16 position.
+  display.pixel(64, 16, 1)
+  # Set a pixel in the opposite 127, 31 position.
+  display.pixel(127, 31, 1)
+  display.show()
 
 More examples and details can be found in the `adafruit_framebuf docs <https://circuitpython.readthedocs.io/projects/framebuf/en/latest>`__.
 
 
 Contributing
 ============
```

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1306
-Version: 2.9.1
+Version: 2.9.2
 Summary: CircuitPython library for SSD1306 OLED displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1306
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
@@ -93,14 +93,21 @@
         
           # Clear the display.  Always call show after changing pixels to make the display
           # update visible!
           display.fill(0)
         
           display.show()
         
+          # Set a pixel in the origin 0,0 position.
+          display.pixel(0, 0, 1)
+          # Set a pixel in the middle 64, 16 position.
+          display.pixel(64, 16, 1)
+          # Set a pixel in the opposite 127, 31 position.
+          display.pixel(127, 31, 1)
+          display.show()
         
         More examples and details can be found in the `adafruit_framebuf docs <https://circuitpython.readthedocs.io/projects/framebuf/en/latest>`__.
         
         
         Contributing
         ============
```

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/adafruit_circuitpython_ssd1306.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1306-2.9.2/adafruit_circuitpython_ssd1306.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/adafruit_ssd1306.py` & `adafruit-circuitpython-ssd1306-2.9.2/adafruit_ssd1306.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1306-2.9.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/docs/conf.py` & `adafruit-circuitpython-ssd1306-2.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/docs/index.rst` & `adafruit-circuitpython-ssd1306-2.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/happycat_oled_32.ppm` & `adafruit-circuitpython-ssd1306-2.9.2/examples/happycat_oled_32.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/happycat_oled_64.ppm` & `adafruit-circuitpython-ssd1306-2.9.2/examples/happycat_oled_64.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_bonnet_buttons.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_bonnet_buttons.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_bouncing_ball.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_bouncing_ball.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_framebuftest.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_framebuftest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_animate.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_animate.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_clock.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_clock.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_demo.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_image_display.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_image_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_images.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_images.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_ip.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_ip.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_shapes.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_shapes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_pillow_text.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_pillow_text.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_simpletest.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/examples/ssd1306_stats.py` & `adafruit-circuitpython-ssd1306-2.9.2/examples/ssd1306_stats.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1306-2.9.1/setup.py` & `adafruit-circuitpython-ssd1306-2.9.2/setup.py`

 * *Files identical despite different names*

