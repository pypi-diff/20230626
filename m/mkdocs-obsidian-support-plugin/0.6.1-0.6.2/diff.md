# Comparing `tmp/mkdocs-obsidian-support-plugin-0.6.1.tar.gz` & `tmp/mkdocs-obsidian-support-plugin-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-obsidian-support-plugin-0.6.1.tar", last modified: Mon Feb 27 15:46:27 2023, max compression
+gzip compressed data, was "mkdocs-obsidian-support-plugin-0.6.2.tar", last modified: Mon Jun 26 13:27:25 2023, max compression
```

## Comparing `mkdocs-obsidian-support-plugin-0.6.1.tar` & `mkdocs-obsidian-support-plugin-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-02-27 15:46:27.914604 mkdocs-obsidian-support-plugin-0.6.1/
--rw-r--r--   0 deukyun    (501) staff       (20)     1066 2023-02-20 02:38:44.000000 mkdocs-obsidian-support-plugin-0.6.1/LICENSE
--rw-r--r--   0 deukyun    (501) staff       (20)     1773 2023-02-27 15:46:27.914460 mkdocs-obsidian-support-plugin-0.6.1/PKG-INFO
--rw-r--r--   0 deukyun    (501) staff       (20)      911 2023-02-21 11:13:00.000000 mkdocs-obsidian-support-plugin-0.6.1/README.md
-drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-02-27 15:46:27.912845 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/
--rw-r--r--   0 deukyun    (501) staff       (20)     1773 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 deukyun    (501) staff       (20)      693 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 deukyun    (501) staff       (20)        1 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 deukyun    (501) staff       (20)       82 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/entry_points.txt
--rw-r--r--   0 deukyun    (501) staff       (20)       14 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/requires.txt
--rw-r--r--   0 deukyun    (501) staff       (20)       17 2023-02-27 15:46:27.000000 mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-02-27 15:46:27.913743 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/
--rw-r--r--   0 deukyun    (501) staff       (20)        0 2023-02-19 18:11:27.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/__init__.py
--rw-r--r--   0 deukyun    (501) staff       (20)      813 2023-02-27 15:45:16.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/abstract_conversion.py
-drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-02-27 15:46:27.914275 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/
--rw-r--r--   0 deukyun    (501) staff       (20)        0 2023-02-21 05:56:11.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/__init__.py
--rw-r--r--   0 deukyun    (501) staff       (20)     1181 2023-02-27 15:45:02.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/admonition.py
--rw-r--r--   0 deukyun    (501) staff       (20)     1294 2023-02-27 15:45:05.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/excalidraw.py
--rw-r--r--   0 deukyun    (501) staff       (20)     2212 2023-02-27 15:45:10.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/image_link.py
--rw-r--r--   0 deukyun    (501) staff       (20)      417 2023-02-21 13:29:03.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/markdown_code_extract.py
--rw-r--r--   0 deukyun    (501) staff       (20)     1520 2023-02-27 15:45:28.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/markdown_convert.py
--rw-r--r--   0 deukyun    (501) staff       (20)      787 2023-02-27 15:45:58.000000 mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/plugin.py
--rw-r--r--   0 deukyun    (501) staff       (20)       38 2023-02-27 15:46:27.914646 mkdocs-obsidian-support-plugin-0.6.1/setup.cfg
--rw-r--r--   0 deukyun    (501) staff       (20)     1358 2023-02-27 15:46:25.000000 mkdocs-obsidian-support-plugin-0.6.1/setup.py
+drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-06-26 13:27:25.918007 mkdocs-obsidian-support-plugin-0.6.2/
+-rw-r--r--   0 deukyun    (501) staff       (20)     1066 2023-06-21 11:41:35.000000 mkdocs-obsidian-support-plugin-0.6.2/LICENSE
+-rw-r--r--   0 deukyun    (501) staff       (20)     1773 2023-06-26 13:27:25.917869 mkdocs-obsidian-support-plugin-0.6.2/PKG-INFO
+-rw-r--r--   0 deukyun    (501) staff       (20)      911 2023-06-21 11:41:35.000000 mkdocs-obsidian-support-plugin-0.6.2/README.md
+drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-06-26 13:27:25.915770 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/
+-rw-r--r--   0 deukyun    (501) staff       (20)     1773 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 deukyun    (501) staff       (20)      746 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 deukyun    (501) staff       (20)        1 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 deukyun    (501) staff       (20)       82 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 deukyun    (501) staff       (20)       14 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/requires.txt
+-rw-r--r--   0 deukyun    (501) staff       (20)       17 2023-06-26 13:27:25.000000 mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-06-26 13:27:25.916545 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/
+-rw-r--r--   0 deukyun    (501) staff       (20)        0 2023-06-21 11:41:35.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/__init__.py
+-rw-r--r--   0 deukyun    (501) staff       (20)      813 2023-06-21 11:54:59.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/abstract_conversion.py
+drwxr-xr-x   0 deukyun    (501) staff       (20)        0 2023-06-26 13:27:25.917537 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/
+-rw-r--r--   0 deukyun    (501) staff       (20)        0 2023-06-21 11:41:35.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/__init__.py
+-rw-r--r--   0 deukyun    (501) staff       (20)     1181 2023-06-21 11:54:59.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/admonition.py
+-rw-r--r--   0 deukyun    (501) staff       (20)     1299 2023-06-26 13:21:57.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/admonition_backquotes.py
+-rw-r--r--   0 deukyun    (501) staff       (20)     1271 2023-06-21 11:56:20.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/excalidraw.py
+-rw-r--r--   0 deukyun    (501) staff       (20)     2212 2023-06-21 11:41:35.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/image_link.py
+-rw-r--r--   0 deukyun    (501) staff       (20)      418 2023-06-26 13:21:57.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/markdown_code_extract.py
+-rw-r--r--   0 deukyun    (501) staff       (20)     1521 2023-06-26 13:21:57.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/markdown_convert.py
+-rw-r--r--   0 deukyun    (501) staff       (20)      961 2023-06-26 13:21:57.000000 mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/plugin.py
+-rw-r--r--   0 deukyun    (501) staff       (20)       38 2023-06-26 13:27:25.918052 mkdocs-obsidian-support-plugin-0.6.2/setup.cfg
+-rw-r--r--   0 deukyun    (501) staff       (20)     1358 2023-06-26 13:21:57.000000 mkdocs-obsidian-support-plugin-0.6.2/setup.py
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/LICENSE` & `mkdocs-obsidian-support-plugin-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/PKG-INFO` & `mkdocs-obsidian-support-plugin-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-obsidian-support-plugin
-Version: 0.6.1
+Version: 0.6.2
 Summary: A MkDocs plugin that supports obsidian to mkdocs convert
 Home-page: https://github.com/ndy2/mkdocs-obsidian-support-plugin
 Author: ndy2
 Author-email: emrdbs12@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/README.md` & `mkdocs-obsidian-support-plugin-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/PKG-INFO` & `mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-obsidian-support-plugin
-Version: 0.6.1
+Version: 0.6.2
 Summary: A MkDocs plugin that supports obsidian to mkdocs convert
 Home-page: https://github.com/ndy2/mkdocs-obsidian-support-plugin
 Author: ndy2
 Author-email: emrdbs12@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/mkdocs_obsidian_support_plugin.egg-info/SOURCES.txt` & `mkdocs-obsidian-support-plugin-0.6.2/mkdocs_obsidian_support_plugin.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 obsidian_support/__init__.py
 obsidian_support/abstract_conversion.py
 obsidian_support/markdown_code_extract.py
 obsidian_support/markdown_convert.py
 obsidian_support/plugin.py
 obsidian_support/conversion/__init__.py
 obsidian_support/conversion/admonition.py
+obsidian_support/conversion/admonition_backquotes.py
 obsidian_support/conversion/excalidraw.py
 obsidian_support/conversion/image_link.py
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/abstract_conversion.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/abstract_conversion.py`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/admonition.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/admonition.py`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/excalidraw.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/excalidraw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
-from inspect import cleandoc
 
-from obsidian_support.abstract_conversion import AbstractConversion, SyntaxGroup
 from mkdocs.structure.pages import Page
 
+from obsidian_support.abstract_conversion import AbstractConversion, SyntaxGroup
+
 """
 a strategy that convert [excalidraw link] to [excalidraw kroki code block]
 """
 
 EXCALIDRAW_LINK_REGEX = "!\\[\\[(?P<excalidraw_path>[^\\|^\\]]+.excalidraw)\\]\\]"
 EXCALIDRAW_LINK_REGEX_GROUPS = ['excalidraw_path']
 EXCALIDRAW_JSON_PATTERN = re.compile("```json\n(?P<json>[\\s\\S]+)\n```")
@@ -17,19 +17,19 @@
     def __init__(self):
         super().__init__(EXCALIDRAW_LINK_REGEX, EXCALIDRAW_LINK_REGEX_GROUPS)
 
     def convert(self, syntax_groups: SyntaxGroup, page: Page) -> str:
         return convert_excalidraw(*syntax_groups, page)
 
 
-def convert_excalidraw(excalidraw_path: str, page:Page) -> str:
+def convert_excalidraw(excalidraw_path: str, page: Page) -> str:
     src_uri = page.file.src_uri
-    src_dir_index = src_uri[:len(src_uri)-1].rfind('/')
+    src_dir_index = src_uri[:len(src_uri) - 1].rfind('/')
     src_dir_path = src_uri[:src_dir_index] + "/"
-    excalidraw_file_path = "docs/" + src_dir_path + excalidraw_path+'.md'
+    excalidraw_file_path = "docs/" + src_dir_path + excalidraw_path + '.md'
 
     f = open(excalidraw_file_path, 'r')
     excalidraw_markdown = f.read()
     excalidraw_json_match = EXCALIDRAW_JSON_PATTERN.search(excalidraw_markdown)
     excalidraw_json = excalidraw_json_match.group('json')
     f.close()
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/conversion/image_link.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/conversion/image_link.py`

 * *Files identical despite different names*

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/markdown_convert.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/markdown_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 A template method that applies conversion for every regex matches
 """
 
 
 def markdown_convert(markdown: str, page: Page, conversion: AbstractConversion) -> str:
     converted_markdown = ""
     index = 0
+
     for obsidian_syntax in conversion.obsidian_regex_pattern.finditer(markdown):
         ## found range of markdown where the obsidian_regex matches
         start = obsidian_syntax.start()
         end = obsidian_syntax.end() - 1
 
         ## continue if match is in excluded range
         if __is_excluded(start, end, get_excluded_indices(markdown)):
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/obsidian_support/plugin.py` & `mkdocs-obsidian-support-plugin-0.6.2/obsidian_support/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from mkdocs.plugins import BasePlugin
 
 from obsidian_support.conversion.admonition import AdmonitionConvert
+from obsidian_support.conversion.admonition_backquotes import AdmonitionBackquotesConvert
 from obsidian_support.conversion.excalidraw import ExcalidrawConvert
 from obsidian_support.conversion.image_link import ImageLinkConvert
 from obsidian_support.markdown_convert import markdown_convert
 
 """
 A mkdocs plugin that support conversion from
 'obsidian syntax' to 'mkdocs-material syntax'
 """
 
 
 class ObsidianSupportPlugin(BasePlugin):
 
     def on_page_markdown(self, markdown, page, config, files):
         ## apply conversions
+
         markdown = markdown_convert(markdown, page, AdmonitionConvert())
+        markdown = markdown_convert(markdown, page, AdmonitionBackquotesConvert())
         markdown = markdown_convert(markdown, page, ExcalidrawConvert())
         markdown = markdown_convert(markdown, page, ImageLinkConvert())
 
         return markdown
```

### Comparing `mkdocs-obsidian-support-plugin-0.6.1/setup.py` & `mkdocs-obsidian-support-plugin-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup, find_packages
 
-VERSION_NUMBER = '0.6.1'
+VERSION_NUMBER = '0.6.2'
 
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
```

