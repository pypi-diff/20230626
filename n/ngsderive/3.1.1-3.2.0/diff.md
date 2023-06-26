# Comparing `tmp/ngsderive-3.1.1.tar.gz` & `tmp/ngsderive-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngsderive-3.1.1.tar", max compression
+gzip compressed data, was "ngsderive-3.2.0.tar", max compression
```

## Comparing `ngsderive-3.1.1.tar` & `ngsderive-3.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1077 2023-05-08 20:12:05.819838 ngsderive-3.1.1/LICENSE.md
--rw-r--r--   0        0        0     4846 2023-05-08 20:12:05.819838 ngsderive-3.1.1/README.md
--rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/__init__.py
--rwxr-xr-x   0        0        0     9781 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/__main__.py
--rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/__init__.py
--rw-r--r--   0        0        0     2482 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/encoding.py
--rwxr-xr-x   0        0        0     9238 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/instrument.py
--rw-r--r--   0        0        0    11008 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/junction_annotation.py
--rwxr-xr-x   0        0        0     2260 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/readlen.py
--rwxr-xr-x   0        0        0    11914 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/strandedness.py
--rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/readers/__init__.py
--rwxr-xr-x   0        0        0       13 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/readers/bam.py
--rwxr-xr-x   0        0        0    14826 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/utils.py
--rw-r--r--   0        0        0     1585 2023-05-08 20:12:47.616349 ngsderive-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 ngsderive-3.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-06-26 14:48:03.089408 ngsderive-3.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4846 2023-06-26 14:48:03.089408 ngsderive-3.2.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/__init__.py
+-rwxr-xr-x   0        0        0     9781 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/__init__.py
+-rw-r--r--   0        0        0     2482 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/encoding.py
+-rwxr-xr-x   0        0        0     9658 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/instrument.py
+-rw-r--r--   0        0        0    11008 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/junction_annotation.py
+-rwxr-xr-x   0        0        0     2260 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/readlen.py
+-rwxr-xr-x   0        0        0    11914 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/commands/strandedness.py
+-rwxr-xr-x   0        0        0        0 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/readers/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/readers/bam.py
+-rwxr-xr-x   0        0        0    14826 2023-06-26 14:48:03.089408 ngsderive-3.2.0/ngsderive/utils.py
+-rw-r--r--   0        0        0     1585 2023-06-26 14:48:49.776485 ngsderive-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5908 1970-01-01 00:00:00.000000 ngsderive-3.2.0/PKG-INFO
```

### Comparing `ngsderive-3.1.1/LICENSE.md` & `ngsderive-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/README.md` & `ngsderive-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/__main__.py` & `ngsderive-3.2.0/ngsderive/__main__.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/commands/encoding.py` & `ngsderive-3.2.0/ngsderive/commands/encoding.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/commands/instrument.py` & `ngsderive-3.2.0/ngsderive/commands/instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -223,30 +223,42 @@
             continue
 
         instruments = set()
         flowcells = set()
         malformed_read_names = False
 
         # accumulate instrument and flowcell IDs
-        for read in itertools.islice(ngsfile, n_samples):
-            parts = read["query_name"].split(":")
-            if len(parts) != 7:  # not Illumina format
-                malformed_read_names = True
-                iid = parts[0]  # attempt to recover machine name
+        try:
+            for read in itertools.islice(ngsfile, n_samples):
+                parts = read["query_name"].split(":")
+                if len(parts) != 7:  # not Illumina format
+                    malformed_read_names = True
+                    iid = parts[0]  # attempt to recover machine name
+                    instruments.add(iid)
+                    for rg in ngsfile.handle.header.to_dict()["RG"]:
+                        if rg["ID"] == read["read_group"]:
+                            if "PU" in rg:
+                                flowcells.add(rg["PU"])
+                            if "PM" in rg:
+                                instruments.add(rg["PM"])
+                    continue
+                iid, fcid = parts[0], parts[2]
                 instruments.add(iid)
-                for rg in ngsfile.handle.header.to_dict()["RG"]:
-                    if rg["ID"] == read["read_group"]:
-                        if "PU" in rg:
-                            flowcells.add(rg["PU"])
-                        if "PM" in rg:
-                            instruments.add(rg["PM"])
-                continue
-            iid, fcid = parts[0], parts[2]
-            instruments.add(iid)
-            flowcells.add(fcid)
+                flowcells.add(fcid)
+        except KeyError:  # no RG tag is present
+            result = {
+                "File": ngsfilepath,
+                "Instrument": "unknown",
+                "Confidence": "no confidence",
+                "Basis": "no RG tag present",
+            }
+            writer.writerow(result)
+            outfile.flush()
+            continue
+
         if malformed_read_names:
             logger.warning(
                 "Encountered read names not in Illumina format. Recovery attempted."
             )
         (
             possible_instruments_by_iid,
             detected_instrument_by_iid,
```

### Comparing `ngsderive-3.1.1/ngsderive/commands/junction_annotation.py` & `ngsderive-3.2.0/ngsderive/commands/junction_annotation.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/commands/readlen.py` & `ngsderive-3.2.0/ngsderive/commands/readlen.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/commands/strandedness.py` & `ngsderive-3.2.0/ngsderive/commands/strandedness.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/ngsderive/utils.py` & `ngsderive-3.2.0/ngsderive/utils.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.1/pyproject.toml` & `ngsderive-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "ngsderive"
-version = "3.1.1"
+version = "3.2.0"
 description = "Forensic analysis tool useful in backwards computing information from next-generation sequencing data."
 license = "MIT"
 authors = [
     "Clay McLeod <Clay.McLeod@STJUDE.org>",
     "Andrew Frantz <andrew.frantz@STJUDE.org"
 ]
 readme = "README.md"
```

### Comparing `ngsderive-3.1.1/PKG-INFO` & `ngsderive-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ngsderive
-Version: 3.1.1
+Version: 3.2.0
 Summary: Forensic analysis tool useful in backwards computing information from next-generation sequencing data.
 Home-page: https://github.com/claymcleod/ngsderive
 License: MIT
 Keywords: bioinformatics,genomics,sam,bam,fastq
 Author: Clay McLeod
 Author-email: Clay.McLeod@STJUDE.org
 Requires-Python: >=3.8,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
 Requires-Dist: gtfparse (>=1.2.1,<2.0.0)
 Requires-Dist: pysam (>=0.18,<0.19)
 Requires-Dist: pytabix (>=0.1,<0.2)
 Requires-Dist: rstr (>=3.0.0,<4.0.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: ngsderive Version: 3.1.1 Summary: Forensic analysis
+Metadata-Version: 2.1 Name: ngsderive Version: 3.2.0 Summary: Forensic analysis
 tool useful in backwards computing information from next-generation sequencing
 data. Home-page: https://github.com/claymcleod/ngsderive License: MIT Keywords:
 bioinformatics,genomics,sam,bam,fastq Author: Clay McLeod Author-email:
 Clay.McLeod@STJUDE.org Requires-Python: >=3.8,<3.10 Classifier: Development
 Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Dist: colorlog (>=6.6.0,<7.0.0) Requires-Dist: gtfparse
-(>=1.2.1,<2.0.0) Requires-Dist: pysam (>=0.18,<0.19) Requires-Dist: pytabix
-(>=0.1,<0.2) Requires-Dist: rstr (>=3.0.0,<4.0.0) Requires-Dist:
-sortedcontainers (>=2.4.0,<3.0.0) Project-URL: Repository, https://github.com/
-claymcleod/ngsderive Description-Content-Type: text/markdown
+Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
+Engineering :: Bio-Informatics Requires-Dist: colorlog (>=6.6.0,<7.0.0)
+Requires-Dist: gtfparse (>=1.2.1,<2.0.0) Requires-Dist: pysam (>=0.18,<0.19)
+Requires-Dist: pytabix (>=0.1,<0.2) Requires-Dist: rstr (>=3.0.0,<4.0.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0) Project-URL: Repository,
+https://github.com/claymcleod/ngsderive Description-Content-Type: text/markdown
                             ****** ngsderive ******
 [Actions:_CI_Status] [PyPI] [PyPI:_Downloads] [PyPI:_Downloads] [License:_MIT]
   Forensic analysis tool useful in backwards computing information from next-
          generation sequencing data and annotating splice junctions.
                              Explore_the_docs_Â»
 
      Request_Feature Â· Report_Bug Â· â­ Consider starring the repo! â­
```

