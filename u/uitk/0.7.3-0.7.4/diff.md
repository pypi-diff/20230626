# Comparing `tmp/uitk-0.7.3.tar.gz` & `tmp/uitk-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.7.3.tar", last modified: Sun Jun 25 23:04:26 2023, max compression
+gzip compressed data, was "uitk-0.7.4.tar", last modified: Mon Jun 26 16:56:42 2023, max compression
```

## Comparing `uitk-0.7.3.tar` & `uitk-0.7.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 23:04:26.705375 uitk-0.7.3/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.3/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3671 2023-06-25 23:04:26.705375 uitk-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-25 23:04:26.705375 uitk-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2455 2023-06-22 16:49:58.000000 uitk-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 23:04:26.663619 uitk-0.7.3/uitk/
--rw-rw-rw-   0        0        0     2937 2023-06-25 23:04:23.000000 uitk-0.7.3/uitk/__init__.py
--rw-rw-rw-   0        0        0    14483 2023-06-24 19:54:52.000000 uitk-0.7.3/uitk/events.py
--rw-rw-rw-   0        0        0   104090 2023-06-25 22:58:39.000000 uitk-0.7.3/uitk/switchboard.py
--rw-rw-rw-   0        0        0   102727 2023-06-24 17:53:40.000000 uitk-0.7.3/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-25 23:04:26.695376 uitk-0.7.3/uitk/widgets/
--rw-rw-rw-   0        0        0    18631 2023-06-25 22:12:21.000000 uitk-0.7.3/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.3/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15870 2023-06-24 02:15:31.000000 uitk-0.7.3/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     4207 2023-06-02 17:31:37.000000 uitk-0.7.3/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     8332 2023-06-20 19:15:01.000000 uitk-0.7.3/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     7036 2023-06-10 13:16:59.000000 uitk-0.7.3/uitk/widgets/draggableHeader.py
--rw-rw-rw-   0        0        0    22380 2023-06-02 21:56:26.000000 uitk-0.7.3/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0     2498 2023-06-02 17:31:37.000000 uitk-0.7.3/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3295 2023-06-15 19:41:53.000000 uitk-0.7.3/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    23456 2023-06-19 14:36:41.000000 uitk-0.7.3/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.3/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-06-25 23:04:26.704378 uitk-0.7.3/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.3/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    12614 2023-06-25 19:11:11.000000 uitk-0.7.3/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.3/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.3/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0     5044 2023-06-17 23:02:35.000000 uitk-0.7.3/uitk/widgets/mixins/menu_instance.py
--rw-rw-rw-   0        0        0     1878 2023-06-25 14:56:00.000000 uitk-0.7.3/uitk/widgets/mixins/state_manager.py
--rw-rw-rw-   0        0        0    48184 2023-06-24 02:14:57.000000 uitk-0.7.3/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.3/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    11099 2023-05-12 17:26:59.000000 uitk-0.7.3/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6204 2023-06-10 12:44:09.000000 uitk-0.7.3/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.3/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     3069 2023-06-15 19:57:41.000000 uitk-0.7.3/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.3/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3709 2023-06-12 14:42:27.000000 uitk-0.7.3/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-06-25 23:04:26.677632 uitk-0.7.3/uitk.egg-info/
--rw-rw-rw-   0        0        0     3671 2023-06-25 23:04:26.000000 uitk-0.7.3/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.3/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1022 2023-06-25 23:04:26.000000 uitk-0.7.3/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.3/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-25 23:04:26.000000 uitk-0.7.3/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-25 23:04:26.000000 uitk-0.7.3/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 16:56:42.414828 uitk-0.7.4/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.4/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3691 2023-06-26 16:56:42.413828 uitk-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-26 16:56:42.414828 uitk-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2455 2023-06-22 16:49:58.000000 uitk-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:56:42.361939 uitk-0.7.4/uitk/
+-rw-rw-rw-   0        0        0     2937 2023-06-26 16:56:37.000000 uitk-0.7.4/uitk/__init__.py
+-rw-rw-rw-   0        0        0    14483 2023-06-24 19:54:52.000000 uitk-0.7.4/uitk/events.py
+-rw-rw-rw-   0        0        0   103939 2023-06-26 15:34:23.000000 uitk-0.7.4/uitk/switchboard.py
+-rw-rw-rw-   0        0        0   102727 2023-06-24 17:53:40.000000 uitk-0.7.4/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-26 16:56:42.403986 uitk-0.7.4/uitk/widgets/
+-rw-rw-rw-   0        0        0    19057 2023-06-26 16:31:32.000000 uitk-0.7.4/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.4/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15870 2023-06-24 02:15:31.000000 uitk-0.7.4/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     4207 2023-06-02 17:31:37.000000 uitk-0.7.4/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     8332 2023-06-20 19:15:01.000000 uitk-0.7.4/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     7036 2023-06-10 13:16:59.000000 uitk-0.7.4/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22380 2023-06-02 21:56:26.000000 uitk-0.7.4/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2498 2023-06-02 17:31:37.000000 uitk-0.7.4/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3295 2023-06-15 19:41:53.000000 uitk-0.7.4/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    23456 2023-06-19 14:36:41.000000 uitk-0.7.4/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.4/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:56:42.413828 uitk-0.7.4/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.4/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    12614 2023-06-25 19:11:11.000000 uitk-0.7.4/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.4/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.4/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0     5044 2023-06-17 23:02:35.000000 uitk-0.7.4/uitk/widgets/mixins/menu_instance.py
+-rw-rw-rw-   0        0        0     1878 2023-06-25 14:56:00.000000 uitk-0.7.4/uitk/widgets/mixins/state_manager.py
+-rw-rw-rw-   0        0        0    48184 2023-06-24 02:14:57.000000 uitk-0.7.4/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.4/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11099 2023-05-12 17:26:59.000000 uitk-0.7.4/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6204 2023-06-10 12:44:09.000000 uitk-0.7.4/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.4/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     3069 2023-06-15 19:57:41.000000 uitk-0.7.4/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.4/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3709 2023-06-12 14:42:27.000000 uitk-0.7.4/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:56:42.388977 uitk-0.7.4/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3691 2023-06-26 16:56:42.000000 uitk-0.7.4/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.4/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1022 2023-06-26 16:56:42.000000 uitk-0.7.4/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.4/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:56:42.000000 uitk-0.7.4/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 16:56:42.000000 uitk-0.7.4/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.7.3/COPYING.LESSER` & `uitk-0.7.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/PKG-INFO` & `uitk-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.3
+Version: 0.7.4
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
@@ -16,20 +16,21 @@
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots and styles, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
 
 - Dynamic UI file loading
-- Custom widget registration and usage
+- Custom widget registration
 - Utility properties for MainWindow and child widget subclassing
-- Efficient management of slot connections and event handling
+- Management of slot connections and event handling
 - Support for UI hierarchy navigation and submenus
 - Custom event behavior through UI tags
 - UI and slot history storage and retrieval
+- Widget syncing and state management.
 
 ## Module Overview
 
 Module | Description
 ------- | -------
 [switchboard](https://github.com/m3trik/uitk/blob/main/uitk/switchboard.py) | Handles dynamic UI loading, assigns convenience properties, and manages slot connections.
 [events](https://github.com/m3trik/uitk/blob/main/uitk/events.py) | Manages event handling for dynamic UI widgets.
```

### Comparing `uitk-0.7.3/setup.py` & `uitk-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/__init__.py` & `uitk-0.7.4/uitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import pkgutil
 import inspect
 from .switchboard import signals  # Make signals accessible at package root
 
 
 __package__ = "uitk"
-__version__ = '0.7.3'
+__version__ = '0.7.4'
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
```

### Comparing `uitk-0.7.3/uitk/events.py` & `uitk-0.7.4/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/switchboard.py` & `uitk-0.7.4/uitk/switchboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,17 @@
 
         calling_frame = inspect.currentframe().f_back
         # Get calling module directory.
         self.default_dir = self.get_module_dir_from_frame(calling_frame)
         self.module_dir = ptk.get_filepath(__file__)  # the directory of this module.
 
         # initialize the files dicts before the location dicts (dependancies).
-        self.ui_files = {}  # UI paths.
-        self.widget_files = {}  # widget paths.
-        self.slots_files = {}  # slot class paths.
+        self.ui_files = {}  # UI filepaths.
+        self.widget_files = {}  # widget filepaths.
+        self.slots_files = {}  # slot class filepaths.
 
         # use the relative filepath of this module if None is given.
         self.ui_location = ui_location or f"{self.module_dir}/ui"
         self.widgets_location = widgets_location or f"{self.module_dir}/widgets"
         self.slots_location = slots_location or f"{self.module_dir}/slots"
 
         self.ui_name_delimiters = ui_name_delimiters
@@ -649,16 +649,16 @@
 
     def _get_widgets_from_dir(self, path) -> dict:
         """Get all widget class objects from a given directory, module filepath or module name.
 
         Parameters:
             path (str): A directory, fullpath to a widget module, or the name of a module residing in the 'widgets' directory.
                         For example: - 'path_to/uitk/widgets'
-                                                 - 'path_to/uitk/widgets/comboBox.py'
-                                                 - 'comboBox'
+                                    - 'path_to/uitk/widgets/comboBox.py'
+                                    - 'comboBox'
         Returns:
             (dict) keys are widget names and the values are the widget class objects.
             Returns an empty dictionary if no widgets were found or an error occurred.
         """
         mod_name = ptk.format_path(path, "name")
         if mod_name:
             wgt_name = ptk.set_case(mod_name, "pascal")
@@ -1062,21 +1062,15 @@
             return filtered  # return entire list if index is None
         else:
             try:
                 return filtered[index]  # return slot(s) based on the index
             except IndexError:
                 return [] if isinstance(index, int) else None
 
-    def ui_history(
-        self,
-        index=None,
-        allow_duplicates=False,
-        inc=[],
-        exc=[],
-    ):
+    def ui_history(self, index=None, allow_duplicates=False, inc=[], exc=[]):
         """Get the UI history.
 
         Parameters:
             index (int/slice, optional): Index or slice to return from the history. If not provided, returns the full list.
             allow_duplicates (bool): When returning a list, allows for duplicate names in the returned list.
             inc (str/int/list): The objects(s) to include.
                         supports using the '*' operator: startswith*, *endswith, *contains*
@@ -1109,20 +1103,15 @@
         else:
             try:
                 return filtered[index]  # return UI(s) based on the index
             except IndexError:
                 return [] if isinstance(index, int) else None
 
     def get_ui_relatives(
-        self,
-        ui,
-        upstream=False,
-        exact=False,
-        downstream=False,
-        reverse=False,
+        self, ui, upstream=False, exact=False, downstream=False, reverse=False
     ):
         """Get the UI relatives based on the hierarchy matching.
 
         Parameters:
             ui (str or obj): A dynamic UI object or its name for which relatives are to be found.
             upstream (bool, optional): If True, return the relatives that are upstream of the target UI. Defaults to False.
             exact (bool, optional): If True, return only the relatives that exactly match the target UI. Defaults to False.
@@ -1747,20 +1736,18 @@
         Example:
             get_methods_by_name(<ui>, 'slot1,slot2,slot3')
         """
         if not isinstance(clss, object):
             raise ValueError(f"Invalid datatype: {type(clss)}")
 
         result = []
-        for n in Switchboard.unpack_names(name_string):
-            # try:
-            s = getattr(clss, n)
-            result.append(s)
-            # except AttributeError:
-            # self.logger.info(traceback.format_exc())
+        for method_name in Switchboard.unpack_names(name_string):
+            method = getattr(clss, method_name, None)
+            if method is not None:
+                result.append(method)
 
         return result
 
     def create_button_groups(self, ui, *args):
         """Create button groups for a set of widgets.
         The created groups later be accessed through the grouped buttons using the 'button_group' attribute.
```

### Comparing `uitk-0.7.3/uitk/switchboard.py.bak` & `uitk-0.7.4/uitk/switchboard.py.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/MainWindow.py` & `uitk-0.7.4/uitk/widgets/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,17 +164,15 @@
         widget.type = widget.__class__
         widget.derived_type = ptk.get_derived_type(widget, module="QtWidgets")
 
         widget.get_slot = lambda w=widget: getattr(
             self.sb.get_slots(w.ui), w.name, None
         )
 
-        widget.get_slot_init = lambda w=widget: getattr(
-            self.sb.get_slots(w.ui), f"{w.name}_init", None
-        )
+        widget.init_slot = lambda w=widget: self.init_slot(w)
 
         widget.connect_slot = lambda w=widget, s=None: self.sb.connect_slot(s)
         widget.refresh = True
         widget.is_initialized = False
         widget.installEventFilter(self)
 
         ptk.set_attributes(widget, **kwargs)
@@ -354,31 +352,43 @@
         """
         method = partial(func, *args)
         if priority in self._deferred:
             self._deferred[priority] += (method,)
         else:
             self._deferred[priority] = (method,)
 
+    def init_slot(self, widget):
+        """ """
+        # Obtain the slot init function based on widget and its name
+        slots = self.sb.get_slots(widget.ui)
+        slot_init = getattr(slots, f"{widget.name}_init", None)
+
+        if slot_init and widget.refresh:
+            widget.refresh = False  # Default to False before calling init where you can choose to set refresh to True.
+            slot_init(widget)
+
     def eventFilter(self, widget, event):
         """Filter out specific events related to the widget."""
         if event.type() == QtCore.QEvent.ChildPolished:
             child = event.child()
             if isinstance(child, QtWidgets.QWidget):
                 self.init_child(child)
 
         elif event.type() == QtCore.QEvent.Show:
             if widget is not self:
-                slot_init = widget.get_slot_init()
-                if slot_init and widget.refresh:
-                    widget.refresh = False  # Default to False before calling init where you can choose to set refresh to True.
-                    slot_init(widget)
-
-            if not widget.is_initialized:
-                self.sb.restore_widget_state(widget)
-                widget.is_initialized = True
+                for relative in self.sb.get_ui_relatives(
+                    widget.ui, exact=True, upstream=True, downstream=True
+                ):
+                    rel_widget = getattr(relative, widget.name, None)
+                    if rel_widget is not None:
+                        rel_widget.init_slot()
+
+                if not widget.is_initialized:
+                    self.sb.restore_widget_state(widget)
+                    widget.is_initialized = True
 
         return super().eventFilter(widget, event)
 
     def setVisible(self, state):
         """Called every time the widget is shown or hidden on screen.
         If the widget is set to be prevented from hiding, it will not be hidden when state is False.
```

### Comparing `uitk-0.7.3/uitk/widgets/__init__.py` & `uitk-0.7.4/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/attributeWindow.py` & `uitk-0.7.4/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/checkBox.py` & `uitk-0.7.4/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/comboBox.py` & `uitk-0.7.4/uitk/widgets/comboBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/draggableHeader.py` & `uitk-0.7.4/uitk/widgets/draggableHeader.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/expandableList.py` & `uitk-0.7.4/uitk/widgets/expandableList.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/label.py` & `uitk-0.7.4/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/lineEdit.py` & `uitk-0.7.4/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/menu.py` & `uitk-0.7.4/uitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/messageBox.py` & `uitk-0.7.4/uitk/widgets/messageBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/__init__.py` & `uitk-0.7.4/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/attributes.py` & `uitk-0.7.4/uitk/widgets/mixins/attributes.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/convert.py` & `uitk-0.7.4/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/docking.py` & `uitk-0.7.4/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/menu_instance.py` & `uitk-0.7.4/uitk/widgets/mixins/menu_instance.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/state_manager.py` & `uitk-0.7.4/uitk/widgets/mixins/state_manager.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/style_sheet.py` & `uitk-0.7.4/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/tasks.py` & `uitk-0.7.4/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/mixins/text.py` & `uitk-0.7.4/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/optionBox.py` & `uitk-0.7.4/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/progressBar.py` & `uitk-0.7.4/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/pushButton.py` & `uitk-0.7.4/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/region.py` & `uitk-0.7.4/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk/widgets/textEdit.py` & `uitk-0.7.4/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk.egg-info/PKG-INFO` & `uitk-0.7.4/uitk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.3
+Version: 0.7.4
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
@@ -16,20 +16,21 @@
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots and styles, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
 
 - Dynamic UI file loading
-- Custom widget registration and usage
+- Custom widget registration
 - Utility properties for MainWindow and child widget subclassing
-- Efficient management of slot connections and event handling
+- Management of slot connections and event handling
 - Support for UI hierarchy navigation and submenus
 - Custom event behavior through UI tags
 - UI and slot history storage and retrieval
+- Widget syncing and state management.
 
 ## Module Overview
 
 Module | Description
 ------- | -------
 [switchboard](https://github.com/m3trik/uitk/blob/main/uitk/switchboard.py) | Handles dynamic UI loading, assigns convenience properties, and manages slot connections.
 [events](https://github.com/m3trik/uitk/blob/main/uitk/events.py) | Manages event handling for dynamic UI widgets.
```

### Comparing `uitk-0.7.3/uitk.egg-info/PKG-INFO.bak` & `uitk-0.7.4/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk.egg-info/SOURCES.txt` & `uitk-0.7.4/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-0.7.3/uitk.egg-info/SOURCES.txt.bak` & `uitk-0.7.4/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

