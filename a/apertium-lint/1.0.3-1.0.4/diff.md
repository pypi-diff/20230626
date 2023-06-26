# Comparing `tmp/apertium_lint-1.0.3.tar.gz` & `tmp/apertium_lint-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium_lint-1.0.3.tar", last modified: Fri Mar 17 00:46:55 2023, max compression
+gzip compressed data, was "apertium_lint-1.0.4.tar", last modified: Mon Jun 26 19:16:25 2023, max compression
```

## Comparing `apertium_lint-1.0.3.tar` & `apertium_lint-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.864426 apertium_lint-1.0.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.3/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-03-17 00:46:55.864426 apertium_lint-1.0.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.3/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.852425 apertium_lint-1.0.3/apertium_lint/
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)     3381 2022-12-27 16:30:47.000000 apertium_lint-1.0.3/apertium_lint/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2023-03-15 16:13:32.000000 apertium_lint-1.0.3/apertium_lint/file_linter.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.856425 apertium_lint-1.0.3/apertium_lint/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.3/apertium_lint/tests/base.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.3/apertium_lint/tests/test_cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2022-12-23 17:32:06.000000 apertium_lint-1.0.3/apertium_lint/tests/test_lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.3/apertium_lint/tests/test_modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.3/apertium_lint/tests/test_rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.3/apertium_lint/tests/test_transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.3/apertium_lint/tests/test_twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.860425 apertium_lint-1.0.3/apertium_lint/tree_sitter/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5052 2022-12-27 16:13:50.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/lexc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5645 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/tree_sitter_linter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.3/apertium_lint/tree_sitter/twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.864426 apertium_lint-1.0.3/apertium_lint/xml/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/xml/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9731 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/xml/dix.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/xml/lrx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/xml/modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1804 2022-12-23 17:26:03.000000 apertium_lint-1.0.3/apertium_lint/xml/transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/apertium_lint/xml/xml.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-03-17 00:46:55.856425 apertium_lint-1.0.3/apertium_lint.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1007 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-03-17 00:46:55.000000 apertium_lint-1.0.3/apertium_lint.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2023-03-17 00:46:55.864426 apertium_lint-1.0.3/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.3/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.4/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.4/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)     3381 2022-12-27 16:30:47.000000 apertium_lint-1.0.4/apertium_lint/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2023-03-15 16:13:32.000000 apertium_lint-1.0.4/apertium_lint/file_linter.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.4/apertium_lint/tests/base.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.4/apertium_lint/tests/test_cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2022-12-23 17:32:06.000000 apertium_lint-1.0.4/apertium_lint/tests/test_lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.4/apertium_lint/tests/test_modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.4/apertium_lint/tests/test_rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.4/apertium_lint/tests/test_transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.4/apertium_lint/tests/test_twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/tree_sitter/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5052 2022-12-27 16:13:50.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/lexc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5645 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/tree_sitter_linter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/apertium_lint/xml/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10037 2023-04-02 20:54:00.000000 apertium_lint-1.0.4/apertium_lint/xml/dix.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/lrx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3249 2023-06-26 19:14:41.000000 apertium_lint-1.0.4/apertium_lint/xml/transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/xml.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1007 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/setup.py
```

### Comparing `apertium_lint-1.0.3/LICENSE` & `apertium_lint-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/PKG-INFO` & `apertium_lint-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium_lint
-Version: 1.0.3
+Version: 1.0.4
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.3/README.md` & `apertium_lint-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/__init__.py` & `apertium_lint-1.0.4/apertium_lint/__init__.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/file_linter.py` & `apertium_lint-1.0.4/apertium_lint/file_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tests/base.py` & `apertium_lint-1.0.4/apertium_lint/tests/base.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tests/test_transfer.py` & `apertium_lint-1.0.4/apertium_lint/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/cg.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/cg.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/lexc.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/lexc.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/lexd.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/lexd.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/rtx.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/rtx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/tree_sitter_linter.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/tree_sitter_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/tree_sitter/twolc.py` & `apertium_lint-1.0.4/apertium_lint/tree_sitter/twolc.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/xml/dix.py` & `apertium_lint-1.0.4/apertium_lint/xml/dix.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from collections import defaultdict
 import re
 
 class DixLinter(XmlLinter):
     nodes_with_text = ['i', 'l', 'r', 'g', 'ig']
     nodes_in_text = ['a', 'b', 'm', 'g', 'j', 's']
     ReportTypes = {
-        'LitSpace': (Verbosity.Warn, 'Spaces in entries should be written with <b/>.')
+        'LitSpace': (Verbosity.Warn, 'Spaces in entries should be written with <b/>.'),
+        'OtherSpace': (Verbosity.Error, 'Entries should not contain space characters.'),
     }
     def collect_child_strings(self, node, nonempty=False):
         ret = []
         l = ''
         r = ''
         if node.text and node.tag in self.nodes_with_text:
             l = node.text
@@ -37,17 +38,21 @@
         if nonempty and not ret:
             ret.append(('', '', ''))
         return ret
     def collect_strings(self, node): # -> (L, R, par)
         if node.tag in self.nodes_with_text:
             if node.text and ' ' in node.text:
                 self.record('LitSpace', node)
+            elif any(c.isspace() for c in node.text or ''):
+                self.record('OtherSpace', node)
         elif node.tag in self.nodes_in_text:
             if node.tail and ' ' in node.tail:
                 self.record('LitSpace', node)
+            elif any(c.isspace() for c in node.tail or ''):
+                self.record('OtherSpace', node)
         if node.tag == 'a':
             return ('~', '~', '')
         elif node.tag == 'b':
             return (' ', ' ', '')
         elif node.tag == 'm':
             return ('>', '>', '')
         elif node.tag == 'j':
```

### Comparing `apertium_lint-1.0.3/apertium_lint/xml/lrx.py` & `apertium_lint-1.0.4/apertium_lint/xml/lrx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/xml/modes.py` & `apertium_lint-1.0.4/apertium_lint/xml/modes.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint/xml/xml.py` & `apertium_lint-1.0.4/apertium_lint/xml/xml.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/apertium_lint.egg-info/PKG-INFO` & `apertium_lint-1.0.4/apertium_lint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium-lint
-Version: 1.0.3
+Version: 1.0.4
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.3/apertium_lint.egg-info/SOURCES.txt` & `apertium_lint-1.0.4/apertium_lint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.3/setup.cfg` & `apertium_lint-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apertium_lint
-version = 1.0.3
+version = 1.0.4
 description = static analysis of Apertium files
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = apertium, linter
 license = GPLv3+
 license_files = LICENSE
 author = Daniel Swanson
```

