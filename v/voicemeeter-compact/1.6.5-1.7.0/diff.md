# Comparing `tmp/voicemeeter-compact-1.6.5.tar.gz` & `tmp/voicemeeter-compact-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-compact-1.6.5.tar", max compression
+gzip compressed data, was "voicemeeter-compact-1.7.0.tar", max compression
```

## Comparing `voicemeeter-compact-1.6.5.tar` & `voicemeeter-compact-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.6.5/LICENSE
--rw-r--r--   0        0        0      716 2022-10-19 13:52:20.737199 voicemeeter-compact-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.6.5/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.6.5/vmcompact/__init__.py
--rw-r--r--   0        0        0     4007 2022-10-19 13:37:51.433827 voicemeeter-compact-1.6.5/vmcompact/app.py
--rw-r--r--   0        0        0     1022 2022-07-07 14:44:58.583605 voicemeeter-compact-1.6.5/vmcompact/banner.py
--rw-r--r--   0        0        0    23199 2022-10-05 21:58:29.117384 voicemeeter-compact-1.6.5/vmcompact/builders.py
--rw-r--r--   0        0        0    10621 2022-10-05 22:30:49.614304 voicemeeter-compact-1.6.5/vmcompact/channels.py
--rw-r--r--   0        0        0     8656 2022-09-15 23:39:31.398225 voicemeeter-compact-1.6.5/vmcompact/config.py
--rw-r--r--   0        0        0     1475 2022-09-29 09:49:37.500035 voicemeeter-compact-1.6.5/vmcompact/configurations.py
--rw-r--r--   0        0        0     1882 2022-09-15 22:41:23.144367 voicemeeter-compact-1.6.5/vmcompact/data.py
--rw-r--r--   0        0        0       87 2022-07-07 14:44:58.586603 voicemeeter-compact-1.6.5/vmcompact/errors.py
--rw-r--r--   0        0        0     8752 2022-10-05 22:34:24.004350 voicemeeter-compact-1.6.5/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.6.5/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    14180 2022-10-19 13:44:53.007069 voicemeeter-compact-1.6.5/vmcompact/menu.py
--rw-r--r--   0        0        0     3660 2022-09-29 11:21:34.528069 voicemeeter-compact-1.6.5/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.6.5/vmcompact/subject.py
--rw-r--r--   0        0        0     7177 2022-10-19 13:55:13.566630 voicemeeter-compact-1.6.5/setup.py
--rw-r--r--   0        0        0     6853 2022-10-19 13:55:13.566630 voicemeeter-compact-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.7.0/LICENSE
+-rw-r--r--   0        0        0      729 2023-06-26 11:42:27.727679 voicemeeter-compact-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.7.0/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.7.0/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-26 12:54:41.153598 voicemeeter-compact-1.7.0/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.7.0/vmcompact/banner.py
+-rw-r--r--   0        0        0    23293 2023-06-25 22:00:45.712304 voicemeeter-compact-1.7.0/vmcompact/builders.py
+-rw-r--r--   0        0        0    10827 2023-06-24 21:16:46.007160 voicemeeter-compact-1.7.0/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.7.0/vmcompact/config.py
+-rw-r--r--   0        0        0     1771 2023-06-26 08:23:22.875020 voicemeeter-compact-1.7.0/vmcompact/configurations.py
+-rw-r--r--   0        0        0     1882 2022-09-15 22:41:23.144367 voicemeeter-compact-1.7.0/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.7.0/vmcompact/errors.py
+-rw-r--r--   0        0        0     8878 2023-06-24 22:19:08.257020 voicemeeter-compact-1.7.0/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.7.0/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    14589 2023-06-26 12:22:49.788371 voicemeeter-compact-1.7.0/vmcompact/menu.py
+-rw-r--r--   0        0        0     3705 2023-06-26 08:38:15.234618 voicemeeter-compact-1.7.0/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.7.0/vmcompact/subject.py
+-rw-r--r--   0        0        0     7183 2023-06-26 13:01:33.303290 voicemeeter-compact-1.7.0/setup.py
+-rw-r--r--   0        0        0     6857 2023-06-26 13:01:33.304290 voicemeeter-compact-1.7.0/PKG-INFO
```

### Comparing `voicemeeter-compact-1.6.5/LICENSE` & `voicemeeter-compact-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.6.5/pyproject.toml` & `voicemeeter-compact-1.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.6.5"
+version = "1.7.0"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
-packages = [
-    { include = "vmcompact" },
-]
+packages = [{ include = "vmcompact" }]
 include = ["vmcompact/img/cat.ico"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sv-ttk = "^2.0"
+sv-ttk = "^2.4.5"
 tomli = { version = "^2.0.1", python = "<3.11" }
-voicemeeter-api = "^0.8.4"
-vban-cmd = "^1.8.1"
+voicemeeter-api = "^2.0.1"
+vban-cmd = "^2.0.0"
 
 [tool.poetry.dev-dependencies]
-black = {version = "^22.6.0", allow-prereleases = true}
+black = { version = "^22.6.0", allow-prereleases = true }
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voicemeeter-compact-1.6.5/README.md` & `voicemeeter-compact-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.6.5/vmcompact/app.py` & `voicemeeter-compact-1.7.0/vmcompact/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tkinter as tk
 from pathlib import Path
 from tkinter import ttk
 from typing import NamedTuple
 
 from .builders import MainFrameBuilder
 from .data import _base_values, _configuration, _kinds_all
-from .errors import VMCompactErrors
+from .errors import VMCompactError
 from .menu import Menus
 from .subject import Subject
 
 
 class App(tk.Tk):
     """App mainframe"""
 
@@ -30,16 +30,16 @@
         )
         return APP_cls
 
     def __init__(self, vmr):
         super().__init__()
 
         self._vmr = vmr
-        self._vmr.event.ldirty = True
-        self._vmr.event.remove(["mdirty", "midi"])
+        self._vmr.event.add(["pdirty", "ldirty"])
+        self._vmr.init_thread()
         icon_path = Path(__file__).parent.resolve() / "img" / "cat.ico"
         if icon_path.is_file():
             self.iconbitmap(str(icon_path))
         self.minsize(275, False)
         self.subject = Subject()
         self["menu"] = Menus(self, vmr)
         self.styletable = ttk.Style()
@@ -47,14 +47,17 @@
             vmr.apply_config(_configuration.config)
 
         self.build_app()
 
         self.drag_id = ""
         self.bind("<Configure>", self.dragging)
 
+    def __str__(self):
+        return f"{type(self).__name__}App"
+
     @property
     def target(self):
         """returns the current interface"""
 
         return self._vban if _base_values.vban_connected else self._vmr
 
     @property
@@ -71,36 +74,36 @@
 
     def build_app(self, kind=None, vban=None):
         """builds the app frames according to a kind"""
         self._vban = vban
         if kind:
             self.kind = kind
 
-        # register app as observer
-        self.target.subject.add(self)
+        # register event callbacks
+        self.target.subject.add([self.on_pdirty, self.on_ldirty])
 
         self.bus_frame = None
         self.submix_frame = None
         self.builder = MainFrameBuilder(self)
         self.builder.setup()
         self.builder.create_channelframe("strip")
         self.builder.create_separator()
         self.builder.create_navframe()
         if _configuration.extended:
             self.nav_frame.extend.set(True)
             self.nav_frame.extend_frame()
         if self.kind.name == "potato":
             self.builder.create_banner()
 
-    def on_update(self, subject):
-        """called whenever notified of update"""
-
-        if subject == "pdirty" and _base_values.run_update:
+    def on_pdirty(self):
+        if _base_values.run_update:
             self.after(1, self.subject.notify, "pdirty")
-        elif subject == "ldirty" and not _base_values.dragging:
+
+    def on_ldirty(self):
+        if not _base_values.dragging:
             self.after(1, self.subject.notify, "ldirty")
 
     def _destroy_top_level_frames(self):
         """
         Clear observables.
 
         Deregister app as observer.
@@ -133,9 +136,9 @@
 
 def connect(kind_id: str, vmr) -> App:
     """return App of the kind requested"""
 
     try:
         VMMIN_cls = _apps[kind_id]
     except KeyError:
-        raise VMCompactErrors(f"Invalid kind: {kind_id}")
+        raise VMCompactError(f"Invalid kind: {kind_id}")
     return VMMIN_cls(vmr)
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/builders.py` & `voicemeeter-compact-1.7.0/vmcompact/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from .banner import Banner
 from .channels import _make_channelframe
 from .config import BusConfig, StripConfig
 from .data import _base_values, _configuration
 from .navigation import Navigation
 
+logger = logging.getLogger(__name__)
+
 
 class AbstractBuilder(abc.ABC):
     @abc.abstractmethod
     def setup(self):
         """register as observable"""
         pass
 
@@ -24,19 +26,18 @@
         """deregister as observable"""
         pass
 
 
 class MainFrameBuilder(AbstractBuilder):
     """Responsible for building the frames that sit directly on the mainframe"""
 
-    logger = logging.getLogger("builders.mainframebuilder")
-
     def __init__(self, app):
         self.kind = app.kind
         self.app = app
+        self.logger = logger.getChild(self.__class__.__name__)
 
     def setup(self):
         self.app.title(
             f'Voicemeeter{self.kind}.Compact [{"Local" if not _base_values.vban_connected else "Network"} Connection]'
         )
         self.app.resizable(False, False)
         if _configuration.themes_enabled:
@@ -332,15 +333,15 @@
     """Responsible for building channel configframe widgets"""
 
     def setup(self):
         if self.configframe.parent.kind.name == "basic":
             self.configframe.slider_params = ("audibility",)
             self.configframe.slider_vars = (tk.DoubleVar(),)
         else:
-            self.configframe.slider_params = ("comp", "gate", "limit")
+            self.configframe.slider_params = ("comp.knob", "gate.knob", "limit")
             self.configframe.slider_vars = [
                 tk.DoubleVar() for _ in self.configframe.slider_params
             ]
 
         self.configframe.phys_out_params = [
             f"A{i+1}" for i in range(self.configframe.phys_out)
         ]
@@ -389,48 +390,48 @@
         comp_scale = ttk.Scale(
             self.configframe,
             from_=0.0,
             to=10.0,
             orient="horizontal",
             length=_configuration.level_width,
             variable=self.configframe.slider_vars[
-                self.configframe.slider_params.index("comp")
+                self.configframe.slider_params.index("comp.knob")
             ],
-            command=partial(self.configframe.scale_callback, "comp"),
+            command=partial(self.configframe.scale_callback, "comp.knob"),
         )
         comp_scale.bind(
-            "<Double-Button-1>", partial(self.configframe.reset_scale, "comp", 0)
+            "<Double-Button-1>", partial(self.configframe.reset_scale, "comp.knob", 0)
         )
         comp_scale.bind("<Button-1>", self.configframe.scale_press)
         comp_scale.bind("<ButtonRelease-1>", self.configframe.scale_release)
-        comp_scale.bind("<Enter>", partial(self.configframe.scale_enter, "comp"))
+        comp_scale.bind("<Enter>", partial(self.configframe.scale_enter, "comp.knob"))
         comp_scale.bind("<Leave>", self.configframe.scale_leave)
 
         comp_label.grid(column=0, row=0)
         comp_scale.grid(column=1, row=0)
 
     def create_gate_slider(self):
         gate_label = ttk.Label(self.configframe, text="Gate")
         gate_scale = ttk.Scale(
             self.configframe,
             from_=0.0,
             to=10.0,
             orient="horizontal",
             length=_configuration.level_width,
             variable=self.configframe.slider_vars[
-                self.configframe.slider_params.index("gate")
+                self.configframe.slider_params.index("gate.knob")
             ],
-            command=partial(self.configframe.scale_callback, "gate"),
+            command=partial(self.configframe.scale_callback, "gate.knob"),
         )
         gate_scale.bind(
-            "<Double-Button-1>", partial(self.configframe.reset_scale, "gate", 0)
+            "<Double-Button-1>", partial(self.configframe.reset_scale, "gate.knob", 0)
         )
         gate_scale.bind("<Button-1>", self.configframe.scale_press)
         gate_scale.bind("<ButtonRelease-1>", self.configframe.scale_release)
-        gate_scale.bind("<Enter>", partial(self.configframe.scale_enter, "gate"))
+        gate_scale.bind("<Enter>", partial(self.configframe.scale_enter, "gate.knob"))
         gate_scale.bind("<Leave>", self.configframe.scale_leave)
 
         gate_label.grid(column=2, row=0)
         gate_scale.grid(column=3, row=0)
 
     def create_limit_slider(self):
         limit_label = ttk.Label(self.configframe, text="Limit")
@@ -559,15 +560,15 @@
             "upmix61": "Up Mix 6.1",
             "centeronly": "Center Only",
             "lfeonly": "LFE Only",
             "rearonly": "Rear Only",
         }
         self.configframe.bus_modes = list(self.configframe.bus_mode_map.keys())
         # fmt: on
-        self.configframe.params = ("mono", "eq", "eq_ab")
+        self.configframe.params = ("mono", "eq.on", "eq.ab")
         self.configframe.param_vars = [tk.BooleanVar() for _ in self.configframe.params]
         self.configframe.bus_mode_label_text = tk.StringVar(
             value=self.configframe.bus_mode_map[self.configframe.current_bus_mode()]
         )
 
     def create_bus_mode_button(self):
         self.configframe.busmode_button = ttk.Button(
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/channels.py` & `voicemeeter-compact-1.7.0/vmcompact/channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 import tkinter as tk
-from math import log
 from tkinter import ttk
 
 from . import builders
 from .data import _base_values, _configuration
 
+logger = logging.getLogger(__name__)
+
 
 class ChannelLabelFrame(ttk.LabelFrame):
     """Base class for a single channel"""
 
     def __init__(self, parent, index, id):
         super().__init__(parent)
         self.parent = parent
         self.index = index
         self.id = id
+        self.logger = logger.getChild(self.__class__.__name__)
         self.styletable = self.parent.parent.styletable
 
         self.builder = builders.ChannelLabelFrameBuilder(self, index, id)
         self.builder.setup()
         self.builder.add_progressbar()
         self.builder.add_scale()
         self.builder.add_mute_button()
@@ -36,26 +39,29 @@
     @property
     def target(self):
         """returns the current interface"""
 
         return self.parent.target
 
     def getter(self, param):
-        if hasattr(self.target, param):
+        try:
             return getattr(self.target, param)
+        except AttributeError as e:
+            self.logger(f"{type(e).__name__}: {e}")
 
     def setter(self, param, value):
-        if hasattr(self.target, param):
+        if param in dir(self.target):  # avoid calling getattr (with hasattr)
             setattr(self.target, param, value)
 
     def scale_callback(self, *args):
         """callback function for scale widget"""
 
-        self.setter("gain", self.gain.get())
-        self.gainlabel.set(round(self.gain.get(), 1))
+        val = round(self.gain.get(), 1)
+        self.setter("gain", val)
+        self.gainlabel.set(val)
 
     def toggle_mute(self, *args):
         self.target.mute = self.mute.get()
         if not _configuration.themes_enabled:
             self.styletable.configure(
                 f"{self.identifier}Mute{self.index}.TButton",
                 background=f'{"red" if self.mute.get() else "white"}',
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/config.py` & `voicemeeter-compact-1.7.0/vmcompact/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import tkinter as tk
-from functools import partial
+import logging
 from tkinter import ttk
 
 from . import builders
 from .data import _base_values, _configuration
 
+logger = logging.getLogger(__name__)
+
 
 class Config(ttk.Frame):
     def __init__(self, parent, index, _id):
         super().__init__(parent)
         self.parent = parent
         self.index = index
         self.id = _id
+        self.logger = logger.getChild(self.__class__.__name__)
         self.styletable = parent.styletable
         self.phys_in, self.virt_in = parent.kind.ins
         self.phys_out, self.virt_out = parent.kind.outs
 
         self.parent.subject.add(self)
 
     @property
@@ -25,20 +27,34 @@
     @property
     def target(self):
         """returns the current interface"""
 
         return self.parent.target
 
     def getter(self, param):
-        if hasattr(self.target, param):
-            return getattr(self.target, param)
+        param = param.split(".")
+        try:
+            if len(param) == 2:
+                target = getattr(self.target, param[0])
+                return getattr(target, param[1])
+            else:
+                return getattr(self.target, param[0])
+        except AttributeError as e:
+            self.logger.error(f"{type(e).__name__}: {e}")
 
     def setter(self, param, value):
-        if hasattr(self.target, param):
-            setattr(self.target, param, value)
+        param = param.split(".")
+        try:
+            if len(param) == 2:
+                target = getattr(self.target, param[0])
+                setattr(target, param[1], value)
+            else:
+                setattr(self.target, param[0], value)
+        except AttributeError as e:
+            self.logger(f"{type(e).__name__}: {e}")
 
     def scale_press(self, *args):
         self.after(1, self.remove_events)
 
     def remove_events(self):
         self.parent.target.event.remove("pdirty")
         self.parent.target.event.remove("ldirty")
@@ -62,15 +78,15 @@
     def scale_leave(self, *args):
         self.parent.nav_frame.info_text.set("")
 
     def scale_callback(self, param, *args):
         """callback function for scale widget"""
 
         val = self.slider_vars[self.slider_params.index(param)].get()
-        self.setter(param, val)
+        self.setter(param, round(val, 1))
         self.parent.nav_frame.info_text.set(round(val, 1))
 
     def reset_scale(self, param, val, *args):
         self.setter(param, val)
         self.slider_vars[self.slider_params.index(param)].set(val)
 
     def toggle_p(self, param):
@@ -94,14 +110,15 @@
         self.builder = builders.StripConfigFrameBuilder(self)
         self.builder.setup()
         self.make_row_0()
         self.make_row_1()
         self.make_row_2()
         self.builder.grid_configure()
 
+        self.parent.target.clear_dirty()
         self.sync()
 
     @property
     def target(self):
         """returns the strip class for this configframe in the current interface"""
 
         _target = super(StripConfig, self).target
@@ -151,14 +168,20 @@
             self.virt_out_params_vars[i].set(self.getter(param))
             for i, param in enumerate(self.virt_out_params)
         ]
         [
             self.param_vars[i].set(self.getter(param))
             for i, param in enumerate(self.params)
         ]
+        if not _base_values.vban_connected:  # slider vars not defined in RT Packet
+            [
+                self.slider_vars[i].set(self.getter(param))
+                for i, param in enumerate(self.slider_params)
+                if self.index < self.phys_in
+            ]
 
         if not _configuration.themes_enabled:
             [
                 self.styletable.configure(
                     f"{param}.TButton",
                     background=f'{"green" if self.phys_out_params_vars[i].get() else "white"}',
                 )
@@ -189,14 +212,15 @@
             self.grid(column=0, row=3, columnspan=4, padx=(2,))
         self.builder = builders.BusConfigFrameBuilder(self)
         self.builder.setup()
         self.make_row_0()
         self.make_row_1()
         self.builder.grid_configure()
 
+        self.parent.target.clear_dirty()
         self.sync()
 
     @property
     def target(self):
         """returns the bus class for this configframe in the current interface"""
 
         _target = super(BusConfig, self).target
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/configurations.py` & `voicemeeter-compact-1.7.0/vmcompact/configurations.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 from pathlib import Path
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
-LOGGER = logging.getLogger("configurations")
+logger = logging.getLogger(__name__)
 
 configuration = {}
 
-config_path = [Path.cwd() / "configs"]
-for path in config_path:
-    if path.is_dir():
-        filenames = list(path.glob("*.toml"))
-        configs = {}
-        for filename in filenames:
-            name = filename.with_suffix("").stem
-            try:
-                with open(filename, "rb") as f:
-                    configs[name] = tomllib.load(f)
-            except tomllib.TOMLDecodeError:
-                print(f"Invalid TOML config: configs/{filename.stem}")
-
-        for name, cfg in configs.items():
-            LOGGER.info(f"Loaded configuration configs/{name}")
-            configuration[name] = cfg
+configpaths = [
+    Path.cwd() / "configs",
+    Path.home() / ".config" / "vm-compact" / "configs",
+    Path.home() / "Documents" / "Voicemeeter" / "configs",
+]
+for configpath in configpaths:
+    if configpath.is_dir():
+        filepaths = list(configpath.glob("*.toml"))
+        if any(f.stem in ("app", "vban") for f in filepaths):
+            configs = {}
+            for filepath in filepaths:
+                filename = filepath.with_suffix("").stem
+                if filename in ("app", "vban"):
+                    try:
+                        with open(filepath, "rb") as f:
+                            configs[filename] = tomllib.load(f)
+                        logger.info(f"{filename} loaded into memory")
+                    except tomllib.TOMLDecodeError:
+                        logger.error(f"Invalid TOML config: configs/{filename.stem}")
+
+            configuration |= configs
+            break
 
 _defaults = {
     "configs": {
         "config": None,
     },
     "theme": {
         "enabled": True,
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/data.py` & `voicemeeter-compact-1.7.0/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.6.5/vmcompact/gainlayer.py` & `voicemeeter-compact-1.7.0/vmcompact/gainlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tkinter as tk
-from math import log
 from tkinter import ttk
 
 from . import builders
 from .data import _base_values, _configuration
 
 
 class GainLayer(ttk.LabelFrame):
@@ -38,31 +37,34 @@
         return _target.strip[self.index].gainlayer[self.j]
 
     @property
     def identifier(self):
         return "gainlayer"
 
     def getter(self, param):
-        if hasattr(self.target, param):
+        try:
             return getattr(self.target, param)
+        except AttributeError as e:
+            self.logger(f"{type(e).__name__}: {e}")
 
     def setter(self, param, value):
-        if hasattr(self.target, param):
+        if param in dir(self.target):  # avoid calling getattr (with hasattr)
             setattr(self.target, param, value)
 
     def reset_gain(self, *args):
         self.setter("gain", 0)
         self.gain.set(0)
         self.gainlabel.set(self.gain.get())
 
     def scale_callback(self, *args):
         """callback function for scale widget"""
 
-        self.setter("gain", self.gain.get())
-        self.gainlabel.set(round(self.gain.get(), 1))
+        val = round(self.gain.get(), 1)
+        self.setter("gain", val)
+        self.gainlabel.set(val)
 
     def scale_press(self, *args):
         self.after(1, self.remove_events)
 
     def remove_events(self):
         self.parent.target.event.remove("pdirty")
         self.parent.target.event.remove("ldirty")
@@ -153,15 +155,16 @@
         """
 
         if self.parent.target.strip[self.index].levels.is_updated:
             val = max(self.parent.target.strip[self.index].levels.prefader)
             self.level.set(
                 (
                     0
-                    if self.parent.target.strip[self.index].mute or not self.on.get()
+                    if self.parent.parent.strip_frame.strips[self.index].mute.get()
+                    or not self.on.get()
                     else 72 + val - 12 + self.gain.get()
                 )
             )
 
     def grid_configure(self):
         [
             child.grid_configure(padx=1, pady=1, sticky=(tk.N, tk.S, tk.W, tk.E))
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/img/cat.ico` & `voicemeeter-compact-1.7.0/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.6.5/vmcompact/menu.py` & `voicemeeter-compact-1.7.0/vmcompact/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 import tkinter as tk
 import webbrowser
 from functools import partial
-from tkinter import messagebox, ttk
+from tkinter import messagebox
 
 import sv_ttk
 import vban_cmd
-from vban_cmd.error import VBANCMDError
+from vban_cmd.error import VBANCMDConnectionError
 
 from .data import _base_values, _configuration, get_configuration, kind_get
 
+logger = logging.getLogger(__name__)
 
-class Menus(tk.Menu):
-    logger = logging.getLogger("menu.menus")
 
+class Menus(tk.Menu):
     def __init__(self, parent, vmr):
         super().__init__()
         self.parent = parent
         self.vmr = vmr
+        self.logger = logger.getChild(self.__class__.__name__)
         self.vban_config = get_configuration("vban")
         self.app_config = get_configuration("app")
         self._is_topmost = tk.BooleanVar()
         self._lock = tk.BooleanVar()
         self._unlock = tk.BooleanVar()
         self._selected_bus = list(tk.BooleanVar() for _ in range(8))
 
@@ -209,22 +210,27 @@
     def action_set_voicemeeter(self, cmd, val=True):
         if cmd == "lock":
             self._lock.set(val)
             self._unlock.set(not self._lock.get())
         setattr(self.target.command, cmd, val)
 
     def load_profile(self, profile):
+        self.logger.info(f"loading user profile {profile}")
         self.target.apply_config(profile)
 
     def load_defaults(self):
-        resp = messagebox.askyesno(
-            message="Are you sure you want to Reset values to defaults?\nPhysical strips B1, Virtual strips A1\nMono, Solo, Mute, EQ all OFF"
+        msg = (
+            "Are you sure you want to Reset values to defaults?",
+            "Physical strips B1, Virtual strips A1",
+            "Mono, Solo, Mute, EQ all OFF",
+            "Gain sliders for Strip/Bus at 0.0",
         )
+        resp = messagebox.askyesno(message="\n".join(msg))
         if resp:
-            self.target.apply_config("reset")
+            self.load_profile("reset")
 
     def always_on_top(self):
         self.parent.attributes("-topmost", self._is_topmost.get())
 
     def switch_orientation(self, extends_horizontal: bool = True, *args):
         _configuration.extends_horizontal = extends_horizontal
         if extends_horizontal:
@@ -238,14 +244,15 @@
         if _configuration.submixes != i:
             _configuration.submixes = i
             if self.parent.submix_frame is not None:
                 self.parent.submix_frame.teardown()
                 self.parent.nav_frame.show_submix()
             for j, var in enumerate(self._selected_bus):
                 var.set(i == j)
+            self.parent.subject.notify("submix")
 
     def load_theme(self, theme):
         sv_ttk.set_theme(theme)
         _configuration.theme_mode = theme
         self.menu_themes.entryconfig(
             0,
             state=f"{'disabled' if theme == 'light' else 'normal'}",
@@ -308,24 +315,27 @@
         opts |= self.vban_config[f"connection-{i+1}"]
         kind_id = opts.pop("kind")
         self.vban = vban_cmd.api(kind_id, **opts)
         # login to vban interface
         try:
             self.logger.info(f"Attempting vban connection to {opts.get('ip')}")
             self.vban.login()
-        except VBANCMDError as e:
+        except VBANCMDConnectionError as e:
             self.vban.logout()
-            msg = (str(e), f"Please check your connection settings")
+            msg = (
+                f"Timeout attempting to establish connection to {opts.get('ip')}",
+                f"Please check your connection settings",
+            )
             messagebox.showerror("Connection Error", "\n".join(msg))
             msg = (str(e), f"resuming local connection")
             self.logger.error(", ".join(msg))
             self.after(1, self.enable_vban_menus)
             return
         self.menu_teardown(i)
-        self.vban.event.ldirty = True
+        self.vban.event.add(["pdirty", "ldirty"])
         # destroy the current App frames
         self.parent._destroy_top_level_frames()
         _base_values.vban_connected = True
         self.vmr.end_thread()
 
         # build new app frames according to a kind
         kind = kind_get(kind_id)
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/navigation.py` & `voicemeeter-compact-1.7.0/vmcompact/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import tkinter as tk
 from tkinter import ttk
 
 from . import builders
 from .data import _configuration
 from .gainlayer import SubMixFrame
 
+logger = logging.getLogger(__name__)
 
-class Navigation(ttk.Frame):
-    logger = logging.getLogger("navigation.navigation")
 
+class Navigation(ttk.Frame):
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
+        self.logger = logger.getChild(self.__class__.__name__)
         self.grid(row=0, column=3, padx=(0, 2), pady=(5, 5), sticky=(tk.W, tk.E))
         self.styletable = self.parent.styletable
 
         self.builder = builders.NavigationFrameBuilder(self)
         self.builder.setup()
         self.builder.create_submix_button()
         self.builder.create_channel_button()
```

### Comparing `voicemeeter-compact-1.6.5/vmcompact/subject.py` & `voicemeeter-compact-1.7.0/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.6.5/setup.py` & `voicemeeter-compact-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 packages = \
 ['vmcompact']
 
 package_data = \
 {'': ['*'], 'vmcompact': ['img/*']}
 
 install_requires = \
-['sv-ttk>=2.0,<3.0', 'vban-cmd>=1.8.1,<2.0.0', 'voicemeeter-api>=0.8.4,<0.9.0']
+['sv-ttk>=2.4.5,<3.0.0',
+ 'vban-cmd>=2.0.0,<3.0.0',
+ 'voicemeeter-api>=2.0.1,<3.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'voicemeeter-compact',
-    'version': '1.6.5',
+    'version': '1.7.0',
     'description': 'A Compact Voicemeeter Remote App',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![OS: Windows](https://img.shields.io/badge/os-windows-red)\n\n![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)\n\n# Voicemeeter Compact\n\nA compact Voicemeeter remote app, works locally and over LAN.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Prerequisites\n\n-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)\n-   Python 3.10 or greater\n\n## Installation\n\nFor a step-by-step guide [click here](INSTALLATION.md)\n\n```\npip install voicemeeter-compact\n```\n\n## Usage\n\nExample `__main__.py` file:\n\n```python\nimport voicemeeterlib\nimport vmcompact\n\n\ndef main():\n    # pass the kind_id and the vm object to the app\n    with voicemeeterlib.api(kind_id) as vm:\n        app = vmcompact.connect(kind_id, vm)\n        app.mainloop()\n\n\nif __name__ == "__main__":\n    # choose the kind of Voicemeeter (Local connection)\n    kind_id = "banana"\n\n    main()\n```\n\nIt\'s important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.\n\n![Image of unlabelled app](./doc_imgs/nolabels.png)\n\nIf the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).\n\n### kind_id\n\nSet the kind of Voicemeeter, kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## TOML Files\n\nThis is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.\nDirectly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.\nInside each kind directory you may place as many custom toml configurations as you wish.\n\n.\n\n├── `__main__.py`\n\n├── configs\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n## Configs\n\n### app.toml\n\nConfigure certain startup states for the app.\n\n-   `configs`\n    Configure a user config to load on app startup. Don\'t include the .toml extension in the config name.\n\n-   `theme`\n    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.\n\n-   `extends`\n    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.\n\n-   `channel`\n    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.\n\n-   `mwscroll_step`\n    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.\n\n-   `submixes`\n    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.\n\n### vban.toml\n\nConfigure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.\n\nFor vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.\n\nA valid `vban.toml` might look like this:\n\n```toml\n[connection-1]\nkind = \'banana\'\nip = \'192.168.1.2\'\nstreamname = \'worklaptop\'\nport = 6980\n\n[connection-2]\nkind = \'potato\'\nip = \'192.168.1.3\'\nstreamname = \'streampc\'\nport = 6990\n```\n\n### basic/ banana/ potato/\n\nThree example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the \'multiple-parameters\' section for more info:\n\n[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)\n\n[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)\n\nUser configs may be loaded at any time via the menu.\n\n## Special Thanks\n\n[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!\n\n[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-compact',
```

### Comparing `voicemeeter-compact-1.6.5/PKG-INFO` & `voicemeeter-compact-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.6.5
+Version: 1.7.0
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: sv-ttk (>=2.0,<3.0)
+Requires-Dist: sv-ttk (>=2.4.5,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
-Requires-Dist: vban-cmd (>=1.8.1,<2.0.0)
-Requires-Dist: voicemeeter-api (>=0.8.4,<0.9.0)
+Requires-Dist: vban-cmd (>=2.0.0,<3.0.0)
+Requires-Dist: voicemeeter-api (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-compact
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![OS: Windows](https://img.shields.io/badge/os-windows-red)
```

