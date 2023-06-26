# Comparing `tmp/varvamp-0.8.2.tar.gz` & `tmp/varvamp-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.8.2.tar", last modified: Fri Apr 28 10:34:09 2023, max compression
+gzip compressed data, was "varvamp-0.8.3.tar", last modified: Mon Jun 26 16:09:33 2023, max compression
```

## Comparing `varvamp-0.8.2.tar` & `varvamp-0.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:34:09.119833 varvamp-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-28 10:34:09.119833 varvamp-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-28 10:33:51.000000 varvamp-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:34:09.119833 varvamp-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 10:33:51.000000 varvamp-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:34:09.115833 varvamp-0.8.2/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:34:09.119833 varvamp-0.8.2/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-28 10:33:51.000000 varvamp-0.8.2/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:34:09.115833 varvamp-0.8.2/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:34:08.000000 varvamp-0.8.2/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 10:34:09.000000 varvamp-0.8.2/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-26 16:09:33.775199 varvamp-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-26 16:09:15.000000 varvamp-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:09:33.775199 varvamp-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 16:09:15.000000 varvamp-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.771199 varvamp-0.8.3/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16242 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-26 16:09:15.000000 varvamp-0.8.3/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:09:33.775199 varvamp-0.8.3/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 16:09:33.000000 varvamp-0.8.3/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.8.2/PKG-INFO` & `varvamp-0.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8.2
+Version: 0.8.3
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -17,32 +17,33 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="./docs/varvamp.png" alt="varVAMP logo" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
-<img src="./docs/sanger.png" alt="sanger" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/sanger.png" alt="sanger" />
 
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
-<img src="./docs/tiled.png" alt="tiled" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/tiled.png" alt="tiled" />
 
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
-<img src="./docs/qpcr.png" alt="qpcr" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/qpcr.png" alt="qpcr" />
 
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
```

### Comparing `varvamp-0.8.2/README.md` & `varvamp-0.8.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="./docs/varvamp.png" alt="varVAMP logo" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
-<img src="./docs/sanger.png" alt="sanger" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/sanger.png" alt="sanger" />
 
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
-<img src="./docs/tiled.png" alt="tiled" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/tiled.png" alt="tiled" />
 
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
-<img src="./docs/qpcr.png" alt="qpcr" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/qpcr.png" alt="qpcr" />
 
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
```

### Comparing `varvamp-0.8.2/setup.py` & `varvamp-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/command.py` & `varvamp-0.8.3/varvamp/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     """
 
     # find best primers and create primer dict
     all_primers = primers.find_best_primers(left_primer_candidates, right_primer_candidates)
     logging.varvamp_progress(
         log_file,
         progress=0.7,
-        job="Considering only high scoring primers.",
+        job="Considering non-overlapping low scoring primers.",
         progress_text=f"{len(all_primers['+'])} fw and {len(all_primers['-'])} rw primers"
     )
 
     # find all possible amplicons
     amplicons = scheme.find_amplicons(
         all_primers,
         args.opt_length,
```

### Comparing `varvamp-0.8.2/varvamp/scripts/alignment.py` & `varvamp-0.8.3/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/config.py` & `varvamp-0.8.3/varvamp/scripts/config.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/consensus.py` & `varvamp-0.8.3/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/logging.py` & `varvamp-0.8.3/varvamp/scripts/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,50 +155,50 @@
                 exit=True
             )
         if args.overlap > args.opt_length/2:
             raise_error(
                 "your intended overlap is higher than half of your optimal length. This reduces how well varvamps will find overlapping amplicons. Consider decreasing.",
                 log_file
             )
-        # QPCR specific warnings
-        if args.mode == "qpcr":
-            if args.pn_ambig < 0:
-                raise_error(
-                    "number of ambiguous characters in the qPCR probe cannot be 0.",
-                    log_file,
-                    exit=True
-                )
-            if args.pn_ambig > args.n_ambig:
-                raise_error(
-                    "the degeneracy of qPCR probes should not be higher than that of qPCR primers to retain specificity",
-                    log_file,
-                    exit=True
-                )
-            if args.test_n <= 0:
-                raise_error(
-                    "if the number of tested qPCR amplicons is 0 or lower, no amplicons will be reported.",
-                    log_file,
-                    exit=True
-                )
+    # QPCR specific warnings
+    if args.mode == "qpcr":
+        if args.pn_ambig < 0:
+            raise_error(
+                "number of ambiguous characters in the qPCR probe cannot be 0.",
+                log_file,
+                exit=True
+            )
+        if args.pn_ambig > args.n_ambig:
+            raise_error(
+                "the degeneracy of qPCR probes should not be higher than that of qPCR primers to retain specificity",
+                log_file,
+                exit=True
+            )
+        if args.test_n <= 0:
+            raise_error(
+                "if the number of tested qPCR amplicons is 0 or lower, no amplicons will be reported.",
+                log_file,
+                exit=True
+            )
 
-            if args.test_n > 200:
-                raise_error(
-                    "checking the deltaG of amplicons is computationally intensive. setting this higher than 200 will likely take a bit to compute.",
-                    log_file
-                )
-            if args.pn_ambig > 2:
-                raise_error(
-                    "setting the degeneracy of probes higher than 2 can result in variable probe design. Consider reducing!",
-                    log_file
-                )
-            if args.deltaG > 0:
-                raise_error(
-                    "setting the deltaG cutoff larger than 0 is not recommended!",
-                    log_file
-                )
+        if args.test_n > 200:
+            raise_error(
+                "checking the deltaG of amplicons is computationally intensive. setting this higher than 200 will likely take a bit to compute.",
+                log_file
+            )
+        if args.pn_ambig > 2:
+            raise_error(
+                "setting the degeneracy of probes higher than 2 can result in variable probe design. Consider reducing!",
+                log_file
+            )
+        if args.deltaG > 0:
+            raise_error(
+                "setting the deltaG cutoff larger than 0 is not recommended!",
+                log_file
+            )
 
 
 def confirm_config(args, log_file):
     """
     checks the config. raises error and warnings
     if nececarry. writes settings to log
     """
```

### Comparing `varvamp-0.8.2/varvamp/scripts/param_estimation.py` & `varvamp-0.8.3/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/primers.py` & `varvamp-0.8.3/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/qpcr.py` & `varvamp-0.8.3/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/regions.py` & `varvamp-0.8.3/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/reporting.py` & `varvamp-0.8.3/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp/scripts/scheme.py` & `varvamp-0.8.3/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.8.2/varvamp.egg-info/PKG-INFO` & `varvamp-0.8.3/varvamp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.8.2
+Version: 0.8.3
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -17,32 +17,33 @@
 [![License: GPL v3](https://img.shields.io/github/license/jonas-fuchs/varvamp)](https://www.gnu.org/licenses/gpl-3.0)
 [![PiPy](https://img.shields.io/pypi/v/varvamp?label=pypi%20version)](https://pypi.org/project/varvamp/)
 [![PiPy](https://static.pepy.tech/personalized-badge/varvamp?period=total&units=international_system&left_color=grey&right_color=green&left_text=pypi%20downloads)](https://pypi.org/project/varvamp/)
 [![CONDA](https://img.shields.io/conda/v/bioconda/varvamp?label=conda%20version)](https://anaconda.org/bioconda/varvamp)
 [![CONDA](https://img.shields.io/conda/dn/bioconda/varvamp?label=conda%20downloads)](https://anaconda.org/bioconda/varvamp)
 <img src= https://anaconda.org/conda-forge/r-clv/badges/platforms.svg />
 [![DOI](https://zenodo.org/badge/606756158.svg)](https://zenodo.org/badge/latestdoi/606756158)
+[![CodeFactor](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/badge/master)](https://www.codefactor.io/repository/github/jonas-fuchs/varvamp/overview/master)
 
 For a lot of virus genera it is difficult to design pan-specific primers. varVAMP solves this by introducing ambiguous characters into primers and minimizes mismatches at the 3' end. Primers might not work for some sequences of your input alignment but should recognize the large majority.
 
 **varVAMP comes in three different flavors:**
 
-<img src="./docs/varvamp.png" alt="varVAMP logo" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/varvamp.png" alt="varVAMP logo" />
 
 **SANGER**: varVAMP searches for the very best primers and reports back non-overlapping amplicons which can be used for PCR-based screening approaches.
 
-<img src="./docs/sanger.png" alt="sanger" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/sanger.png" alt="sanger" />
 
 **TILED**: varVAMP uses a graph based approach to design overlapping amplicons that tile the entire viral genome. This designs amplicons that are suitable for Oxford Nanopore or Illumina based full-genome sequencing.
 
-<img src="./docs/tiled.png" alt="tiled" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/tiled.png" alt="tiled" />
 
 **QPCR**: varVAMP searches for small amplicons with an optimized internal probe (TaqMan). It minimizes temperature differences between the primers and checks for amplicon secondary structures.
 
-<img src="./docs/qpcr.png" alt="qpcr" />
+<img src="https://github.com/jonas-fuchs/varVAMP/blob/master/docs/qpcr.png" alt="qpcr" />
 
 This program is currently being developed and in an alpha state. You are welcome to use this software. If you successfully design primers, drop me a mail. It might be possible to collaborate! Ideas and suggestions are highly welcome.
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
```

### Comparing `varvamp-0.8.2/varvamp.egg-info/SOURCES.txt` & `varvamp-0.8.3/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

