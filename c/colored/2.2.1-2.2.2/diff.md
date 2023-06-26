# Comparing `tmp/colored-2.2.1.tar.gz` & `tmp/colored-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "colored-2.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-2.2.1.tar` & `colored-2.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3007 2023-06-25 19:28:05.000000 colored-2.2.1/README.md
--rw-r--r--   0        0        0      374 2023-06-25 19:28:05.000000 colored-2.2.1/colored/__init__.py
--rw-r--r--   0        0        0     2085 2023-06-25 19:28:05.000000 colored-2.2.1/colored/attributes.py
--rw-r--r--   0        0        0     2137 2023-06-25 19:28:05.000000 colored-2.2.1/colored/background.py
--rw-r--r--   0        0        0    10859 2023-06-25 19:28:05.000000 colored-2.2.1/colored/colored.py
--rw-r--r--   0        0        0     1966 2023-06-25 19:28:05.000000 colored-2.2.1/colored/controls.py
--rw-r--r--   0        0        0     1574 2023-06-25 19:28:05.000000 colored-2.2.1/colored/cprint.py
--rw-r--r--   0        0        0     1086 2023-06-25 19:28:05.000000 colored-2.2.1/colored/exceptions.py
--rw-r--r--   0        0        0     2105 2023-06-25 19:28:05.000000 colored-2.2.1/colored/foreground.py
--rw-r--r--   0        0        0     1854 2023-06-25 19:28:05.000000 colored-2.2.1/colored/hexadecimal.py
--rw-r--r--   0        0        0    15604 2023-06-25 19:28:05.000000 colored-2.2.1/colored/library.py
--rw-r--r--   0        0        0     2628 2023-06-25 19:28:05.000000 colored-2.2.1/colored/utilities.py
--rw-r--r--   0        0        0     1067 2023-06-25 19:28:05.000000 colored-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 colored-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3007 2023-06-26 14:22:25.000000 colored-2.2.2/README.md
+-rw-r--r--   0        0        0      374 2023-06-26 14:22:25.000000 colored-2.2.2/colored/__init__.py
+-rw-r--r--   0        0        0     1999 2023-06-26 14:22:25.000000 colored-2.2.2/colored/attributes.py
+-rw-r--r--   0        0        0     1774 2023-06-26 14:22:25.000000 colored-2.2.2/colored/background.py
+-rw-r--r--   0        0        0    10378 2023-06-26 14:22:25.000000 colored-2.2.2/colored/colored.py
+-rw-r--r--   0        0        0     1873 2023-06-26 14:22:25.000000 colored-2.2.2/colored/controls.py
+-rw-r--r--   0        0        0     1574 2023-06-26 14:22:25.000000 colored-2.2.2/colored/cprint.py
+-rw-r--r--   0        0        0     1086 2023-06-26 14:22:25.000000 colored-2.2.2/colored/exceptions.py
+-rw-r--r--   0        0        0     1742 2023-06-26 14:22:25.000000 colored-2.2.2/colored/foreground.py
+-rw-r--r--   0        0        0     1853 2023-06-26 14:22:25.000000 colored-2.2.2/colored/hexadecimal.py
+-rw-r--r--   0        0        0    15757 2023-06-26 14:22:25.000000 colored-2.2.2/colored/library.py
+-rw-r--r--   0        0        0     4006 2023-06-26 14:22:25.000000 colored-2.2.2/colored/utilities.py
+-rw-r--r--   0        0        0     1067 2023-06-26 14:22:25.000000 colored-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 colored-2.2.2/PKG-INFO
```

### Comparing `colored-2.2.1/README.md` & `colored-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `colored-2.2.1/colored/attributes.py` & `colored-2.2.2/colored/attributes.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
     _utils = Utilities()
     _ESC: str = Library.ESC
     _END: str = Library.END
     _STYLES: dict = Library.STYLES
     _UNDER: str = Library.UNDERLINE_COLOR
     _COLORS: dict = Library.COLORS
-    DEFAULT_STYLE: str = Library.DEFAULT_STYLE
-    default_style: str = DEFAULT_STYLE
 
     for _style, _code in _STYLES.items():
         vars()[_style] = f'{_ESC}{_code}{_END}'
         vars()[_style.upper()] = f'{_ESC}{_code}{_END}'
 
     @classmethod
     def underline_color(cls, color: str | int) -> str:
```

### Comparing `colored-2.2.1/colored/background.py` & `colored-2.2.2/colored/background.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 class Back(metaclass=MetaBack):
 
     _utils = Utilities()
     _END: str = Library.END
     _COLORS: dict = Library.COLORS
     _BACKGROUND_256: str = Library.BACKGROUND_256
     _BACKGROUND_RGB: str = Library.BACKGROUND_RGB
-    DEFAULT_BACKGROUND_256: str = Library.DEFAULT_BACKGROUND_256
-    DEFAULT_BACKGROUND_RGB: str = Library.DEFAULT_BACKGROUND_RGB
-    default_background_256: str = DEFAULT_BACKGROUND_256
-    default_background_rgb: str = DEFAULT_BACKGROUND_RGB
 
     for _color, _code in _COLORS.items():
         vars()[_color] = f'{_BACKGROUND_256}{_code}{_END}'
         vars()[_color.upper()] = f'{_BACKGROUND_256}{_code}{_END}'
 
     @classmethod
     def rgb(cls, r: int | str, g: int | str, b: int | str) -> str:
@@ -38,21 +34,16 @@
             r: Sets the Red color.
             g: Sets the Green color.
             b: Sets the Blue color.
 
         Returns:
             str: Background RGB code.
         """
-        r, g, b = cls._utils.is_percentages((r, g, b))
-
-        pattern: str = f'{cls._BACKGROUND_RGB}{r};{g};{b}{cls._END}'
-        if not any((r, g, b)):
-            pattern: str = cls.DEFAULT_BACKGROUND_RGB
-
-        return pattern
+        r, g, b = cls._utils.is_percentage((r, g, b))
+        return f'{cls._BACKGROUND_RGB}{r};{g};{b}{cls._END}'
 
     @classmethod
     def RGB(cls, r: int | str, g: int | str, b: int | str) -> str:
         """ Combination with text returns color background with text.
 
         Args:
             r: Sets the Red color.
```

### Comparing `colored-2.2.1/colored/colored.py` & `colored-2.2.2/colored/colored.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         self._hex_color: str = ''
         self._hex = Hex()
         self._utils = Utilities()
 
         self._ESC: str = Library.ESC
         self._END: str = Library.END
 
-        self.DEFAULT_STYLE: str = Library.DEFAULT_STYLE
-        self.DEFAULT_FOREGROUND_256: str = Library.DEFAULT_FOREGROUND_256
-        self.DEFAULT_BACKGROUND_256: str = Library.DEFAULT_BACKGROUND_256
-
         self._STYLES: dict = Library.STYLES
         self._FOREGROUND_256: str = Library.FOREGROUND_256
         self._BACKGROUND_256: str = Library.BACKGROUND_256
 
         self._COLORS: dict = Library.COLORS
         self._HEX_COLORS: dict = Library.HEX_COLORS
         self._UNDERLINE_COLOR: str = Library.UNDERLINE_COLOR
@@ -56,67 +52,64 @@
 
         Args:
             line_color: Sets color of the underline.
 
         Returns:
             str: Style code.
         """
-        if not self._name:
-            return self.DEFAULT_STYLE
-
-        self._utils.is_style_exist(self._name)
-
+        formatting: str = self._name
         if not self.enabled():
             return ''
 
-        if self._name in ('underline', '4') and line_color:
-            line_color: str = str(line_color).lower()
-            self._utils.is_color_exist(line_color)
-            if not line_color.isdigit():
-                line_color: str = self._COLORS[line_color]
-            return f'{self._UNDERLINE_COLOR}{line_color}{self._END}'
+        if self._name:
+            self._utils.is_style_exist(self._name)
+
+            if self._name in ('underline', '4') and line_color:
+                line_color: str = str(line_color).lower()
+                self._utils.is_color_exist(line_color)
+                if not line_color.isdigit():
+                    line_color: str = self._COLORS[line_color]
+                return f'{self._UNDERLINE_COLOR}{line_color}{self._END}'
 
-        if not self._name.isdigit():
-            self._name: str = self._STYLES[self._name]
+            if not self._name.isdigit():
+                formatting: str = self._STYLES[self._name]
 
-        return f'{self._ESC}{self._name}{self._END}'
+        return f'{self._ESC}{formatting}{self._END}'
 
     def foreground(self) -> str:
         """ Returns a foreground 256 color code. """
-        if not self._name:
-            return self.DEFAULT_FOREGROUND_256
-
-        self._utils.is_color_exist(self._name)
-
+        color: str = self._name
         if not self.enabled():
             return ''
 
-        if self._name.startswith('#'):
-            return f'{self._FOREGROUND_256}{self._hex_color}{self._END}'
-        elif not self._name.isdigit():
-            self._name: str = self._COLORS[self._name]
+        if self._name:
+            self._utils.is_color_exist(self._name)
+
+            if self._name.startswith('#'):
+                color: str = self._hex_color
+            elif not self._name.isdigit():
+                color: str = self._COLORS[self._name]
 
-        return f'{self._FOREGROUND_256}{self._name}{self._END}'
+        return f'{self._FOREGROUND_256}{color}{self._END}'
 
     def background(self) -> str:
         """ Returns a background 256 color code. """
-        if not self._name:
-            return self.DEFAULT_BACKGROUND_256
-
-        self._utils.is_color_exist(self._name)
-
+        color: str = self._name
         if not self.enabled():
             return ''
 
-        if self._name.startswith('#'):
-            return f'{self._BACKGROUND_256}{self._hex_color}{self._END}'
-        elif not self._name.isdigit():
-            self._name: str = self._COLORS[self._name]
+        if self._name:
+            self._utils.is_color_exist(self._name)
+
+            if self._name.startswith('#'):
+                color: str = self._hex_color
+            elif not self._name.isdigit():
+                color: str = self._COLORS[self._name]
 
-        return f'{self._BACKGROUND_256}{self._name}{self._END}'
+        return f'{self._BACKGROUND_256}{color}{self._END}'
 
     @staticmethod
     def enable_windows_terminal_mode() -> Any:
         """ Contribution by: Andreas Fredrik Klasson, Magnus Heskestad,
         Dimitris Papadopoulos.
 
         Enable virtual terminal processing in Windows terminal. Does
@@ -233,42 +226,32 @@
         g: Green color.
         b: Blue color.
 
     Returns:
         str: Foreground RGB code.
     """
     utils = Utilities()
-    r, g, b = utils.is_percentages((r, g, b))
-
-    pattern: str = f'{Library.FOREGROUND_RGB}{r};{g};{b}{Library.END}'
-    if not any((r, g, b)):
-        pattern: str = Library.DEFAULT_FOREGROUND_RGB
-
-    return pattern
+    r, g, b = utils.is_percentage((r, g, b))
+    return f'{Library.FOREGROUND_RGB}{r};{g};{b}{Library.END}'
 
 
 def back_rgb(r: int | str, g: int | str, b: int | str) -> str:
     """ Combination with text returns color background with text.
 
     Args:
         r: Red color.
         g: Green color.
         b: Blue color.
 
     Returns:
         str: Background RGB code.
     """
     utils = Utilities()
-    r, g, b = utils.is_percentages((r, g, b))
-
-    pattern: str = f'{Library.BACKGROUND_RGB}{r};{g};{b}{Library.END}'
-    if not any((r, g, b)):
-        pattern: str = Library.DEFAULT_BACKGROUND_RGB
-
-    return pattern
+    r, g, b = utils.is_percentage((r, g, b))
+    return f'{Library.BACKGROUND_RGB}{r};{g};{b}{Library.END}'
 
 
 def attr(name: int | str) -> str:
     """ This will be deprecated in the future, do not use with version >= 2.0.0,
     instead please use style() function (See issue #28).
 
     Args:
```

### Comparing `colored-2.2.1/colored/controls.py` & `colored-2.2.2/colored/controls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from .library import Library
+from .utilities import Utilities
 from .exceptions import InvalidControl
 
 
 class Controls:
 
     def __init__(self):
+        self._utils = Utilities()
         self._ESC: str = Library.ESC
         self._CONTROLS: dict = Library.CONTROLS
 
     def nav(self, name: str, row: int, column=None) -> str:
         """ Moves the cursor n (default 1) cells in the given direction.
             If the cursor is already at the edge of the screen, this has no effect.
             Reference: https://en.wikipedia.org/wiki/ANSI_escape_code#CSI
@@ -35,25 +37,21 @@
             ESC[ row S: Scroll Up
             ESC[ row T: Scroll Down
 
         Raises:
             InvalidControl: Raises an Exception.
         """
         self._is_str_object(name)
-        self._is_n_exist(name)
+        self._utils.is_control_exist(name)
 
         if column:
             if name.lower() == 'position':
                 return f'{self._ESC}{row};{column}{self._CONTROLS[name.lower()]}'
             else:
                 raise InvalidControl(f"{InvalidControl.__name__}: {name}: Expected 'position'")
 
         return f'{self._ESC}{row}{self._CONTROLS[name.lower()]}'
 
     @staticmethod
     def _is_str_object(move: str) -> None:
         if not isinstance(move, str):
             raise AttributeError("'str' object required")
-
-    def _is_n_exist(self, move: str) -> None:
-        if move.lower() not in self._CONTROLS.keys():
-            raise InvalidControl(f'{InvalidControl.__name__}: {move}')
```

### Comparing `colored-2.2.1/colored/cprint.py` & `colored-2.2.2/colored/cprint.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.1/colored/exceptions.py` & `colored-2.2.2/colored/exceptions.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.1/colored/foreground.py` & `colored-2.2.2/colored/foreground.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 class Fore(metaclass=MetaFore):
 
     _utils = Utilities()
     _END: str = Library.END
     _COLORS: dict = Library.COLORS
     _FOREGROUND_256: str = Library.FOREGROUND_256
     _FOREGROUND_RGB: str = Library.FOREGROUND_RGB
-    DEFAULT_FOREGROUND_256: str = Library.DEFAULT_FOREGROUND_256
-    DEFAULT_FOREGROUND_RGB: str = Library.DEFAULT_FOREGROUND_RGB
-    default_foreground_256: str = DEFAULT_FOREGROUND_256
-    default_foreground_rgb: str = DEFAULT_FOREGROUND_RGB
 
     for _color, _code in _COLORS.items():
         vars()[_color] = f'{_FOREGROUND_256}{_code}{_END}'
         vars()[_color.upper()] = f'{_FOREGROUND_256}{_code}{_END}'
 
     @classmethod
     def rgb(cls, r: int | str, g: int | str, b: int | str) -> str:
@@ -38,21 +34,16 @@
             r: Sets the Red color.
             g: Sets the Green color.
             b: Sets the Blue color.
 
         Returns:
             str: Foreground RGB code.
         """
-        r, g, b = cls._utils.is_percentages((r, g, b))
-
-        pattern: str = f'{cls._FOREGROUND_RGB}{r};{g};{b}{cls._END}'
-        if not any((r, g, b)):
-            pattern: str = cls.DEFAULT_FOREGROUND_RGB
-
-        return pattern
+        r, g, b = cls._utils.is_percentage((r, g, b))
+        return f'{cls._FOREGROUND_RGB}{r};{g};{b}{cls._END}'
 
     @classmethod
     def RGB(cls, r: int | str, g: int | str, b: int | str) -> str:
         """ Combination with text returns color text.
 
         Args:
             r: Sets the Red color.
```

### Comparing `colored-2.2.1/colored/hexadecimal.py` & `colored-2.2.2/colored/hexadecimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 class Hex:
 
     def find(self, color: str | int) -> str:
         """ Contribution by Fredrik Klasson """
 
         # Extend shorthand #ABC -> #AABBCC, like in CSS
-
         if len(color) == 4:
             color: str = '#' + color[1] * 2 + color[2] * 2 + color[3] * 2
 
         # Try an exact lookup, trying to favor lower numbers
         # (e.g. find 10 instead of 46 for #00FF00)
         for code, hex_color in Library.HEX_COLORS.items():
             if hex_color == color:
```

### Comparing `colored-2.2.1/colored/library.py` & `colored-2.2.2/colored/library.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,24 @@
 
 from dataclasses import dataclass
 
 
 @dataclass
 class Library:
 
+    # ASCII sequences values.
     ESC: str = '\x1b['
     END: str = 'm'
     FOREGROUND_256: str = f'{ESC}38;5;'
     BACKGROUND_256: str = f'{ESC}48;5;'
     FOREGROUND_RGB: str = f'{ESC}38;2;'
     BACKGROUND_RGB: str = f'{ESC}48;2;'
     UNDERLINE_COLOR: str = f'{ESC}4;58;5;'
 
-    DEFAULT_STYLE: str = f'{ESC}{END}'
-    DEFAULT_FOREGROUND_256: str = f'{FOREGROUND_256}{END}'
-    DEFAULT_BACKGROUND_256: str = f'{BACKGROUND_256}{END}'
-    DEFAULT_FOREGROUND_RGB: str = f'{FOREGROUND_RGB}{END}'
-    DEFAULT_BACKGROUND_RGB: str = f'{BACKGROUND_RGB}{END}'
-
+    # Values of CSI (Control Sequence Introducer) sequences.
     CONTROLS = {
         'up': 'A',
         'down': 'B',
         'right': 'C',
         'left': 'D',
         'next': 'E',
         'previous': 'F',
@@ -32,14 +28,15 @@
         'position': 'H',
         'erase_display': 'J',
         'erase_line': 'K',
         'scroll_up': 'S',
         'scroll_down': 'T'
     }
 
+    # Values of SGR (Select Graphic Rendition) parameters.
     STYLES = {
         'bold': '1',
         'dim': '2',
         'italic': '3',
         'underline': '4',
         'blink': '5',
         'reverse': '7',
@@ -51,14 +48,25 @@
         'res_underline': '24',
         'res_blink': '25',
         'res_reverse': '27',
         'res_hidden': '28',
         'res_underline_color': '59'
     }
 
+    # Values of $COLORTERM environment variable.
+    COLORTERM = {
+        'truecolor': 255,
+        '8bit': 255,
+        '12bit': 4095,
+        '16bit': 65535,
+        '24bit': 16777215,
+        '32bit': 4294967295
+    }
+
+    # Values of 256 colors.
     COLORS = {
         'black': '0',
         'red': '1',
         'green': '2',
         'yellow': '3',
         'blue': '4',
         'magenta': '5',
@@ -310,14 +318,15 @@
         'grey_78': '251',
         'grey_82': '252',
         'grey_85': '253',
         'grey_89': '254',
         'grey_93': '255',
     }
 
+    # Values of HEX colors.
     HEX_COLORS = {
         '0': '#000000',
         '1': '#800000',
         '2': '#008000',
         '3': '#808000',
         '4': '#000080',
         '5': '#800080',
```

### Comparing `colored-2.2.1/pyproject.toml` & `colored-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "colored"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Simple python library for color and formatting to terminal"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
```

### Comparing `colored-2.2.1/PKG-INFO` & `colored-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colored
-Version: 2.2.1
+Version: 2.2.2
 Summary: Simple python library for color and formatting to terminal
 Keywords: xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colored Version: 2.2.1 Summary: Simple python
+Metadata-Version: 2.1 Name: colored Version: 2.2.2 Summary: Simple python
 library for color and formatting to terminal Keywords:
 xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows Author-email:
 Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Other Classifier: Operating System :: POSIX ::
```

