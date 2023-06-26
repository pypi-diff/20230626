# Comparing `tmp/turnip_text-0.0.2.tar.gz` & `tmp/turnip_text-0.0.3.tar.gz`

## Comparing `turnip_text-0.0.2.tar` & `turnip_text-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 turnip_text-0.0.2/Cargo.toml
--rw-r--r--   0     1001      123      202 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.cargo/config.toml
--rw-r--r--   0     1001      123     2745 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.github/workflows/CI.yaml
--rw-r--r--   0     1001      123       73 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.gitignore
--rw-r--r--   0     1001      123      734 2023-06-21 21:13:30.000000 turnip_text-0.0.2/.vscode/settings.json
--rw-r--r--   0     1001      123    10847 2023-06-21 21:13:30.000000 turnip_text-0.0.2/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-21 21:13:30.000000 turnip_text-0.0.2/LICENSE-MIT
--rw-r--r--   0     1001      123     4391 2023-06-21 21:13:30.000000 turnip_text-0.0.2/README.md
--rw-r--r--   0     1001      123       10 2023-06-21 21:13:38.000000 turnip_text-0.0.2/dist/turnip_text-0.0.2.tar.gz
--rw-r--r--   0     1001      123      858 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/experiment.pytext
--rw-r--r--   0     1001      123     2503 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/phdprop.py
--rw-r--r--   0     1001      123    21583 2023-06-21 21:13:30.000000 turnip_text-0.0.2/examples/phdprop.ttxt
--rw-r--r--   0     1001      123     6171 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/asciidoctor.md
--rw-r--r--   0     1001      123        0 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/docbook.md
--rw-r--r--   0     1001      123      113 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/latex.md
--rw-r--r--   0     1001      123      135 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/restructuredtext.md
--rw-r--r--   0     1001      123       22 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/analysis/sphinx.md
--rw-r--r--   0     1001      123    10973 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/code_syntax.md
--rw-r--r--   0     1001      123    10166 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/content_v_formatting.md
--rw-r--r--   0     1001      123      188 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/goals.md
--rw-r--r--   0     1001      123     2476 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/opinionated_text.md
--rw-r--r--   0     1001      123     2151 2023-06-21 21:13:30.000000 turnip_text-0.0.2/notes/pandoc.md
--rw-r--r--   0     1001      123      768 2023-06-21 21:13:30.000000 turnip_text-0.0.2/pyproject.toml
--rw-r--r--   0     1001      123      857 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/__init__.py
--rw-r--r--   0     1001      123     2267 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/helpers.py
--rw-r--r--   0     1001      123        0 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/py.typed
--rw-r--r--   0     1001      123     9465 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/__init__.py
--rw-r--r--   0     1001      123     2921 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/dictify.py
--rw-r--r--   0     1001      123       31 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/__init__.py
--rw-r--r--   0     1001      123     1432 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/base.py
--rw-r--r--   0     1001      123    11656 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/latex/plugins.py
--rw-r--r--   0     1001      123       35 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/__init__.py
--rw-r--r--   0     1001      123     1431 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/base.py
--rw-r--r--   0     1001      123    16642 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/markdown/plugins.py
--rw-r--r--   0     1001      123     2802 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/renderers/std_plugins.py
--rw-r--r--   0     1001      123     1767 2023-06-21 21:13:30.000000 turnip_text-0.0.2/python/turnip_text/turnip_text.pyi
--rw-r--r--   0     1001      123    11510 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/cli.rs
--rw-r--r--   0     1001      123    19518 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lexer.rs
--rw-r--r--   0     1001      123     1905 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lexer_charofs_row_col.rs
--rw-r--r--   0     1001      123      102 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/lib.rs
--rw-r--r--   0     1001      123    11860 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interop.rs
--rw-r--r--   0     1001      123     3877 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/eval_bracket.rs
--rw-r--r--   0     1001      123    24158 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/mod.rs
--rw-r--r--   0     1001      123    27965 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/interp/para.rs
--rw-r--r--   0     1001      123      943 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/mod.rs
--rw-r--r--   0     1001      123     2815 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/python/typeclass.rs
--rw-r--r--   0     1001      123      502 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/mod.rs
--rw-r--r--   0     1001      123    11327 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_lexer.rs
--rw-r--r--   0     1001      123    11105 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_lexer_parser.rs
--rw-r--r--   0     1001      123    29870 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/tests/test_parser.rs
--rw-r--r--   0     1001      123     1287 2023-06-21 21:13:30.000000 turnip_text-0.0.2/src/util.rs
--rw-r--r--   0     1001      123     9901 2023-06-21 21:13:30.000000 turnip_text-0.0.2/Cargo.lock
--rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 turnip_text-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 turnip_text-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      123      202 2023-06-26 11:00:32.000000 turnip_text-0.0.3/.cargo/config.toml
+-rw-r--r--   0     1001      123     2745 2023-06-26 11:00:32.000000 turnip_text-0.0.3/.github/workflows/CI.yaml
+-rw-r--r--   0     1001      123       73 2023-06-26 11:00:32.000000 turnip_text-0.0.3/.gitignore
+-rw-r--r--   0     1001      123      734 2023-06-26 11:00:32.000000 turnip_text-0.0.3/.vscode/settings.json
+-rw-r--r--   0     1001      123    10847 2023-06-26 11:00:32.000000 turnip_text-0.0.3/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-26 11:00:32.000000 turnip_text-0.0.3/LICENSE-MIT
+-rw-r--r--   0     1001      123     4391 2023-06-26 11:00:32.000000 turnip_text-0.0.3/README.md
+-rw-r--r--   0     1001      123       10 2023-06-26 11:00:41.000000 turnip_text-0.0.3/dist/turnip_text-0.0.3.tar.gz
+-rw-r--r--   0     1001      123      858 2023-06-26 11:00:32.000000 turnip_text-0.0.3/examples/experiment.pytext
+-rw-r--r--   0     1001      123     2503 2023-06-26 11:00:32.000000 turnip_text-0.0.3/examples/phdprop.py
+-rw-r--r--   0     1001      123    21583 2023-06-26 11:00:32.000000 turnip_text-0.0.3/examples/phdprop.ttxt
+-rw-r--r--   0     1001      123     6171 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/analysis/asciidoctor.md
+-rw-r--r--   0     1001      123        0 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/analysis/docbook.md
+-rw-r--r--   0     1001      123      113 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/analysis/latex.md
+-rw-r--r--   0     1001      123      135 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/analysis/restructuredtext.md
+-rw-r--r--   0     1001      123       22 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/analysis/sphinx.md
+-rw-r--r--   0     1001      123    10973 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/code_syntax.md
+-rw-r--r--   0     1001      123    10166 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/content_v_formatting.md
+-rw-r--r--   0     1001      123      188 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/goals.md
+-rw-r--r--   0     1001      123     2476 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/opinionated_text.md
+-rw-r--r--   0     1001      123     2151 2023-06-26 11:00:32.000000 turnip_text-0.0.3/notes/pandoc.md
+-rw-r--r--   0     1001      123      768 2023-06-26 11:00:32.000000 turnip_text-0.0.3/pyproject.toml
+-rw-r--r--   0     1001      123      857 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/__init__.py
+-rw-r--r--   0     1001      123     2267 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/helpers.py
+-rw-r--r--   0     1001      123        0 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/py.typed
+-rw-r--r--   0     1001      123    10089 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/__init__.py
+-rw-r--r--   0     1001      123     3022 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/dictify.py
+-rw-r--r--   0     1001      123       31 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/latex/__init__.py
+-rw-r--r--   0     1001      123     1432 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/latex/base.py
+-rw-r--r--   0     1001      123    11525 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/latex/plugins.py
+-rw-r--r--   0     1001      123       35 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/markdown/__init__.py
+-rw-r--r--   0     1001      123     1431 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/markdown/base.py
+-rw-r--r--   0     1001      123    16642 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/markdown/plugins.py
+-rw-r--r--   0     1001      123     2802 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/renderers/std_plugins.py
+-rw-r--r--   0     1001      123     1767 2023-06-26 11:00:32.000000 turnip_text-0.0.3/python/turnip_text/turnip_text.pyi
+-rw-r--r--   0     1001      123    11510 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/cli.rs
+-rw-r--r--   0     1001      123    19518 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/lexer.rs
+-rw-r--r--   0     1001      123     1905 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/lexer_charofs_row_col.rs
+-rw-r--r--   0     1001      123      102 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      123    11860 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/interop.rs
+-rw-r--r--   0     1001      123     3877 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/interp/eval_bracket.rs
+-rw-r--r--   0     1001      123    24158 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/interp/mod.rs
+-rw-r--r--   0     1001      123    27965 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/interp/para.rs
+-rw-r--r--   0     1001      123      943 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/mod.rs
+-rw-r--r--   0     1001      123     2815 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/python/typeclass.rs
+-rw-r--r--   0     1001      123      502 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/tests/mod.rs
+-rw-r--r--   0     1001      123    11327 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/tests/test_lexer.rs
+-rw-r--r--   0     1001      123    11105 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/tests/test_lexer_parser.rs
+-rw-r--r--   0     1001      123    29870 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/tests/test_parser.rs
+-rw-r--r--   0     1001      123     1287 2023-06-26 11:00:32.000000 turnip_text-0.0.3/src/util.rs
+-rw-r--r--   0     1001      123     9901 2023-06-26 11:00:32.000000 turnip_text-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 turnip_text-0.0.3/PKG-INFO
```

### Comparing `turnip_text-0.0.2/Cargo.toml` & `turnip_text-0.0.3/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "turnip_text"
-version = "0.0.2"
+version = "0.0.3"
 description = "Document description language that allows embedded Python to describe document structure"
 license = "MIT OR Apache-2.0"
 authors = ["Samuel Stark"]
 edition = "2021"
 
 # "cdylib" is necessary to produce a shared library for Python to import from.
 #
```

### Comparing `turnip_text-0.0.2/.github/workflows/CI.yaml` & `turnip_text-0.0.3/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/.vscode/settings.json` & `turnip_text-0.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/LICENSE-APACHE` & `turnip_text-0.0.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/LICENSE-MIT` & `turnip_text-0.0.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/README.md` & `turnip_text-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/examples/experiment.pytext` & `turnip_text-0.0.3/examples/experiment.pytext`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/examples/phdprop.py` & `turnip_text-0.0.3/examples/phdprop.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/examples/phdprop.ttxt` & `turnip_text-0.0.3/examples/phdprop.ttxt`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/notes/analysis/asciidoctor.md` & `turnip_text-0.0.3/notes/analysis/asciidoctor.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/notes/code_syntax.md` & `turnip_text-0.0.3/notes/code_syntax.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/notes/content_v_formatting.md` & `turnip_text-0.0.3/notes/content_v_formatting.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/notes/opinionated_text.md` & `turnip_text-0.0.3/notes/opinionated_text.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/notes/pandoc.md` & `turnip_text-0.0.3/notes/pandoc.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/pyproject.toml` & `turnip_text-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "turnip_text"
-version = "0.0.2"
+version = "0.0.3"
 description = "Document description language that allows embedded Python to describe document structure"
 license = { text = "MIT OR Apache-2.0" }
 readme = "README.md"
 authors = [{ name = "Samuel Stark", email = "popgoestoast@gmail.com" }]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `turnip_text-0.0.2/python/turnip_text/__init__.py` & `turnip_text-0.0.3/python/turnip_text/__init__.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/helpers.py` & `turnip_text-0.0.3/python/turnip_text/helpers.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/__init__.py` & `turnip_text-0.0.3/python/turnip_text/renderers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 from os import PathLike
 from typing import (
+    Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
     Tuple,
@@ -111,14 +112,15 @@
 
 
 class Renderer(abc.ABC):
     PARAGRAPH_SEP: str
     SENTENCE_SEP: str
 
     plugins: List["RendererPlugin"]
+    ctx: "RendererContext"
 
     block_handlers: TypeToRenderMap[Block]
     inline_handlers: TypeToRenderMap[Inline]
     preamble_handlers: AmbleMap
     postamble_handlers: AmbleMap
 
     def __init__(self, plugins: List["RendererPlugin"]) -> None:
@@ -151,33 +153,24 @@
             for inl_t_func in p._inline_handlers():
                 self.inline_handlers.push_association(inl_t_func)
             for preamble_id, preamble_func in p._preamble_handlers():
                 self.preamble_handlers.push_handler(preamble_id, preamble_func)
             for postamble_id, postamble_func in p._postamble_handlers():
                 self.postamble_handlers.push_handler(postamble_id, postamble_func)
 
+        self.ctx = RendererContext(plugins)
+
     def request_preamble_order(self, preamble_id_order: List[str]):
         self.preamble_handlers.reorder_handlers(preamble_id_order)
 
     def request_postamble_order(self, postamble_id_order: List[str]):
         self.postamble_handlers.reorder_handlers(postamble_id_order)
 
     def parse_file(self, p: PathLike) -> BlockScope:
-        # TODO this seems super icky
-        # The problem: we want to be able to call e.g. [footnote] inside the turniptext file.
-        # But if footnote were a free function, it would mutate global state -- we don't want that.
-        # A hack! Require a 'renderer object' to be passed in - this encapsulates the local state.
-        # Create a new dictionary, holding all of the Renderer's public fields,
-        # and use that as the locals for parse_file_local.
-
-        locals = {}
-        for plugin in self.plugins:
-            locals.update(dictify(plugin))
-
-        return parse_file_native(str(p), locals)
+        return parse_file_native(str(p), self.ctx.__dict__)
 
     def render_unescapedtext(self, t: UnescapedText) -> str:
         """The baseline - take text and return a string that will look like that text exactly in the given backend."""
         raise NotImplementedError(f"Need to implement render_unescapedtext")
 
     def render_doc(self, doc_block: BlockScope) -> str:
         doc = ""
@@ -211,29 +204,60 @@
 
     def render_sentence(self, s: Sentence) -> str:
         # Default: join internal inline elements directly
         # TODO could be extended by e.g. latex to ensure you get sentence-break-whitespace at the end of each sentence?
         return "".join(self.render_inline(i) for i in s)
 
 
+class RendererContext:
+    def __init__(self, plugins: Iterable["RendererPlugin"]) -> None:
+        self.__dict__ = {}
+        for plugin in plugins:
+            # Strip things beginning with _ from plugin._interface()
+            i = plugin._interface()
+            for key in i.keys():
+                if key.startswith("_"):
+                    del i[key]
+            self.__dict__.update(i)
+            plugin._ctx_setup(self)
+
+
 class RendererPlugin(abc.ABC):
     """
     Plugins should export a consistent set of functions for documents to rely on.
 
     These should only use 'pure' properties, that don't mutate state, because they won't be called multiple times - see `dictify_renderer()` function for details why.
     'Pure' properties need to be marked with `@dictify_pure_property`.
 
     If you want impure results (i.e. once that mutate state) without function call syntax, you can use Builders.
     e.g. the `footnote` property is pure, but returns a single builder object that mutates the internal list of footnotes whenever `.build()` is called.
     """
 
+    # The current RendererContext.
+    # Only None until this plugin is made part of a RendererContext, at which moment it is set to a non-None.
+    _ctx: RendererContext = None  # type: ignore
+
+    def _ctx_setup(self, ctx: RendererContext):
+        assert self._ctx is None
+        assert ctx is not None
+        self._ctx = ctx
+
     @property
     def _plugin_name(self) -> str:
         return type(self).__name__
 
+    def _interface(self) -> Dict[str, Any]:
+        """Define the interface available to the renderer context,
+        and thus all eval-brackets in evaluated documents.
+
+        By default, uses dictify() to find all public variables, member functions, and static functions.
+
+        May be overridden."""
+        return dictify(self)
+
     def _block_handlers(self) -> Iterable[CustomRenderFunc[Block]]:
         return ()
 
     def _inline_handlers(self) -> Iterable[CustomRenderFunc[Inline]]:
         return ()
 
     def _preamble_handlers(self) -> Iterable[Tuple[str, Callable[[Renderer], str]]]:
```

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/dictify.py` & `turnip_text-0.0.3/python/turnip_text/renderers/dictify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Any, Dict, List, Mapping
 
 
 class dictify_pure_property(property):
     """Equivalent to `property`, but acts as a purity marker.
     This should only be used if invoking the property itself DOESN'T MUTATE STATE.
-    This means calling it once is equivalent to calling it many times, which is a useful property when dictifying."""
+    This means calling it once is equivalent to calling it many times, which is a useful property when dictifying.
+    """
+
     pass
 
+
 def dictify(r: Any) -> Dict[str, Any]:
     """
     Given an object implementing `Renderer`, get a dict of all functions, methods, and fields it exposes publically.
 
     Public = does not begin with '_'. This hides internal Python methods (e.g. `__str__`), name-mangled variables (both the original var `__name_mangled` and the mangled `_ExampleClass__name_mangled`, and any variables the programmer doesn't wish to expose `_plz_dont_modify_directly`.
 
     These are retrieved as follows:
@@ -24,27 +27,26 @@
     This can be used as the execution environment for code inside a turnip_text file.
 
     [1]: Information on Python "descriptors" https://docs.python.org/3.8/howto/descriptor.html
     """
 
     from inspect import isdatadescriptor
 
-    r_obj_public_fields: List[str] = [
-        k
-        for k in dir(r)
-        if not k.startswith("_")
-    ]
-    
+    r_obj_public_fields: List[str] = [k for k in dir(r) if not k.startswith("_")]
+
     r_type_dict: Mapping[str, Any] = type(r).__dict__
-    
+
     # Warn about impure data descriptor fields
     for k in r_obj_public_fields:
-        if isdatadescriptor(r_type_dict[k]) and not isinstance(r_type_dict[k], dictify_pure_property):
-            print(f"dictify_renderer Warning: renderer {r} exposes a public 'data descriptor' (e.g. a property) "
-                  f"named {k!r}. This will be evaluated exactly once, and the result will be stored in the "
-                  f"returned dict, instead of evaluating the property each time the dict is accessed. "
-                  f"DO NOT USE THESE IF YOU CAN AVOID IT. Use a normal field instead.")
-
-    return {
-        k: getattr(r, k)
-        for k in r_obj_public_fields
-    }
+        if (
+            k in r_type_dict  # TODO figure out how to warn about keys from superclasses
+            and isdatadescriptor(r_type_dict[k])
+            and not isinstance(r_type_dict[k], dictify_pure_property)
+        ):
+            print(
+                f"dictify_renderer Warning: renderer {r} exposes a public 'data descriptor' (e.g. a property) "
+                f"named {k!r}. This will be evaluated exactly once, and the result will be stored in the "
+                f"returned dict, instead of evaluating the property each time the dict is accessed. "
+                f"DO NOT USE THESE IF YOU CAN AVOID IT. Use a normal field instead."
+            )
+
+    return {k: getattr(r, k) for k in r_obj_public_fields}
```

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/latex/base.py` & `turnip_text-0.0.3/python/turnip_text/renderers/latex/base.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/latex/plugins.py` & `turnip_text-0.0.3/python/turnip_text/renderers/latex/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,19 +159,15 @@
 
         return footnote_builder
 
     def footnote_ref(self, label: str) -> Inline:
         return FootnoteAnchor(label)
 
     def footnote_text(self, label: str) -> BlockScopeBuilder:
-        # Return a callable which is invoked with the contents of the following inline scope
-        # Example usage:
-        # [footnote_text("label")]{text}
-        # equivalent to
-        # [footnote_text("label")(r"text")]
+        # Store the contents of a block scope and associate them with a specific footnote label
         @block_scope_builder
         def handle_block_contents(contents: BlockScope) -> Optional[Block]:
             self._footnotes[label] = contents
             return None
 
         return handle_block_contents
```

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/markdown/base.py` & `turnip_text-0.0.3/python/turnip_text/renderers/markdown/base.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/markdown/plugins.py` & `turnip_text-0.0.3/python/turnip_text/renderers/markdown/plugins.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/renderers/std_plugins.py` & `turnip_text-0.0.3/python/turnip_text/renderers/std_plugins.py`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/python/turnip_text/turnip_text.pyi` & `turnip_text-0.0.3/python/turnip_text/turnip_text.pyi`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/cli.rs` & `turnip_text-0.0.3/src/cli.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/lexer.rs` & `turnip_text-0.0.3/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/lexer_charofs_row_col.rs` & `turnip_text-0.0.3/src/lexer_charofs_row_col.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/interop.rs` & `turnip_text-0.0.3/src/python/interop.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/interp/eval_bracket.rs` & `turnip_text-0.0.3/src/python/interp/eval_bracket.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/interp/mod.rs` & `turnip_text-0.0.3/src/python/interp/mod.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/interp/para.rs` & `turnip_text-0.0.3/src/python/interp/para.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/mod.rs` & `turnip_text-0.0.3/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/python/typeclass.rs` & `turnip_text-0.0.3/src/python/typeclass.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/tests/test_lexer.rs` & `turnip_text-0.0.3/src/tests/test_lexer.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/tests/test_lexer_parser.rs` & `turnip_text-0.0.3/src/tests/test_lexer_parser.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/tests/test_parser.rs` & `turnip_text-0.0.3/src/tests/test_parser.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/src/util.rs` & `turnip_text-0.0.3/src/util.rs`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.2/Cargo.lock` & `turnip_text-0.0.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -279,15 +279,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "turnip_text"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "annotate-snippets",
  "anyhow",
  "argh",
  "lexer-rs",
  "pyo3",
  "thiserror",
```

### Comparing `turnip_text-0.0.2/PKG-INFO` & `turnip_text-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turnip_text
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Dist: mypy ; extra == 'typing'
 Requires-Dist: black ; extra == 'fmt'
 Provides-Extra: typing
```

