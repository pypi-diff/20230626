# Comparing `tmp/textual_textarea-0.3.0.tar.gz` & `tmp/textual_textarea-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.3.0.tar", max compression
+gzip compressed data, was "textual_textarea-0.3.1.tar", max compression
```

## Comparing `textual_textarea-0.3.0.tar` & `textual_textarea-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/LICENSE
--rw-r--r--   0        0        0     4475 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/README.md
--rw-r--r--   0        0        0     1555 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      491 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0      175 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     3510 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/comments.py
--rw-r--r--   0        0        0     1091 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3374 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/messages.py
--rw-r--r--   0        0        0        0 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    28491 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     5418 1970-01-01 00:00:00.000000 textual_textarea-0.3.0/setup.py
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 textual_textarea-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4475 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/README.md
+-rw-r--r--   0        0        0     1555 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0      175 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/cancellable_input.py
+-rw-r--r--   0        0        0     1028 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     3510 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/comments.py
+-rw-r--r--   0        0        0     1091 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3374 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    28352 2023-06-26 18:06:19.000717 textual_textarea-0.3.1/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     5418 1970-01-01 00:00:00.000000 textual_textarea-0.3.1/setup.py
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 textual_textarea-0.3.1/PKG-INFO
```

### Comparing `textual_textarea-0.3.0/LICENSE` & `textual_textarea-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/README.md` & `textual_textarea-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/pyproject.toml` & `textual_textarea-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.3.0"
+version = "0.3.1"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
@@ -20,15 +20,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 textual = {version="0.21.0", extras=["dev"]}
 
 [tool.poetry.group.static.dependencies]
 black = "^23.3.0"
-ruff = ">=0.0.264,<0.0.273"
+ruff = ">=0.0.264,<0.0.276"
 mypy = "^1.2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [tool.ruff]
```

### Comparing `textual_textarea-0.3.0/src/textual_textarea/colors.py` & `textual_textarea-0.3.1/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/comments.py` & `textual_textarea-0.3.1/src/textual_textarea/comments.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/containers.py` & `textual_textarea-0.3.1/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/error_modal.py` & `textual_textarea-0.3.1/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/key_handlers.py` & `textual_textarea-0.3.1/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/messages.py` & `textual_textarea-0.3.1/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.3.0/src/textual_textarea/textarea.py` & `textual_textarea-0.3.1/src/textual_textarea/textarea.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,53 @@
         self.update(self._content)
 
     def on_blur(self) -> None:
         self.blink_timer.pause()
         self.cursor_visible = False
         self.update(self._content)
 
+    def on_mouse_down(self, event: events.MouseDown) -> None:
+        """
+        Moves the anchor and cursor to the click.
+        """
+        event.stop()
+        self.cursor_visible = True
+        self.blink_timer.reset()
+        self.selection_anchor = Cursor.from_mouse_event(event)
+        self.move_cursor(event.x - 1, event.y)
+        self.focus()
+
+    def on_mouse_move(self, event: events.MouseMove) -> None:
+        """
+        Updates the cursor if the button is pressed while the mouse
+        is moving.
+        """
+        if event.button == 1:
+            self.move_cursor(event.x - 1, event.y)
+
+    def on_mouse_up(self, event: events.MouseUp) -> None:
+        """
+        Moves the cursor to the click.
+        """
+        event.stop()
+        self.cursor_visible = True
+        self.blink_timer.reset()
+        if self.selection_anchor == Cursor.from_mouse_event(event):
+            # simple click
+            self.selection_anchor = None
+        else:
+            self.move_cursor(event.x - 1, event.y)
+        self.focus()
+
+    def on_click(self, event: events.Click) -> None:
+        """
+        Click duplicates MouseUp and MouseDown, so we just capture and kill this event.
+        """
+        event.stop()
+
     def on_paste(self, event: events.Paste) -> None:
         """
         If the user hits ctrl+v, we don't get that keypress;
         we get a Paste event instead.
 
         This ignores the contents of the Paste message and mimics the behavior of
         ctrl+u.
@@ -475,18 +514,18 @@
         if self.cursor.pos == 0:
             return None
         else:
             return self.lines[cursor.lno][cursor.pos - 1]
 
     def move_cursor(self, x: int, y: int) -> None:
         max_y = len(self.lines) - 1
-        safe_y = min(max_y, y)
+        safe_y = max(0, min(max_y, y))
         max_x = len(self.lines[safe_y]) - 1
-        safe_x = min(max_x, x)
-        self.cursor = Cursor(lno=max(0, safe_y), pos=max(0, safe_x))
+        safe_x = max(0, min(max_x, x))
+        self.cursor = Cursor(lno=safe_y, pos=safe_x)
         self.update(self._content)
 
 
 class TextArea(Widget, can_focus=True, can_focus_children=False):
     """
     A Widget that presents a feature-rich, multiline text editor interface.
 
@@ -616,62 +655,22 @@
         )
         input.styles.background = self.theme_colors.bgcolor
         input.styles.border = "round", self.theme_colors.contrast_text_color
         input.styles.color = self.theme_colors.contrast_text_color
         self.footer.mount(input)
         input.focus()
 
-    def on_mouse_down(self, event: events.MouseDown) -> None:
-        """
-        Moves the anchor and cursor to the click.
-        """
-        event.stop()
-        self.capture_mouse()
-        self.text_input.cursor_visible = True
-        self.text_input.blink_timer.reset()
-        self.text_input.selection_anchor = Cursor.from_mouse_event(event)
-        self.text_input.move_cursor(event.x - 1, event.y)
-        self.text_input.focus()
-
-    def on_mouse_move(self, event: events.MouseMove) -> None:
-        """
-        Updates the cursor if the button is pressed
-        """
-        if event.button == 1:
-            self.text_input.move_cursor(event.x - 1, event.y)
-
-    def on_mouse_up(self, event: events.MouseUp) -> None:
-        """
-        Moves the cursor to the click.
-        """
-        event.stop()
-        self.release_mouse()
-        self.text_input.cursor_visible = True
-        self.text_input.blink_timer.reset()
-        if self.text_input.selection_anchor == Cursor.from_mouse_event(event):
-            # simple click
-            self.text_input.selection_anchor = None
-        else:
-            self.text_input.move_cursor(event.x - 1, event.y)
-        self.text_input.focus()
-
-    def on_click(self, event: events.Click) -> None:
-        """
-        Click duplicates MouseUp and MouseDown, so we just capture and kill this event.
-        """
-        event.stop()
-
     def on_text_area_cursor_moved(self, event: TextAreaCursorMoved) -> None:
         """
         Scrolls the container so the cursor is visible.
         """
         event.stop()
         container = self.text_container
-        x_buffer = container.window_region.width // 4
-        y_buffer = container.window_region.height // 4
+        x_buffer = max(container.window_region.width // 6, 2)
+        y_buffer = max(container.window_region.height // 6, 2)
         if event.cursor_x < container.window_region.x + x_buffer:  # scroll left
             container.scroll_to(event.cursor_x - x_buffer, container.window_region.y)
         elif (
             event.cursor_x
             >= container.window_region.x + container.window_region.width - x_buffer
         ):  # scroll right
             container.scroll_to(
```

### Comparing `textual_textarea-0.3.0/setup.py` & `textual_textarea-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyperclip>=1.8.2,<2.0.0', 'textual>=0.21.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
     'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd> or click and drag.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
```

### Comparing `textual_textarea-0.3.0/PKG-INFO` & `textual_textarea-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.3.0
+Version: 0.3.1
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

