# Comparing `tmp/voicemeeter-compact-1.7.0.tar.gz` & `tmp/voicemeeter-compact-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-compact-1.7.0.tar", max compression
+gzip compressed data, was "voicemeeter-compact-1.7.1.tar", max compression
```

## Comparing `voicemeeter-compact-1.7.0.tar` & `voicemeeter-compact-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.7.0/LICENSE
--rw-r--r--   0        0        0      729 2023-06-26 11:42:27.727679 voicemeeter-compact-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.7.0/README.md
--rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.7.0/vmcompact/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-26 12:54:41.153598 voicemeeter-compact-1.7.0/vmcompact/app.py
--rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.7.0/vmcompact/banner.py
--rw-r--r--   0        0        0    23293 2023-06-25 22:00:45.712304 voicemeeter-compact-1.7.0/vmcompact/builders.py
--rw-r--r--   0        0        0    10827 2023-06-24 21:16:46.007160 voicemeeter-compact-1.7.0/vmcompact/channels.py
--rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.7.0/vmcompact/config.py
--rw-r--r--   0        0        0     1771 2023-06-26 08:23:22.875020 voicemeeter-compact-1.7.0/vmcompact/configurations.py
--rw-r--r--   0        0        0     1882 2022-09-15 22:41:23.144367 voicemeeter-compact-1.7.0/vmcompact/data.py
--rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.7.0/vmcompact/errors.py
--rw-r--r--   0        0        0     8878 2023-06-24 22:19:08.257020 voicemeeter-compact-1.7.0/vmcompact/gainlayer.py
--rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.7.0/vmcompact/img/cat.ico
--rw-r--r--   0        0        0    14589 2023-06-26 12:22:49.788371 voicemeeter-compact-1.7.0/vmcompact/menu.py
--rw-r--r--   0        0        0     3705 2023-06-26 08:38:15.234618 voicemeeter-compact-1.7.0/vmcompact/navigation.py
--rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.7.0/vmcompact/subject.py
--rw-r--r--   0        0        0     7183 2023-06-26 13:01:33.303290 voicemeeter-compact-1.7.0/setup.py
--rw-r--r--   0        0        0     6857 2023-06-26 13:01:33.304290 voicemeeter-compact-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-04-11 12:14:57.626259 voicemeeter-compact-1.7.1/LICENSE
+-rw-r--r--   0        0        0      729 2023-06-26 15:07:46.680784 voicemeeter-compact-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6125 2022-09-03 16:03:26.518297 voicemeeter-compact-1.7.1/README.md
+-rw-r--r--   0        0        0       51 2022-07-07 14:44:58.582602 voicemeeter-compact-1.7.1/vmcompact/__init__.py
+-rw-r--r--   0        0        0     4248 2023-06-26 14:34:16.801058 voicemeeter-compact-1.7.1/vmcompact/app.py
+-rw-r--r--   0        0        0     1123 2023-06-24 22:06:19.553026 voicemeeter-compact-1.7.1/vmcompact/banner.py
+-rw-r--r--   0        0        0    23293 2023-06-25 22:00:45.712304 voicemeeter-compact-1.7.1/vmcompact/builders.py
+-rw-r--r--   0        0        0    10827 2023-06-24 21:16:46.007160 voicemeeter-compact-1.7.1/vmcompact/channels.py
+-rw-r--r--   0        0        0     9634 2023-06-26 08:40:26.219945 voicemeeter-compact-1.7.1/vmcompact/config.py
+-rw-r--r--   0        0        0     2438 2023-06-26 15:00:20.558979 voicemeeter-compact-1.7.1/vmcompact/configurations.py
+-rw-r--r--   0        0        0     1882 2022-09-15 22:41:23.144367 voicemeeter-compact-1.7.1/vmcompact/data.py
+-rw-r--r--   0        0        0       86 2023-06-25 11:25:22.327174 voicemeeter-compact-1.7.1/vmcompact/errors.py
+-rw-r--r--   0        0        0     8878 2023-06-24 22:19:08.257020 voicemeeter-compact-1.7.1/vmcompact/gainlayer.py
+-rw-r--r--   0        0        0   112922 2022-07-01 01:04:51.170192 voicemeeter-compact-1.7.1/vmcompact/img/cat.ico
+-rw-r--r--   0        0        0    16124 2023-06-26 14:51:26.442226 voicemeeter-compact-1.7.1/vmcompact/menu.py
+-rw-r--r--   0        0        0     3705 2023-06-26 08:38:15.234618 voicemeeter-compact-1.7.1/vmcompact/navigation.py
+-rw-r--r--   0        0        0      854 2022-08-02 08:43:15.749028 voicemeeter-compact-1.7.1/vmcompact/subject.py
+-rw-r--r--   0        0        0     7183 2023-06-26 15:09:12.001068 voicemeeter-compact-1.7.1/setup.py
+-rw-r--r--   0        0        0     6857 2023-06-26 15:09:12.001068 voicemeeter-compact-1.7.1/PKG-INFO
```

### Comparing `voicemeeter-compact-1.7.0/LICENSE` & `voicemeeter-compact-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/pyproject.toml` & `voicemeeter-compact-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-compact"
-version = "1.7.0"
+version = "1.7.1"
 description = "A Compact Voicemeeter Remote App"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-compact"
 
 packages = [{ include = "vmcompact" }]
```

### Comparing `voicemeeter-compact-1.7.0/README.md` & `voicemeeter-compact-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/app.py` & `voicemeeter-compact-1.7.1/vmcompact/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import tkinter as tk
+from functools import cached_property
 from pathlib import Path
 from tkinter import ttk
 from typing import NamedTuple
 
 from .builders import MainFrameBuilder
+from .configurations import loader
 from .data import _base_values, _configuration, _kinds_all
 from .errors import VMCompactError
 from .menu import Menus
 from .subject import Subject
 
 
 class App(tk.Tk):
@@ -37,14 +39,15 @@
         self._vmr.event.add(["pdirty", "ldirty"])
         self._vmr.init_thread()
         icon_path = Path(__file__).parent.resolve() / "img" / "cat.ico"
         if icon_path.is_file():
             self.iconbitmap(str(icon_path))
         self.minsize(275, False)
         self.subject = Subject()
+        self._configs = None
         self["menu"] = Menus(self, vmr)
         self.styletable = ttk.Style()
         if _configuration.config:
             vmr.apply_config(_configuration.config)
 
         self.build_app()
 
@@ -126,14 +129,19 @@
                 self.after_cancel(self.drag_id)
             self.drag_id = self.after(100, self.stop_drag)
 
     def stop_drag(self):
         self.drag_id = ""
         _base_values.dragging = False
 
+    @cached_property
+    def userconfigs(self):
+        self._configs = loader(self.kind.name)
+        return self._configs
+
 
 _apps = {kind.name: App.make(kind) for kind in _kinds_all}
 
 
 def connect(kind_id: str, vmr) -> App:
     """return App of the kind requested"""
```

### Comparing `voicemeeter-compact-1.7.0/vmcompact/banner.py` & `voicemeeter-compact-1.7.1/vmcompact/banner.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/builders.py` & `voicemeeter-compact-1.7.1/vmcompact/builders.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/channels.py` & `voicemeeter-compact-1.7.1/vmcompact/channels.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/config.py` & `voicemeeter-compact-1.7.1/vmcompact/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/configurations.py` & `voicemeeter-compact-1.7.1/vmcompact/configurations.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             configs = {}
             for filepath in filepaths:
                 filename = filepath.with_suffix("").stem
                 if filename in ("app", "vban"):
                     try:
                         with open(filepath, "rb") as f:
                             configs[filename] = tomllib.load(f)
-                        logger.info(f"{filename} loaded into memory")
+                        logger.info(f"configuration: {filename} loaded into memory")
                     except tomllib.TOMLDecodeError:
                         logger.error(f"Invalid TOML config: configs/{filename.stem}")
 
             configuration |= configs
             break
 
 _defaults = {
@@ -62,7 +62,23 @@
 else:
     configuration["app"] = _defaults
 
 
 def get_configuration(key):
     if key in configuration:
         return configuration[key]
+
+
+def loader(kind_id):
+    configs = {}
+    userconfigpath = Path.home() / ".config" / "vm-compact" / "configs" / kind_id
+    if userconfigpath.exists():
+        filepaths = list(userconfigpath.glob("*.toml"))
+        for filepath in filepaths:
+            identifier = filepath.with_suffix("").stem
+            try:
+                with open(filepath, "rb") as f:
+                    configs[identifier] = tomllib.load(f)
+                logger.info(f"loader: {identifier} loaded into memory")
+            except tomllib.TOMLDecodeError:
+                logger.error(f"Invalid TOML config: configs/{filename.stem}")
+    return configs
```

### Comparing `voicemeeter-compact-1.7.0/vmcompact/data.py` & `voicemeeter-compact-1.7.1/vmcompact/data.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/gainlayer.py` & `voicemeeter-compact-1.7.1/vmcompact/gainlayer.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/img/cat.ico` & `voicemeeter-compact-1.7.1/vmcompact/img/cat.ico`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/menu.py` & `voicemeeter-compact-1.7.1/vmcompact/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,22 @@
             [
                 self.menu_configs_load.add_command(
                     label=profile, command=partial(self.load_profile, profile)
                 )
                 for profile in self.target.configs.keys()
                 if profile not in self.config_defaults
             ]
+        elif self.parent.userconfigs:
+            [
+                self.menu_configs_load.add_command(
+                    label=name, command=partial(self.load_custom_profile, data)
+                )
+                for name, data in self.parent.userconfigs.items()
+                if name not in self.config_defaults
+            ]
         else:
             self.menu_configs.entryconfig(0, state="disabled")
         self.menu_configs.add_command(
             label="Reset to defaults", command=self.load_defaults
         )
 
         # layout menu
@@ -209,14 +217,18 @@
 
     def action_set_voicemeeter(self, cmd, val=True):
         if cmd == "lock":
             self._lock.set(val)
             self._unlock.set(not self._lock.get())
         setattr(self.target.command, cmd, val)
 
+    def load_custom_profile(self, profile):
+        self.logger.info(f"loading user profile {profile}")
+        self.target.apply(profile)
+
     def load_profile(self, profile):
         self.logger.info(f"loading user profile {profile}")
         self.target.apply_config(profile)
 
     def load_defaults(self):
         msg = (
             "Are you sure you want to Reset values to defaults?",
@@ -285,14 +297,19 @@
     def menu_teardown(self, i):
         # remove config load menus
         [
             self.menu_configs_load.delete(key)
             for key in self.target.configs.keys()
             if key not in self.config_defaults
         ]
+        [
+            self.menu_configs_load.delete(key)
+            for key in self.parent.userconfigs.keys()
+            if key not in self.config_defaults
+        ]
 
         [
             self.menu_vban.entryconfig(j, state="disabled")
             for j, _ in enumerate(self.menu_vban.winfo_children())
             if j != i
         ]
 
@@ -303,14 +320,22 @@
             [
                 self.menu_configs_load.add_command(
                     label=profile, command=partial(self.load_profile, profile)
                 )
                 for profile in self.target.configs.keys()
                 if profile not in self.config_defaults
             ]
+        elif self.parent.userconfigs:
+            [
+                self.menu_configs_load.add_command(
+                    label=name, command=partial(self.load_custom_profile, data)
+                )
+                for name, data in self.parent.userconfigs.items()
+                if name not in self.config_defaults
+            ]
         else:
             self.menu_configs.entryconfig(0, state="disabled")
 
     def vban_connect(self, i):
         opts = {}
         opts |= self.vban_config[f"connection-{i+1}"]
         kind_id = opts.pop("kind")
@@ -342,14 +367,19 @@
         self.parent.build_app(kind, self.vban)
         target_menu = getattr(self, f"menu_vban_{i+1}")
         target_menu.entryconfig(0, state="disabled")
         target_menu.entryconfig(1, state="normal")
         self.menu_layout.entryconfig(
             0, state=f"{'normal' if kind.name == 'potato' else 'disabled'}"
         )
+        # ensure the configs are reloaded into memory
+        if "config" in self.parent.target.__dict__:
+            del self.parent.target.__dict__["config"]
+        if "userconfigs" in self.parent.__dict__:
+            del self.parent.__dict__["userconfigs"]
         self.menu_setup()
 
     def vban_disconnect(self, i):
         self.menu_teardown(i)
 
         # destroy the current App frames
         self.parent._destroy_top_level_frames()
@@ -362,14 +392,19 @@
         self.parent.build_app(kind, None)
         target_menu = getattr(self, f"menu_vban_{i+1}")
         target_menu.entryconfig(0, state="normal")
         target_menu.entryconfig(1, state="disabled")
         self.menu_layout.entryconfig(
             0, state=f"{'normal' if kind.name == 'potato' else 'disabled'}"
         )
+        # ensure the configs are reloaded into memory
+        if "config" in self.parent.target.__dict__:
+            del self.parent.target.__dict__["config"]
+        if "userconfigs" in self.parent.__dict__:
+            del self.parent.__dict__["userconfigs"]
         self.menu_setup()
 
         self.after(15000, self.enable_vban_menus)
 
     def documentation(self):
         webbrowser.open_new(r"https://voicemeeter.com/")
```

### Comparing `voicemeeter-compact-1.7.0/vmcompact/navigation.py` & `voicemeeter-compact-1.7.1/vmcompact/navigation.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/vmcompact/subject.py` & `voicemeeter-compact-1.7.1/vmcompact/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-compact-1.7.0/setup.py` & `voicemeeter-compact-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'voicemeeter-api>=2.0.1,<3.0.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'voicemeeter-compact',
-    'version': '1.7.0',
+    'version': '1.7.1',
     'description': 'A Compact Voicemeeter Remote App',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-compact.svg)](https://badge.fury.io/py/voicemeeter-compact)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-compact/blob/main/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![OS: Windows](https://img.shields.io/badge/os-windows-red)\n\n![Image of app/potato size comparison](./doc_imgs/potatocomparisonsmaller.png)\n\n# Voicemeeter Compact\n\nA compact Voicemeeter remote app, works locally and over LAN.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Prerequisites\n\n-   [Voicemeeter](https://voicemeeter.com/) (Basic v1.0.8.4), (Banana v2.0.6.4) or (Potato v3.0.2.4)\n-   Python 3.10 or greater\n\n## Installation\n\nFor a step-by-step guide [click here](INSTALLATION.md)\n\n```\npip install voicemeeter-compact\n```\n\n## Usage\n\nExample `__main__.py` file:\n\n```python\nimport voicemeeterlib\nimport vmcompact\n\n\ndef main():\n    # pass the kind_id and the vm object to the app\n    with voicemeeterlib.api(kind_id) as vm:\n        app = vmcompact.connect(kind_id, vm)\n        app.mainloop()\n\n\nif __name__ == "__main__":\n    # choose the kind of Voicemeeter (Local connection)\n    kind_id = "banana"\n\n    main()\n```\n\nIt\'s important to know that only labelled strips and buses will appear in the Channel frames. Removing a Channels label will cause the GUI to grow/shrink in real time.\n\n![Image of unlabelled app](./doc_imgs/nolabels.png)\n\nIf the GUI looks like the above when you first load it, then no channels are labelled. From the menu, `Configs->Load config` you may load an example config. Save your current Voicemeeter settings first :).\n\n### kind_id\n\nSet the kind of Voicemeeter, kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## TOML Files\n\nThis is how your files should be organised. Wherever your `__main__.py` file is located (after install this can be any location), `configs` should be in the same location.\nDirectly inside of configs directory you may place an app.toml, vban.toml and a directory for each kind.\nInside each kind directory you may place as many custom toml configurations as you wish.\n\n.\n\n├── `__main__.py`\n\n├── configs\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── app.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── vban.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── basic\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── streaming_config.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── banana\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── other.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── potato\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── example.toml\n\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── ...\n\n## Configs\n\n### app.toml\n\nConfigure certain startup states for the app.\n\n-   `configs`\n    Configure a user config to load on app startup. Don\'t include the .toml extension in the config name.\n\n-   `theme`\n    By default the app loads up the [Sun Valley light or dark theme](https://github.com/rdbende/Sun-Valley-ttk-theme) by @rdbende. You have the option to load up the app without any theme loaded. Simply set `enabled` to false and `mode` will take no effect.\n\n-   `extends`\n    Extending the app will show both strips and buses. In reduced mode only one or the other. This app will extend both horizontally and vertically, simply set `extends_horizontal` true or false accordingly.\n\n-   `channel`\n    For each channel labelframe the width and height may be adjusted which effects the spacing between widgets and the length of the scales and progressbars respectively.\n\n-   `mwscroll_step`\n    Sets the amount (in db) the gain slider moves with a single mousewheel step. Default 3.\n\n-   `submixes`\n    Select the default submix bus when Submix frame is shown. For example, a dedicated bus for OBS.\n\n### vban.toml\n\nConfigure as many vban connections as you wish. This allows the app to work over a LAN connection as well as with a local Voicemeeter installation.\n\nFor vban connections to work correctly VBAN TEXT incoming stream MUST be configured correctly on the remote machine. Both pcs ought to be connected to a local private network and should be able to ping one another.\n\nA valid `vban.toml` might look like this:\n\n```toml\n[connection-1]\nkind = \'banana\'\nip = \'192.168.1.2\'\nstreamname = \'worklaptop\'\nport = 6980\n\n[connection-2]\nkind = \'potato\'\nip = \'192.168.1.3\'\nstreamname = \'streampc\'\nport = 6990\n```\n\n### basic/ banana/ potato/\n\nThree example user configs are included with the package, one for each kind of Voicemeeter. Use these to configure parameter startup states. Any parameter supported by the underlying interfaces may be used. Check the \'multiple-parameters\' section for more info:\n\n[Python Interface for Voicemeeter API](https://github.com/onyx-and-iris/voicemeeter-api-python#multiple-parameters)\n\n[Python Interface for VBAN CMD](https://github.com/onyx-and-iris/vban-cmd-python#multiple-parameters)\n\nUser configs may be loaded at any time via the menu.\n\n## Special Thanks\n\n[Vincent Burel](https://github.com/vburel2018) for creating Voicemeeter, its SDK, the C Remote API, the RT Packet service and Streamer View app!\n\n[Rdbende](https://github.com/rdbende) for creating the beautiful Sun Valley Tkinter theme and adding it to Pypi!\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-compact',
```

### Comparing `voicemeeter-compact-1.7.0/PKG-INFO` & `voicemeeter-compact-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-compact
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Compact Voicemeeter Remote App
 Home-page: https://github.com/onyx-and-iris/voicemeeter-compact
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

