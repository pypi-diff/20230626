# Comparing `tmp/plastik-0.4.2.tar.gz` & `tmp/plastik-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastik-0.4.2.tar", max compression
+gzip compressed data, was "plastik-0.4.3.tar", max compression
```

## Comparing `plastik-0.4.2.tar` & `plastik-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-23 15:13:38.774265 plastik-0.4.2/LICENSE
--rw-r--r--   0        0        0      818 2023-06-23 15:13:38.774265 plastik-0.4.2/README.md
--rw-r--r--   0        0        0     1050 2023-06-23 15:13:57.738723 plastik-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      263 2023-06-23 15:13:38.782267 plastik-0.4.2/src/plastik/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-23 15:13:38.782267 plastik-0.4.2/src/plastik/axes.py
--rw-r--r--   0        0        0     9597 2023-06-23 15:13:57.738723 plastik-0.4.2/src/plastik/colors.py
--rw-r--r--   0        0        0      942 2023-06-23 15:13:38.786268 plastik-0.4.2/src/plastik/default.mplstyle
--rw-r--r--   0        0        0     5514 2023-06-23 15:13:38.786268 plastik-0.4.2/src/plastik/legends.py
--rw-r--r--   0        0        0    12220 2023-06-23 15:13:38.786268 plastik-0.4.2/src/plastik/ridge.py
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 plastik-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-26 08:32:12.863410 plastik-0.4.3/LICENSE
+-rw-r--r--   0        0        0      820 2023-06-26 08:32:28.263753 plastik-0.4.3/README.md
+-rw-r--r--   0        0        0     1072 2023-06-26 08:32:28.263753 plastik-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/axes.py
+-rw-r--r--   0        0        0    11084 2023-06-26 08:32:28.263753 plastik-0.4.3/src/plastik/colors.py
+-rw-r--r--   0        0        0      942 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/default.mplstyle
+-rw-r--r--   0        0        0     5514 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/legends.py
+-rw-r--r--   0        0        0    12220 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/ridge.py
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 plastik-0.4.3/PKG-INFO
```

### Comparing `plastik-0.4.2/LICENSE` & `plastik-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plastik-0.4.2/README.md` & `plastik-0.4.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # plastik
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 > plt assist, plastic surgery for plt
 
-## TODO
-
-* Add and set up tests in pre-commit
-
 ## Install
 
-This module is available through [PyPI]:
+`plastik` is available through [PyPI]:
 
-```sh
+```bash
 pip install plastik
 ```
 
 Installing the development version is done using [poetry]:
 
-```sh
+```bash
 git clone https://github.com/engeir/plastik.git
 cd plastik
 poetry install
 ```
 
 ## Usage
 
 ### Functions
 
-* `dark_theme`
-* `log_tick_format`
-* `topside_legends`
+- `dark_theme`
+- `log_tick_format`
+- `topside_legends`
 
 ### Classes
 
-* `Ridge`
+- `Ridge`
 
 ### Example use
 
-See [examples](examples/example.ipynb).
+See [examples](./examples/example.py).
+
+## To do
+
+- Add and set up tests in pre-commit
 
 [PyPI]: https://pypi.org/
 [poetry]: https://python-poetry.org
```

### Comparing `plastik-0.4.2/pyproject.toml` & `plastik-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plastik"
-version = "0.4.2"
+version = "0.4.3"
 description = "plastic surgery for plt"
 authors = ["Eirik Rolland Enger <eirroleng@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/engeir/plastik"
 repository = "https://github.com/engeir/plastik"
 documentation = "https://plastik.readthedocs.io/en/latest/"
@@ -19,14 +19,15 @@
 python = "^3.8"
 numpy = "^1.21.4"
 matplotlib = "^3.5.0"
 attrs = "^21.4.0"
 importlib-metadata = "^6.1.0"
 pywaffle = "^1.1.0"
 cmcrameri = "^1.5"
+palettable = "^3.3.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.10.1"
 pre-commit = "^2.15.0"
 pre-commit-hooks = "^4.0.1"
 pyupgrade = "^2.29.1"
```

### Comparing `plastik-0.4.2/src/plastik/axes.py` & `plastik-0.4.3/src/plastik/axes.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.2/src/plastik/colors.py` & `plastik-0.4.3/src/plastik/colors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import inspect
 import sys
 from typing import Literal, Sequence, overload
 
 import cmcrameri  # noqa
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
+import palettable  # noqa
 import pywaffle
 
 
 @overload
 def create_colorlist(
     color_specifier: Sequence | str, n: int, map: Literal[False] = False
 ) -> list[str]:
@@ -58,15 +60,28 @@
     Raises
     ------
     AttributeError
         If the type of the ``color_specifier`` is not recognized.
 
     See also
     --------
-    cosmoplots.generate_hex_colors : Color generator based on standard color maps.
+    `Palettable<https://jiffyclub.github.io/palettable/#documentation>`_ is a collection
+    of predefined colour maps that include the matplotlib colours, cmcrameri colours and
+    many more (colour maps from the Wes Anderson movies being one of them!). Let us look
+    at an example::
+
+        import matplotlib.pyplot as plt
+        from palettable.wesanderson import Moonrise1_5 as wes_clr
+        import plastik
+        plastik.colors.make_color_swatch(
+            plt.figure(figsize=(12, 3)).gca(),
+            wes_clr.hex_colors,
+        )
+
+    cosmoplots.generate_hex_colors : Color generator based on standard colour maps.
 
     Note
     ----
     With `colour<https://github.com/vaab/colour>`_ we can do it like this::
 
         import colour
         c_grad = [
@@ -158,14 +173,36 @@
         mpl.colors.to_hex(c)
         for c in mpl.colors.LinearSegmentedColormap.from_list("Custom", colors, N=n)(
             range(n)
         )
     ]
 
 
+def palettable_help() -> None:
+    print(
+        "This package includes `palettable` as a dependency, but do not implement any"
+        " of its colour maps. Rather, have a look at their documentation at"
+        " https://jiffyclub.github.io/palettable/#documentation and use it as its own"
+        " package. "
+    )
+    print(
+        "Integrating it with `plastik` is simple, just load any palette, and for"
+        " example call the `hex_colors` attribute they all have (again, see the"
+        " `palettable` documentation). This is a list of HEX colours that can then be"
+        " given to `make_color_swatch`."
+    )
+    print(
+        "And just to tease you a bit more, here is a list of the available colour"
+        " palette modules:"
+    )
+    for i in inspect.getmembers(palettable, inspect.ismodule):
+        if i[0] not in ["utils", "palette"]:
+            print("\t", i[0])
+
+
 def make_color_swatch(
     ax: plt.Axes,
     c_bar: mpl.colors.Colormap | list[str],
     vertical: bool = False,
     resolution: int = 90,
     ratio: int = 8,
     no_border: bool = False,
```

### Comparing `plastik-0.4.2/src/plastik/default.mplstyle` & `plastik-0.4.3/src/plastik/default.mplstyle`

 * *Files identical despite different names*

### Comparing `plastik-0.4.2/src/plastik/legends.py` & `plastik-0.4.3/src/plastik/legends.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.2/src/plastik/ridge.py` & `plastik-0.4.3/src/plastik/ridge.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.2/PKG-INFO` & `plastik-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastik
-Version: 0.4.2
+Version: 0.4.3
 Summary: plastic surgery for plt
 Home-page: https://github.com/engeir/plastik
 License: GPLv3
 Author: Eirik Rolland Enger
 Author-email: eirroleng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -14,58 +14,59 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: cmcrameri (>=1.5,<2.0)
 Requires-Dist: importlib-metadata (>=6.1.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
+Requires-Dist: palettable (>=3.3.3,<4.0.0)
 Requires-Dist: pywaffle (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://plastik.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/engeir/plastik
 Description-Content-Type: text/markdown
 
 # plastik
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 > plt assist, plastic surgery for plt
 
-## TODO
-
-* Add and set up tests in pre-commit
-
 ## Install
 
-This module is available through [PyPI]:
+`plastik` is available through [PyPI]:
 
-```sh
+```bash
 pip install plastik
 ```
 
 Installing the development version is done using [poetry]:
 
-```sh
+```bash
 git clone https://github.com/engeir/plastik.git
 cd plastik
 poetry install
 ```
 
 ## Usage
 
 ### Functions
 
-* `dark_theme`
-* `log_tick_format`
-* `topside_legends`
+- `dark_theme`
+- `log_tick_format`
+- `topside_legends`
 
 ### Classes
 
-* `Ridge`
+- `Ridge`
 
 ### Example use
 
-See [examples](examples/example.ipynb).
+See [examples](./examples/example.py).
+
+## To do
+
+- Add and set up tests in pre-commit
 
 [PyPI]: https://pypi.org/
 [poetry]: https://python-poetry.org
```

