# Comparing `tmp/irene_pro-0.0.70.tar.gz` & `tmp/irene_pro-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.70.tar", last modified: Mon Jun 26 06:53:57 2023, max compression
+gzip compressed data, was "irene_pro-0.0.71.tar", last modified: Mon Jun 26 08:46:08 2023, max compression
```

## Comparing `irene_pro-0.0.70.tar` & `irene_pro-0.0.71.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 06:53:57.216830 irene_pro-0.0.70/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.70/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.70/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-26 06:53:57.215831 irene_pro-0.0.70/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.70/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 06:53:57.190898 irene_pro-0.0.70/irene_gui_pkg/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.70/irene_gui_pkg/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.70/irene_gui_pkg/logic.py
--rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.70/irene_gui_pkg/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:53:57.199875 irene_pro-0.0.70/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.70/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.70/irene_pro/logic.py
--rw-rw-rw-   0        0        0    34254 2023-06-23 08:42:05.000000 irene_pro-0.0.70/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:53:57.213837 irene_pro-0.0.70/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-26 06:53:57.000000 irene_pro-0.0.70/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-26 06:53:57.000000 irene_pro-0.0.70/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 06:53:57.000000 irene_pro-0.0.70/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-26 06:53:57.000000 irene_pro-0.0.70/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-26 06:53:57.000000 irene_pro-0.0.70/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 06:53:57.216830 irene_pro-0.0.70/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-26 06:52:48.000000 irene_pro-0.0.70/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:46:08.833861 irene_pro-0.0.71/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.71/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.71/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-26 08:46:08.831862 irene_pro-0.0.71/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.71/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 08:46:08.790971 irene_pro-0.0.71/irene_gui_pkg/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.71/irene_gui_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.71/irene_gui_pkg/logic.py
+-rw-rw-rw-   0        0        0    33413 2023-06-22 07:03:53.000000 irene_pro-0.0.71/irene_gui_pkg/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:46:08.805930 irene_pro-0.0.71/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.71/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5924 2023-06-26 06:52:40.000000 irene_pro-0.0.71/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    34545 2023-06-26 08:44:18.000000 irene_pro-0.0.71/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:46:08.826874 irene_pro-0.0.71/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-26 08:46:08.000000 irene_pro-0.0.71/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-26 08:46:08.000000 irene_pro-0.0.71/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:46:08.000000 irene_pro-0.0.71/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-26 08:46:08.000000 irene_pro-0.0.71/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-26 08:46:08.000000 irene_pro-0.0.71/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:46:08.834854 irene_pro-0.0.71/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-26 08:45:08.000000 irene_pro-0.0.71/setup.py
```

### Comparing `irene_pro-0.0.70/PKG-INFO` & `irene_pro-0.0.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.70
+Version: 0.0.71
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.70/README.md` & `irene_pro-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.70/irene_gui_pkg/logic.py` & `irene_pro-0.0.71/irene_gui_pkg/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.70/irene_gui_pkg/widgets.py` & `irene_pro-0.0.71/irene_gui_pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.70/irene_pro/logic.py` & `irene_pro-0.0.71/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.70/irene_pro/widgets.py` & `irene_pro-0.0.71/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,27 +363,36 @@
             if len(str(self.get()).strip()) == 0:
                 self.insert(END, default)
                 self.config(fg = "gray50")
 
 
 #=====================COMBOBOX=======================
 class combo(ttk.Combobox):
-    def __init__(self, master, label_txt = None, label_side = LEFT,bd_color = "#0b4", **kwargs):
+    def __init__(self, master, label_txt = None, label_side = LEFT,bd_color = "#0b4", default = None, **kwargs):
         super().__init__(master, font = ('arial', w(12)),**kwargs)
         self.master = master
         self.st = ttk.Style()
         self.st.theme_use('clam')
         
         self.st.configure('comb.TCombobox', foreground = "#023", fieldbackground = self.master['bg'],
                             bordercolor = bd_color, background = bd_color)
         try:
             if label_txt:
                 label(master=self.master, text = label_txt).pack(side = label_side, padx = w(2), pady=w(2))
         except Exception:
             pass
+        
+        def remove_default():
+            if self.get() == default:
+                self.set('')
+
+        if self.cget('state') != 'readonly':
+            if default:
+                self.set(default)
+                self.bind("<Button-1>", remove_default)
 
     
 class checkb(ttk.Checkbutton):
     def __init__(self, master, **kwargs):
         super().__init__(master = master, **kwargs)
         style = ttk.Style()
         style.configure("TCheckbutton", background = master['bg'], foreground="#023", font=("Arial", w(12)))
```

### Comparing `irene_pro-0.0.70/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.71/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.70
+Version: 0.0.71
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.70/setup.py` & `irene_pro-0.0.71/setup.py`

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
-00000100: 2027 302e 302e 3730 270d 0a44 4553 4352   '0.0.70'..DESCR
+00000100: 2027 302e 302e 3731 270d 0a44 4553 4352   '0.0.71'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

