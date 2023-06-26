# Comparing `tmp/irene_pro-0.0.74.tar.gz` & `tmp/irene_pro-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.74.tar", last modified: Mon Jun 26 12:27:23 2023, max compression
+gzip compressed data, was "irene_pro-0.0.75.tar", last modified: Mon Jun 26 12:36:38 2023, max compression
```

## Comparing `irene_pro-0.0.74.tar` & `irene_pro-0.0.75.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 12:27:23.746145 irene_pro-0.0.74/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.74/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.74/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-26 12:27:23.742154 irene_pro-0.0.74/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.74/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 12:27:23.689306 irene_pro-0.0.74/irene_gui_pkg/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.74/irene_gui_pkg/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.74/irene_gui_pkg/logic.py
--rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.74/irene_gui_pkg/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:27:23.709231 irene_pro-0.0.74/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.74/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.74/irene_pro/logic.py
--rw-rw-rw-   0        0        0    34928 2023-06-26 12:26:29.000000 irene_pro-0.0.74/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:27:23.737165 irene_pro-0.0.74/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-26 12:27:23.000000 irene_pro-0.0.74/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-26 12:27:23.000000 irene_pro-0.0.74/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 12:27:23.000000 irene_pro-0.0.74/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-26 12:27:23.000000 irene_pro-0.0.74/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-26 12:27:23.000000 irene_pro-0.0.74/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 12:27:23.747153 irene_pro-0.0.74/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-26 12:23:58.000000 irene_pro-0.0.74/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:36:38.838207 irene_pro-0.0.75/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.75/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.75/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-26 12:36:38.835214 irene_pro-0.0.75/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.75/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 12:36:38.703555 irene_pro-0.0.75/irene_gui_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.75/irene_gui_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.75/irene_gui_pkg/logic.py
+-rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.75/irene_gui_pkg/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:36:38.785348 irene_pro-0.0.75/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.75/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.75/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    34972 2023-06-26 12:31:39.000000 irene_pro-0.0.75/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:36:38.828234 irene_pro-0.0.75/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-26 12:36:38.000000 irene_pro-0.0.75/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-26 12:36:38.000000 irene_pro-0.0.75/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 12:36:38.000000 irene_pro-0.0.75/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-26 12:36:38.000000 irene_pro-0.0.75/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-26 12:36:38.000000 irene_pro-0.0.75/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 12:36:38.840254 irene_pro-0.0.75/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-26 12:35:42.000000 irene_pro-0.0.75/setup.py
```

### Comparing `irene_pro-0.0.74/PKG-INFO` & `irene_pro-0.0.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.74
+Version: 0.0.75
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.74/README.md` & `irene_pro-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.74/irene_gui_pkg/logic.py` & `irene_pro-0.0.75/irene_gui_pkg/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.74/irene_gui_pkg/widgets.py` & `irene_pro-0.0.75/irene_gui_pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.74/irene_pro/logic.py` & `irene_pro-0.0.75/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.74/irene_pro/widgets.py` & `irene_pro-0.0.75/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,14 +382,15 @@
             pass
         
         def remove_default():
             if self.get() == default:
                 self.set('')
         
         def set_default():
+            print("LEAVING COMBOBOX.....")
             if self.get().strip() == "" or len(self.get().strip()) == 0:
                 self.set(default)
                 print("[DEFAULT SET]")
             else:
                 print(f"COMBO VALUE FOUND: {self.get().strip()}: length: {len(self.get().strip())}")
 
         if self.cget('state') != 'readonly':
```

### Comparing `irene_pro-0.0.74/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.75/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.74
+Version: 0.0.75
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.74/setup.py` & `irene_pro-0.0.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3734 270d 0a44 4553 4352   '0.0.74'..DESCR
+00000100: 2027 302e 302e 3735 270d 0a44 4553 4352   '0.0.75'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

