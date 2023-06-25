# Comparing `tmp/musketeer-1.3.0.tar.gz` & `tmp/musketeer-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musketeer-1.3.0.tar", last modified: Sat Jun 24 19:40:04 2023, max compression
+gzip compressed data, was "musketeer-1.3.1.tar", last modified: Sun Jun 25 23:16:47 2023, max compression
```

## Comparing `musketeer-1.3.0.tar` & `musketeer-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.397315 musketeer-1.3.0/
--rw-rw-rw-   0        0        0       66 2023-01-17 16:05:36.000000 musketeer-1.3.0/.flake8
--rw-rw-rw-   0        0        0       70 2023-06-24 19:22:11.000000 musketeer-1.3.0/.gitignore
--rw-rw-rw-   0        0        0     1093 2021-05-07 10:14:54.000000 musketeer-1.3.0/LICENSE
--rw-rw-rw-   0        0        0       35 2021-07-24 12:56:15.000000 musketeer-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      867 2023-06-24 19:40:04.394317 musketeer-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-02-23 14:24:54.000000 musketeer-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.352317 musketeer-1.3.0/musketeer/
--rw-rw-rw-   0        0        0       23 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/__init__.py
--rw-rw-rw-   0        0        0    10662 2023-05-04 16:25:02.000000 musketeer-1.3.0/musketeer/__main__.py
--rw-rw-rw-   0        0        0     1082 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/combineResiduals.py
--rw-rw-rw-   0        0        0     8000 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/contributingSpecies.py
--rw-rw-rw-   0        0        0    19032 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/contributors.py
--rw-rw-rw-   0        0        0     8404 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/editData.py
--rw-rw-rw-   0        0        0    13925 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/equilibriumConstants.py
--rw-rw-rw-   0        0        0     8433 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/fitSignals.py
--rw-rw-rw-   0        0        0    10506 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/knownSignals.py
--rw-rw-rw-   0        0        0      937 2021-01-06 01:52:42.000000 musketeer-1.3.0/musketeer/logo small.png
--rw-rw-rw-   0        0        0     5452 2023-06-24 19:16:36.000000 musketeer-1.3.0/musketeer/moduleFrame.py
--rw-rw-rw-   0        0        0     8875 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/patchMatplotlib.py
--rw-rw-rw-   0        0        0     1266 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/proportionality.py
--rw-rw-rw-   0        0        0    12401 2023-05-04 16:25:44.000000 musketeer-1.3.0/musketeer/scrolledFrame.py
--rw-rw-rw-   0        0        0    22687 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/speciation.py
--rw-rw-rw-   0        0        0      607 2023-04-19 11:14:04.000000 musketeer-1.3.0/musketeer/style.py
--rw-rw-rw-   0        0        0    17174 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/table.py
--rw-rw-rw-   0        0        0     9381 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titration.py
--rw-rw-rw-   0        0        0    48125 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titrationFrame.py
--rw-rw-rw-   0        0        0     8950 2023-06-24 19:22:11.000000 musketeer-1.3.0/musketeer/titrationReader.py
--rw-rw-rw-   0        0        0    17120 2023-04-19 11:14:04.000000 musketeer-1.3.0/musketeer/totalConcentrations.py
--rw-rw-rw-   0        0        0     2903 2023-03-09 17:30:25.000000 musketeer-1.3.0/musketeer/windowsHighDpiPatch.py
-drwxrwxrwx   0        0        0        0 2023-06-24 19:40:04.391317 musketeer-1.3.0/musketeer.egg-info/
--rw-rw-rw-   0        0        0      867 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 19:40:03.000000 musketeer-1.3.0/musketeer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 19:40:04.397315 musketeer-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1836 2023-04-19 11:14:04.000000 musketeer-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:16:37.125744 musketeer-1.3.1/
+-rw-rw-rw-   0        0        0      118 2023-06-25 21:15:48.000000 musketeer-1.3.1/.flake8
+-rw-rw-rw-   0        0        0      107 2023-06-25 23:14:54.000000 musketeer-1.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1093 2021-05-07 10:14:54.000000 musketeer-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0       35 2021-07-24 12:56:15.000000 musketeer-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      867 2023-06-25 23:16:47.628323 musketeer-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-02-23 14:24:54.000000 musketeer-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 23:16:36.991743 musketeer-1.3.1/cx_freeze/
+-rw-rw-rw-   0        0        0    21310 2023-06-25 23:03:25.000000 musketeer-1.3.1/cx_freeze/logo 48px.ico
+-rw-rw-rw-   0        0        0    38648 2023-06-25 00:00:13.000000 musketeer-1.3.1/cx_freeze/logo 512px.png
+-rw-rw-rw-   0        0        0      781 2023-06-25 23:10:18.000000 musketeer-1.3.1/cx_freeze/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:16:37.081744 musketeer-1.3.1/musketeer/
+-rw-rw-rw-   0        0        0       23 2023-06-25 22:01:09.000000 musketeer-1.3.1/musketeer/__init__.py
+-rw-rw-rw-   0        0        0    12128 2023-06-25 21:46:41.000000 musketeer-1.3.1/musketeer/__main__.py
+-rw-rw-rw-   0        0        0     1082 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/combineResiduals.py
+-rw-rw-rw-   0        0        0     8068 2023-06-25 22:00:40.000000 musketeer-1.3.1/musketeer/contributingSpecies.py
+-rw-rw-rw-   0        0        0    19168 2023-06-25 22:00:19.000000 musketeer-1.3.1/musketeer/contributors.py
+-rw-rw-rw-   0        0        0     8404 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/editData.py
+-rw-rw-rw-   0        0        0    14743 2023-06-25 21:59:35.000000 musketeer-1.3.1/musketeer/equilibriumConstants.py
+-rw-rw-rw-   0        0        0     8433 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/fitSignals.py
+-rw-rw-rw-   0        0        0    10506 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/knownSignals.py
+-rw-rw-rw-   0        0        0     2007 2023-06-25 00:19:37.000000 musketeer-1.3.1/musketeer/logo 48px.png
+-rw-rw-rw-   0        0        0    38648 2023-06-25 00:00:13.000000 musketeer-1.3.1/musketeer/logo 512px.png
+-rw-rw-rw-   0        0        0     5452 2023-06-24 19:16:36.000000 musketeer-1.3.1/musketeer/moduleFrame.py
+-rw-rw-rw-   0        0        0     8875 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/patchMatplotlib.py
+-rw-rw-rw-   0        0        0     1266 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/proportionality.py
+-rw-rw-rw-   0        0        0    12401 2023-05-04 16:25:44.000000 musketeer-1.3.1/musketeer/scrolledFrame.py
+-rw-rw-rw-   0        0        0    22755 2023-06-25 22:00:34.000000 musketeer-1.3.1/musketeer/speciation.py
+-rw-rw-rw-   0        0        0      607 2023-04-19 11:14:04.000000 musketeer-1.3.1/musketeer/style.py
+-rw-rw-rw-   0        0        0    17174 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/table.py
+-rw-rw-rw-   0        0        0     9381 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/titration.py
+-rw-rw-rw-   0        0        0    48125 2023-06-24 19:22:11.000000 musketeer-1.3.1/musketeer/titrationFrame.py
+-rw-rw-rw-   0        0        0     8961 2023-06-25 22:45:55.000000 musketeer-1.3.1/musketeer/titrationReader.py
+-rw-rw-rw-   0        0        0    17310 2023-06-25 22:00:29.000000 musketeer-1.3.1/musketeer/totalConcentrations.py
+-rw-rw-rw-   0        0        0     2903 2023-03-09 17:30:25.000000 musketeer-1.3.1/musketeer/windowsHighDpiPatch.py
+drwxrwxrwx   0        0        0        0 2023-06-25 23:16:47.626324 musketeer-1.3.1/musketeer.egg-info/
+-rw-rw-rw-   0        0        0      867 2023-06-25 23:16:46.000000 musketeer-1.3.1/musketeer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      895 2023-06-25 23:16:47.000000 musketeer-1.3.1/musketeer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 23:16:46.000000 musketeer-1.3.1/musketeer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-25 23:16:46.000000 musketeer-1.3.1/musketeer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 23:16:46.000000 musketeer-1.3.1/musketeer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 23:16:47.632322 musketeer-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1836 2023-04-19 11:14:04.000000 musketeer-1.3.1/setup.py
```

### Comparing `musketeer-1.3.0/LICENSE` & `musketeer-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/PKG-INFO` & `musketeer-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musketeer
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool for fitting data from titration experiments.
 Home-page: https://github.com/daniilS/Musketeer
 Author: Daniil Soloviev
 Author-email: dos23@cam.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `musketeer-1.3.0/musketeer/__main__.py` & `musketeer-1.3.1/musketeer/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import ctypes
 import importlib.resources as res
 import tkinter as tk
 import tkinter.filedialog as fd
 import tkinter.messagebox as mb
 import tkinter.ttk as ttk
-from pathlib import PurePath
 from tkinter import font
 
-import numpy as np
 import ttkbootstrap
-from ttkbootstrap.widgets import InteractiveNotebook
 
-from . import patchMatplotlib, titrationReader, windowsHighDpiPatch
-from .style import defaultFigureParams, figureParams, padding
-from .table import ButtonFrame
-from .titration import Titration
-from .titrationFrame import TitrationFrame
+from . import windowsHighDpiPatch
+from .style import padding
 
-patchMatplotlib.applyPatch()
 try:
     appId = "daniilS.musketeer"
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(appId)
 except Exception:
     pass
 
 
-DEBUG = True
+fullErrorMessages = True
 olderror = mb.showerror
 
 
+# TODO: convert to simple error message, with an option to expand to the full one
 def newshowerror(title, message, *args, **kwargs):
     import traceback
 
-    if DEBUG and isinstance(message, Exception):
+    if fullErrorMessages and isinstance(message, Exception):
         message = traceback.format_exc()
     return olderror(title, message, *args, **kwargs)
 
 
 mb.showerror = newshowerror
 
 
@@ -52,26 +46,68 @@
     # Windows and OS X
     root.state("zoomed")
 except tk.TclError:
     # X11
     root.attributes("-zoomed", True)
 root.title("Musketeer")
 
+
+# notes on preferred icon size on Windows:
+# title bar: prefers 16px, actual size 16px (or 24px at 1.5x scaling)
+# if the icon set without calling update() first, the title bar also prefers 32, but
+# will be blurry
+# task bar: prefers 32px, actual size 24px (or 36px at 1.5x scaling)
+# if the preferred size is not provided, the first file provided will be used
+# the least common multiple of 16, 24, and 36 is 144, but using that causes the title
+# bar icon to be blurry
+# 48px seems to give the best quality at all scaling factors
+
+# on Linux, tk documentation recommends providing no more than 2 icons, placing the
+# largest one first
+# on MacOS, only the first icon is used, and it is recommended to provide as large an
+# icon as possible
+
 try:
-    iconData = res.read_binary(__package__, "logo small.png")
-    icon = tk.PhotoImage(data=iconData)
-    root.iconphoto(True, icon)
+    root.update()  # without this, the title bar icon is blurry on Windows
+    iconData48 = res.read_binary(__package__, "logo 48px.png")
+    iconData512 = res.read_binary(__package__, "logo 512px.png")
+    icon48 = tk.PhotoImage(data=iconData48)
+    icon512 = tk.PhotoImage(data=iconData512)
+
+    if root._windowingsystem == "win32":
+        root.iconphoto(True, icon48, icon512)
+    else:
+        root.iconphoto(True, icon512, icon48)
 except Exception:
     # Should currently never happen, but if anything changes about the API in
     # the future, we can survive without an icon.
     pass
 frame = ttk.Frame(root, padding=padding)
 frame.pack(expand=True, fill="both")
 
 
+# Especially on the first startup, when matplotlib needs to build the font cache,
+# importing everything may take a while. So we defer all other imports until now.
+root.tk.eval("tk busy .")
+root.update()
+
+from pathlib import PurePath
+
+import numpy as np
+from ttkbootstrap.widgets import InteractiveNotebook
+
+from . import patchMatplotlib, titrationReader
+from .style import defaultFigureParams, figureParams
+from .table import ButtonFrame
+from .titration import Titration
+from .titrationFrame import TitrationFrame
+
+patchMatplotlib.applyPatch()
+
+
 class DpiPopup(tk.Toplevel):
     def __init__(self, master, saveCallback, *args, **kwargs):
         super().__init__(
             master,
             padx=padding,
             pady=padding,
             *args,
@@ -307,8 +343,9 @@
                 titrationFrame.updateDpi()
         self.update()
 
 
 notebook = TitrationsNotebook(frame)
 notebook.pack(expand=True, fill="both")
 
+root.tk.eval("tk busy forget .")
 root.mainloop()
```

### Comparing `musketeer-1.3.0/musketeer/combineResiduals.py` & `musketeer-1.3.1/musketeer/combineResiduals.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/contributingSpecies.py` & `musketeer-1.3.1/musketeer/contributingSpecies.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,17 @@
             text=(
                 "For each signal, specify which molecule (free and in complexes) it is"
                 " caused by."
             ),
         )
         label.pack(expand=False, fill="both")
 
-        scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
+        scrolledFrame = ScrolledFrame(
+            self.frame, max_width=self.winfo_toplevel().master.winfo_width() - 200
+        )
         scrolledFrame.pack(expand=True, fill="both")
         self.innerFrame = scrolledFrame.display_widget(ttk.Frame, stretch=True)
 
         self.mapVars = []
 
         radioFrame = ttk.Frame(self.innerFrame)
         radioFrame.pack(expand=True, fill="both")
```

### Comparing `musketeer-1.3.0/musketeer/contributors.py` & `musketeer-1.3.1/musketeer/contributors.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,17 @@
             ),
         )
         contributorsLabel.pack(expand=False, fill="both")
 
         buttonFrame = ButtonFrame(self.frame, self.reset, self.saveData, self.destroy)
         buttonFrame.pack(expand=False, fill="both", side="bottom")
 
-        scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
+        scrolledFrame = ScrolledFrame(
+            self.frame, max_width=self.winfo_toplevel().master.winfo_width() - 200
+        )
         scrolledFrame.pack(expand=True, fill="both")
         self.innerFrame = scrolledFrame.display_widget(ttk.Frame, stretch=True)
         self.createTable()
 
     def createTable(self):
         self.contributorsTable = ContributorsTable(
             self.innerFrame,
@@ -160,15 +162,17 @@
             ),
         )
         contributorsLabel.pack(expand=False, fill="both")
 
         buttonFrame = ButtonFrame(self.frame, self.reset, self.saveData, self.destroy)
         buttonFrame.pack(expand=False, fill="both", side="bottom")
 
-        scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
+        scrolledFrame = ScrolledFrame(
+            self.frame, max_width=self.winfo_toplevel().master.winfo_width() - 200
+        )
         scrolledFrame.pack(expand=True, fill="both")
         self.innerFrame = scrolledFrame.display_widget(ttk.Frame, stretch=True)
         self.createNotebook()
 
     def createNotebook(self):
         self.notebook = ttk.Notebook(self.innerFrame, style="Flat.TNotebook")
         self.notebook.pack(expand=True, fill="both", padx=padding, pady=padding)
```

### Comparing `musketeer-1.3.0/musketeer/editData.py` & `musketeer-1.3.1/musketeer/editData.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/equilibriumConstants.py` & `musketeer-1.3.1/musketeer/equilibriumConstants.py`

 * *Files 6% similar despite different names*

```diff
@@ -209,41 +209,47 @@
             self.frame,
             text=(
                 "Each row represents a variable that will be optimised. Each column"
                 " represents a complex. The global K for each complex is the product of"
                 " a statistical factor, and all the variables raised to the exponents"
                 " specified in that column.\n\nIn the final column, specify a value to"
                 " fix the variable, leave empty to optimise the variable, or write"
-                " ~number to provide an initial guess for the optimisation."
+                " ~number to provide an initial guess for the optimisation.\n\nThe K"
+                " for each complex is the global equilibrium constant. For polymers, K₂"
+                " is the constant for the formation of the dimer, and Kₙ the constant"
+                " for each subsequent binding."
             ),
             padding=5,
         )
         customKsLabel.pack(expand=False, fill="both")
 
-        scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
+        buttonFrame = ButtonFrame(self.frame, self.reset, self.saveData, self.destroy)
+        buttonFrame.pack(expand=False, fill="both", side="bottom")
+
+        scrolledFrame = ScrolledFrame(
+            self.frame, max_width=self.winfo_toplevel().master.winfo_width() - 200
+        )
+        scrolledFrame.pack(expand=True, fill="both")
         scrolledFrame.pack(expand=True, fill="both")
 
         self.innerFrame = scrolledFrame.display_widget(ttk.Frame, stretch=True)
 
         self.customKsTable = CustomKsTable(self.innerFrame, titration)
         self.customKsTable.pack(expand=True, fill="both")
 
         self.labelFont = font.nametofont("TkTextFont").copy()
         self.labelFont["size"] = int(1.3 * self.labelFont["size"])
 
         self.equationsLabel = ttk.Label(
-            self.frame, anchor="center", font=self.labelFont, padding=5
+            self.innerFrame, anchor="center", font=self.labelFont, padding=5
         )
         self.equationsLabel.pack(fill="both")
         self.customKsTable.equationsLabel = self.equationsLabel
         self.customKsTable.createLabels()
 
-        buttonFrame = ButtonFrame(self.frame, self.reset, self.saveData, self.destroy)
-        buttonFrame.pack(expand=False, fill="both", side="bottom")
-
     def reset(self):
         self.customKsTable.destroy()
         self.customKsTable = CustomKsTable(self.innerFrame, self.titration)
         self.customKsTable.pack(expand=True, fill="both")
         self.customKsTable.label = self.equationsLabel
         self.customKsTable.createLabels()
 
@@ -334,26 +340,35 @@
         return string
 
 
 class KnownKsPopup(moduleFrame.Popup):
     def __init__(self, titration, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.titration = titration
-        self.title("Enter known equilibrium constants")
-
         height = int(self.master.winfo_height() * 0.4)
-        frame = ScrolledFrame(self, height=height, max_width=1500)
+        frame = ScrolledFrame(
+            self,
+            height=height,
+            max_width=self.winfo_toplevel().master.winfo_width() - 200,
+        )
+        frame.pack(expand=True, fill="both")
+        frame = ScrolledFrame(
+            self, height=height, max_width=self.winfo_toplevel().winfo_width() - 200
+        )
         frame.pack(expand=True, fill="both")
 
         innerFrame = frame.display_widget(ttk.Frame, stretch=True)
         knownKsLabel = WrappedLabel(
             innerFrame,
             text=(
                 "Enter known K values, leave empty to optimise the value, or write"
-                " ~number to provide an initial guess for the optimisation."
+                " ~number to provide an initial guess for the optimisation.\n\nThe K"
+                " for each complex is the global equilibrium constant. For polymers, K₂"
+                " is the constant for the formation of the dimer, and Kₙ the constant"
+                " for each subsequent binding."
             ),
             padding=5,
         )
         knownKsLabel.pack(expand=False, fill="both")
 
         self.knownKsTable = KnownKsTable(innerFrame, titration)
         self.knownKsTable.pack(expand=True, fill="both")
```

### Comparing `musketeer-1.3.0/musketeer/fitSignals.py` & `musketeer-1.3.1/musketeer/fitSignals.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/knownSignals.py` & `musketeer-1.3.1/musketeer/knownSignals.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/moduleFrame.py` & `musketeer-1.3.1/musketeer/moduleFrame.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/patchMatplotlib.py` & `musketeer-1.3.1/musketeer/patchMatplotlib.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/proportionality.py` & `musketeer-1.3.1/musketeer/proportionality.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/scrolledFrame.py` & `musketeer-1.3.1/musketeer/scrolledFrame.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/speciation.py` & `musketeer-1.3.1/musketeer/speciation.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,17 @@
                 " Define each complex by adding a row with the stoichiometry of each"
                 " molecule in the complex. For polymers, use 'n'. Leaving a cell blank"
                 " is identical to entering '0'."
             ),
         )
         label.pack(expand=False, fill="both")
 
-        scrolledFrame = ScrolledFrame(self.frame, max_width=1500)
+        scrolledFrame = ScrolledFrame(
+            self.frame, max_width=self.winfo_toplevel().master.winfo_width() - 200
+        )
         scrolledFrame.pack(expand=True, fill="both")
         self.innerFrame = scrolledFrame.display_widget(ttk.Frame, stretch=True)
 
         self.speciationTable = SpeciationTable(self.innerFrame, titration)
         self.speciationTable.pack(expand=True, fill="both")
 
         buttonFrame = ButtonFrame(self.frame, self.reset, self.saveData, self.destroy)
```

### Comparing `musketeer-1.3.0/musketeer/style.py` & `musketeer-1.3.1/musketeer/style.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/table.py` & `musketeer-1.3.1/musketeer/table.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/titration.py` & `musketeer-1.3.1/musketeer/titration.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/titrationFrame.py` & `musketeer-1.3.1/musketeer/titrationFrame.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer/titrationReader.py` & `musketeer-1.3.1/musketeer/titrationReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,11 +268,11 @@
     serialised = np.load(filePath, allow_pickle=False)
     return [serialised]
 
 
 fileReaders = np.array(
     [
         ["Musketeer file", "*.fit", readMusketeer],
-        ["UV-Vis csv file", "*.csv", readUV],
-        ["NMR peak list", "*.csv", readNMR],
+        ["Cary UV-Vis csv file", "*.csv", readUV],
+        ["Mnova NMR peak list", "*.csv", readNMR],
     ]
 )
```

### Comparing `musketeer-1.3.0/musketeer/totalConcentrations.py` & `musketeer-1.3.1/musketeer/totalConcentrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,19 @@
 class VolumesPopup(moduleFrame.Popup):
     def __init__(self, titration, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.titration = titration
         self.title("Enter volumes")
 
         height = int(self.master.winfo_height() * 0.8)
-        frame = ScrolledFrame(self, height=height, max_width=1500)
+        frame = ScrolledFrame(
+            self,
+            height=height,
+            max_width=self.winfo_toplevel().master.winfo_width() - 200,
+        )
         frame.pack(expand=True, fill="both")
 
         innerFrame = frame.display_widget(ttk.Frame, stretch=True)
 
         unknownConcsFrame = ttk.Frame(innerFrame, borderwidth=5)
         unknownConcsFrame.pack(expand=True, fill="both")
         unknownConcsLabel = WrappedLabel(
@@ -443,15 +447,19 @@
 class ConcsPopup(moduleFrame.Popup):
     def __init__(self, titration, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.titration = titration
         self.title("Enter concentrations")
 
         height = int(self.master.winfo_height() * 0.8)
-        frame = ScrolledFrame(self, height=height, max_width=1500)
+        frame = ScrolledFrame(
+            self,
+            height=height,
+            max_width=self.winfo_toplevel().master.winfo_width() - 200,
+        )
         frame.pack(expand=True, fill="both")
 
         innerFrame = frame.display_widget(ttk.Frame, stretch=True)
 
         self.concsTable = ConcsTable(innerFrame, titration)
         self.concsTable.pack(expand=True, fill="both")
```

### Comparing `musketeer-1.3.0/musketeer/windowsHighDpiPatch.py` & `musketeer-1.3.1/musketeer/windowsHighDpiPatch.py`

 * *Files identical despite different names*

### Comparing `musketeer-1.3.0/musketeer.egg-info/PKG-INFO` & `musketeer-1.3.1/musketeer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musketeer
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool for fitting data from titration experiments.
 Home-page: https://github.com/daniilS/Musketeer
 Author: Daniil Soloviev
 Author-email: dos23@cam.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `musketeer-1.3.0/musketeer.egg-info/SOURCES.txt` & `musketeer-1.3.1/musketeer.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 .flake8
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+cx_freeze/logo 48px.ico
+cx_freeze/logo 512px.png
+cx_freeze/setup.py
 musketeer/__init__.py
 musketeer/__main__.py
 musketeer/combineResiduals.py
 musketeer/contributingSpecies.py
 musketeer/contributors.py
 musketeer/editData.py
 musketeer/equilibriumConstants.py
 musketeer/fitSignals.py
 musketeer/knownSignals.py
-musketeer/logo small.png
+musketeer/logo 48px.png
+musketeer/logo 512px.png
 musketeer/moduleFrame.py
 musketeer/patchMatplotlib.py
 musketeer/proportionality.py
 musketeer/scrolledFrame.py
 musketeer/speciation.py
 musketeer/style.py
 musketeer/table.py
```

### Comparing `musketeer-1.3.0/setup.py` & `musketeer-1.3.1/setup.py`

 * *Files identical despite different names*

