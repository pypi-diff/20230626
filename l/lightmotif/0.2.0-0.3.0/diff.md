# Comparing `tmp/lightmotif-0.2.0.tar.gz` & `tmp/lightmotif-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightmotif-0.2.0.tar", last modified: Wed May 17 14:53:14 2023, max compression
+gzip compressed data, was "lightmotif-0.3.0.tar", last modified: Sun Jun 25 21:46:49 2023, max compression
```

## Comparing `lightmotif-0.2.0.tar` & `lightmotif-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 14:53:09.000000 lightmotif-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-17 14:53:09.000000 lightmotif-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 14:53:09.000000 lightmotif-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 14:53:13.997680 lightmotif-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-17 14:53:09.000000 lightmotif-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.993680 lightmotif-0.2.0/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/benches/ecoli.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/abc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/dense.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/err.rs
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/num.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/pli/
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/src/pli/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/avx2.rs
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/neon.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/platform/sse2.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pli/scores.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/pwm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/src/seq.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif/tests/dna.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-17 14:53:09.000000 lightmotif-0.2.0/lightmotif-py/lightmotif/tests/unittest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:53:13.997680 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:53:13.000000 lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 14:53:13.000000 lightmotif-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 14:53:13.997680 lightmotif-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-17 14:53:09.000000 lightmotif-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-25 21:46:42.000000 lightmotif-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-25 21:46:42.000000 lightmotif-0.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-25 21:46:42.000000 lightmotif-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-25 21:46:49.945176 lightmotif-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-25 21:46:42.000000 lightmotif-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.941176 lightmotif-0.3.0/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/benches/ecoli.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/abc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/dense.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/err.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/num.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif/src/pli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif/src/pli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/platform/avx2.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/platform/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/platform/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/platform/neon.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/platform/sse2.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pli/scores.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/pwm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/src/seq.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif/tests/dna.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.941176 lightmotif-0.3.0/lightmotif-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.941176 lightmotif-0.3.0/lightmotif-py/lightmotif/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/lightmotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/lightmotif/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.945176 lightmotif-0.3.0/lightmotif-py/lightmotif/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/lightmotif/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/lightmotif/tests/test_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-25 21:46:42.000000 lightmotif-0.3.0/lightmotif-py/lightmotif/tests/unittest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:46:49.941176 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-25 21:46:49.000000 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-25 21:46:49.000000 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:46:49.000000 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 21:46:49.000000 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:46:49.000000 lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 21:46:49.000000 lightmotif-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-25 21:46:49.945176 lightmotif-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-25 21:46:42.000000 lightmotif-0.3.0/setup.py
```

### Comparing `lightmotif-0.2.0/CHANGELOG.md` & `lightmotif-0.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/lightmotif/compare/v0.2.0...HEAD
+[Unreleased]: https://github.com/althonos/lightmotif/compare/v0.3.0...HEAD
+
+
+## [v0.3.0] - 2023-06-25
+[v0.3.0]: https://github.com/althonos/lightmotif/compare/v0.2.0...v0.3.0
+
+### Changed
+- Rewrite the SSE2 maximum search implementation using a generic number of columns.
+- Refactor `lightmotif::pwm` to avoid infinite odds-ratio for columns with zero background frequencies.
+
+### Added
+- `lightmotif-tfmpvalue` crate implementing the TFMPvalue for computing p-values for a `ScoringMatrix`.
+- `DenseMatrix::from_rows` method to create a dense matrix from an iterable of rows.
+- `PartialEq` implementation for matrices in `lightmotif`.
+- Methods to compute the minimum and maximum scores of a `ScoringMatrix`.
 
 
 ## [v0.2.0] - 2023-05-15
 [v0.2.0]: https://github.com/althonos/lightmotif/compare/v0.1.1...v0.2.0
 
 ### Changed
 - Crate structure to avoid cluttering the main `lightmotif` module namespace.
```

### Comparing `lightmotif-0.2.0/COPYING` & `lightmotif-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/PKG-INFO` & `lightmotif-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.2.0
+Version: 0.3.0
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
@@ -114,32 +114,32 @@
 
 # Create a PSSM with 0.1 pseudocounts and uniform background frequencies
 pwm = motif.counts.normalize(0.1)
 pssm = pwm.log_odds()
 
 # Encode the target sequence into a striped matrix
 seq = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG"
-encoded = lightmotif.EncodedSequence(seq)
-striped = encoded.stripe()
+striped = lightmotif.stripe(seq)
 
 # Compute scores using the fastest backend implementation for the host machine
 scores = pssm.calculate(sseq)
 ```
 
 ## ⏱️ Benchmarks
 
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
-Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
+lightmotif (avx2):      8,065,653 ns/iter    (+/- 4,068,613) = 548.8 MiB/s
+Bio.motifs:           337,416,172 ns/iter   (+/- 24,825,573) =  13.1 MiB/s
+MOODS.scan:           179,858,685 ns/iter    (+/- 8,296,251) =  24.6 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.2.0/README.md` & `lightmotif-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -71,44 +71,43 @@
 assert_eq!(v[0], -23.07094);
 
 // The highest scoring position can be searched with a pipeline as well.
 let best = pli.best_position(&scores).unwrap();
 assert_eq!(best, 18);
 
 ```
-
-Not specifying a vector type will cause the `Pipeline` to use the best
-vector type available based on the selected target features. To explicitly
-use the AVX2, SSSE3, or generic implementation, use `Pipeline<Dna, __m256i>`,
-`Pipeline<Dna, __m128i>`, or `Pipeline<Dna, u8>` respectively.
+This example uses the *generic* pipeline, which is not platform accelerated.
+To use the much faster AVX2 code, create an AVX2 pipeline with 
+`Pipeline::avx2` instead: this returns a `Result` which is `Ok` if AVX2 
+is supported on the local platform.
 
 ## ⏱️ Benchmarks
 
 Both benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain.
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 - Score every position of the genome with the motif weight matrix:
   ```console
   running 3 tests
-  test bench_avx2    ... bench:   6,948,169 ns/iter (+/- 16,477) = 668 MB/s
-  test bench_ssse3   ... bench:  29,079,674 ns/iter (+/- 875,880) = 159 MB/s
-  test bench_generic ... bench: 331,656,134 ns/iter (+/- 5,310,490) = 13 MB/s
+  test bench_avx2    ... bench:   5,795,415 ns/iter (+/-    43,021) = 800 MB/s
+  test bench_sse2    ... bench:  30,405,655 ns/iter (+/-   184,109) = 152 MB/s
+  test bench_generic ... bench: 315,272,609 ns/iter (+/- 1,682,900) =  14 MB/s
   ```
 
 - Find the highest-scoring position for a motif in a 10kb sequence
   (compared to the PSSM algorithm implemented in
   [`bio::pattern_matching::pssm`](https://docs.rs/bio/1.1.0/bio/pattern_matching/pssm/index.html)):
   ```console
-  test bench_avx2    ... bench:      49,259 ns/iter (+/- 1,489) = 203 MB/s
-  test bench_bio     ... bench:   1,440,705 ns/iter (+/- 5,291) = 6 MB/s
-  test bench_generic ... bench:     706,361 ns/iter (+/- 1,726) = 14 MB/s
-  test bench_sssee   ... bench:      94,152 ns/iter (+/- 36) = 106 MB/s
+  test bench_avx2    ... bench:      15,725 ns/iter (+/-     21) = 635 MB/s
+  test bench_sse2    ... bench:      67,190 ns/iter (+/-    118) = 148 MB/s
+  test bench_generic ... bench:     711,948 ns/iter (+/-  3,386) =  14 MB/s
+  test bench_bio     ... bench:   1,423,256 ns/iter (+/- 24,119) =   7 MB/s
   ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.2.0/lightmotif/Cargo.toml` & `lightmotif-0.3.0/lightmotif/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lightmotif"
-version = "0.2.0"
+version = "0.3.0"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 edition = "2021"
 license = "MIT"
 description = "A lightweight platform-accelerated library for biological motif scanning using position weight matrices."
 repository = "https://github.com/althonos/lightmotif"
 homepage = "https://github.com/althonos/lightmotif"
 readme = "README.md"
```

### Comparing `lightmotif-0.2.0/lightmotif/README.md` & `lightmotif-0.3.0/lightmotif/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -71,44 +71,43 @@
 assert_eq!(v[0], -23.07094);
 
 // The highest scoring position can be searched with a pipeline as well.
 let best = pli.best_position(&scores).unwrap();
 assert_eq!(best, 18);
 
 ```
-
-Not specifying a vector type will cause the `Pipeline` to use the best
-vector type available based on the selected target features. To explicitly
-use the AVX2, SSSE3, or generic implementation, use `Pipeline<Dna, __m256i>`,
-`Pipeline<Dna, __m128i>`, or `Pipeline<Dna, u8>` respectively.
+This example uses the *generic* pipeline, which is not platform accelerated.
+To use the much faster AVX2 code, create an AVX2 pipeline with 
+`Pipeline::avx2` instead: this returns a `Result` which is `Ok` if AVX2 
+is supported on the local platform.
 
 ## ⏱️ Benchmarks
 
 Both benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain.
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 - Score every position of the genome with the motif weight matrix:
   ```console
   running 3 tests
-  test bench_avx2    ... bench:   6,948,169 ns/iter (+/- 16,477) = 668 MB/s
-  test bench_ssse3   ... bench:  29,079,674 ns/iter (+/- 875,880) = 159 MB/s
-  test bench_generic ... bench: 331,656,134 ns/iter (+/- 5,310,490) = 13 MB/s
+  test bench_avx2    ... bench:   5,795,415 ns/iter (+/-    43,021) = 800 MB/s
+  test bench_sse2    ... bench:  30,405,655 ns/iter (+/-   184,109) = 152 MB/s
+  test bench_generic ... bench: 315,272,609 ns/iter (+/- 1,682,900) =  14 MB/s
   ```
 
 - Find the highest-scoring position for a motif in a 10kb sequence
   (compared to the PSSM algorithm implemented in
   [`bio::pattern_matching::pssm`](https://docs.rs/bio/1.1.0/bio/pattern_matching/pssm/index.html)):
   ```console
-  test bench_avx2    ... bench:      49,259 ns/iter (+/- 1,489) = 203 MB/s
-  test bench_bio     ... bench:   1,440,705 ns/iter (+/- 5,291) = 6 MB/s
-  test bench_generic ... bench:     706,361 ns/iter (+/- 1,726) = 14 MB/s
-  test bench_sssee   ... bench:      94,152 ns/iter (+/- 36) = 106 MB/s
+  test bench_avx2    ... bench:      15,725 ns/iter (+/-     21) = 635 MB/s
+  test bench_sse2    ... bench:      67,190 ns/iter (+/-    118) = 148 MB/s
+  test bench_generic ... bench:     711,948 ns/iter (+/-  3,386) =  14 MB/s
+  test bench_bio     ... bench:   1,423,256 ns/iter (+/- 24,119) =   7 MB/s
   ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.2.0/lightmotif/benches/ecoli.rs` & `lightmotif-0.3.0/lightmotif/benches/ecoli.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/src/abc.rs` & `lightmotif-0.3.0/lightmotif/src/abc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     fn complement(&self) -> Self;
 }
 
 // --- Alphabet ----------------------------------------------------------------
 
 /// A biological alphabet with associated metadata.
 pub trait Alphabet: Debug + Copy + Default + 'static {
-    type Symbol: Symbol;
-    type K: Unsigned + NonZero + ArrayLength<f32>;
+    type Symbol: Symbol + Debug;
+    type K: Unsigned + NonZero + ArrayLength<f32> + Debug;
 
     /// Get the default symbol for this alphabet.
     fn default_symbol() -> Self::Symbol {
         Default::default()
     }
 
     /// Get all the symbols of this alphabet.
@@ -62,15 +62,15 @@
         s.complement()
     }
 }
 
 // --- DNA ---------------------------------------------------------------------
 
 /// The standard DNA alphabet composed of 4 deoxyribonucleotides and a wildcard.
-#[derive(Default, Debug, Clone, Copy)]
+#[derive(Default, Debug, Clone, Copy, PartialEq, Eq)]
 pub struct Dna;
 
 impl Alphabet for Dna {
     type Symbol = Nucleotide;
     type K = U5;
 
     fn symbols() -> &'static [Nucleotide] {
@@ -153,15 +153,15 @@
         }
     }
 }
 
 // --- Protein -----------------------------------------------------------------
 
 /// The standard protein alphabet composed of 20 residues and a wildcard.
-#[derive(Default, Debug, Clone, Copy)]
+#[derive(Default, Debug, Clone, Copy, PartialEq, Eq)]
 pub struct Protein;
 
 impl Alphabet for Protein {
     type Symbol = AminoAcid;
     type K = U21;
 
     fn symbols() -> &'static [AminoAcid] {
@@ -283,15 +283,15 @@
         }
     }
 }
 
 // --- Background --------------------------------------------------------------
 
 /// The background frequencies for an alphabet.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq)]
 pub struct Background<A: Alphabet> {
     frequencies: GenericArray<f32, A::K>,
     alphabet: std::marker::PhantomData<A>,
 }
 
 impl<A: Alphabet> Background<A> {
     /// Create a new background with the given frequencies.
@@ -373,15 +373,15 @@
         Self::uniform()
     }
 }
 
 // --- Pseudocounts ------------------------------------------------------------
 
 /// A structure for storing the pseudocounts over an alphabet.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq)]
 pub struct Pseudocounts<A: Alphabet> {
     counts: GenericArray<f32, A::K>,
     alphabet: std::marker::PhantomData<A>,
 }
 
 impl<A: Alphabet> Pseudocounts<A> {
     pub fn counts(&self) -> &[f32] {
```

### Comparing `lightmotif-0.2.0/lightmotif/src/dense.rs` & `lightmotif-0.3.0/lightmotif/src/dense.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 use std::ptr::NonNull;
 
 use typenum::marker_traits::Unsigned;
 
 // --- DenseMatrix -------------------------------------------------------------
 
 /// An aligned dense matrix of with a constant number of columns.
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, PartialEq, Eq)]
 pub struct DenseMatrix<T: Default + Copy, C: Unsigned> {
     data: Vec<T>,
     indices: Vec<usize>,
     _columns: std::marker::PhantomData<C>,
 }
 
 impl<T: Default + Copy, C: Unsigned> DenseMatrix<T, C> {
@@ -35,15 +35,15 @@
     /// Create a new *uninitialized* matrix with the given number of rows.
     pub unsafe fn uninitialized(rows: usize) -> Self {
         // alway over-allocate columns to avoid alignment issues.
         let c = C::USIZE.next_power_of_two();
 
         // NOTE: this is unsafe but given that we require `T` to be
         //       copy, this should be fine, as `Copy` prevents the
-        //       type to be `Dorp` as well.
+        //       type to be `Drop` as well.
         // reserve the vector without initializing the data
         let mut data = Vec::with_capacity((rows + 1) * c);
         data.set_len((rows + 1) * c);
 
         // compute offset to aligned memory
         let mut offset = 0;
         while data[offset..].as_ptr() as usize % c > 0 {
@@ -56,14 +56,36 @@
         Self {
             data,
             indices,
             _columns: std::marker::PhantomData,
         }
     }
 
+    /// Create a new dense matrix from an iterable of rows.
+    ///
+    /// # Panics
+    ///
+    /// Panics if any of the rows does not have the number of elements
+    /// corresponding to the dense matrix columns.
+    pub fn from_rows<I>(rows: I) -> Self
+    where
+        I: IntoIterator,
+        <I as IntoIterator>::Item: AsRef<[T]>,
+        <I as IntoIterator>::IntoIter: ExactSizeIterator,
+    {
+        let it = rows.into_iter();
+        let mut dense = Self::new(it.len());
+
+        for (i, row) in it.enumerate() {
+            dense[i].copy_from_slice(row.as_ref());
+        }
+
+        dense
+    }
+
     /// The number of columns of the matrix.
     #[inline]
     pub const fn columns(&self) -> usize {
         C::USIZE
     }
 
     /// The number of rows of the matrix.
```

### Comparing `lightmotif-0.2.0/lightmotif/src/err.rs` & `lightmotif-0.3.0/lightmotif/src/err.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/src/pli/mod.rs` & `lightmotif-0.3.0/lightmotif/src/pli/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,22 @@
         S: AsRef<StripedSequence<A, C>>,
         M: AsRef<ScoringMatrix<A>>,
     {
         Sse2::score_into(seq, pssm, scores)
     }
 }
 
-impl<A: Alphabet> BestPosition<<Sse2 as Backend>::LANES> for Pipeline<A, Sse2> {
-    fn best_position(&self, scores: &StripedScores<<Sse2 as Backend>::LANES>) -> Option<usize> {
+impl<A, C> BestPosition<C> for Pipeline<A, Sse2>
+where
+    A: Alphabet,
+    C: StrictlyPositive + Rem<U16> + Div<U16>,
+    <C as Rem<U16>>::Output: Zero,
+    <C as Div<U16>>::Output: Unsigned,
+{
+    fn best_position(&self, scores: &StripedScores<C>) -> Option<usize> {
         Sse2::best_position(scores)
     }
 }
 
 // --- AVX2 pipeline -----------------------------------------------------------
 
 impl<A: Alphabet> Pipeline<A, Avx2> {
```

### Comparing `lightmotif-0.2.0/lightmotif/src/pli/platform/avx2.rs` & `lightmotif-0.3.0/lightmotif/src/pli/platform/avx2.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/src/pli/platform/neon.rs` & `lightmotif-0.3.0/lightmotif/src/pli/platform/neon.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/src/pli/platform/sse2.rs` & `lightmotif-0.3.0/lightmotif/src/pli/platform/sse2.rs`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     <C as Rem<U16>>::Output: Zero,
     <C as Div<U16>>::Output: Unsigned,
 {
     // mask vectors for broadcasting uint8x16_t to uint32x4_t to floatx4_t
     let zero = _mm_setzero_si128();
     // process columns of the striped matrix, any multiple of 16 is supported
     let data = scores.matrix_mut();
-    for offset in (0..<C as Div<U16>>::Output::USIZE).map(|i| i * <Sse2 as Backend>::LANES::USIZE) {
+    for offset in (0..<C as Div<U16>>::Output::USIZE).map(|i| i * U16::USIZE) {
         // process every position of the sequence data
         for i in 0..seq.data.rows() - seq.wrap {
             // reset sums for current position
             let mut s1 = _mm_setzero_ps();
             let mut s2 = _mm_setzero_ps();
             let mut s3 = _mm_setzero_ps();
             let mut s4 = _mm_setzero_ps();
@@ -84,73 +84,94 @@
             _mm_storeu_ps(row[offset + 12..].as_mut_ptr(), s4);
         }
     }
 }
 
 #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
 #[target_feature(enable = "sse2")]
-unsafe fn best_position_sse2(scores: &StripedScores<<Sse2 as Backend>::LANES>) -> Option<usize> {
+unsafe fn best_position_sse2<C>(scores: &StripedScores<C>) -> Option<usize>
+where
+    C: StrictlyPositive + Rem<U16> + Div<U16>,
+    <C as Rem<U16>>::Output: Zero,
+    <C as Div<U16>>::Output: Unsigned,
+{
     if scores.len() == 0 {
         None
     } else {
         let data = scores.matrix();
         unsafe {
-            // the row index for the best score in each column
-            // (these are 32-bit integers but for use with `_mm256_blendv_ps`
-            // they get stored in 32-bit float vectors).
-            let mut p1 = _mm_setzero_ps();
-            let mut p2 = _mm_setzero_ps();
-            let mut p3 = _mm_setzero_ps();
-            let mut p4 = _mm_setzero_ps();
-            // store the best scores for each column
-            let mut s1 = _mm_load_ps(data[0][0x00..].as_ptr());
-            let mut s2 = _mm_load_ps(data[0][0x04..].as_ptr());
-            let mut s3 = _mm_load_ps(data[0][0x08..].as_ptr());
-            let mut s4 = _mm_load_ps(data[0][0x0c..].as_ptr());
-            // process all rows iteratively
-            for (i, row) in data.iter().enumerate() {
-                // record the current row index
-                let index = _mm_castsi128_ps(_mm_set1_epi32(i as i32));
-                // load scores for the current row
-                let r1 = _mm_load_ps(row[0x00..].as_ptr());
-                let r2 = _mm_load_ps(row[0x04..].as_ptr());
-                let r3 = _mm_load_ps(row[0x08..].as_ptr());
-                let r4 = _mm_load_ps(row[0x0c..].as_ptr());
-                // compare scores to local maxima
-                let c1 = _mm_cmplt_ps(s1, r1);
-                let c2 = _mm_cmplt_ps(s2, r2);
-                let c3 = _mm_cmplt_ps(s3, r3);
-                let c4 = _mm_cmplt_ps(s4, r4);
-                // NOTE: code below could use `_mm_blendv_ps` instead,
-                //       but this instruction is only available on SSE4.1
-                //       while the rest of the code is actually using SSE2
-                //       instructions only.
-                // replace indices of new local maxima
-                p1 = _mm_or_ps(_mm_andnot_ps(c1, p1), _mm_and_ps(index, c1));
-                p2 = _mm_or_ps(_mm_andnot_ps(c2, p2), _mm_and_ps(index, c2));
-                p3 = _mm_or_ps(_mm_andnot_ps(c3, p3), _mm_and_ps(index, c3));
-                p4 = _mm_or_ps(_mm_andnot_ps(c4, p4), _mm_and_ps(index, c4));
-                // replace values of new local maxima
-                s1 = _mm_or_ps(_mm_andnot_ps(c1, s1), _mm_and_ps(r1, c1));
-                s2 = _mm_or_ps(_mm_andnot_ps(c2, s2), _mm_and_ps(r2, c2));
-                s3 = _mm_or_ps(_mm_andnot_ps(c3, s3), _mm_and_ps(r3, c3));
-                s4 = _mm_or_ps(_mm_andnot_ps(c4, s4), _mm_and_ps(r4, c4));
-            }
-            // find the global maximum across all columns
-            let mut x: [u32; 16] = [0; 16];
-            _mm_storeu_si128(x[0x00..].as_mut_ptr() as *mut _, _mm_castps_si128(p1));
-            _mm_storeu_si128(x[0x04..].as_mut_ptr() as *mut _, _mm_castps_si128(p2));
-            _mm_storeu_si128(x[0x08..].as_mut_ptr() as *mut _, _mm_castps_si128(p3));
-            _mm_storeu_si128(x[0x0c..].as_mut_ptr() as *mut _, _mm_castps_si128(p4));
+            let mut best_col = [0u32; 16];
             let mut best_pos = 0;
             let mut best_score = -f32::INFINITY;
-            for (col, &row) in x.iter().enumerate() {
-                if data[row as usize][col] > best_score {
-                    best_score = data[row as usize][col];
-                    best_pos = col * data.rows() + row as usize;
+            for offset in (0..<C as Div<U16>>::Output::USIZE).map(|i| i * U16::USIZE) {
+                // the row index for the best score in each column
+                // (these are 32-bit integers but for use with `_mm256_blendv_ps`
+                // they get stored in 32-bit float vectors).
+                let mut p1 = _mm_setzero_ps();
+                let mut p2 = _mm_setzero_ps();
+                let mut p3 = _mm_setzero_ps();
+                let mut p4 = _mm_setzero_ps();
+                // store the best scores for each column
+                let mut s1 = _mm_load_ps(data[0][offset + 0x00..].as_ptr());
+                let mut s2 = _mm_load_ps(data[0][offset + 0x04..].as_ptr());
+                let mut s3 = _mm_load_ps(data[0][offset + 0x08..].as_ptr());
+                let mut s4 = _mm_load_ps(data[0][offset + 0x0c..].as_ptr());
+                // process all rows iteratively
+                for (i, row) in data.iter().enumerate() {
+                    // record the current row index
+                    let index = _mm_castsi128_ps(_mm_set1_epi32(i as i32));
+                    // load scores for the current row
+                    let r1 = _mm_load_ps(row[offset + 0x00..].as_ptr());
+                    let r2 = _mm_load_ps(row[offset + 0x04..].as_ptr());
+                    let r3 = _mm_load_ps(row[offset + 0x08..].as_ptr());
+                    let r4 = _mm_load_ps(row[offset + 0x0c..].as_ptr());
+                    // compare scores to local maxima
+                    let c1 = _mm_cmplt_ps(s1, r1);
+                    let c2 = _mm_cmplt_ps(s2, r2);
+                    let c3 = _mm_cmplt_ps(s3, r3);
+                    let c4 = _mm_cmplt_ps(s4, r4);
+                    // NOTE: code below could use `_mm_blendv_ps` instead,
+                    //       but this instruction is only available on SSE4.1
+                    //       while the rest of the code is actually using SSE2
+                    //       instructions only.
+                    // replace indices of new local maxima
+                    p1 = _mm_or_ps(_mm_andnot_ps(c1, p1), _mm_and_ps(index, c1));
+                    p2 = _mm_or_ps(_mm_andnot_ps(c2, p2), _mm_and_ps(index, c2));
+                    p3 = _mm_or_ps(_mm_andnot_ps(c3, p3), _mm_and_ps(index, c3));
+                    p4 = _mm_or_ps(_mm_andnot_ps(c4, p4), _mm_and_ps(index, c4));
+                    // replace values of new local maxima
+                    s1 = _mm_or_ps(_mm_andnot_ps(c1, s1), _mm_and_ps(r1, c1));
+                    s2 = _mm_or_ps(_mm_andnot_ps(c2, s2), _mm_and_ps(r2, c2));
+                    s3 = _mm_or_ps(_mm_andnot_ps(c3, s3), _mm_and_ps(r3, c3));
+                    s4 = _mm_or_ps(_mm_andnot_ps(c4, s4), _mm_and_ps(r4, c4));
+                }
+                // find the global maximum across all columns
+                _mm_storeu_si128(
+                    best_col[0x00..].as_mut_ptr() as *mut _,
+                    _mm_castps_si128(p1),
+                );
+                _mm_storeu_si128(
+                    best_col[0x04..].as_mut_ptr() as *mut _,
+                    _mm_castps_si128(p2),
+                );
+                _mm_storeu_si128(
+                    best_col[0x08..].as_mut_ptr() as *mut _,
+                    _mm_castps_si128(p3),
+                );
+                _mm_storeu_si128(
+                    best_col[0x0c..].as_mut_ptr() as *mut _,
+                    _mm_castps_si128(p4),
+                );
+                for k in 0..U16::USIZE {
+                    let row = best_col[k] as usize;
+                    let col = k + offset;
+                    if data[row][col] > best_score {
+                        best_score = data[row][col];
+                        best_pos = col * data.rows() + row as usize;
+                    }
                 }
             }
             Some(best_pos)
         }
     }
 }
 
@@ -181,15 +202,20 @@
             score_sse2(seq, pssm, scores);
         }
         #[cfg(not(any(target_arch = "x86", target_arch = "x86_64")))]
         panic!("attempting to run SSE2 code on a non-x86 host")
     }
 
     #[allow(unused)]
-    pub fn best_position(scores: &StripedScores<<Sse2 as Backend>::LANES>) -> Option<usize> {
+    pub fn best_position<C>(scores: &StripedScores<C>) -> Option<usize>
+    where
+        C: StrictlyPositive + Rem<U16> + Div<U16>,
+        <C as Rem<U16>>::Output: Zero,
+        <C as Div<U16>>::Output: Unsigned,
+    {
         #[cfg(any(target_arch = "x86", target_arch = "x86_64"))]
         unsafe {
             best_position_sse2(scores)
         }
         #[cfg(not(any(target_arch = "x86", target_arch = "x86_64")))]
         panic!("attempting to run SSE2 code on a non-x86 host")
     }
```

### Comparing `lightmotif-0.2.0/lightmotif/src/pli/scores.rs` & `lightmotif-0.3.0/lightmotif/src/pli/scores.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/src/pwm.rs` & `lightmotif-0.3.0/lightmotif/src/pwm.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,48 @@
 //! Storage types for the different stages of a PSSM construction.
 
+use std::ops::Index;
+
 use typenum::marker_traits::Unsigned;
 
 use super::abc::Alphabet;
 use super::abc::Background;
 use super::abc::ComplementableAlphabet;
 use super::abc::Pseudocounts;
 use super::abc::Symbol;
 use super::dense::DenseMatrix;
 use super::err::InvalidData;
 use super::seq::EncodedSequence;
 
+macro_rules! matrix_traits {
+    ($mx:ident, $t:ty) => {
+        impl<A: Alphabet> AsRef<$mx<A>> for $mx<A> {
+            fn as_ref(&self) -> &Self {
+                self
+            }
+        }
+        impl<A: Alphabet> AsRef<DenseMatrix<$t, A::K>> for $mx<A> {
+            fn as_ref(&self) -> &DenseMatrix<$t, A::K> {
+                &self.data
+            }
+        }
+        impl<A: Alphabet> Index<usize> for $mx<A> {
+            type Output = <DenseMatrix<$t, A::K> as Index<usize>>::Output;
+            #[inline]
+            fn index(&self, index: usize) -> &Self::Output {
+                self.data.index(index)
+            }
+        }
+    };
+}
+
 // --- CountMatrix -------------------------------------------------------------
 
 /// A matrix storing symbol occurences at each position.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq, Eq)]
 pub struct CountMatrix<A: Alphabet> {
     /// The alphabet of the count matrix.
     alphabet: std::marker::PhantomData<A>,
     /// The actual counts for each position of the motif.
     data: DenseMatrix<u32, A::K>,
     /// The number of sequences from which this count matrix was obtained.
     #[allow(unused)]
@@ -117,33 +141,29 @@
                 data[i][s.as_index()] = row[A::complement(s).as_index()];
             }
         }
         Self::new_unchecked(data, self.n)
     }
 }
 
-impl<A: Alphabet> AsRef<DenseMatrix<u32, A::K>> for CountMatrix<A> {
-    fn as_ref(&self) -> &DenseMatrix<u32, A::K> {
-        &self.data
-    }
-}
-
 impl<A: Alphabet> FromIterator<EncodedSequence<A>> for Result<CountMatrix<A>, InvalidData> {
     fn from_iter<I>(iter: I) -> Self
     where
         I: IntoIterator<Item = EncodedSequence<A>>,
     {
         CountMatrix::from_sequences(iter)
     }
 }
 
+matrix_traits!(CountMatrix, u32);
+
 // --- FrequencyMatrix ---------------------------------------------------------
 
 /// A matrix storing symbol frequencies at each position.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq)]
 pub struct FrequencyMatrix<A: Alphabet> {
     alphabet: std::marker::PhantomData<A>,
     data: DenseMatrix<f32, A::K>,
 }
 
 impl<A: Alphabet> FrequencyMatrix<A> {
     /// Create a new frequency matrix without checking the contents.
@@ -151,67 +171,80 @@
         Self {
             alphabet: std::marker::PhantomData,
             data,
         }
     }
 
     /// Convert to a weight matrix using the given background frequencies.
+    ///
+    /// # Note
+    /// By convention, columns with null background frequencies receive an
+    /// odds-ratio of zero, which will then translate into a log-odds-ratio
+    /// of `-f32::INFINITY` in the resulting scoring matrix.
     pub fn to_weight<B>(&self, background: B) -> WeightMatrix<A>
     where
         B: Into<Option<Background<A>>>,
     {
         let bg = background.into().unwrap_or_default();
         let mut weight = DenseMatrix::new(self.data.rows());
         for (src, dst) in self.data.iter().zip(weight.iter_mut()) {
             for (j, (&x, &f)) in src.iter().zip(bg.frequencies()).enumerate() {
-                dst[j] = x / f;
+                if f <= 0.0 {
+                    dst[j] = 0.0;
+                } else {
+                    dst[j] = x / f;
+                }
             }
         }
         WeightMatrix::new_unchecked(bg, weight)
     }
 
     /// Convert to a scoring matrix using the given background frequencies.
+    ///
+    /// # Note
+    /// By convention, columns with null background frequencies receive a
+    /// log-odds-ratio of `-f32::INFINITY`.
     pub fn to_scoring<B>(&self, background: B) -> ScoringMatrix<A>
     where
         B: Into<Option<Background<A>>>,
     {
         let bg = background.into().unwrap_or_default();
         let mut scores = DenseMatrix::new(self.data.rows());
         for (src, dst) in self.data.iter().zip(scores.iter_mut()) {
             for (j, (&x, &f)) in src.iter().zip(bg.frequencies()).enumerate() {
-                dst[j] = (x / f).log2();
+                if f <= 0.0 {
+                    dst[j] = -f32::INFINITY;
+                } else {
+                    dst[j] = (x / f).log2();
+                }
             }
         }
-        ScoringMatrix::new_unchecked(bg, scores)
-    }
-}
-
-impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for FrequencyMatrix<A> {
-    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
-        &self.data
+        ScoringMatrix::new(bg, scores)
     }
 }
 
 impl<A: ComplementableAlphabet> FrequencyMatrix<A> {
-    /// Get the reverse-complement of this count matrix.
+    /// Get the reverse-complement of this frequency matrix.
     pub fn reverse_complement(&self) -> Self {
         let mut data = DenseMatrix::new(self.data.rows());
         for (i, row) in self.data.iter().rev().enumerate() {
             for &s in A::symbols() {
                 data[i][s.as_index()] = row[A::complement(s).as_index()];
             }
         }
         Self::new_unchecked(data)
     }
 }
 
+matrix_traits!(FrequencyMatrix, f32);
+
 // --- WeightMatrix ------------------------------------------------------------
 
 /// A matrix storing odds ratio of symbol occurences at each position.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq)]
 pub struct WeightMatrix<A: Alphabet> {
     background: Background<A>,
     data: DenseMatrix<f32, A::K>,
 }
 
 impl<A: Alphabet> WeightMatrix<A> {
     /// Create a new weight matrix without checking the contents.
@@ -266,81 +299,71 @@
         let background = self.background.clone();
         let mut data = self.data.clone();
         for row in data.iter_mut() {
             for item in row.iter_mut() {
                 *item = item.log2();
             }
         }
-        ScoringMatrix::new_unchecked(background, data)
+        ScoringMatrix::new(background, data)
     }
 }
 
 impl<A: ComplementableAlphabet> WeightMatrix<A> {
-    /// Get the reverse-complement of this count matrix.
+    /// Get the reverse-complement of this weight matrix.
     pub fn reverse_complement(&self) -> Self {
         let mut data = DenseMatrix::new(self.data.rows());
         for (i, row) in self.data.iter().rev().enumerate() {
             for &s in A::symbols() {
                 data[i][s.as_index()] = row[A::complement(s).as_index()];
             }
         }
         Self::new_unchecked(self.background.clone(), data)
     }
 }
 
-impl<A: Alphabet> AsRef<WeightMatrix<A>> for WeightMatrix<A> {
-    fn as_ref(&self) -> &Self {
-        self
-    }
-}
-
-impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for WeightMatrix<A> {
-    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
-        &self.data
-    }
-}
-
 impl<A: Alphabet> From<ScoringMatrix<A>> for WeightMatrix<A> {
     fn from(pwm: ScoringMatrix<A>) -> Self {
         let background = pwm.background;
         let mut data = pwm.data;
         for row in data.iter_mut() {
             for item in row.iter_mut() {
                 *item = 2f32.powf(*item);
             }
         }
         WeightMatrix { background, data }
     }
 }
 
+matrix_traits!(WeightMatrix, f32);
+
 // --- ScoringMatrix -----------------------------------------------------------
 
 /// A matrix storing odds ratio of symbol occurences at each position.
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, PartialEq)]
 pub struct ScoringMatrix<A: Alphabet> {
     background: Background<A>,
     data: DenseMatrix<f32, A::K>,
 }
 
 impl<A: ComplementableAlphabet> ScoringMatrix<A> {
-    /// Get the reverse-complement of this count matrix.
+    /// Get the reverse-complement of this scoring matrix.
     pub fn reverse_complement(&self) -> Self {
         let mut data = DenseMatrix::new(self.data.rows());
         for (i, row) in self.data.iter().rev().enumerate() {
             for &s in A::symbols() {
                 data[i][s.as_index()] = row[A::complement(s).as_index()];
             }
         }
-        Self::new_unchecked(self.background.clone(), data)
+        Self::new(self.background.clone(), data)
     }
 }
 
 impl<A: Alphabet> ScoringMatrix<A> {
-    /// Create a new scoring matrix without checking the contents.
-    fn new_unchecked(background: Background<A>, data: DenseMatrix<f32, A::K>) -> Self {
+    /// Create a new scoring matrix from the given log-odds matrix.
+    pub fn new(background: Background<A>, data: DenseMatrix<f32, A::K>) -> Self {
         Self { background, data }
     }
 
     /// The length of the motif encoded in this scoring matrix.
     #[inline]
     pub fn len(&self) -> usize {
         self.data.rows()
@@ -353,33 +376,32 @@
     }
 
     /// The background frequencies of the position weight matrix.
     #[inline]
     pub fn background(&self) -> &Background<A> {
         &self.background
     }
-}
 
-impl<A: Alphabet> AsRef<ScoringMatrix<A>> for ScoringMatrix<A> {
-    fn as_ref(&self) -> &Self {
-        self
+    /// The lowest score that can be obtained with this scoring matrix.
+    pub fn min_score(&self) -> f32 {
+        self.data
+            .iter()
+            .map(|row| row.iter().min_by(|a, b| a.partial_cmp(b).unwrap()).unwrap())
+            .sum()
     }
-}
 
-impl<A: Alphabet> AsRef<DenseMatrix<f32, A::K>> for ScoringMatrix<A> {
-    fn as_ref(&self) -> &DenseMatrix<f32, A::K> {
-        &self.data
+    /// The highest score that can be obtained with this scoring matrix.
+    pub fn max_score(&self) -> f32 {
+        self.data
+            .iter()
+            .map(|row| row.iter().max_by(|a, b| a.partial_cmp(b).unwrap()).unwrap())
+            .sum()
     }
 }
 
 impl<A: Alphabet> From<WeightMatrix<A>> for ScoringMatrix<A> {
     fn from(pwm: WeightMatrix<A>) -> Self {
-        let background = pwm.background;
-        let mut data = pwm.data;
-        for row in data.iter_mut() {
-            for item in row.iter_mut() {
-                *item = item.log2();
-            }
-        }
-        ScoringMatrix { background, data }
+        pwm.to_scoring()
     }
 }
+
+matrix_traits!(ScoringMatrix, f32);
```

### Comparing `lightmotif-0.2.0/lightmotif/src/seq.rs` & `lightmotif-0.3.0/lightmotif/src/seq.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif/tests/dna.rs` & `lightmotif-0.3.0/lightmotif/tests/dna.rs`

 * *Files 9% similar despite different names*

```diff
@@ -108,14 +108,21 @@
 #[cfg(target_feature = "sse2")]
 #[test]
 fn test_score_sse2_32() {
     let pli = Pipeline::sse2().unwrap();
     test_score::<U32, _>(&pli);
 }
 
+#[cfg(target_feature = "sse2")]
+#[test]
+fn test_best_position_sse2_32() {
+    let pli = Pipeline::sse2().unwrap();
+    test_best_position::<U32, _>(&pli);
+}
+
 #[cfg(target_feature = "avx2")]
 #[test]
 fn test_score_avx2() {
     let pli = Pipeline::avx2().unwrap();
     test_score(&pli);
 }
```

### Comparing `lightmotif-0.2.0/lightmotif-py/Cargo.toml` & `lightmotif-0.3.0/lightmotif-py/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lightmotif-py"
-version = "0.2.0"
+version = "0.3.0"
 authors = ["Martin Larralde <martin.larralde@embl.de>"]
 edition = "2021"
 license = "MIT"
 description = "PyO3 bindings and Python interface to the lightmotif crate."
 repository = "https://github.com/althonos/lightmotif"
 homepage = "https://github.com/althonos/lightmotif"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 path = "lightmotif/lib.rs"
 
 [dependencies.lightmotif]
 path = "../lightmotif"
-version = "0.2.0"
+version = "0.3.0"
 [dependencies]
 pyo3 = "0.18.3"
 generic-array = "0.14"
 
 [features]
 default = []
 built = []
```

### Comparing `lightmotif-0.2.0/lightmotif-py/README.md` & `lightmotif-0.3.0/lightmotif-py/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,32 @@
 
 # Create a PSSM with 0.1 pseudocounts and uniform background frequencies
 pwm = motif.counts.normalize(0.1)
 pssm = pwm.log_odds()
 
 # Encode the target sequence into a striped matrix
 seq = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG"
-encoded = lightmotif.EncodedSequence(seq)
-striped = encoded.stripe()
+striped = lightmotif.stripe(seq)
 
 # Compute scores using the fastest backend implementation for the host machine
 scores = pssm.calculate(sseq)
 ```
 
 ## ⏱️ Benchmarks
 
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
-Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
+lightmotif (avx2):      8,065,653 ns/iter    (+/- 4,068,613) = 548.8 MiB/s
+Bio.motifs:           337,416,172 ns/iter   (+/- 24,825,573) =  13.1 MiB/s
+MOODS.scan:           179,858,685 ns/iter    (+/- 8,296,251) =  24.6 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.2.0/lightmotif-py/lightmotif/lib.rs` & `lightmotif-0.3.0/lightmotif-py/lightmotif/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 #![doc = include_str!("../README.md")]
 
 extern crate generic_array;
 extern crate lightmotif;
 extern crate pyo3;
 
+use lightmotif::abc::Alphabet;
 use lightmotif::abc::Symbol;
+use lightmotif::dense::DenseMatrix;
 use lightmotif::num::Unsigned;
 use lightmotif::pli::platform::Backend;
 use lightmotif::pli::Pipeline;
 use lightmotif::pli::Score;
 
 use pyo3::exceptions::PyBufferError;
 use pyo3::exceptions::PyIndexError;
+use pyo3::exceptions::PyKeyError;
 use pyo3::exceptions::PyTypeError;
 use pyo3::exceptions::PyValueError;
 use pyo3::ffi::Py_ssize_t;
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
+use pyo3::types::PyList;
 use pyo3::types::PyString;
 use pyo3::AsPyPointer;
 
 use generic_array::GenericArray;
 
 // --- Compile-time constants --------------------------------------------------
 
@@ -110,14 +114,57 @@
 #[derive(Clone, Debug)]
 pub struct CountMatrix {
     data: lightmotif::CountMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl CountMatrix {
+    /// Create a new count matrix.
+    #[new]
+    pub fn __init__(_alphabet: &PyString, values: &PyDict) -> PyResult<PyClassInitializer<Self>> {
+        let mut data: Option<DenseMatrix<u32, <lightmotif::Dna as Alphabet>::K>> = None;
+        for s in lightmotif::Dna::symbols() {
+            let key = String::from(s.as_char());
+            let column = values
+                .get_item(&key)
+                .ok_or(PyKeyError::new_err(key))?
+                .downcast::<PyList>()?;
+
+            if data.is_none() {
+                data = Some(DenseMatrix::new(column.len()));
+            }
+
+            let matrix = data.as_mut().unwrap();
+            if matrix.rows() != column.len() {
+                return Err(PyValueError::new_err("Invalid number of rows"));
+            }
+
+            for (i, x) in column.iter().enumerate() {
+                matrix[i][s.as_index()] = x.extract::<u32>()?;
+            }
+        }
+
+        match data {
+            None => Err(PyValueError::new_err("Invalid count matrix")),
+            Some(matrix) => match lightmotif::CountMatrix::new(matrix) {
+                Ok(counts) => Ok(Self::from(counts).into()),
+                Err(_) => Err(PyValueError::new_err("Inconsistent rows in count matrix")),
+            },
+        }
+    }
+
+    pub fn __eq__(&self, object: &PyAny) -> PyResult<bool> {
+        let py = object.py();
+        if let Ok(other) = object.extract::<Py<Self>>() {
+            Ok(self.data == other.borrow(py).data)
+        } else {
+            Ok(false)
+        }
+    }
+
     pub fn normalize(&self, pseudocount: Option<PyObject>) -> PyResult<WeightMatrix> {
         let pseudo = Python::with_gil(|py| {
             if let Some(obj) = pseudocount {
                 if let Ok(x) = obj.extract::<f32>(py) {
                     Ok(lightmotif::abc::Pseudocounts::from(x))
                 } else if let Ok(d) = obj.extract::<&PyDict>(py) {
                     let p = dict_to_alphabet_array::<lightmotif::Dna>(d)?;
@@ -146,14 +193,23 @@
 #[derive(Clone, Debug)]
 pub struct WeightMatrix {
     data: lightmotif::pwm::WeightMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl WeightMatrix {
+    pub fn __eq__(&self, object: &PyAny) -> PyResult<bool> {
+        let py = object.py();
+        if let Ok(other) = object.extract::<Py<Self>>() {
+            Ok(self.data == other.borrow(py).data)
+        } else {
+            Ok(false)
+        }
+    }
+
     pub fn log_odds(&self, background: Option<PyObject>) -> PyResult<ScoringMatrix> {
         // extract the background from the method argument
         let bg = Python::with_gil(|py| {
             if let Some(obj) = background {
                 if let Ok(d) = obj.extract::<&PyDict>(py) {
                     let p = dict_to_alphabet_array::<lightmotif::Dna>(d)?;
                     lightmotif::abc::Background::new(p)
@@ -186,14 +242,23 @@
 #[derive(Clone, Debug)]
 pub struct ScoringMatrix {
     data: lightmotif::ScoringMatrix<lightmotif::Dna>,
 }
 
 #[pymethods]
 impl ScoringMatrix {
+    pub fn __eq__(&self, object: &PyAny) -> PyResult<bool> {
+        let py = object.py();
+        if let Ok(other) = object.extract::<Py<Self>>() {
+            Ok(self.data == other.borrow(py).data)
+        } else {
+            Ok(false)
+        }
+    }
+
     /// Return the PSSM score for all positions of the given sequence.
     pub fn calculate(
         slf: PyRef<'_, Self>,
         sequence: &mut StripedSequence,
     ) -> PyResult<StripedScores> {
         let pssm = &slf.data;
         let seq = &mut sequence.data;
```

### Comparing `lightmotif-0.2.0/lightmotif-py/lightmotif/tests/test_dna.py` & `lightmotif-0.3.0/lightmotif-py/lightmotif/tests/test_dna.py`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif-py/lightmotif/tests/unittest.rs` & `lightmotif-0.3.0/lightmotif-py/lightmotif/tests/unittest.rs`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/PKG-INFO` & `lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightmotif
-Version: 0.2.0
+Version: 0.3.0
 Summary: PyO3 bindings and Python interface to lightmotif, a library for platform-accelerated biological motif scanning using position weight matrices.
 Home-page: https://github.com/althonos/lightmotif
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/lightmotif/issues
 Project-URL: Changelog, https://github.com/althonos/lightmotif/blob/master/CHANGELOG.md
@@ -114,32 +114,32 @@
 
 # Create a PSSM with 0.1 pseudocounts and uniform background frequencies
 pwm = motif.counts.normalize(0.1)
 pssm = pwm.log_odds()
 
 # Encode the target sequence into a striped matrix
 seq = "ATGTCCCAACAACGATACCCCGAGCCCATCGCCGTCATCGGCTCGGCATGCAGATTCCCAGGCG"
-encoded = lightmotif.EncodedSequence(seq)
-striped = encoded.stripe()
+striped = lightmotif.stripe(seq)
 
 # Compute scores using the fastest backend implementation for the host machine
 scores = pssm.calculate(sseq)
 ```
 
 ## ⏱️ Benchmarks
 
 Benchmarks use the [MX000001](https://www.prodoric.de/matrix/MX000001.html)
 motif from [PRODORIC](https://www.prodoric.de/)[\[4\]](#ref4), and the
 [complete genome](https://www.ncbi.nlm.nih.gov/nuccore/U00096) of an
 *Escherichia coli K12* strain. 
 *Benchmarks were run on a [i7-10710U CPU](https://ark.intel.com/content/www/us/en/ark/products/196448/intel-core-i7-10710u-processor-12m-cache-up-to-4-70-ghz.html) running @1.10GHz, compiled with `--target-cpu=native`*.
 
 ```console
-lightmotif (avx2):      9,125,495 ns/iter    (+/- 6,392,241) = 485.1 MiB/s
-Bio.motifs:           284,696,651 ns/iter    (+/- 6,454,945) =  15.5 MiB/s
+lightmotif (avx2):      8,065,653 ns/iter    (+/- 4,068,613) = 548.8 MiB/s
+Bio.motifs:           337,416,172 ns/iter   (+/- 24,825,573) =  13.1 MiB/s
+MOODS.scan:           179,858,685 ns/iter    (+/- 8,296,251) =  24.6 MiB/s
 ```
 
 
 ## 💭 Feedback
 
 ### ⚠️ Issue Tracker
```

### Comparing `lightmotif-0.2.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt` & `lightmotif-0.3.0/lightmotif-py/lightmotif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/setup.cfg` & `lightmotif-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lightmotif-0.2.0/setup.py` & `lightmotif-0.3.0/setup.py`

 * *Files identical despite different names*

