# Comparing `tmp/fastgedcom-0.0.6.tar.gz` & `tmp/fastgedcom-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.6.tar", last modified: Mon Jun 19 15:21:41 2023, max compression
+gzip compressed data, was "fastgedcom-0.0.7.tar", last modified: Mon Jun 26 17:27:15 2023, max compression
```

## Comparing `fastgedcom-0.0.6.tar` & `fastgedcom-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4561 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.010228 fastgedcom-0.0.6/fastgedcom/
--rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-0.0.6/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     9710 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/base.py
--rw-rw-rw-   0        0        0    10766 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/family_link.py
--rw-rw-rw-   0        0        0     9568 2023-06-19 15:12:18.000000 fastgedcom-0.0.6/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     5215 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.6/fastgedcom/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.024765 fastgedcom-0.0.6/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     4561 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-16 22:46:04.000000 fastgedcom-0.0.6/fastgedcom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 15:21:40.000000 fastgedcom-0.0.6/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1408 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 15:21:41.031775 fastgedcom-0.0.6/test/
--rw-rw-rw-   0        0        0     1573 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_base.py
--rw-rw-rw-   0        0        0     7527 2023-06-19 15:18:01.000000 fastgedcom-0.0.6/test/test_date_helpers.py
--rw-rw-rw-   0        0        0     4632 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_family_link.py
--rw-rw-rw-   0        0        0     1670 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_helpers.py
--rw-rw-rw-   0        0        0     4605 2023-06-19 15:00:32.000000 fastgedcom-0.0.6/test/test_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.758745 fastgedcom-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4562 2023-06-26 17:27:15.752748 fastgedcom-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2023-06-25 20:57:19.000000 fastgedcom-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.706748 fastgedcom-0.0.7/fastgedcom/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:40:35.000000 fastgedcom-0.0.7/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     9663 2023-06-25 22:07:46.000000 fastgedcom-0.0.7/fastgedcom/base.py
+-rw-rw-rw-   0        0        0    10946 2023-06-25 22:04:48.000000 fastgedcom-0.0.7/fastgedcom/family_link.py
+-rw-rw-rw-   0        0        0     9568 2023-06-19 15:12:18.000000 fastgedcom-0.0.7/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     5215 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.7/fastgedcom/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.741782 fastgedcom-0.0.7/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     4562 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 17:27:15.000000 fastgedcom-0.0.7/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1116 2023-06-26 17:21:40.000000 fastgedcom-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:27:15.758745 fastgedcom-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 17:27:15.750746 fastgedcom-0.0.7/test/
+-rw-rw-rw-   0        0        0     2144 2023-06-26 16:00:30.000000 fastgedcom-0.0.7/test/test_base.py
+-rw-rw-rw-   0        0        0     7527 2023-06-19 15:25:59.000000 fastgedcom-0.0.7/test/test_date_helpers.py
+-rw-rw-rw-   0        0        0     4859 2023-06-25 22:04:27.000000 fastgedcom-0.0.7/test/test_family_link.py
+-rw-rw-rw-   0        0        0     1670 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/test/test_helpers.py
+-rw-rw-rw-   0        0        0     4605 2023-06-19 15:00:32.000000 fastgedcom-0.0.7/test/test_parser.py
```

### Comparing `fastgedcom-0.0.6/LICENSE` & `fastgedcom-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/PKG-INFO` & `fastgedcom-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.6
+Version: 0.0.7
 Summary: A lightweight tool to parse, browse and edit gedcom files.
-Author: Gatien Bouyer
-Author-email: gatien.bouyer.dev@gmail.com
-License: MIT
-Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
+Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
-Keywords: fastgedcom gedcom parser genealogy
+Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastgedcom-0.0.6/README.md` & `fastgedcom-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/fastgedcom/base.py` & `fastgedcom-0.0.7/fastgedcom/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 	def payload(self) -> str:
 		"""See the description of :py:class:`.TrueLine` class."""
 
 	@property
 	@abstractmethod
 	def payload_with_cont(self) -> str:
 		"""The content of this gedcom field, namely the payload combined
-		with all CONT sub-lines payload as a new line, and
-		with all CONC sub-lines payload as a space."""
+		with all CONT and CONC sub-lines."""
 
 	@abstractmethod
 	def get_sub_lines(self, tag: str) -> list['TrueLine']:
 		"""Return the all sub-lines having the given :any:`tag`.
 		An empty list if no line matches."""
 
 	def __rshift__(self, tag: str) -> list['TrueLine']:
@@ -207,18 +206,19 @@
 	def __repr__(self) -> str:
 		"""Return the string representation of the class."""
 		return f"<{self.__class__.__qualname__} {self.level} {self.tag} {self.payload} -> {len(self.sub_lines)}>"
 
 	@property
 	def payload_with_cont(self) -> str:
 		text = self.payload
-		for cont in self.get_sub_lines("CONT"):
-			text += '\n' + cont.payload
-		for conc in self.get_sub_lines("CONC"):
-			text += ' ' + conc.payload
+		for sub_line in self.sub_lines:
+			if sub_line.tag == "CONT":
+				text += '\n' + sub_line.payload
+			elif sub_line.tag == "CONC":
+				text += sub_line.payload
 		return text
 
 
 Record: TypeAlias = TrueLine
 """A level 0 line referenced by an XRef in the document."""
```

### Comparing `fastgedcom-0.0.6/fastgedcom/family_link.py` & `fastgedcom-0.0.7/fastgedcom/family_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -186,24 +186,28 @@
 
 	def get_stepsiblings(self, indi: IndiRef) -> list[Record]:
 		"""Return the stepsiblings of the person.
 		Siblings excluded."""
 		return [self.document.records[stepsibling]
 			for stepsibling in self.get_stepsiblings_ref(indi)]
 
-	def get_spouse_in_fam_ref(self, indi: IndiRef, fam: Record) -> IndiRef:
+	def get_spouse_in_fam_ref(self, indi: IndiRef, fam: Record) -> IndiRef | None:
 		"""Return the spouse's reference of the family that is not the person's."""
 		husban = fam >= "HUSB"
 		wife = fam >= "WIFE"
-		if wife == indi: return husban
-		return wife
+		if indi == wife and husban not in ("", "@VOID@"):
+			return husban
+		if indi == husban and wife not in ("", "@VOID@"):
+			return wife
+		return None
 
-	def get_spouse_in_fam(self, indi: IndiRef, fam: Record) -> Record:
+	def get_spouse_in_fam(self, indi: IndiRef, fam: Record) -> Record | FakeLine:
 		"""Return the spouse's record of the family that is not the person's."""
-		return self.document.records[self.get_spouse_in_fam_ref(indi, fam)]
+		spouse_ref = self.get_spouse_in_fam_ref(indi, fam)
+		return self.document.records[spouse_ref] if spouse_ref else fake_line
 
 	def traverse_ref(self, indi: IndiRef,
 			ascent: int = 0, descent: int = 0
 			) -> list[IndiRef]:
 		"""
 		Recursively traverse the parents of the person and then their children.
```

### Comparing `fastgedcom-0.0.6/fastgedcom/helpers.py` & `fastgedcom-0.0.7/fastgedcom/helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/fastgedcom/parser.py` & `fastgedcom-0.0.7/fastgedcom/parser.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/fastgedcom.egg-info/PKG-INFO` & `fastgedcom-0.0.7/fastgedcom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.6
+Version: 0.0.7
 Summary: A lightweight tool to parse, browse and edit gedcom files.
-Author: Gatien Bouyer
-Author-email: gatien.bouyer.dev@gmail.com
-License: MIT
-Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
+Author-email: Gatien Bouyer <gatien.bouyer.dev@gmail.com>
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
 Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
-Keywords: fastgedcom gedcom parser genealogy
+Keywords: fastgedcom,gedcom,parser,genealogy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastgedcom-0.0.6/test/test_base.py` & `fastgedcom-0.0.7/test/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,21 +23,31 @@
 			TrueLine(1, "CHIL", "@I7@"), TrueLine(1, "CHIL", "@I41@")
 		])
 		self.assertListEqual(list(doc["@F99@"] >> "CHIL"), [])
 
 	def test_payload_with_cont(self) -> None:
 		note_text1 = "This is a text\non several\nlines"
 		note_line1 = TrueLine(1, "NOTE", "This is a text", [
-			TrueLine(1, "CONT", "on several"),
-			TrueLine(1, "CONT", "lines"),
+			TrueLine(2, "CONT", "on several"),
+			TrueLine(2, "CONT", "lines"),
 		])
 		self.assertEqual(note_line1.payload_with_cont, note_text1)
 		note_text2 = "This is a very long text that is split"
 		note_line2 = TrueLine(1, "NOTE", "This is a very", [
-			TrueLine(1, "CONC", "long text"),
-			TrueLine(1, "CONC", "that is split"),
+			TrueLine(2, "CONC", " long text th"),
+			TrueLine(2, "CONC", "at is split"),
 		])
 		self.assertEqual(note_line2.payload_with_cont, note_text2)
+		note_text3 = "This text is on several lines:\nTo present a very long text that is split.\n\nAnd a second one:\nAlso a very long sentence that is split."
+		note_line3 = TrueLine(1, "NOTE", "This text is on several lines:", [
+			TrueLine(2, "CONT", "To present a very long"),
+			TrueLine(2, "CONC", " text that is split."),
+			TrueLine(2, "CONT", ""),
+			TrueLine(2, "CONT", "And a second one:"),
+			TrueLine(2, "CONT", "Also a very long sent"),
+			TrueLine(2, "CONC", "ence that is split."),
+		])
+		self.assertEqual(note_line3.payload_with_cont, note_text3)
 
 
 if __name__ == '__main__':
 	unittest.main()
```

### Comparing `fastgedcom-0.0.6/test/test_date_helpers.py` & `fastgedcom-0.0.7/test/test_date_helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/test/test_family_link.py` & `fastgedcom-0.0.7/test/test_family_link.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,22 @@
 		self.assertCountEqual(self.linker.get_spouses_ref("@I1@"), ["@I4@", "@I5@"])
 
 	def test_get_spouse_in_fam(self) -> None:
 		self.assertEqual(
 			self.linker.get_spouse_in_fam_ref("@I1@", self.document.records["@F2@"]),
 			"@I4@"
 		)
+		self.assertEqual(
+			self.linker.get_spouse_in_fam_ref("@I1@", self.document.records["@F10@"]),
+			None
+		)
+		self.assertEqual(
+			self.linker.get_spouse_in_fam_ref("@I6@", self.document.records["@F4@"]),
+			None
+		)
 
 	def test_get_children(self) -> None:
 		self.assertCountEqual(self.linker.get_children_ref("@I1@"), ["@I6@", "@I7@", "@I41@"])
 
 	def test_get_children_with(self) -> None:
 		self.assertCountEqual(self.linker.get_children_with_ref("@I1@", "@I5@"), ["@I7@", "@I41@"])
```

### Comparing `fastgedcom-0.0.6/test/test_helpers.py` & `fastgedcom-0.0.7/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.6/test/test_parser.py` & `fastgedcom-0.0.7/test/test_parser.py`

 * *Files identical despite different names*

