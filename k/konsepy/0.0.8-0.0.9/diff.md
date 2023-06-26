# Comparing `tmp/konsepy-0.0.8.tar.gz` & `tmp/konsepy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "konsepy-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `konsepy-0.0.8.tar` & `konsepy-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      996 2023-06-13 22:15:28.630545 konsepy-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-06-13 22:15:28.630545 konsepy-0.0.8/.gitignore
--rw-r--r--   0        0        0     1002 2023-06-13 22:15:28.630545 konsepy-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      335 2023-06-13 22:15:28.630545 konsepy-0.0.8/README.md
--rw-r--r--   0        0        0      905 2023-06-13 22:15:28.630545 konsepy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4149 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     3056 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/constants.py
--rw-r--r--   0        0        0     4480 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/importer.py
--rw-r--r--   0        0        0     5396 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/regex.py
--rw-r--r--   0        0        0     2469 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     5285 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/types.py
--rw-r--r--   0        0        0     1297 2023-06-13 22:15:28.630545 konsepy-0.0.8/test/build.ps1
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-06-23 20:28:55.079392 konsepy-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-06-23 20:28:55.079392 konsepy-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1160 2023-06-23 20:28:55.079392 konsepy-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      335 2023-06-23 20:28:55.079392 konsepy-0.0.9/README.md
+-rw-r--r--   0        0        0      905 2023-06-23 20:28:55.079392 konsepy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4149 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     3056 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4480 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5396 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2469 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     5344 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-06-23 20:28:55.079392 konsepy-0.0.9/src/konsepy/types.py
+-rw-r--r--   0        0        0     1297 2023-06-23 20:28:55.079392 konsepy-0.0.9/test/build.ps1
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.9/PKG-INFO
```

### Comparing `konsepy-0.0.8/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/CHANGELOG.md` & `konsepy-0.0.9/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 * `Added`: for new features.
 * `Changed`: for changes in existing functionality.
 * `Deprecated`: for soon-to-be removed features.
 * `Removed`: for now removed features.
 * `Fixed`: for any bug fixes.
 * `Security`: in case of vulnerabilities.
 
+## [0.0.9] - 2023-06-23
+
+### Fixed
+
+* When checking SAS columns, check for its presence in the header rather than if it is None since it has a default value
+
 ## [0.0.7] & [0.0.8] - 2023-06-13
 
 ### Fixed
 
 * Fixed where `noteorder_label` didn't yet get correctly passed around
 * `enum.EnumType` is only available in 3.11+, so reverted to old `enum.EnumMeta`
```

### Comparing `konsepy-0.0.8/pyproject.toml` & `konsepy-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/bio_tag.py` & `konsepy-0.0.9/src/konsepy/bio_tag.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/cli.py` & `konsepy-0.0.9/src/konsepy/cli.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/get_text_snippets.py` & `konsepy-0.0.9/src/konsepy/get_text_snippets.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/importer.py` & `konsepy-0.0.9/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/regex.py` & `konsepy-0.0.9/src/konsepy/regex.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/run_all.py` & `konsepy-0.0.9/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/rxutils.py` & `konsepy-0.0.9/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/src/konsepy/textio.py` & `konsepy-0.0.9/src/konsepy/textio.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,18 @@
     with SAS7BDAT(input_file, skip_header=False, encoding=encoding) as fh:
         header = []
         for row in fh:
             if not header:
                 header = row
                 continue
             mrn = row[header.index(id_label)]
-            date = row[header.index(notedate_label)] if notedate_label else ''
+            date = row[header.index(notedate_label)] if notedate_label and notedate_label in header else ''
             text = row[header.index(noteid_label)]
             noteid = row[header.index(notetext_label)]
-            order = row[header.index(noteorder_label)] if noteorder_label else None
+            order = row[header.index(noteorder_label)] if noteorder_label and noteorder_label in header else None
             yield mrn, text, noteid, date, order
 
 
 def _extract_csv_file(input_file, encoding, id_label, noteid_label, notedate_label,
                       notetext_label, noteorder_label=None):
     with open(input_file, encoding=encoding) as fh:
         for row in csv.DictReader(fh):
```

### Comparing `konsepy-0.0.8/test/build.ps1` & `konsepy-0.0.9/test/build.ps1`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.8/PKG-INFO` & `konsepy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

