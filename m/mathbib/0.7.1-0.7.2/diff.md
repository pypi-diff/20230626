# Comparing `tmp/mathbib-0.7.1.tar.gz` & `tmp/mathbib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.7.1.tar", max compression
+gzip compressed data, was "mathbib-0.7.2.tar", max compression
```

## Comparing `mathbib-0.7.1.tar` & `mathbib-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.1/LICENSE
--rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.1/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.1/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.1/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.1/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.7.1/mathbib/citegen.py
--rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.1/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.1/mathbib/partition.py
--rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.1/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.1/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.1/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.1/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.1/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.1/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.1/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.1/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.1/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.1/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6688 2023-06-04 07:25:26.040065 mathbib-0.7.1/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.1/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.1/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.1/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.1/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-06-04 07:25:49.098944 mathbib-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.2/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.2/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.2/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.2/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2836 2023-06-26 12:15:04.737547 mathbib-0.7.2/mathbib/citegen.py
+-rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.2/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.2/mathbib/partition.py
+-rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.2/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.2/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.2/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.2/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.2/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.2/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.2/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.2/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.2/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.2/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6688 2023-06-04 07:43:41.660653 mathbib-0.7.2/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.2/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.2/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.2/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.2/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-06-26 12:15:30.216145 mathbib-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.2/PKG-INFO
```

### Comparing `mathbib-0.7.1/LICENSE` & `mathbib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/README.md` & `mathbib-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/bibtex.py` & `mathbib-0.7.2/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/citegen.py` & `mathbib-0.7.2/mathbib/citegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def get_citekeys(tex: str) -> frozenset[str]:
     """Retern an iterable of all citation keys contained in the provided string."""
     # a citation is a non-commented string of the form
     # \<citecommand>[...]{key1, key2, ...} first match for {key1, key2, ...}
     # and then extract the keys
     rx_citecommand = re.compile(
-        r"(?<!\\)%.+|(\\(?:|paren|foot|text|super|auto|no)citep?"
+        r"(?<!\\)%.+|(\\(?:|paren|foot|text|super|auto|no|full)citep?"
         r"(?:\[[^\]]*\])?\{((?!\*)[^{}]+)\})"
     )
     rx_citekey: Final = re.compile(r"([^\s,{}\[\]\(\)\\%#~]+)")
 
     cite_commands = (
         match.group(2) for match in rx_citecommand.finditer(tex) if match.group(2)
     )
```

### Comparing `mathbib-0.7.1/mathbib/command.py` & `mathbib-0.7.2/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/partition.py` & `mathbib-0.7.2/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/record.py` & `mathbib-0.7.2/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/__init__.py` & `mathbib-0.7.2/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/arxiv.py` & `mathbib-0.7.2/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/doi.py` & `mathbib-0.7.2/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/error.py` & `mathbib-0.7.2/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/isbn.py` & `mathbib-0.7.2/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/ol.py` & `mathbib-0.7.2/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/utils.py` & `mathbib-0.7.2/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/zbl.py` & `mathbib-0.7.2/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/remote/zbmath.py` & `mathbib-0.7.2/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/request.py` & `mathbib-0.7.2/mathbib/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,18 @@
                 [(str(keyid.key), keyid.identifier)]
                 + [rel for rel in candidates if rel is not None],
             )
 
         return None, status, []
 
     def load_record(self, keyid: KeyId) -> tuple[Optional[dict], list[tuple[str, str]]]:
-        """Attempt to load the record associated with keyid and cache a list of
-        related records. At this stage, the related records are not "final": they are
-        resolved (so they are strings) but otherwise the related records may not actually
-        be real records.
+        """Attempt to load the record associated with keyid and cache a list of related
+        records. At this stage, the related records are not "final": they are resolved
+        (so they are strings) but otherwise the related records may not actually be real
+        records.
         """
         remote_record = get_remote_record(keyid)
 
         if not remote_record.validate_identifier(keyid.identifier):
             return None, []
 
         # load cached record
```

### Comparing `mathbib-0.7.1/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.2/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/session.py` & `mathbib-0.7.2/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/mathbib/term.py` & `mathbib-0.7.2/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.1/pyproject.toml` & `mathbib-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.7.1"
+version = "0.7.2"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.7.1/PKG-INFO` & `mathbib-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.7.1
+Version: 0.7.2
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

