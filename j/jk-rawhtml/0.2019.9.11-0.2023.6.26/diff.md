# Comparing `tmp/jk_rawhtml-0.2019.9.11.tar.gz` & `tmp/jk_rawhtml-0.2023.6.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jk_rawhtml-0.2019.9.11.tar", last modified: Wed Sep 11 11:25:00 2019, max compression
+gzip compressed data, was "jk_rawhtml-0.2023.6.26.tar", last modified: Mon Jun 26 20:50:18 2023, max compression
```

## Comparing `jk_rawhtml-0.2019.9.11.tar` & `jk_rawhtml-0.2023.6.26.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxr-x   0 jknauth   (1000) jknauth   (1000)        0 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/
--rw-r-----   0 jknauth   (1000) jknauth   (1000)    11360 2019-09-11 11:23:02.000000 jk_rawhtml-0.2019.9.11/LICENSE.txt
-drwxrwxr-x   0 jknauth   (1000) jknauth   (1000)        0 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      293 2019-01-19 09:01:39.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/htmlgeneral.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      720 2019-04-07 09:03:02.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLRawText.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     3024 2019-04-07 21:28:43.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLElement.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     1256 2019-04-05 15:58:15.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5RootElement.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      344 2019-01-19 09:52:43.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/_HTMLRawTextProto.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      745 2019-04-05 15:58:30.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLRawCSS.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     3215 2019-01-20 11:50:51.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/ColorSpectrum.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      331 2019-01-19 18:23:19.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/_HTMLRawCSSProto.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      308 2019-01-23 01:48:27.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/__init__.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     1130 2019-04-05 15:58:19.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5HeadElement.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      344 2019-01-19 09:52:40.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/_HTMLCommentProto.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     2526 2019-01-19 14:54:56.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/Color.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      895 2019-04-05 15:58:07.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLComment.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     8492 2019-01-19 18:11:18.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5Scope.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      829 2019-01-20 08:16:42.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/CSSMap.py
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)     1304 2019-04-07 21:23:31.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml/_HTMLElementProto.py
-drwxrwxr-x   0 jknauth   (1000) jknauth   (1000)        0 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)       11 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/top_level.txt
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)    12320 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/PKG-INFO
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)      679 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/SOURCES.txt
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)        1 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/dependency_links.txt
--rw-r--r--   0 jknauth   (1000) jknauth   (1000)        1 2019-01-19 11:14:46.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/not-zip-safe
--rw-rw-r--   0 jknauth   (1000) jknauth   (1000)       11 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/requires.txt
--rw-r-----   0 jknauth   (1000) jknauth   (1000)       38 2019-09-11 11:23:02.000000 jk_rawhtml-0.2019.9.11/MANIFEST.in
--rw-rw-r--   0 jknauth   (1000) jknauth   (1000)     9137 2019-09-11 11:23:02.000000 jk_rawhtml-0.2019.9.11/README.md
--rw-r-----   0 jknauth   (1000) jknauth   (1000)     1480 2019-04-05 15:25:58.000000 jk_rawhtml-0.2019.9.11/setup.py
--rw-rw-r--   0 jknauth   (1000) jknauth   (1000)    12320 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/PKG-INFO
--rw-rw-r--   0 jknauth   (1000) jknauth   (1000)       38 2019-09-11 11:25:00.000000 jk_rawhtml-0.2019.9.11/setup.cfg
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-26 20:50:18.932358 jk_rawhtml-0.2023.6.26/
+-rw-r-----   0 woodoo    (1000) woodoo    (1000)    10173 2023-06-09 14:16:42.000000 jk_rawhtml-0.2023.6.26/LICENSE.txt
+-rw-r-----   0 woodoo    (1000) woodoo    (1000)       38 2020-01-20 22:37:00.000000 jk_rawhtml-0.2023.6.26/MANIFEST.in
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)    12185 2023-06-26 20:50:18.932358 jk_rawhtml-0.2023.6.26/PKG-INFO
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     9137 2020-01-20 22:36:59.000000 jk_rawhtml-0.2023.6.26/README.md
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-26 20:50:18.932358 jk_rawhtml-0.2023.6.26/jk_rawhtml/
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2144 2023-06-10 07:56:22.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/CSSMap.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2976 2021-02-23 20:19:58.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/CSSStyleGroup.py
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     2526 2023-06-23 20:01:47.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/Color.py
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     3215 2023-06-23 20:01:50.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/ColorSpectrum.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1130 2019-04-05 15:58:19.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5HeadElement.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1256 2019-04-05 15:58:15.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5RootElement.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10421 2023-06-17 18:46:50.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5Scope.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      895 2019-04-05 15:58:07.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLComment.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3974 2023-06-26 20:47:37.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLElement.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      744 2021-02-23 14:28:29.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLRawCSS.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      720 2019-04-07 09:03:02.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLRawText.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1132 2023-06-10 06:28:02.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLStyleElement.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      958 2021-07-12 22:04:48.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLText.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1660 2023-06-10 06:17:33.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLCSSProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1642 2023-06-10 06:17:07.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLCommentProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2781 2023-06-10 11:25:16.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLElementProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1629 2023-06-10 06:18:26.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLRawCSSProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1642 2023-06-10 06:19:10.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLRawTextProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1630 2023-06-10 06:18:47.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLTextProto.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      603 2023-06-26 20:38:46.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/__init__.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      763 2023-06-10 11:24:50.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml/htmlgeneral.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-26 20:50:18.932358 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)    12185 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/PKG-INFO
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)      818 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/SOURCES.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/dependency_links.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/not-zip-safe
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       29 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/requires.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       11 2023-06-26 20:50:18.000000 jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/top_level.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2023-06-26 20:50:18.932358 jk_rawhtml-0.2023.6.26/setup.cfg
+-rw-r-----   0 woodoo    (1000) woodoo    (1000)     1398 2023-06-26 20:38:46.000000 jk_rawhtml-0.2023.6.26/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jk_rawhtml-0.2019.9.11/LICENSE.txt` & `jk_rawhtml-0.2023.6.26/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿                                 Apache License
+                                 Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
@@ -170,32 +170,7 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright {yyyy} {name of copyright owner}
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLRawText.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLRawText.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLElement.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLElement.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 from .htmlgeneral import *
 from .CSSMap import CSSMap
 
 
 
 
+
 class HTMLElement(object):
 
-	def __init__(self, proto, name):
+	def __init__(self, proto, name:str):
 		self.name = name
 		self.attributes = {}
 		self.children = []
-		self._proto = proto
+		self._proto = proto			# this is _HTMLElementProto; we cant's specify this as otherwise we'd create circular dependencies
 	#
 
 	def addAttributes(self, **attrs):
 		for k, v in attrs.items():
 			if k.startswith("_"):
 				self.attributes[k[1:]] = v
 			else:
@@ -70,29 +71,55 @@
 		self._attrsToStr(ret)
 		ret.append(">")
 		return ret
 	#
 
 	def _attrsToStr(self, ret:list):
 		for k, v in self.attributes.items():
+			if v is None:
+				continue
+
 			if k == "style":
 				if isinstance(v, str):
 					v = v.strip()
 					if v:
 						ret.extend((" style=\"", v, "\""))
 				elif isinstance(v, CSSMap):
 					if v:
 						ret.extend((" style=\"", str(v), "\""))
+				elif isinstance(v, dict):
+					if v:
+						_ruleset = CSSMap(**v)
+						ret.extend((" style=\"", str(_ruleset), "\""))
+				else:
+					raise Exception("Unexpected value specified for HTML tag attribute '" + k + "': type " + str(type(v)) + ", value " + repr(v))
+
+			elif k == "class":
+				if isinstance(v, str):
+					ret.extend((" ", k, "=\"", htmlEscape(v), "\""))
+				elif isinstance(v, list):
+					_xList = []
+					for x in v:
+						if not x:
+							continue
+						assert isinstance(x, str)
+						if x not in _xList:
+							_xList.append(x)
+					if _xList:
+						ret.extend((" ", k, "=\"", htmlEscape(" ".join(_xList)), "\""))
 				else:
 					raise Exception("Unexpected value specified for HTML tag attribute '" + k + "': type " + str(type(v)) + ", value " + repr(v))
+
 			else:
 				if isinstance(v, (int, float)):
 					ret.extend((" ", k, "=\"", str(v), "\""))
 				elif isinstance(v, str):
 					ret.extend((" ", k, "=\"", htmlEscape(v), "\""))
+				elif v is None:
+					ret.extend((" ", k, "=\"\""))
 				else:
 					raise Exception("Unexpected value specified for HTML tag attribute '" + k + "': type " + str(type(v)) + ", value " + repr(v))
 	#
 
 	def _closingTagData(self):
 		return [ "</", self.name, ">" ]
 	#
@@ -104,15 +131,19 @@
 	#
 
 	def _serialize(self, w:HWriter):
 		if self._proto.bLineBreakOuter:
 			w.lineBreak()
 		w.write(self._openingTagData())
 
-		if self._proto.bHasClosingTag:
+		bHasClosingTag = self._proto.bHasClosingTag
+		if bHasClosingTag is HTML_CLOSING_TAG_MAYBE:
+			bHasClosingTag = len(self.children) > 0
+
+		if bHasClosingTag:
 			w.incrementIndent()
 			if self._proto.bLineBreakInner:
 				if self.children:
 					w.lineBreak()
 					for child in self.children:
 						if isinstance(child, (int, float, str)):
 							w.write(htmlEscape(str(child)))
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5RootElement.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5RootElement.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLRawCSS.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLRawCSS.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	def __init__(self, textOrTextList):
 		if isinstance(textOrTextList, str):
 			self.texts = [ textOrTextList ]
 		else:
 			self.texts = list(textOrTextList)
 	#
 
-	def __call__(self, **attrs):
+	def __call__(self, *attrs):
 		self.texts.append("".join(attrs))
 		return self
 	#
 
 	def __getitem__(self, textOrTexts):
 		if hasattr(type(textOrTexts), "__iter__"):
 			self.texts.extend(textOrTexts)
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/ColorSpectrum.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/ColorSpectrum.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5HeadElement.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5HeadElement.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/Color.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/Color.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTMLComment.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTMLComment.py`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/HTML5Scope.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/HTML5Scope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,159 @@
 
 
 
+import typing
 
 from .htmlgeneral import *
 from ._HTMLElementProto import _HTMLElementProto, HTMLElement
 from ._HTMLCommentProto import _HTMLCommentProto, HTMLComment
 from ._HTMLRawTextProto import _HTMLRawTextProto, HTMLRawText
+from ._HTMLTextProto import _HTMLTextProto, HTMLText
 from ._HTMLRawCSSProto import _HTMLRawCSSProto, HTMLRawCSS
+from ._HTMLCSSProto import _HTMLCSSProto
 from .HTML5RootElement import HTML5RootElement
 from .HTML5HeadElement import HTML5HeadElement
 
 
 
 
 
+
+HTML5Scope = typing.NewType("HTML5Scope", object)
+
 class HTML5Scope(object):
 
-	a = _HTMLElementProto("a", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	abbr = _HTMLElementProto("abbr", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	address = _HTMLElementProto("address", tagType=HTML_TAG_TYPE_STRUCTURE)
-	area = _HTMLElementProto("area", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	article = _HTMLElementProto("article", tagType=HTML_TAG_TYPE_STRUCTURE)
-	audio = _HTMLElementProto("audio", tagType=HTML_TAG_TYPE_STRUCTURE)
-	b = _HTMLElementProto("b", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	big = _HTMLElementProto("big", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	base = _HTMLElementProto("base", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# bdi = _HTMLElementProto("bdi", tagType=XXXXX)
-	# bdo = _HTMLElementProto("bdo", tagType=XXXXX)
-	blockquote = _HTMLElementProto("blockquote", tagType=HTML_TAG_TYPE_STRUCTURE)
-	body = _HTMLElementProto("body", tagType=HTML_TAG_TYPE_STRUCTURE)
-	br = _HTMLElementProto("br", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	button = _HTMLElementProto("button", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	# canvas = _HTMLElementProto("canvas", tagType=XXXXX)
-	caption = _HTMLElementProto("caption", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	cite = _HTMLElementProto("cite", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	code = _HTMLElementProto("code", tagType=HTML_TAG_TYPE_STRUCTURE)
-	col = _HTMLElementProto("col", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	colgroup = _HTMLElementProto("colgroup", tagType=HTML_TAG_TYPE_STRUCTURE)
-	command = _HTMLElementProto("command", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_ALL)
-	data = _HTMLElementProto("data", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	datalist = _HTMLElementProto("datalist", tagType=HTML_TAG_TYPE_STRUCTURE)
-	_del = _HTMLElementProto("del", tagType=HTML_TAG_TYPE_INLINE_ALL)			# problem
-	details = _HTMLElementProto("details", tagType=HTML_TAG_TYPE_STRUCTURE)
-	dfn = _HTMLElementProto("dfn", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	dl = _HTMLElementProto("dl", tagType=HTML_TAG_TYPE_STRUCTURE)
-	dt = _HTMLElementProto("dt", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	dd = _HTMLElementProto("dd", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	div = _HTMLElementProto("div", tagType=HTML_TAG_TYPE_STRUCTURE)
-	em = _HTMLElementProto("em", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	embed = _HTMLElementProto("embed", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	fieldset = _HTMLElementProto("fieldset", tagType=HTML_TAG_TYPE_STRUCTURE)
-	figcaption = _HTMLElementProto("figcaption", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	figure = _HTMLElementProto("figure", tagType=HTML_TAG_TYPE_STRUCTURE)
-	footer = _HTMLElementProto("footer", tagType=HTML_TAG_TYPE_STRUCTURE)
-	form = _HTMLElementProto("form", tagType=HTML_TAG_TYPE_STRUCTURE)
-	h1 = _HTMLElementProto("h1", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	h2 = _HTMLElementProto("h2", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	h3 = _HTMLElementProto("h3", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	h4 = _HTMLElementProto("h4", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	h5 = _HTMLElementProto("h5", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	h6 = _HTMLElementProto("h6", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	head = _HTMLElementProto("head", tagType=HTML_TAG_TYPE_STRUCTURE, implClass=HTML5HeadElement)
-	header = _HTMLElementProto("header", tagType=HTML_TAG_TYPE_STRUCTURE)
-	hr = _HTMLElementProto("hr", bHasClosingTag=False, tagType=HTML_TAG_TYPE_STRUCTURE)
-	html = _HTMLElementProto("html", tagType=HTML_TAG_TYPE_STRUCTURE, implClass=HTML5RootElement)
-	i = _HTMLElementProto("i", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	img = _HTMLElementProto("img", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_ALL)
-	_input = _HTMLElementProto("input", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)			# problem
-	ins = _HTMLElementProto("ins", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# kbd = _HTMLElementProto("kbd", tagType=XXXXX)
-	# keygen = _HTMLElementProto("keygen", bHasClosingTag=False, tagType=XXXXX)
-	label = _HTMLElementProto("label", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	legend = _HTMLElementProto("legend", tagType=HTML_TAG_TYPE_STRUCTURE)
-	li = _HTMLElementProto("li", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	link = _HTMLElementProto("link", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	main = _HTMLElementProto("main", tagType=HTML_TAG_TYPE_STRUCTURE)
-	_map = _HTMLElementProto("map", tagType=HTML_TAG_TYPE_STRUCTURE)			# problem
-	mark = _HTMLElementProto("mark", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# math = _HTMLElementProto("math", tagType=XXXXX)		# https://developer.mozilla.org/de/docs/Web/MathML/Element/math
-	menu = _HTMLElementProto("menu", tagType=HTML_TAG_TYPE_STRUCTURE)
-	menuitem = _HTMLElementProto("menuitem", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	meta = _HTMLElementProto("meta", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	meter = _HTMLElementProto("meter", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	_object = _HTMLElementProto("object", tagType=HTML_TAG_TYPE_STRUCTURE)		# problem
-	ol = _HTMLElementProto("ol", tagType=HTML_TAG_TYPE_STRUCTURE)
-	optgroup = _HTMLElementProto("optgroup", tagType=HTML_TAG_TYPE_STRUCTURE)
-	option = _HTMLElementProto("option", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	output = _HTMLElementProto("output", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	p = _HTMLElementProto("p", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	param = _HTMLElementProto("param", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	picture = _HTMLElementProto("picture", tagType=HTML_TAG_TYPE_STRUCTURE)
-	# pre = _HTMLElementProto("pre", tagType=XXXXX)
-	progress = _HTMLElementProto("progress", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	q = _HTMLElementProto("q", tagType=HTML_TAG_TYPE_STRUCTURE)
-	section = _HTMLElementProto("section", tagType=HTML_TAG_TYPE_STRUCTURE)
-	s = _HTMLElementProto("s", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	samp = _HTMLElementProto("samp", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# script = _HTMLElementProto("script", tagType=XXXXX)
-	select = _HTMLElementProto("select", tagType=HTML_TAG_TYPE_STRUCTURE)
-	small = _HTMLElementProto("small", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	source = _HTMLElementProto("source", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	span = _HTMLElementProto("span", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	strong = _HTMLElementProto("strong", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# style = _HTMLElementProto("style", bHasClosingTag=False, tagType=XXXXX)
-	summary = _HTMLElementProto("summary", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	sub = _HTMLElementProto("sub", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	sup = _HTMLElementProto("sup", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# svg = _HTMLElementProto("svg", tagType=XXXXX)
-	table = _HTMLElementProto("table", tagType=HTML_TAG_TYPE_STRUCTURE)
-	textarea = _HTMLElementProto("textarea", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	tbody = _HTMLElementProto("tbody", tagType=HTML_TAG_TYPE_STRUCTURE)
-	td = _HTMLElementProto("td", tagType=HTML_TAG_TYPE_STRUCTURE)
-	tfoot = _HTMLElementProto("tfoot", tagType=HTML_TAG_TYPE_STRUCTURE)
-	th = _HTMLElementProto("td", tagType=HTML_TAG_TYPE_STRUCTURE)
-	thead = _HTMLElementProto("thead", tagType=HTML_TAG_TYPE_STRUCTURE)
-	time = _HTMLElementProto("time", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	title = _HTMLElementProto("title", tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	tr = _HTMLElementProto("tr", tagType=HTML_TAG_TYPE_STRUCTURE)
-	track = _HTMLElementProto("track", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_CONTENT)
-	u = _HTMLElementProto("u", tagType=HTML_TAG_TYPE_INLINE_ALL)
-	ul = _HTMLElementProto("ul", tagType=HTML_TAG_TYPE_STRUCTURE)
-	var = _HTMLElementProto("var", tagType=HTML_TAG_TYPE_STRUCTURE)
-	video = _HTMLElementProto("video", tagType=HTML_TAG_TYPE_STRUCTURE)
-	wbr = _HTMLElementProto("wbr", bHasClosingTag=False, tagType=HTML_TAG_TYPE_INLINE_ALL)
-	# TODO: add support for comments
+	a =				_HTMLElementProto("a",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	abbr =			_HTMLElementProto("abbr",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	address =		_HTMLElementProto("address",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	area =			_HTMLElementProto("area", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	article =		_HTMLElementProto("article",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	audio =			_HTMLElementProto("audio",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	b =				_HTMLElementProto("b",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	big =			_HTMLElementProto("big",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	base =			_HTMLElementProto("base", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_ALL)
+	# bdi =			_HTMLElementProto("bdi",												tagType=XXXXX)
+	# bdo =			_HTMLElementProto("bdo",												tagType=XXXXX)
+	blockquote =	_HTMLElementProto("blockquote",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	body =			_HTMLElementProto("body",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	br =			_HTMLElementProto("br",			bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	button =		_HTMLElementProto("button",												tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	# canvas =		_HTMLElementProto("canvas",												tagType=XXXXX)
+	caption =		_HTMLElementProto("caption",											tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	cite =			_HTMLElementProto("cite",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	code =			_HTMLElementProto("code",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	col =			_HTMLElementProto("col", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	colgroup =		_HTMLElementProto("colgroup",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	command =		_HTMLElementProto("command", 	bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_ALL)
+	data =			_HTMLElementProto("data",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	datalist =		_HTMLElementProto("datalist",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	_del =			_HTMLElementProto("del",												tagType=HTML_TAG_TYPE_INLINE_ALL)			# problem
+	details =		_HTMLElementProto("details",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	dfn =			_HTMLElementProto("dfn",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	dl =			_HTMLElementProto("dl",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	dt =			_HTMLElementProto("dt",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	dd =			_HTMLElementProto("dd",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	div =			_HTMLElementProto("div",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	em =			_HTMLElementProto("em",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	embed =			_HTMLElementProto("embed",		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	fieldset =		_HTMLElementProto("fieldset",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	figcaption =	_HTMLElementProto("figcaption",											tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	figure =		_HTMLElementProto("figure",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	footer =		_HTMLElementProto("footer",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	form =			_HTMLElementProto("form",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	formInput =		_HTMLElementProto("input", 		bHasClosingTag=HTML_CLOSING_TAG_MAYBE,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h1 =			_HTMLElementProto("h1",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h2 =			_HTMLElementProto("h2",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h3 =			_HTMLElementProto("h3",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h4 =			_HTMLElementProto("h4",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h5 =			_HTMLElementProto("h5",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	h6 =			_HTMLElementProto("h6",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	head =			_HTMLElementProto("head",												tagType=HTML_TAG_TYPE_STRUCTURE, implClass=HTML5HeadElement)
+	header =		_HTMLElementProto("header",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	hr =			_HTMLElementProto("hr", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_STRUCTURE)
+	html =			_HTMLElementProto("html",												tagType=HTML_TAG_TYPE_STRUCTURE, implClass=HTML5RootElement)
+	i =				_HTMLElementProto("i",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	img =			_HTMLElementProto("img",		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_ALL)
+	_input =		_HTMLElementProto("input",		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)			# problem
+	ins =			_HTMLElementProto("ins",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	# kbd =			_HTMLElementProto("kbd",												tagType=XXXXX)
+	# keygen =		_HTMLElementProto("keygen",		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=XXXXX)
+	label =			_HTMLElementProto("label",		bHasClosingTag=HTML_CLOSING_TAG_ALWAYS,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	legend =		_HTMLElementProto("legend",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	li =			_HTMLElementProto("li",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	link =			_HTMLElementProto("link", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	main =			_HTMLElementProto("main",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	_map =			_HTMLElementProto("map",												tagType=HTML_TAG_TYPE_STRUCTURE)			# problem
+	mark =			_HTMLElementProto("mark",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	# math =		_HTMLElementProto("math",												tagType=XXXXX)		# https://developer.mozilla.org/de/docs/Web/MathML/Element/math
+	menu =			_HTMLElementProto("menu",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	menuitem =		_HTMLElementProto("menuitem",											tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	meta =			_HTMLElementProto("meta", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	meter =			_HTMLElementProto("meter",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	nav =			_HTMLElementProto("nav",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	_object =		_HTMLElementProto("object",												tagType=HTML_TAG_TYPE_STRUCTURE)		# problem
+	ol =			_HTMLElementProto("ol",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	optgroup =		_HTMLElementProto("optgroup",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	option =		_HTMLElementProto("option", 	bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	output =		_HTMLElementProto("output",												tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	p =				_HTMLElementProto("p",													tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	param =			_HTMLElementProto("param", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	picture =		_HTMLElementProto("picture",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	# pre =			_HTMLElementProto("pre",												tagType=XXXXX)
+	progress =		_HTMLElementProto("progress",											tagType=HTML_TAG_TYPE_INLINE_ALL)
+	q =				_HTMLElementProto("q",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	section =		_HTMLElementProto("section",											tagType=HTML_TAG_TYPE_STRUCTURE)
+	s =				_HTMLElementProto("s",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	samp =			_HTMLElementProto("samp",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	script =		_HTMLElementProto("script",												tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	select =		_HTMLElementProto("select",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	small =			_HTMLElementProto("small",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	source =		_HTMLElementProto("source", 	bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	span =			_HTMLElementProto("span",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	strong =		_HTMLElementProto("strong",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	# style =		_HTMLElementProto("style", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=XXXXX)
+	summary =		_HTMLElementProto("summary",											tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	sub =			_HTMLElementProto("sub",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	sup =			_HTMLElementProto("sup",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	# svg =			_HTMLElementProto("svg",												tagType=XXXXX)
+	table =			_HTMLElementProto("table",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	textarea =		_HTMLElementProto("textarea",											tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	tbody =			_HTMLElementProto("tbody",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	td =			_HTMLElementProto("td",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	tfoot =			_HTMLElementProto("tfoot",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	th =			_HTMLElementProto("th",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	thead =			_HTMLElementProto("thead",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	time =			_HTMLElementProto("time",												tagType=HTML_TAG_TYPE_INLINE_ALL)
+	title =			_HTMLElementProto("title",												tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	tr =			_HTMLElementProto("tr",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	track =			_HTMLElementProto("track", 		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_CONTENT)
+	u =				_HTMLElementProto("u",													tagType=HTML_TAG_TYPE_INLINE_ALL)
+	ul =			_HTMLElementProto("ul",													tagType=HTML_TAG_TYPE_STRUCTURE)
+	var =			_HTMLElementProto("var",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	video =			_HTMLElementProto("video",												tagType=HTML_TAG_TYPE_STRUCTURE)
+	wbr =			_HTMLElementProto("wbr",		bHasClosingTag=HTML_CLOSING_TAG_NEVER,	tagType=HTML_TAG_TYPE_INLINE_ALL)
 
-	def __enter__(self):
+	def __enter__(self) -> HTML5Scope:
 		return self
 	#
 
 	def __exit__(self, exc_type, exc_val, exc_tb):
 		pass
 	#
 
 	comment = _HTMLCommentProto()
 
 	raw_html = _HTMLRawTextProto()
 
 	raw_style_css = _HTMLRawCSSProto()
 
+	style_css = _HTMLCSSProto()
+
+	_text = _HTMLTextProto()
+
 #
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml/_HTMLElementProto.py` & `jk_rawhtml-0.2023.6.26/jk_rawhtml/_HTMLElementProto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 
 
+import typing
+
+import jk_prettyprintobj
+
 from .HTMLElement import HTMLElement
 from .htmlgeneral import *
 
 
 
 
-class _HTMLElementProto(object):
+class _HTMLElementProto(jk_prettyprintobj.DumpMixin):
+
+
+	################################################################################################################################
+	## Constructor
+	################################################################################################################################
 
-	def __init__(self, name:str, bHasClosingTag=True, tagType=HTML_TAG_TYPE_INLINE_CONTENT, implClass=HTMLElement, extraAttributes:dict=None):
+	#
+	# Constructor method.
+	#
+	def __init__(self, name:str, bHasClosingTag=HTML_CLOSING_TAG_ALWAYS, tagType=HTML_TAG_TYPE_INLINE_CONTENT, implClass=HTMLElement, extraAttributes:dict=None):
 		assert isinstance(name, str)
-		assert isinstance(bHasClosingTag, bool)
+		if bHasClosingTag is not None:
+			assert isinstance(bHasClosingTag, bool)
 
 		self.name = name
 		self.bHasClosingTag = bHasClosingTag
 		self.tagType = tagType
 		self.implClass = implClass
 
 		if tagType == HTML_TAG_TYPE_INLINE_CONTENT:
@@ -32,15 +45,39 @@
 		if extraAttributes:
 			assert isinstance(extraAttributes, dict)
 			self.extraAttributes = extraAttributes
 		else:
 			self.extraAttributes = None
 	#
 
-	def __call__(self, *args, **attrs):
+	################################################################################################################################
+	## Public Properties
+	################################################################################################################################
+
+	################################################################################################################################
+	## Helper Methods
+	################################################################################################################################
+
+	def _dumpVarNames(self) -> typing.List[str]:
+		return [
+			"name",
+			"bHasClosingTag",
+			"tagType",
+			"implClass",
+			"bLineBreakOuter",
+			"bLineBreakInner",
+			"extraAttributes",
+		]
+	#
+
+	################################################################################################################################
+	## Public Methods
+	################################################################################################################################
+
+	def __call__(self, *args, **attrs) -> HTMLElement:
 		if self.extraAttributes:
 			d = dict(self.extraAttributes)
 			d.update(attrs)
 			return self.implClass(self, self.name)(**d)
 		else:
 			return self.implClass(self, self.name)(**attrs)
 	#
@@ -53,7 +90,11 @@
 
 
 
 
 
 
 
+
+
+
+
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/PKG-INFO` & `jk_rawhtml-0.2023.6.26/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: jk-rawhtml
-Version: 0.2019.9.11
+Name: jk_rawhtml
+Version: 0.2023.6.26
 Summary: This python module provides support for programmatically generating HTML5 code.
-Home-page: https://github.com/jkpubsrc/python-module-jk-rawhtml
+Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
-License: Apache 2.0
-Download-URL: https://github.com/jkpubsrc/python-module-jk-rawhtml/tarball/0.2019.9.11
+License: Apache2
 Description: jk_rawhtml
         ==========
         
         Introduction
         ------------
         
         This python module provides support for programmatically generating HTML5 code.
@@ -325,11 +324,11 @@
         * Apache Software License 2.0
         
         
         
         
 Keywords: html,css,html5
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `jk_rawhtml-0.2019.9.11/jk_rawhtml.egg-info/SOURCES.txt` & `jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 jk_rawhtml/CSSMap.py
+jk_rawhtml/CSSStyleGroup.py
 jk_rawhtml/Color.py
 jk_rawhtml/ColorSpectrum.py
 jk_rawhtml/HTML5HeadElement.py
 jk_rawhtml/HTML5RootElement.py
 jk_rawhtml/HTML5Scope.py
 jk_rawhtml/HTMLComment.py
 jk_rawhtml/HTMLElement.py
 jk_rawhtml/HTMLRawCSS.py
 jk_rawhtml/HTMLRawText.py
+jk_rawhtml/HTMLStyleElement.py
+jk_rawhtml/HTMLText.py
+jk_rawhtml/_HTMLCSSProto.py
 jk_rawhtml/_HTMLCommentProto.py
 jk_rawhtml/_HTMLElementProto.py
 jk_rawhtml/_HTMLRawCSSProto.py
 jk_rawhtml/_HTMLRawTextProto.py
+jk_rawhtml/_HTMLTextProto.py
 jk_rawhtml/__init__.py
 jk_rawhtml/htmlgeneral.py
 jk_rawhtml.egg-info/PKG-INFO
 jk_rawhtml.egg-info/SOURCES.txt
 jk_rawhtml.egg-info/dependency_links.txt
 jk_rawhtml.egg-info/not-zip-safe
 jk_rawhtml.egg-info/requires.txt
```

### Comparing `jk_rawhtml-0.2019.9.11/README.md` & `jk_rawhtml-0.2023.6.26/README.md`

 * *Files identical despite different names*

### Comparing `jk_rawhtml-0.2019.9.11/setup.py` & `jk_rawhtml-0.2023.6.26/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,33 +15,38 @@
 	with open("README.md", "r", encoding="UTF-8-sig") as f:
 		return f.read()
 
 setup(
 	author = "Jürgen Knauth",
 	author_email = "pubsrc@binary-overflow.de",
 	classifiers = [
-		"Programming Language :: Python :: 3",
 		"Development Status :: 4 - Beta",
 		"License :: OSI Approved :: Apache Software License",
+		"Programming Language :: Python :: 3",
 	],
 	description = "This python module provides support for programmatically generating HTML5 code.",
-	download_url = "https://github.com/jkpubsrc/python-module-jk-rawhtml/tarball/0.2019.9.11",
-	include_package_data = False,
+	include_package_data = True,
 	install_requires = [
 		"jk_hwriter",
+		"jk_prettyprintobj",
 	],
 	keywords = [
 		"html",
 		"css",
 		"html5",
 	],
-	license = "Apache 2.0",
+	license = "Apache2",
 	name = "jk_rawhtml",
+	package_data = {
+		"": [
+		],
+	},
 	packages = [
 		"jk_rawhtml",
 	],
-	url = "https://github.com/jkpubsrc/python-module-jk-rawhtml",
-	version = "0.2019.9.11",
+	scripts = [
+	],
+	version = '0.2023.6.26',
 	zip_safe = False,
 	long_description = readme(),
-	long_description_content_type="text/markdown",
+	long_description_content_type = "text/markdown",
 )
```

### Comparing `jk_rawhtml-0.2019.9.11/PKG-INFO` & `jk_rawhtml-0.2023.6.26/jk_rawhtml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: jk_rawhtml
-Version: 0.2019.9.11
+Name: jk-rawhtml
+Version: 0.2023.6.26
 Summary: This python module provides support for programmatically generating HTML5 code.
-Home-page: https://github.com/jkpubsrc/python-module-jk-rawhtml
+Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
-License: Apache 2.0
-Download-URL: https://github.com/jkpubsrc/python-module-jk-rawhtml/tarball/0.2019.9.11
+License: Apache2
 Description: jk_rawhtml
         ==========
         
         Introduction
         ------------
         
         This python module provides support for programmatically generating HTML5 code.
@@ -325,11 +324,11 @@
         * Apache Software License 2.0
         
         
         
         
 Keywords: html,css,html5
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

