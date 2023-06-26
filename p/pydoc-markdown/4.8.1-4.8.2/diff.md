# Comparing `tmp/pydoc_markdown-4.8.1.tar.gz` & `tmp/pydoc_markdown-4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoc_markdown-4.8.1.tar", max compression
+gzip compressed data, was "pydoc_markdown-4.8.2.tar", max compression
```

## Comparing `pydoc_markdown-4.8.1.tar` & `pydoc_markdown-4.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1002 2023-06-10 09:05:27.603322 pydoc_markdown-4.8.1/LICENSE
--rw-r--r--   0        0        0     4379 2023-06-10 09:05:27.603820 pydoc_markdown-4.8.1/README.md
--rw-r--r--   0        0        0     4042 2023-06-21 15:48:21.555580 pydoc_markdown-4.8.1/pyproject.toml
--rw-r--r--   0        0        0     8757 2023-06-21 15:48:21.555767 pydoc_markdown-4.8.1/src/pydoc_markdown/__init__.py
--rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631119 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/__init__.py
--rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631455 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/__init__.py
--rw-r--r--   0        0        0     5722 2023-06-10 09:05:27.631691 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/python.py
--rw-r--r--   0        0        0       81 2023-06-10 09:05:27.632045 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/__init__.py
--rw-r--r--   0        0        0     5520 2023-06-10 09:05:27.632255 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/crossref.py
--rw-r--r--   0        0        0     3954 2023-06-10 09:05:27.632449 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/filter.py
--rw-r--r--   0        0        0     5971 2023-06-10 09:05:27.632657 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/google.py
--rw-r--r--   0        0        0     3875 2023-06-10 09:05:27.632836 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/pydocmd.py
--rw-r--r--   0        0        0     2740 2023-06-10 09:05:27.633020 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/smart.py
--rw-r--r--   0        0        0     5622 2023-06-10 09:05:27.633206 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/sphinx.py
--rw-r--r--   0        0        0       81 2023-06-10 09:05:27.633857 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/__init__.py
--rw-r--r--   0        0        0     6840 2023-06-10 09:05:27.634098 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/docusaurus.py
--rw-r--r--   0        0        0    16977 2023-06-21 15:48:17.310736 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/hugo.py
--rw-r--r--   0        0        0     3947 2023-06-10 09:05:27.634568 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/jinja2.py
--rw-r--r--   0        0        0    22500 2023-06-10 09:05:27.634852 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/markdown.py
--rw-r--r--   0        0        0     7848 2023-06-21 15:19:12.008743 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/mkdocs.py
--rw-r--r--   0        0        0       81 2023-06-10 09:05:27.635527 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/__init__.py
--rw-r--r--   0        0        0     6636 2023-06-10 09:05:27.635845 pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/git.py
--rw-r--r--   0        0        0     6841 2023-06-21 15:48:17.311484 pydoc_markdown-4.8.1/src/pydoc_markdown/interfaces.py
--rw-r--r--   0        0        0    13878 2023-06-10 09:05:27.636497 pydoc_markdown-4.8.1/src/pydoc_markdown/main.py
--rw-r--r--   0        0        0     6467 2023-06-10 09:05:27.637084 pydoc_markdown-4.8.1/src/pydoc_markdown/novella/preprocessor.py
--rw-r--r--   0        0        0        0 2023-06-10 09:05:27.637221 pydoc_markdown-4.8.1/src/pydoc_markdown/py.typed
--rw-r--r--   0        0        0     3375 2023-06-10 09:05:27.637431 pydoc_markdown-4.8.1/src/pydoc_markdown/static.py
--rw-r--r--   0        0        0        5 2023-06-10 09:05:27.637750 pydoc_markdown-4.8.1/src/pydoc_markdown/util/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-10 09:05:27.638093 pydoc_markdown-4.8.1/src/pydoc_markdown/util/docspec.py
--rw-r--r--   0        0        0     4545 2023-06-10 09:05:27.638318 pydoc_markdown-4.8.1/src/pydoc_markdown/util/knownfiles.py
--rw-r--r--   0        0        0      930 2023-06-10 09:05:27.638499 pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc.py
--rw-r--r--   0        0        0      378 2023-06-10 09:05:27.638686 pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc_test.py
--rw-r--r--   0        0        0     7215 2023-06-21 15:48:17.312065 pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages.py
--rw-r--r--   0        0        0      706 2023-06-21 15:48:17.312634 pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages_test.py
--rw-r--r--   0        0        0     2492 2023-06-10 09:05:27.639621 pydoc_markdown-4.8.1/src/pydoc_markdown/util/watchdog.py
--rw-r--r--   0        0        0     2998 2023-06-10 09:05:27.639948 pydoc_markdown-4.8.1/src/pydoc_markdown/util/ytemplate.py
--rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 pydoc_markdown-4.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-10 09:05:27.603322 pydoc_markdown-4.8.2/LICENSE
+-rw-r--r--   0        0        0     4379 2023-06-10 09:05:27.603820 pydoc_markdown-4.8.2/README.md
+-rw-r--r--   0        0        0     4042 2023-06-26 12:36:37.334350 pydoc_markdown-4.8.2/pyproject.toml
+-rw-r--r--   0        0        0     8787 2023-06-26 12:36:37.334544 pydoc_markdown-4.8.2/src/pydoc_markdown/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631119 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.631455 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/loaders/__init__.py
+-rw-r--r--   0        0        0     5722 2023-06-10 09:05:27.631691 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/loaders/python.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.632045 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/__init__.py
+-rw-r--r--   0        0        0     5520 2023-06-10 09:05:27.632255 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/crossref.py
+-rw-r--r--   0        0        0     3954 2023-06-10 09:05:27.632449 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/filter.py
+-rw-r--r--   0        0        0     5971 2023-06-10 09:05:27.632657 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/google.py
+-rw-r--r--   0        0        0     3875 2023-06-10 09:05:27.632836 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/pydocmd.py
+-rw-r--r--   0        0        0     2740 2023-06-10 09:05:27.633020 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/smart.py
+-rw-r--r--   0        0        0     5622 2023-06-10 09:05:27.633206 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/sphinx.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.633857 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/__init__.py
+-rw-r--r--   0        0        0     6840 2023-06-10 09:05:27.634098 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/docusaurus.py
+-rw-r--r--   0        0        0    16977 2023-06-21 15:48:17.310736 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/hugo.py
+-rw-r--r--   0        0        0     3947 2023-06-10 09:05:27.634568 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/jinja2.py
+-rw-r--r--   0        0        0    22500 2023-06-10 09:05:27.634852 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/markdown.py
+-rw-r--r--   0        0        0     7848 2023-06-21 15:19:12.008743 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/mkdocs.py
+-rw-r--r--   0        0        0       81 2023-06-10 09:05:27.635527 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/source_linkers/__init__.py
+-rw-r--r--   0        0        0     6636 2023-06-10 09:05:27.635845 pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/source_linkers/git.py
+-rw-r--r--   0        0        0     6841 2023-06-21 15:48:17.311484 pydoc_markdown-4.8.2/src/pydoc_markdown/interfaces.py
+-rw-r--r--   0        0        0    13878 2023-06-10 09:05:27.636497 pydoc_markdown-4.8.2/src/pydoc_markdown/main.py
+-rw-r--r--   0        0        0     6467 2023-06-10 09:05:27.637084 pydoc_markdown-4.8.2/src/pydoc_markdown/novella/preprocessor.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:05:27.637221 pydoc_markdown-4.8.2/src/pydoc_markdown/py.typed
+-rw-r--r--   0        0        0     3375 2023-06-10 09:05:27.637431 pydoc_markdown-4.8.2/src/pydoc_markdown/static.py
+-rw-r--r--   0        0        0        5 2023-06-10 09:05:27.637750 pydoc_markdown-4.8.2/src/pydoc_markdown/util/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-10 09:05:27.638093 pydoc_markdown-4.8.2/src/pydoc_markdown/util/docspec.py
+-rw-r--r--   0        0        0     4545 2023-06-10 09:05:27.638318 pydoc_markdown-4.8.2/src/pydoc_markdown/util/knownfiles.py
+-rw-r--r--   0        0        0      930 2023-06-10 09:05:27.638499 pydoc_markdown-4.8.2/src/pydoc_markdown/util/misc.py
+-rw-r--r--   0        0        0      378 2023-06-10 09:05:27.638686 pydoc_markdown-4.8.2/src/pydoc_markdown/util/misc_test.py
+-rw-r--r--   0        0        0     7215 2023-06-21 15:48:17.312065 pydoc_markdown-4.8.2/src/pydoc_markdown/util/pages.py
+-rw-r--r--   0        0        0      706 2023-06-21 15:48:17.312634 pydoc_markdown-4.8.2/src/pydoc_markdown/util/pages_test.py
+-rw-r--r--   0        0        0     2492 2023-06-10 09:05:27.639621 pydoc_markdown-4.8.2/src/pydoc_markdown/util/watchdog.py
+-rw-r--r--   0        0        0     2998 2023-06-10 09:05:27.639948 pydoc_markdown-4.8.2/src/pydoc_markdown/util/ytemplate.py
+-rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 pydoc_markdown-4.8.2/PKG-INFO
```

### Comparing `pydoc_markdown-4.8.1/LICENSE` & `pydoc_markdown-4.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/README.md` & `pydoc_markdown-4.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/pyproject.toml` & `pydoc_markdown-4.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoc-markdown"
-version = "4.8.1"
+version = "4.8.2"
 description = "Create Python API documentation in Markdown format."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "pydoc_markdown", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/__init__.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,34 +30,35 @@
 import subprocess
 import typing as t
 from pathlib import Path
 
 import databind.json
 import docspec
 import tomli
-from databind.core import Context as DatabindContext, ExtraKeys, Location, format_context_trace
+import typing_extensions as te
+from databind.core import Alias, Context as DatabindContext, ExtraKeys, format_context_trace
 
 from pydoc_markdown.contrib.loaders.python import PythonLoader
 from pydoc_markdown.contrib.processors.crossref import CrossrefProcessor
 from pydoc_markdown.contrib.processors.filter import FilterProcessor
 from pydoc_markdown.contrib.processors.smart import SmartProcessor
 from pydoc_markdown.contrib.renderers.markdown import MarkdownRenderer
 from pydoc_markdown.interfaces import Builder, Context, Loader, Processor, Renderer, Resolver
 from pydoc_markdown.util import ytemplate
 
 __author__ = "Niklas Rosenstein <rosensteinniklas@gmail.com>"
-__version__ = "4.8.1"
+__version__ = "4.8.2"
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Hooks:
-    pre_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "pre-render"})
-    post_render: t.List[str] = dataclasses.field(default_factory=list, metadata={"alias": "post-render"})
+    pre_render: te.Annotated[t.List[str], Alias("pre-render")] = dataclasses.field(default_factory=list)
+    post_render: te.Annotated[t.List[str], Alias("post-render")] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
 class PydocMarkdown:
     """
     This object represents the main configuration for Pydoc-Markdown.
     """
```

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/loaders/python.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/loaders/python.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/crossref.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/crossref.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/filter.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/filter.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/google.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/google.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/pydocmd.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/pydocmd.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/smart.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/smart.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/processors/sphinx.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/processors/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/docusaurus.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/docusaurus.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/hugo.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/hugo.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/jinja2.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/jinja2.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/markdown.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/renderers/mkdocs.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/renderers/mkdocs.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/contrib/source_linkers/git.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/contrib/source_linkers/git.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/interfaces.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/interfaces.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/main.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/main.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/novella/preprocessor.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/novella/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/static.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/static.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/docspec.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/docspec.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/knownfiles.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/knownfiles.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/misc.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/misc.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/pages.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/pages_test.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/pages_test.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/watchdog.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/watchdog.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/src/pydoc_markdown/util/ytemplate.py` & `pydoc_markdown-4.8.2/src/pydoc_markdown/util/ytemplate.py`

 * *Files identical despite different names*

### Comparing `pydoc_markdown-4.8.1/PKG-INFO` & `pydoc_markdown-4.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoc-markdown
-Version: 4.8.1
+Version: 4.8.2
 Summary: Create Python API documentation in Markdown format.
 License: MIT
 Keywords: documentation,docs,generator,markdown,pydoc
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

