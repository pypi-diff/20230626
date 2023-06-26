# Comparing `tmp/msstitch-3.8.tar.gz` & `tmp/msstitch-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/msstitch-3.8.tar", last modified: Thu Oct 28 07:39:33 2021, max compression
+gzip compressed data, was "/Users/jorrit.boekel/repos/msstitch/dist/tmpf92iygm7/msstitch-3.9.tar", last modified: Mon Feb 14 13:50:27 2022, max compression
```

## Comparing `msstitch-3.8.tar` & `msstitch-3.9.tar`

### file list

```diff
@@ -1,149 +1,155 @@
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:33.095644 msstitch-3.8/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8958 2021-10-28 06:46:04.000000 msstitch-3.8/CHANGELOG.md
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1080 2021-02-17 09:27:37.000000 msstitch-3.8/LICENSE
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      373 2021-02-17 09:27:37.000000 msstitch-3.8/MANIFEST.in
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12495 2021-10-28 07:39:33.095923 msstitch-3.8/PKG-INFO
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    11495 2021-10-28 06:46:04.000000 msstitch-3.8/README.md
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       79 2021-10-28 07:39:33.097005 msstitch-3.8/setup.cfg
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2077 2021-10-28 06:46:04.000000 msstitch-3.8/setup.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.875951 msstitch-3.8/src/
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.885962 msstitch-3.8/src/app/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/__init__.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.896966 msstitch-3.8/src/app/actions/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/__init__.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.900897 msstitch-3.8/src/app/actions/lookups/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/lookups/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6798 2021-02-17 09:57:30.000000 msstitch-3.8/src/app/actions/lookups/quant.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2110 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/lookups/sequence.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1586 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/lookups/spectra.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7528 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/actions/merge.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.906939 msstitch-3.8/src/app/actions/percolator/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/percolator/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3139 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/percolator/filters.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1511 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/percolator/split.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8584 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/proteins.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.916522 msstitch-3.8/src/app/actions/psmtable/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/psmtable/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      567 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/psmtable/filtering.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10378 2021-10-28 06:46:04.000000 msstitch-3.8/src/app/actions/psmtable/isosummarize.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4619 2021-10-19 19:17:53.000000 msstitch-3.8/src/app/actions/psmtable/percolator.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    24596 2021-02-17 09:59:33.000000 msstitch-3.8/src/app/actions/psmtable/refine.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1269 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/psmtable/splitmerge.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5815 2021-02-17 09:29:55.000000 msstitch-3.8/src/app/actions/psmtopeptable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4418 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/actions/sequence.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.920870 msstitch-3.8/src/app/dataformats/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/dataformats/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1246 2021-02-17 09:57:30.000000 msstitch-3.8/src/app/dataformats/mzidtsv.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      564 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/dataformats/peptable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      885 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/dataformats/prottable.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.932748 msstitch-3.8/src/app/drivers/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/drivers/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8090 2021-02-17 09:29:55.000000 msstitch-3.8/src/app/drivers/base.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6330 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/drivers/lookups.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4723 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/drivers/merge.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    29530 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/drivers/options.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6118 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/drivers/peptable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5274 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/drivers/percolator.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5584 2021-02-17 09:29:55.000000 msstitch-3.8/src/app/drivers/prottable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13034 2021-02-17 09:57:30.000000 msstitch-3.8/src/app/drivers/psmtable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2355 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/drivers/sequence.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2456 2021-10-28 06:46:04.000000 msstitch-3.8/src/app/drivers/startup.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.934370 msstitch-3.8/src/app/lookups/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      877 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/base.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.947267 msstitch-3.8/src/app/lookups/sqlite/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/sqlite/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    25771 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/lookups/sqlite/base.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/sqlite/biosets.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    11752 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/lookups/sqlite/peptable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7846 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/lookups/sqlite/protpeptable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12799 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/sqlite/prottable.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    17172 2021-10-19 19:33:03.000000 msstitch-3.8/src/app/lookups/sqlite/psms.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3504 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/lookups/sqlite/quant.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3283 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/sqlite/searchspace.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2080 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/lookups/sqlite/spectra.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1081 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/msstitch.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.955618 msstitch-3.8/src/app/readers/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4853 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/fasta.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3022 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/mzidplus.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1996 2021-02-17 09:57:30.000000 msstitch-3.8/src/app/readers/openms.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1965 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/percolator.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2259 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/spectra.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4124 2021-10-13 09:34:00.000000 msstitch-3.8/src/app/readers/tsv.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2213 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/xml.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      606 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/readers/xmlformatting.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.957707 msstitch-3.8/src/app/writers/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/writers/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1431 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/writers/percolator.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1715 2021-02-17 09:27:37.000000 msstitch-3.8/src/app/writers/tsv.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.961333 msstitch-3.8/src/msstitch.egg-info/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12495 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/PKG-INFO
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4300 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/SOURCES.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        1 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/dependency_links.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       48 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/entry_points.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       21 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/requires.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        4 2021-10-28 07:39:32.000000 msstitch-3.8/src/msstitch.egg-info/top_level.txt
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:32.961839 msstitch-3.8/tests/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/tests/__init__.py
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:33.013103 msstitch-3.8/tests/base_fixtures/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   390495 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/ens99_small.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)  2893030 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/few_spec_timstof.mzML
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)  2632017 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/few_spectra.mzML
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2048 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/known_peptide_lookup.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      312 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/proteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2048 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/rev_known_peptide_lookup.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      137 2021-02-17 09:27:37.000000 msstitch-3.8/tests/base_fixtures/twoproteins.fasta
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:33.083443 msstitch-3.8/tests/fixtures/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     9081 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_peptides.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      138 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_tryprev_minlen_twoproteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      346 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_tryprev_pretryp_twoproteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      153 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_tryprev_targetcheck_twoproteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      153 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_tryprev_twoproteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      193 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoy_twoproteins.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    20480 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/decoycheck.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   200704 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/dinoquant_lookup.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1783 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/ensg.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1329 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/ensg_nopsms.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    46705 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spec_timstof.mzid
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2457 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spec_timstof.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2842 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spec_timstof.tsv_fdr.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    64452 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spectra.consXML
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     9370 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spectra.kr
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   128155 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spectra.mzid
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7428 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spectra.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7528 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/few_spectra.tsv_fdr.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1671 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/genenames.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      895 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/isosum_charge_column.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    28560 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/perco.xml
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2918 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/perco.xml_h0.xml
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6297 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/perco.xml_h1.xml
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10548 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/perco_timstof.xml
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2779 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2204 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins_intensities.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2755 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins_isonorm_log.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2763 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins_isonorm_nolog.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2437 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins_quantonly.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3027 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/proteins_sweep.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   400306 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/protrev_ens99_small.fasta
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   286720 2021-10-13 09:34:00.000000 msstitch-3.8/tests/fixtures/quant_lookup.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6140 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/set1_target_pg.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    98304 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/spectra_lookup.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    69632 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/spectra_lookup_timstof.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5393 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/target.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7592 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/target_pep_quant_norm.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7723 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/target_peptides.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7971 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/target_peptides_sweep.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7955 2021-10-13 09:34:00.000000 msstitch-3.8/tests/fixtures/target_peptides_totalprotnorm.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6682 2021-10-13 09:34:00.000000 msstitch-3.8/tests/fixtures/target_peptides_totalprotnorm_nolog.txt
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12003 2021-10-13 09:34:00.000000 msstitch-3.8/tests/fixtures/target_pg.tsv
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   897024 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/target_psms.sqlite
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      280 2021-02-17 09:27:37.000000 msstitch-3.8/tests/fixtures/trypsinized_twoproteins.fasta
-drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-10-28 07:39:33.094065 msstitch-3.8/tests/integration/
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2021-02-17 09:27:37.000000 msstitch-3.8/tests/integration/__init__.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    17512 2021-02-17 09:55:57.000000 msstitch-3.8/tests/integration/basetests.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    15249 2021-10-13 09:34:00.000000 msstitch-3.8/tests/integration/merge_tests.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    18939 2021-10-13 09:34:00.000000 msstitch-3.8/tests/integration/mslookup_tests.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10958 2021-02-17 09:55:28.000000 msstitch-3.8/tests/integration/peptable_tests.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4063 2021-02-17 09:27:37.000000 msstitch-3.8/tests/integration/percolator_tests.py
--rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    28971 2021-10-19 19:32:43.000000 msstitch-3.8/tests/integration/psmtable_tests.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.462567 msstitch-3.9/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     9405 2022-02-14 13:40:54.000000 msstitch-3.9/CHANGELOG.md
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1080 2018-12-07 10:48:35.000000 msstitch-3.9/LICENSE
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      373 2020-06-04 08:26:15.000000 msstitch-3.9/MANIFEST.in
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13336 2022-02-14 13:50:27.462740 msstitch-3.9/PKG-INFO
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12336 2022-02-14 13:42:16.000000 msstitch-3.9/README.md
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       79 2022-02-14 13:50:27.463346 msstitch-3.9/setup.cfg
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2087 2022-02-14 11:03:08.000000 msstitch-3.9/setup.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.184235 msstitch-3.9/src/
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.189370 msstitch-3.9/src/app/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/__init__.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.194982 msstitch-3.9/src/app/actions/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/actions/__init__.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.198841 msstitch-3.9/src/app/actions/lookups/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/lookups/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6798 2021-02-18 13:47:04.000000 msstitch-3.9/src/app/actions/lookups/quant.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2110 2020-08-27 19:28:04.000000 msstitch-3.9/src/app/actions/lookups/sequence.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1586 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/lookups/spectra.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7586 2022-01-12 10:58:24.000000 msstitch-3.9/src/app/actions/merge.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.202005 msstitch-3.9/src/app/actions/percolator/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/percolator/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3139 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/percolator/filters.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1511 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/percolator/split.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8584 2020-06-03 12:47:42.000000 msstitch-3.9/src/app/actions/proteins.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.211204 msstitch-3.9/src/app/actions/psmtable/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/psmtable/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      567 2020-08-27 09:36:04.000000 msstitch-3.9/src/app/actions/psmtable/filtering.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10922 2022-02-14 09:24:38.000000 msstitch-3.9/src/app/actions/psmtable/isosummarize.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13683 2022-01-04 10:02:18.000000 msstitch-3.9/src/app/actions/psmtable/luciphor.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4065 2022-01-12 09:30:23.000000 msstitch-3.9/src/app/actions/psmtable/percolator.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    24596 2021-02-17 09:19:48.000000 msstitch-3.9/src/app/actions/psmtable/refine.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1269 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/psmtable/splitmerge.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5815 2020-11-30 10:24:16.000000 msstitch-3.9/src/app/actions/psmtopeptable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4418 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/actions/sequence.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.216122 msstitch-3.9/src/app/dataformats/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/dataformats/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      570 2021-07-16 12:39:24.000000 msstitch-3.9/src/app/dataformats/defaultmods.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2013 2022-01-04 10:32:06.000000 msstitch-3.9/src/app/dataformats/mzidtsv.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      583 2022-01-04 12:20:44.000000 msstitch-3.9/src/app/dataformats/peptable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      885 2021-02-25 17:47:51.000000 msstitch-3.9/src/app/dataformats/prottable.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.232079 msstitch-3.9/src/app/drivers/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/drivers/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8090 2020-11-30 10:24:06.000000 msstitch-3.9/src/app/drivers/base.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6330 2021-02-18 13:47:24.000000 msstitch-3.9/src/app/drivers/lookups.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4557 2022-01-04 15:18:27.000000 msstitch-3.9/src/app/drivers/merge.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    33432 2022-02-10 09:49:25.000000 msstitch-3.9/src/app/drivers/options.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     6383 2022-02-10 08:55:46.000000 msstitch-3.9/src/app/drivers/peptable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5274 2020-05-14 09:56:56.000000 msstitch-3.9/src/app/drivers/percolator.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5849 2022-02-10 13:26:20.000000 msstitch-3.9/src/app/drivers/prottable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    17019 2022-02-10 13:35:07.000000 msstitch-3.9/src/app/drivers/psmtable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2355 2020-05-28 09:23:19.000000 msstitch-3.9/src/app/drivers/sequence.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2456 2022-02-14 12:34:15.000000 msstitch-3.9/src/app/drivers/startup.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.233312 msstitch-3.9/src/app/lookups/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/lookups/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      877 2020-09-06 19:52:01.000000 msstitch-3.9/src/app/lookups/base.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.245322 msstitch-3.9/src/app/lookups/sqlite/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/lookups/sqlite/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    26921 2021-11-04 12:14:09.000000 msstitch-3.9/src/app/lookups/sqlite/base.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2020-05-12 13:19:36.000000 msstitch-3.9/src/app/lookups/sqlite/biosets.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12396 2022-01-12 11:08:47.000000 msstitch-3.9/src/app/lookups/sqlite/peptable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     7698 2022-01-04 16:05:44.000000 msstitch-3.9/src/app/lookups/sqlite/protpeptable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13097 2022-01-04 16:05:42.000000 msstitch-3.9/src/app/lookups/sqlite/prottable.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    19549 2022-01-04 09:57:39.000000 msstitch-3.9/src/app/lookups/sqlite/psms.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3504 2021-02-19 16:47:02.000000 msstitch-3.9/src/app/lookups/sqlite/quant.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3283 2020-05-12 13:19:36.000000 msstitch-3.9/src/app/lookups/sqlite/searchspace.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2080 2020-09-04 19:23:14.000000 msstitch-3.9/src/app/lookups/sqlite/spectra.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1081 2020-08-26 19:53:06.000000 msstitch-3.9/src/app/msstitch.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.254721 msstitch-3.9/src/app/readers/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/readers/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4853 2020-06-02 13:14:23.000000 msstitch-3.9/src/app/readers/fasta.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     3022 2020-05-12 13:19:36.000000 msstitch-3.9/src/app/readers/mzidplus.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1996 2021-02-11 08:12:14.000000 msstitch-3.9/src/app/readers/openms.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1965 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/readers/percolator.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2259 2021-02-26 13:52:21.000000 msstitch-3.9/src/app/readers/spectra.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4124 2021-02-26 13:52:41.000000 msstitch-3.9/src/app/readers/tsv.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2213 2020-05-12 13:19:36.000000 msstitch-3.9/src/app/readers/xml.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      606 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/readers/xmlformatting.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.256727 msstitch-3.9/src/app/writers/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/src/app/writers/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1431 2020-05-12 12:37:55.000000 msstitch-3.9/src/app/writers/percolator.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1715 2020-05-27 09:22:29.000000 msstitch-3.9/src/app/writers/tsv.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.259994 msstitch-3.9/src/msstitch.egg-info/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13336 2022-02-14 13:50:26.000000 msstitch-3.9/src/msstitch.egg-info/PKG-INFO
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4532 2022-02-14 13:50:27.000000 msstitch-3.9/src/msstitch.egg-info/SOURCES.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        1 2022-02-14 13:50:26.000000 msstitch-3.9/src/msstitch.egg-info/dependency_links.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       47 2022-02-14 13:50:26.000000 msstitch-3.9/src/msstitch.egg-info/entry_points.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)       28 2022-02-14 13:50:27.000000 msstitch-3.9/src/msstitch.egg-info/requires.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        4 2022-02-14 13:50:27.000000 msstitch-3.9/src/msstitch.egg-info/top_level.txt
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.260326 msstitch-3.9/tests/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:35.000000 msstitch-3.9/tests/__init__.py
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.339532 msstitch-3.9/tests/base_fixtures/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   390495 2020-05-06 13:16:46.000000 msstitch-3.9/tests/base_fixtures/ens99_small.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)  2893030 2020-05-06 13:16:46.000000 msstitch-3.9/tests/base_fixtures/few_spec_timstof.mzML
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795) 10476818 2022-01-05 12:03:26.000000 msstitch-3.9/tests/base_fixtures/few_spectra.mzML
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2048 2020-05-06 19:07:08.000000 msstitch-3.9/tests/base_fixtures/known_peptide_lookup.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      312 2020-05-06 13:25:27.000000 msstitch-3.9/tests/base_fixtures/proteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2048 2020-05-06 19:07:54.000000 msstitch-3.9/tests/base_fixtures/rev_known_peptide_lookup.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      137 2020-05-06 13:16:46.000000 msstitch-3.9/tests/base_fixtures/twoproteins.fasta
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.451774 msstitch-3.9/tests/fixtures/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    45128 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/decoy_peptides.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      138 2022-01-12 11:37:25.000000 msstitch-3.9/tests/fixtures/decoy_tryprev_minlen_twoproteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      346 2022-01-12 11:37:25.000000 msstitch-3.9/tests/fixtures/decoy_tryprev_pretryp_twoproteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      153 2022-01-12 11:37:25.000000 msstitch-3.9/tests/fixtures/decoy_tryprev_targetcheck_twoproteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      153 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/decoy_tryprev_twoproteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      193 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/decoy_twoproteins.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    20480 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/decoycheck.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   630784 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/dinoquant_lookup.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5997 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/ensg.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     5169 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/ensg_nopsms.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    46705 2022-01-12 11:37:54.000000 msstitch-3.9/tests/fixtures/few_spec_timstof.mzid
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2457 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/few_spec_timstof.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     2940 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/few_spec_timstof.tsv_fdr.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   274177 2022-01-12 11:38:39.000000 msstitch-3.9/tests/fixtures/few_spectra.consXML
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    43528 2022-01-12 09:52:29.000000 msstitch-3.9/tests/fixtures/few_spectra.kr
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   612193 2022-01-12 11:38:39.000000 msstitch-3.9/tests/fixtures/few_spectra.mzid
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    40041 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/few_spectra.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    44595 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/few_spectra.tsv_fdr.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     8641 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/genenames.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     1113 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/isosum_charge_column.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   157858 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/perco.xml
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    20422 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/perco.xml_h0.xml
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    49052 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/perco.xml_h1.xml
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10548 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/perco_timstof.xml
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12991 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12988 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_avg.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10180 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_intensities.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13622 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_isonorm_log.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13721 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_isonorm_nolog.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12724 2022-02-14 13:37:23.000000 msstitch-3.9/tests/fixtures/proteins_nonorm_log.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    10734 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_quantonly.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    13726 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/proteins_sweep.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   400306 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/protrev_ens99_small.fasta
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   937984 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/quant_lookup.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    47002 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/set1_target_pg.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)   245760 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/spectra_lookup.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    77824 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/spectra_lookup_timstof.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    42091 2022-01-12 09:52:31.000000 msstitch-3.9/tests/fixtures/target.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    55924 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_pep_quant_norm.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    55883 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_peptides.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    55881 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_peptides_avg.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    57155 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_peptides_sweep.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    56840 2022-02-14 13:37:23.000000 msstitch-3.9/tests/fixtures/target_peptides_totalp_sepnorm.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    56393 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_peptides_totalprotnorm.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    50851 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_peptides_totalprotnorm_nolog.txt
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    92867 2022-01-12 09:52:30.000000 msstitch-3.9/tests/fixtures/target_pg.tsv
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)  1781760 2022-01-12 09:52:31.000000 msstitch-3.9/tests/fixtures/target_psms.sqlite
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)      280 2022-01-12 09:52:31.000000 msstitch-3.9/tests/fixtures/trypsinized_twoproteins.fasta
+drwxr-xr-x   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2022-02-14 13:50:27.461302 msstitch-3.9/tests/integration/
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)        0 2018-12-07 10:48:36.000000 msstitch-3.9/tests/integration/__init__.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    17044 2022-01-11 20:49:16.000000 msstitch-3.9/tests/integration/basetests.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    15306 2022-01-04 16:14:29.000000 msstitch-3.9/tests/integration/merge_tests.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    19288 2022-01-12 11:31:19.000000 msstitch-3.9/tests/integration/mslookup_tests.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    12009 2022-02-14 13:37:23.000000 msstitch-3.9/tests/integration/peptable_tests.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)     4063 2020-05-12 13:19:36.000000 msstitch-3.9/tests/integration/percolator_tests.py
+-rw-r--r--   0 jorrit.boekel (1073262253) SCILIFELAB\Domain Users (754850795)    28975 2022-01-12 11:18:42.000000 msstitch-3.9/tests/integration/psmtable_tests.py
```

### Comparing `msstitch-3.8/CHANGELOG.md` & `msstitch-3.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 # Changelog
 
+## [3.9] - 2022-02-14
+### Added
+- Add PEP (posterior error) from percolator to output
+- Possible to do median-centering on a peptide/protein/gene table using median factors from another table (e.g. PTM peptides centered with a protein table)
+
+### Changed
+- No longer recalculate percolator FDR to avoid mix-max, let user choose in percolator instead
+
+### Fixed
+- Genecentric peptide table merging bug with many identical gene output fixed
+
+
 ## [3.8] - 2021-10-28
-## Changed
+### Changed
 - Field order in peptide/protein tables: channels of all sets, then # of PSMs used to quantify
 
-## Fixed
+### Fixed
 - Deletesets bug where unused peptide sequences where not removed from DB due to a missing commit
 - Fix percolator to TSV ID creation which affected non-scannumbered data (e.g. TIMS data) where multiple PSMs to spectrum occur and it keeps enumerating scans
 
 
 ## [3.7] - 2021-03-13
-## Fixed
+### Fixed
 - Peptide table merge bug that piled on duplicate proteins and exploded in processing time at big datasets
 
 
 ## [3.6] - 2021-03-05
-## Added
+### Added
 - Total protein normalization of PTM peptides
 - PTM FLR stored and output in peptide table merges
 - Precursor ion fraction (purity) from OpenMS to PSM table
 - Precursor purity filter sets PSM quant to NA, keeps PSMs
 
-## Fixed
+### Fixed
 - Do not create duplicate isobaric channels in DB and with that in PSM output
 - Do not add standard fields to PSM refined header that are already there
 - Do not crash on peptide table merge when a peptide has e.g. 600 protein matches
 - Merging no-group peptide tables no longer output multiple identical protein accessions for a peptide
 - Peptide table genecentric merge gets all genes per peptide, not only one
 
 
 ## [3.5] - 2020-09-23
-## Changed
+### Changed
 - Isobaric quant summarizing to features now throws out all PSMs with NA in a channel by default, keep them with --keep-psms-na-quant
 
 
 ## [3.4] - 2020-09-17
 ### Added
 - Isobaric quant summarizing using denominators OR sweep OR median intensity
 - Median normalization possible for isobaric quant
```

### Comparing `msstitch-3.8/LICENSE` & `msstitch-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/PKG-INFO` & `msstitch-3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msstitch
-Version: 3.8
+Version: 3.9
 Summary: MS proteomics post processing utilities
 Home-page: https://github.com/lehtiolab/msstitch
 Author: Jorrit Boekel
 Author-email: jorrit.boekel@scilifelab.se
 Maintainer: Jorrit Boekel
 Maintainer-email: jorrit.boekel@scilifelab.se
 License: MIT
@@ -81,17 +81,25 @@
 
 Or without removing peptide sequences that match to the target DB:
 
 ```
 msstitch makedecoy uniprot.fasta -o decoy.fasta --scramble tryp_rev --ignore-target-hits
 ```
 
+Specify modifications and create a mod-file for MSGF+:
+
+```
+msstitch mods --dbfile db.sqlite --modnames Phospho Oxidation Carbamidomethylation TMT6plex \
+  --msgffile mods.txt
+```
 
 After running two samples of MSGF and percolator, we can start making 
-a more proper set of PSM tables:
+a more proper set of PSM tables by adding percolator data and filtering
+on FDR. The following adds percolator svm-score, q-value (FDR), and posterior
+error as columns to the PSM table:
 
 ```
 # Add percolator data, filter 0.01 FDR
 msstitch perco2psm -i psms1.txt \
   --perco percolator1.xml --mzid psms1.mzIdentML \
   --filtpsm 0.01 --filtpep 0.01
 msstitch perco2psm -i psms2.txt \
@@ -170,15 +178,26 @@
 
 ```
 msstitch peptides -i set1_ptm_psms.txt -o set1_ptm_peptides.txt \
   --scorecolpattern svm --isobquantcolpattern tmt10plex --denompatterns _126 _127C \
   --logisoquant --totalproteome set1_proteins.txt
 ```
 
-Create a protein table, with isobaric quantification as for peptides, the
+For proper median centering of this table (as it would otherwise be impacted by
+sample differences per channel), you may want to median-center. In the case of 
+small and possibly noisy PTM tables, it can be advisable to use another table
+from a global search (or e.g. the full peptide or protein table from the PTM search)
+for determining channel medians. This is possible by specifying the above command
+plus:
+
+```
+  --median-normalize --normalization-factors-table /path/to/set1_global_proteins.txt
+```
+
+To create a protein table, with isobaric quantification as for peptides, the
 average of the top-3 highest intensity peptides for MS1 quantification:
 For all of these, summarizing isobaric PSM data to peptide, protein, gene features 
 is done using medians of log2 PSM quantification values per feature (e.g. a protein). If you'd
 rather use averages, use `--summarize-average` as below, where we also show log2
 transformation of intensities before summarizing and subsequent median-centering:
 
 ```
```

### Comparing `msstitch-3.8/README.md` & `msstitch-3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,17 +55,25 @@
 
 Or without removing peptide sequences that match to the target DB:
 
 ```
 msstitch makedecoy uniprot.fasta -o decoy.fasta --scramble tryp_rev --ignore-target-hits
 ```
 
+Specify modifications and create a mod-file for MSGF+:
+
+```
+msstitch mods --dbfile db.sqlite --modnames Phospho Oxidation Carbamidomethylation TMT6plex \
+  --msgffile mods.txt
+```
 
 After running two samples of MSGF and percolator, we can start making 
-a more proper set of PSM tables:
+a more proper set of PSM tables by adding percolator data and filtering
+on FDR. The following adds percolator svm-score, q-value (FDR), and posterior
+error as columns to the PSM table:
 
 ```
 # Add percolator data, filter 0.01 FDR
 msstitch perco2psm -i psms1.txt \
   --perco percolator1.xml --mzid psms1.mzIdentML \
   --filtpsm 0.01 --filtpep 0.01
 msstitch perco2psm -i psms2.txt \
@@ -144,15 +152,26 @@
 
 ```
 msstitch peptides -i set1_ptm_psms.txt -o set1_ptm_peptides.txt \
   --scorecolpattern svm --isobquantcolpattern tmt10plex --denompatterns _126 _127C \
   --logisoquant --totalproteome set1_proteins.txt
 ```
 
-Create a protein table, with isobaric quantification as for peptides, the
+For proper median centering of this table (as it would otherwise be impacted by
+sample differences per channel), you may want to median-center. In the case of 
+small and possibly noisy PTM tables, it can be advisable to use another table
+from a global search (or e.g. the full peptide or protein table from the PTM search)
+for determining channel medians. This is possible by specifying the above command
+plus:
+
+```
+  --median-normalize --normalization-factors-table /path/to/set1_global_proteins.txt
+```
+
+To create a protein table, with isobaric quantification as for peptides, the
 average of the top-3 highest intensity peptides for MS1 quantification:
 For all of these, summarizing isobaric PSM data to peptide, protein, gene features 
 is done using medians of log2 PSM quantification values per feature (e.g. a protein). If you'd
 rather use averages, use `--summarize-average` as below, where we also show log2
 transformation of intensities before summarizing and subsequent median-centering:
 
 ```
```

### Comparing `msstitch-3.8/setup.py` & `msstitch-3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: Implementation :: CPython',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
-INSTALL_REQUIRES = ['numpy', 'lxml', 'biopython']
+INSTALL_REQUIRES = ['numpy', 'lxml', 'biopython', 'jinja2']
 METADATA = {
-    'version': '3.8',
+    'version': '3.9',
     'title': 'msstitch',
     'description': 'MS proteomics post processing utilities',
     'uri': 'https://github.com/lehtiolab/msstitch',
     'author': 'Jorrit Boekel',
     'email': 'jorrit.boekel@scilifelab.se',
     'license': 'MIT',
     'copyright': 'Copyright (c) 2013 Jorrit Boekel',
```

### Comparing `msstitch-3.8/src/app/actions/lookups/quant.py` & `msstitch-3.9/src/app/actions/lookups/quant.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/lookups/sequence.py` & `msstitch-3.9/src/app/actions/lookups/sequence.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/lookups/spectra.py` & `msstitch-3.9/src/app/actions/lookups/spectra.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/merge.py` & `msstitch-3.9/src/app/actions/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 from app.readers import tsv as tsvreader
 from app.dataformats import prottable as prottabledata
 
 
 def create_lookup(fns, pqdb, poolnames, featcolnr, ms1_qcolpattern,
-        isobqcolpattern, fdrcolpattern, flrcolpattern):
+        isobqcolpattern, fdrcolpattern, pepcolpattern, flrcolpattern):
     psmnrpattern = prottabledata.HEADER_NO_PSMS_SUFFIX
     fullpsmpattern = prottabledata.HEADER_NO_FULLQ_PSMS
-    patterns = [ms1_qcolpattern, fdrcolpattern, fullpsmpattern, flrcolpattern]
-    storefuns = [pqdb.store_precursor_quants, pqdb.store_fdr, pqdb.store_fullq_psms,
-            pqdb.store_ptm_flr]
+    patterns = [ms1_qcolpattern, fdrcolpattern, pepcolpattern, fullpsmpattern,
+            flrcolpattern]
+    storefuns = [pqdb.store_precursor_quants, pqdb.store_fdr, pqdb.store_pep,
+            pqdb.store_fullq_psms, pqdb.store_ptm_flr]
     tablefn_map = create_tablefn_map(fns, pqdb, poolnames)
     feat_map = pqdb.get_feature_map()
     for pattern, storefun in zip(patterns, storefuns):
         if pattern is None:
             continue
         colmap = get_colmap(fns, pattern, single_col=True)
         if colmap:
```

### Comparing `msstitch-3.8/src/app/actions/percolator/filters.py` & `msstitch-3.9/src/app/actions/percolator/filters.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/percolator/split.py` & `msstitch-3.9/src/app/actions/percolator/split.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/proteins.py` & `msstitch-3.9/src/app/actions/proteins.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/psmtable/filtering.py` & `msstitch-3.9/src/app/actions/psmtable/filtering.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/psmtable/isosummarize.py` & `msstitch-3.9/src/app/actions/psmtable/isosummarize.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,35 +10,45 @@
 
 
 ISOQUANTRATIO_FEAT_ACC = '##isoquant_target_acc##'
 
 
 def get_isobaric_ratios(psmfn, psmheader, channels, denom_channels, sweep,
         report_intensity, summarize_by, min_int, targetfeats, target_acc_field, accessioncol,
-        totalprot_feats, totalp_field, totalp_pepfield, logintensities, normalize, keep_na_psms):
+        totalprot_feats, totalp_field, totalp_pepfield, logintensities, mediannormalize,
+        medianfactors, keep_na_psms):
     """Main function to calculate ratios for PSMs, peptides, proteins, genes.
     Can do simple ratios, median-of-ratios, median-centering, log2, etc
     """
     outratios = get_psmratios(psmfn, psmheader, channels, denom_channels,
             sweep, report_intensity, summarize_by, min_int, accessioncol, logintensities,
             keep_na_psms)
     # at this point, outratios look like:
     # [{ch1: 123, ch2: 456, ISOQUANTRATIO_FEAT_ACC: ENSG1244}, ]
     if accessioncol:
-        if normalize:
-            outratios = mediancenter_ratios(outratios, channels, logintensities, psmfn)
-        if targetfeats and totalprot_feats:
+        if mediannormalize:
+            # median center ratios before proceeding to output
+            # with or without factor report (do not need it if using another
+            # table since that is implied to have been analysed elsewhere anyway)
+            if medianfactors:
+                report_factors = False
+            else:
+                report_factors = os.path.basename(psmfn)
+            outratios = mediancenter_ratios(outratios, channels, logintensities, medianfactors, report_factors)
+        if totalprot_feats:
+            # immediately output
             return totalproteome_normalization(outratios, targetfeats, 
                     target_acc_field, channels, totalprot_feats, totalp_field,
                     totalp_pepfield, logintensities)
-        elif targetfeats:
+        if targetfeats:
+            # Output to the target feat table (e.g. existing peptable, protein table etc)
             outratios = {x.pop(ISOQUANTRATIO_FEAT_ACC): x for x in outratios}
             return output_to_targetfeats(targetfeats, target_acc_field, outratios, channels)
         else:
-            # generate new table with accessions
+            # generate new table with accessions if no existing ID table is specified
             return ({(k if not k == ISOQUANTRATIO_FEAT_ACC else accessioncol): v
                      for k, v in ratio.items()} for ratio in outratios)
     else: 
         return paste_to_psmtable(psmfn, psmheader, outratios)
 
 
 def totalproteome_normalization(outratios, targetfeats, acc_field, channels, totalprot,
@@ -60,34 +70,39 @@
             yield outfeat
         else:
             totalp_acc = feat[totalp_field_target]
             norm_q = {k: v for k,v in quants.items()}
             if ';' in totalp_acc or totalp_acc not in totalprot:
                 norm_q.update({ch: 'NA' for ch in channels})
             elif logratios:
-                norm_q.update({ch: str(norm_q[ch] - float(totalprot[totalp_acc][ch]))
+                norm_q.update({ch: norm_q[ch] - float(totalprot[totalp_acc][ch])
                     if quants[ch] != 'NA' and totalprot[totalp_acc][ch] != 'NA'
                     else 'NA' for ch in channels})
             else:
-                norm_q.update({ch: str(norm_q[ch] / float(totalprot[totalp_acc][ch]))
+                norm_q.update({ch: norm_q[ch] / float(totalprot[totalp_acc][ch])
                     if quants[ch] != 'NA' and totalprot[totalp_acc][ch] != 'NA'
                     else 'NA' for ch in channels})
             outfeat.update(norm_q)
             yield outfeat
+        # FIXMNE correct medians? Get 0.0. for all, suspicious
 
-
-def mediancenter_ratios(ratios, channels, logratios, psmfn):
-    flatratios = [[feat[ch] for ch in channels] for feat in ratios]
-    ch_medians = get_medians(channels, flatratios, basename_report=os.path.basename(psmfn))
+        
+def mediancenter_ratios(ratios, channels, logratios, factor_table, report_factors):
+    if factor_table:
+        factor_ratios = [[float(x[ch]) if x[ch] != 'NA' else 'NA'
+            for ch in channels] for x in factor_table]
+    else:
+        factor_ratios = [[x[ch] for ch in channels] for x in ratios]
+    ch_medians = get_medians(channels, factor_ratios, basename_report=report_factors)
     for quant in ratios:
         if logratios:
-            quant.update({ch: str(quant[ch] - ch_medians[ch])
+            quant.update({ch: quant[ch] - ch_medians[ch]
                 if quant[ch] != 'NA' else 'NA' for ch in channels})
         else:
-            quant.update({ch: str(quant[ch] / ch_medians[ch])
+            quant.update({ch: quant[ch] / ch_medians[ch]
                 if quant[ch] != 'NA' else 'NA' for ch in channels})
         yield quant
 
 
 def get_psmratios(psmfn, header, channels, denom_channels, sweep, report_intensity, 
         summarize_by, min_int, acc_col, logintensities, keep_na_psms):
     allfeats, feat_order, psmratios = {}, OrderedDict(), []
@@ -100,15 +115,15 @@
         if acc_col and (psm[acc_col] == '' or 
                 (acc_col != psmh.HEADER_PEPTIDE and ';' in psm[acc_col]) or
                 not {psm[q] for q in channels}.difference({'NA', None, False, ''})
                 ):
             continue
         ratios = calc_psm_ratios_or_int(psm, channels, denom_channels, sweep, 
                 report_intensity, min_int, logintensities)
-        if not keep_na_psms and any((ratios[ix] == 'NA' for ix, q in enumerate(channels))):
+        if acc_col and not keep_na_psms and any((ratios[ix] == 'NA' for ix, q in enumerate(channels))):
             continue
         elif acc_col:
             try:
                 allfeats[psm[acc_col]].append(ratios)
             except KeyError:
                 allfeats[psm[acc_col]] = [ratios]
             feat_order[psm[acc_col]] = 1
@@ -129,22 +144,14 @@
             elif summarize_by == 'average':
                 outfeature.update(summarize_by_averages(channels, quants))
             outfeature.update(get_no_psms(channels, quants))
             outfeatures.append(outfeature)
     return outfeatures
 
 
-def get_ratios_from_fn(fn, header, channels):
-    ratios = []
-    for feat in reader.generate_split_tsv_lines(fn, header):
-        ratios.append([float(feat[ch]) if feat[ch] != 'NA' else 'NA'
-                       for ch in channels])
-    return ratios
-
-
 def paste_to_psmtable(psmfn, header, ratios):
     # loop psms in psmtable, paste the outratios in memory
     for psm, ratio in zip(reader.generate_split_tsv_lines(psmfn, header), ratios):
         ratio.pop(ISOQUANTRATIO_FEAT_ACC)
         ratio = {'ratio_{}'.format(ch): val for ch, val in ratio.items()}
         psm.update(ratio)
         yield psm
```

### Comparing `msstitch-3.8/src/app/actions/psmtable/percolator.py` & `msstitch-3.9/src/app/actions/psmtable/percolator.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,58 +3,50 @@
 from app.readers import tsv as tsvreader
 from app.readers import xml
 from app.readers import percolator as percoreader 
 from app.dataformats import mzidtsv as psmheaders
 
 
 def calculate_target_decoy_competition(percofn):
-    """From a percolator XML output file, use its svm scores to calculate an FDR
-    using TD-competition (not percolator's mixmax method). Output 
-    can be used
-    to deliver 
     """
-    # TODO add option to calculate FDR or not (percolator default one)
+    From a percolator XML output file, take the FDR (q-value) and PEP and apply
+    to the PSM table
+    """
     ns = xml.get_namespace_from_top(percofn, None)
-    # First calculate PSM FDRs
+    # Get PSM FDRs
     psms = {
-            p.attrib['{%s}psm_id' % ns['xmlns']]: (
-                float(p.find('{%s}svm_score' % ns['xmlns']).text),
-                p.attrib['{%s}decoy' % ns['xmlns']] == 'true')
+            p.attrib['{%s}psm_id' % ns['xmlns']]: {
+                'svm': float(p.find('{%s}svm_score' % ns['xmlns']).text),
+                'qval': float(p.find('{%s}q_value' % ns['xmlns']).text),
+                'pep': float(p.find('{%s}pep' % ns['xmlns']).text),
+                'td': 'decoy' if p.attrib['{%s}decoy' % ns['xmlns']] == 'true' else 'target',
+                }
             for p in percoreader.generate_psms(percofn, ns)
             }
-    decoys = {True: 0, False: 0}
-    for psm in sorted([(pid, score, decoy) for pid, (score, decoy) in psms.items()], reverse=True, key=lambda x:x[1]):
-        decoys[psm[2]] += 1
-        try:
-            psms[psm[0]] = {'decoy': psm[2], 'svm': psm[1], 'qval': min(decoys[True]/decoys[False], 1)}  # T-TDC
-        except ZeroDivisionError:
-            psms[psm[0]] = {'decoy': psm[2], 'svm': psm[1], 'qval': 1}  # T-TDC
-    # Then calculate peptide FDRs
-    decoys = {'true': 0, 'false': 0}
-    for svm, decoy, psm_ids in sorted([(float(x.find('{%s}svm_score' % ns['xmlns']).text), x.attrib['{%s}decoy' % ns['xmlns']], x.find('{%s}psm_ids' % ns['xmlns'])) for x in percoreader.generate_peptides(percofn, ns)], reverse=True, key=lambda x:x[0]):
-        decoys[decoy] += 1
-        for pid in psm_ids:
+    # Then get peptide FDRs and add them to PSMs
+    for peptide in percoreader.generate_peptides(percofn, ns):
+        psm_ids = peptide.find('{%s}psm_ids' % ns['xmlns'])
+        for psm_id in psm_ids:
             try:
-                psms[pid.text]['pepqval'] = min(decoys['true']/decoys['false'], 1)
-            except ZeroDivisionError:
-                psms[pid.text]['pepqval'] = 1
+                psms[psm_id.text].update({
+                    'pepqval': float(peptide.find('{%s}q_value' % ns['xmlns']).text),
+                    'peppep': float(peptide.find('{%s}pep' % ns['xmlns']).text),
+                    })
             except KeyError:
                 # Edgecase, sometimes filtering percolator data causes this:
                 # when there is a peptide with a PSM ID not in percolator PSMs 
                 # set all its PSMs pep-q-values to 1
-                [psms[x].update({'pepqval': 1}) for x in psm_ids if x in psms]
+                [psms[x].update({'pepqval': 1, 'peppep': 1}) for x in psm_ids if x in psms]
                 break
     return psms
 
 
 def add_fdr_to_mzidtsv(psms, mzid_specidr, mzns, percodata):
     """Takes PSMs from an mzIdentML and its MSGF+ TSV and a corresponding 
-    percolator XML. Calculate FDR from percolator scores and adds these 
-    to tsv lines. FDR calculation is done outside of percolator to avoid 
-    Mix-max FDR and instead use target-decoy competition.
+    percolator XML. 
     """
     # mzId results and PSM lines can be zipped
     scan = 0
     for specidr in mzid_specidr:
         try:
             scan = int({x.split('=')[0]: x.split('=')[1] for x in specidr.attrib['spectrumID'].split(' ')}['scan'])
         except KeyError:
@@ -70,20 +62,22 @@
                     sii_id=specidi.attrib['id'], sc=scan, rk=specidi.attrib['rank'], ch=psm['Charge'])]
             except KeyError:
                 continue
             outpsm = {k: v for k,v in psm.items()}
             outpsm.update({
                 psmheaders.HEADER_SVMSCORE: percopsm['svm'], 
                 psmheaders.HEADER_PSMQ: percopsm['qval'], 
+                psmheaders.HEADER_PSM_PEP: percopsm['pep'], 
                 psmheaders.HEADER_PEPTIDE_Q: percopsm['pepqval'], 
-                psmheaders.HEADER_TARGETDECOY: 'decoy' if percopsm['decoy'] else 'target', 
+                psmheaders.HEADER_PEPTIDE_PEP: percopsm['peppep'], 
+                psmheaders.HEADER_TARGETDECOY: percopsm['td'],
                 })
             # Remove all decoy protein matches from target proteins, to ensure downstream
             # processing does not trip up on them, e.g. having a decoy master protein.
-            if not percopsm['decoy']:
+            if percopsm['td'] != 'decoy':
                 outprots = []
                 for prot in outpsm[psmheaders.HEADER_PROTEIN].split(';'):
                     if not prot.startswith(psmheaders.DECOY_PREFIX):
                         outprots.append(prot)
                 outpsm[psmheaders.HEADER_PROTEIN] = ';'.join(outprots)
             yield outpsm
```

### Comparing `msstitch-3.8/src/app/actions/psmtable/refine.py` & `msstitch-3.9/src/app/actions/psmtable/refine.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/psmtable/splitmerge.py` & `msstitch-3.9/src/app/actions/psmtable/splitmerge.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/psmtopeptable.py` & `msstitch-3.9/src/app/actions/psmtopeptable.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/actions/sequence.py` & `msstitch-3.9/src/app/actions/sequence.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/dataformats/peptable.py` & `msstitch-3.9/src/app/dataformats/peptable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 HEADER_PEPTIDE = 'Peptide sequence'
 HEADER_NO_PSM = '# PSMs'
 HEADER_AREA = 'MS1 area (highest of all PSMs)'
 HEADER_QVAL = 'q-value'
+HEADER_PEP = 'PEP'
 HEADER_QVAL_MODELED = 'q-value (linear modeled)'
 HEADER_FALSE_LOC_RATE = 'PTM FLR'
 HEADER_LINKED_PSMS = 'Files/scans for peptide'
 HEADER_PROTEINS = 'Protein(s)'
 HEADER_MASTERPROTEINS = 'Master protein(s)'
 HEADER_NO_CONTENTPROTEINS = '# proteins in group'
 HEADER_COVERAGES = 'Coverage(s)'
```

### Comparing `msstitch-3.8/src/app/dataformats/prottable.py` & `msstitch-3.9/src/app/dataformats/prottable.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/drivers/base.py` & `msstitch-3.9/src/app/drivers/base.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/drivers/lookups.py` & `msstitch-3.9/src/app/drivers/lookups.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/drivers/merge.py` & `msstitch-3.9/src/app/drivers/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,32 @@
     command = 'merge'
     commandhelp = ('Create merged gene/protein/peptide tables from multiple '
             'sample set tables')
 
     def set_options(self):
         super().set_options()
         self.options.update(self.define_options(['setnames',
-                                                 'quantcolpattern',
-                                                 'precursorquantcolpattern',
-                                                 'fdrcolpattern',
-                                                 'flrcolpattern',
-                                                 'multifiles', 'featcol'],
-                                                lookup_options))
+            'quantcolpattern', 'precursorquantcolpattern', 'fdrcolpattern',
+            'flrcolpattern', 'multifiles', 
+            'featcol'], lookup_options))
         self.options.update(self.define_options(['lookupfn', 'mergecutoff'],
-                                                prottable_options))
-        self.options.update(self.define_options(['nogroup', 'genecentric'],
-                                                peptable_options))
+            prottable_options))
+        self.options.update(self.define_options(['nogroup', 'pepcolpattern',
+            'genecentric'], peptable_options))
 
     def parse_input(self, **kwargs):
-        self.is_peptidetable = False
         super().parse_input(**kwargs)
         header = tsvreader.get_tsv_header(self.fn[0])
         self.header = [header[0]]
         if header[0] == peph.HEADER_PEPTIDE:
             self.is_peptidetable = True
+        else:
+            self.is_peptidetable = False
+            self.pepcolpattern = None # override input if any
+        if header[0] == peph.HEADER_PEPTIDE:
             if self.genecentric:
                 self.lookuptype = 'peptidegenecentrictable'
                 self.header.extend([peph.HEADER_GENES, peph.HEADER_ASSOCIATED])
             elif self.nogroup:
                 self.lookuptype = 'peptidetableplain'
                 self.header.extend([peph.HEADER_PROTEINS])
             else:
@@ -61,15 +61,15 @@
     def set_features(self):
         # FIXME need check to see same poolnames correlate with self.fn len
         self.initialize_lookup()
         self.featcol = self.featcol - 1
         self.setnames = [x.replace('"', '') for x in self.setnames]
         merge.create_lookup(self.fn, self.lookup, self.setnames, self.featcol,
                 self.precursorquantcolpattern, self.quantcolpattern,
-                self.fdrcolpattern, self.flrcolpattern)
+                self.fdrcolpattern, self.pepcolpattern, self.flrcolpattern)
         for field in self.lookup.stdheaderfields:
             self.header.extend(['{}_{}'.format(x, field) for x in self.setnames])
         if self.fdrcolpattern and not self.is_peptidetable:
             self.header.extend(['{}_{}'.format(x, ph.HEADER_QVAL) for x in self.setnames])
         if self.is_peptidetable:
             if self.flrcolpattern:
                 self.header.extend(['{}_{}'.format(x, peph.HEADER_FALSE_LOC_RATE) for x in self.setnames])
```

### Comparing `msstitch-3.8/src/app/drivers/options.py` & `msstitch-3.9/src/app/drivers/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -158,14 +158,21 @@
     'mediannormalize': {'driverattr': 'mediannormalize',
         'clarg': '--median-normalize', 'default': False, 
         'required': False, 'action': 'store_const', 'const': True,
         'help': 'Median-centering normalization for isobaric quant data on protein or '
         'peptide level. This median-centers the data for each channel by '
         'dividing with the median channel value (or subtracting in case of '
         'log data), for each channel in output features, e.g. proteins.'},
+    'mednorm_factors': {'driverattr': 'mednorm_factors',
+        'clarg': '--normalization-factors-table', 'type': 'file', 'required': False, 
+        'help': 'A protein/peptide/gene table that provides an alternate source '
+        'of normalization factors than the table to be normalized. This can be '
+        'used e.g. when having a PTM table which does not have a large amount '
+        'of peptides or is noisy. Use together with --median-normalize',
+        },
     'ms1mediannormalize': {'driverattr': 'ms1mediannormalize',
         'clarg': '--median-normalize-ms1', 'default': False, 
         'required': False, 'action': 'store_const', 'const': True,
         'help': 'Median-centering normalization for MS1 quant data on protein or '
         'peptide level. This median-centers the data by dividing output MS1 quant '
         'values with the median output MS1 quant value '},
 }
@@ -360,14 +367,60 @@
         'type': 'file', 'nargs': '+'},
     'splitcol': {'driverattr': 'splitcol', 'clarg': '--splitcol',
                  'help': 'Either a column number to split a PSM table on, or '
                  '"TD", "bioset" for splitting on target/decoy or biological '
                  'sample set columns (resulting from msstitch perco2psm or '
                  'msstitch psmtable. First column is number 1.'
                  },
+    'lucitemplate': {'driverattr': 'lucitemplate', 'clarg': '--lucitemplate', 'type': 'file',
+            'help': 'Template for luciphor config file if not using the default one found '
+            'in .. ', # FIXME get default luci template here',
+            },
+    'mods': {'driverattr': 'mods', 'clarg': '--mods', 'nargs': '+', 'type': str,
+            'help': 'All modification names used in the experiment, e.g. Phospho, '
+            'Oxidation, TMT10plex. Needed when not already stored in DB file. '
+            'Specified as either e.g. --mods Oxidation Phospho, or as '
+            '--luciptms Oxidation Phospho:ST,  or for mods not in msstitch data, use the MSGF '
+            'form: --mods "79.966331,STY,opt,any,Phospho" "15.994915,M,opt,any,Oxidation"'
+            'If not specified, the default amino acids will be used '
+            '(here M, for Phospho STY), which can be found in ', ## FIXME get defaults
+            'required': False,
+            },
+    'luciptms': {'driverattr': 'luciptms', 'clarg': '--luciptms', 'nargs': '+', 'type': str,
+            'help': 'PTM names (unimod) and amino acid residues to run luciphor against on '
+            'the PSM table of a sample(set). Specified as either --luciptms Phospho, or as '
+            '--luciptms Phospho:ST . In the first case the default amino acids will be '
+            'used (here STY), which can be found in ', ## FIXME get defaults
+            },
+    'ms2tolerance': {'driverattr': 'ms2tol', 'clarg': '--ms2tol', 'type': str,
+            'help': 'MS2 fragment ion tolerance for Luciphor to use, default is 0.025Da, '
+            'valid units are Da and ppm (e.g. --ms2tol 10ppm).', 'default': '0.025Da',
+            },
+    'luci_minpsms': {'driverattr': 'luci_minpsms', 'clarg': '--luciminpsms', 'type': int,
+            'help': 'Minimum amount of PSMs needed for any charge state in order to build '
+            'a model for that state in Luciphor',
+            },
+    'luci_frag': {'driverattr': 'luci_frag', 'clarg': '--fragmentation', 'type': str,
+        'choices': ['hcd', 'cid'], 'default': 'hcd', 'help': 'Fragmentation type, one of HCD, CID',
+        },
+    'maxlength': {'driverattr': 'maxlength', 'default': 50,
+                  'help': 'Maximum length of peptide to be included in Luciphor analysis',
+                  'type': int, 'clarg': '--maxlen', 'required': False},
+    'maxcharge': {'driverattr': 'maxcharge', 'default': 6,
+                  'help': 'Maximum charge of PSM to be included in Luciphor analysis',
+                  'type': int, 'clarg': '--maxcharge', 'required': False},
+    'lucimemory': {'driverattr': 'lucimem', 'type': int, 'clarg': '--luciXmx',
+            'help': 'Java heap memory maximum for luciphor (in GB, default 1)', 'default': 1,
+            },
+    'lucithread': {'driverattr': 'lucithread', 'type': int, 'clarg': '--lucithread',
+            'help': 'Amount of threads to run Luciphor on, default 1', 'default': 1,
+            },
+    'mzmlpath': {'driverattr': 'mzmlpath', 'type': str, 'clarg': '--mzmlpath',
+        'default': '.', 'help': 'Path to where mzML files can be found',
+            },
 }
 psmtable_options['quantcolpattern'] = {
     k: v for k, v in shared_options['quantcolpattern'].items()}
 psmtable_options['quantcolpattern']['required'] = True
 psmtable_options['featcol'] = {k: v for k, v 
         in shared_options['featcol'].items()}
 psmtable_options['featcol'].update(
@@ -459,22 +512,26 @@
                     'overlapping stepped low-qvalue data of peptides with '
                     'different scores', },
     'qvalthreshold': {'driverattr': 'qvalthreshold',
         'type': float, 'clarg': '--qvalthreshold', 'help': 'Specifies the '
         'inclusion threshold for q-values to fit a linear model to. Any scores/'
         'q-values below this threshold will not be used.', 'default': 10e-4,
         'required': False},
+    'pepcolpattern': {'driverattr': 'pepcolpattern', 'required': False,
+                      'clarg': '--pepcolpattern', 'type': str,
+                      'default': None, 'help': 'Unique text pattern to identify '
+                      'PEP column (given by percolator for peptides) in input table.'},
     'minpeptidenr': {'driverattr': 'minpeptidenr',
         'type': int, 'clarg': '--minpepnr', 'default': 10, 'help': 'Specifies '
         'the minimal amount of peptides (passing the --qvalthreshold) needed '
         'to fit a linear model, default is 10.', 'required': False},
     'totalprotfn': {'driverattr': 'totalprotfn', 'type': 'file', 
         'clarg': '--totalproteome', 'required': False,
         'help': 'File containing total proteome quantification to normalize PTM '
         'peptide quantification against, i.e. Phospho peptides isobaric quant '
         'ratios are divided by their proteins to distinguish differential '
         'phosphorylation from the protein expression variation in the sample. '
         'This file can also be a gene names or ENSG table. Accession should be '
         'in the first column. The file is preferably generated from a search '
-        'without the relevant PTM, and should not be normalized to channel '
-        'medians'},
+        'without the relevant PTM, and can be a median-center normalized table. '
+        },
 })
```

### Comparing `msstitch-3.8/src/app/drivers/peptable.py` & `msstitch-3.9/src/app/drivers/peptable.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         self.infiletype = 'TSV PSM table (MSGF+)'
 
     def set_options(self):
         super().set_options()
         self.options.update(self.define_options(['spectracol', 'scorecolpattern', 
             'quantcolpattern', 'precursorquantcolpattern', 'minint', 'denomcols',
             'denompatterns', 'mediansweep', 'medianintensity', 'median_or_avg',
-            'logisoquant', 'mediannormalize', 'modelqvals', 'qvalthreshold',
-            'keep_psms_na', 'minpeptidenr', 'totalprotfn'], peptable_options))
+            'logisoquant', 'mediannormalize', 'mednorm_factors', 'modelqvals',
+            'qvalthreshold', 'keep_psms_na', 'minpeptidenr', 'totalprotfn'], peptable_options))
 
     def prepare(self):
         self.oldheader = tsvreader.get_tsv_header(self.fn)
         self.get_column_header_for_number(['spectracol'])
         self.scorecol = tsvreader.get_cols_in_file(self.scorecolpattern,
                                                    self.oldheader, True)
         self.precurquantcol = psmtopeptable.get_quantcols(self.precursorquantcolpattern,
@@ -83,32 +83,36 @@
             quantcols = tsvreader.get_columns_by_pattern(self.oldheader,
                                                    self.quantcolpattern)
             totalproteome, tpacc, tp_pepacc = False, False, False
             if self.totalprotfn:
                 pep_tp_accs = [psmh.HEADER_MASTER_PROT, psmh.HEADER_SYMBOL,
                         psmh.HEADER_GENE, peph.HEADER_PROTEINS]
                 totalphead = tsvreader.get_tsv_header(self.totalprotfn)
-                totalproteome = tsvreader.generate_split_tsv_lines(self.totalprotfn, totalphead)
                 totalpfield_found = False
                 for tpacc, tp_pepacc in zip(proth.TPROT_HEADER_ACCS, pep_tp_accs):
                     if totalphead[0] == tpacc and tp_pepacc in self.header:
                         totalpfield_found = True
                         break
                 if not totalpfield_found:
                     print('Could not find correct header field name in the total '
                             'proteome table passed. '
                             'Should be one of {}'.format(proth.TPROT_HEADER_ACCS))
                     sys.exit(1)
+                totalproteome = tsvreader.generate_split_tsv_lines(self.totalprotfn, totalphead)
+            mn_factors = False
+            if self.mednorm_factors:
+                mnhead = tsvreader.get_tsv_header(self.mednorm_factors)
+                mn_factors = tsvreader.generate_split_tsv_lines(self.mednorm_factors, mnhead)
             nopsms = [isosummarize.get_no_psms_field(qf) for qf in quantcols]
             self.header = self.header + quantcols + nopsms + [proth.HEADER_NO_FULLQ_PSMS]
             peptides = isosummarize.get_isobaric_ratios(self.fn, self.oldheader, 
                     quantcols, denomcols, self.mediansweep, self.medianintensity,
                     self.median_or_avg, self.minint, peptides, self.header[0],
                     psmh.HEADER_PEPTIDE, totalproteome, tpacc, tp_pepacc,
-                    self.logisoquant, self.mediannormalize, self.keepnapsms)
+                    self.logisoquant, self.mediannormalize, mn_factors, self.keepnapsms)
         if self.modelqvals:
             qix = self.header.index(peph.HEADER_QVAL) + 1
             self.header = self.header[:qix] + [peph.HEADER_QVAL_MODELED] + self.header[qix:]
             scorecol = tsvreader.get_cols_in_file(self.scorecolpattern,
                     self.oldheader, True)
             peptides = psmtopeptable.recalculate_qvals_linear_model(peptides, 
                     scorecol, self.qvalthreshold, self.minpeptidenr)
```

### Comparing `msstitch-3.8/src/app/drivers/percolator.py` & `msstitch-3.9/src/app/drivers/percolator.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/drivers/prottable.py` & `msstitch-3.9/src/app/drivers/prottable.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class ProttableDriver(PepProttableDriver):
 
     def set_options(self):
         super().set_options()
         options = self.define_options(['decoyfn', 'scorecolpattern', 'minlogscore',
             'quantcolpattern', 'minint', 'denomcols', 'denompatterns', 'mediansweep',
             'medianintensity', 'median_or_avg', 'logisoquant', 'mediannormalize',
-            'keep_psms_na', 'precursor', 'psmfile'], prottable_options)
+            'mednorm_factors', 'keep_psms_na', 'precursor', 'psmfile'], prottable_options)
         self.options.update(options)
 
     def get_td_proteins_bestpep(self, theader, dheader):
         self.header = [self.headeraccfield] + prottabledata.PICKED_HEADER
         tscorecol = tsvreader.get_cols_in_file(self.scorecolpattern, theader, True)
         dscorecol = tsvreader.get_cols_in_file(self.scorecolpattern, dheader, True)
         tpeps = tsvreader.generate_split_tsv_lines(self.fn, theader)
@@ -55,21 +55,25 @@
                         'or regex pattterns to find them, or use median sweep, or '
                         'report median intensities.')
                 sys.exit(1)
             elif self.medianintensity and self.mediannormalize:
                 print('Cannot do median-centering on intensity values, exiting')
                 sys.exit(1)
             quantcols = tsvreader.get_columns_by_pattern(psmheader, self.quantcolpattern)
+            mn_factors = False
+            if self.mednorm_factors:
+                mnhead = tsvreader.get_tsv_header(self.mednorm_factors)
+                mn_factors = tsvreader.generate_split_tsv_lines(self.mednorm_factors, mnhead)
             nopsms = [isosummarize.get_no_psms_field(qf) for qf in quantcols]
             self.header = self.header + quantcols + nopsms + [prottabledata.HEADER_NO_FULLQ_PSMS]
             features = isosummarize.get_isobaric_ratios(self.psmfile, psmheader,
                     quantcols, denomcols, self.mediansweep, self.medianintensity,
                     self.median_or_avg, self.minint, features, self.headeraccfield,
                     self.fixedfeatcol, False, False, False, self.logisoquant, self.mediannormalize,
-                    self.keepnapsms)
+                    mn_factors, self.keepnapsms)
         return features
 
 
 
 
 class ProteinsDriver(ProttableDriver):
     command = 'proteins'
```

### Comparing `msstitch-3.8/src/app/drivers/psmtable.py` & `msstitch-3.9/src/app/drivers/psmtable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import subprocess
 from hashlib import md5
 from itertools import chain
 
 from app.drivers.options import psmtable_options
 from app.drivers.base import PSMDriver
 
 from app.readers import tsv as tsvreader
@@ -12,14 +13,15 @@
 from app.dataformats.prottable import HEADER_NO_FULLQ_PSMS
 
 from app.actions.psmtable import splitmerge as splitmerge
 from app.actions.psmtable import refine as refine
 from app.actions.psmtable import percolator as perco
 from app.actions.psmtable import filtering
 from app.actions.psmtable import isosummarize
+from app.actions.psmtable import luciphor
 
 from app.dataformats import prottable as prottabledata
 
 from app.writers import tsv as writer
 
 
 class TSVConcatenateDriver(PSMDriver):
@@ -240,15 +242,15 @@
                    'PSM table containing raw intensities.')
 
     def set_options(self):
         super().set_options()
         self.options.update(self.define_options(['quantcolpattern', 'denompatterns',
             'denomcols', 'mediansweep', 'medianintensity', 'median_or_avg',
             'keep_psms_na', 'minint', 'featcol', 'logisoquant', 
-            'mediannormalize'], psmtable_options))
+            'mediannormalize', 'mednorm_factors'], psmtable_options))
 
     def set_features(self):
         denomcols = False
         if self.denomcols is not None:
             denomcols = [self.number_to_headerfield(col, self.oldheader)
                          for col in self.denomcols]
         elif self.denompatterns is not None:
@@ -256,25 +258,30 @@
                            for pattern in self.denompatterns]
             denomcols = set([col for cols in denomcolnrs for col in cols])
         elif not self.mediansweep and not self.medianintensity:
             raise RuntimeError('Must define either denominator column numbers '
                                'or regex pattterns to find them')
         quantcols = tsvreader.get_columns_by_pattern(self.oldheader,
                                                self.quantcolpattern)
+        mn_factors = False
+        if self.mednorm_factors:
+            mnhead = tsvreader.get_tsv_header(self.mednorm_factors)
+            mn_factors = tsvreader.generate_split_tsv_lines(self.mednorm_factors, mnhead)
         nopsms = [isosummarize.get_no_psms_field(qf) for qf in quantcols]
         if self.featcol:
             self.get_column_header_for_number(['featcol'], self.oldheader)
             self.header = [self.featcol] + quantcols + nopsms + [HEADER_NO_FULLQ_PSMS]
         else:
             self.header = (self.oldheader +
                            ['ratio_{}'.format(x) for x in quantcols])
         self.psms = isosummarize.get_isobaric_ratios(self.fn, self.oldheader,
                 quantcols, denomcols, self.mediansweep, self.medianintensity,
                 self.median_or_avg, self.minint, False, False, self.featcol,
-                False, False, False, self.logisoquant, self.mediannormalize, self.keepnapsms)
+                False, False, False, self.logisoquant, self.mediannormalize,
+                mn_factors, self.keepnapsms)
 
 
 class DeleteSetDriver(PSMDriver):
     outsuffix = '_deletedset.txt'
     command = 'deletesets'
     lookuptype = 'psm'
     commandhelp = """Remove sample sets from an existing PSM table and its lookup file"""
@@ -287,7 +294,97 @@
     def set_features(self):
         # In rare cases, a lookup is not used and we just filter the PSM table. I.e when
         # making a new lookup from a new+old PSM table.
         if self.lookup:
             self.lookup.delete_sample_set_shift_rows(self.setnames)
         self.header = self.oldheader
         self.psms = filtering.filter_psms_remove_set(self.oldpsms, self.setnames)
+
+
+class LuciphorDriver(PSMDriver):
+    outsuffix = '_lucxor.txt'
+    command = 'luciphor'
+    commandhelp = """Run luciphor on PSM table (of a single set) to get a table 
+    with PSMs with PTMs, containing false-localization rates and Luciphor scoring
+    luci_config_fn = '.luciphor_config.txt'
+    luci_inpsms = '.luciphor_inpsms.txt'
+    luci_in_header = ['srcFile', 'scanNum', 'charge', 'PSMscore', 'peptide', 'modSites')
+    luci_psmfields = [dm.HEADER_SPECFILE, dm.HEADER_SCANNR, dm.HEADER_CHARGE, dm.HEADER_PSMQ]
+    """
+
+    def set_options(self):
+        super().set_options()
+        self.options.update(self.define_options(['lucitemplate', 'mods', 'luciptms',
+            'ms2tolerance', 'luciminpsms', 'luci_frag', 'maxlength', 'maxcharge',
+            'mzmlpath', 'lucimemory', 'lucithread'], psmtable_options))
+
+    def set_features(self):
+        # parse passed mods and get masses etc from/to DB
+        # FIXME error report on this, parse errors of passed self.mods
+        # and errors in DB
+        try:
+            self.lookup_store_mods(luciphor.parse_input_mods(self.mods))
+        except RuntimeError as e:
+            print(e)
+            sys.exit(1)
+
+        # FIXME THIS NEEDS error reporting (PTM not found in DB)
+        luciptms = {}
+        for lptm in self.luciptms:
+            lptm.split(':')
+            aa = lptm[1] if len(lptm) == 2 else ''
+            luciptms[lptm[0]] = aa
+        fixm, varm, ptms = self.lookup.get_ptms_luciphor(luciptms)
+
+        # parse MS2 tolerance
+        if self.ms2tol[-2:] == 'Da':
+            toltype = 0
+            mstol = self.ms2tol[:-2]
+        elif self.ms2tol[-3:] == 'ppm':
+            toltype = 1
+            mstol = self.ms2tol[:-3]
+        else:
+            print('If defining MS2 tolerance, use formats --ms2tol 10ppm or --ms2tol 0.02Da')
+            sys.exit(1)
+        try:
+            float(mstol)
+        except TypeError:
+            print(f'MS2 tolerance value {mstol} should be a number!')
+            sys.exit(1)
+        ptmmods = {}
+        
+        algo = {'hcd': 1, 'cid': 0}[self.luci_frag.lower()]
+
+        # Run luciphor in try block with cleanup
+        # FIXME fix/var mods??
+        try:
+            luci_in = luciphor.create_luciphor_input(self.oldpsms, lucitemplate, self.mods,
+                    self.luciptms, self.luci_psmfields, self.luci_in_header,
+                    mstol, toltype, self.mzmlpath, algo, self.maxcharge, 
+                    self.maxlength, self.luci_minpsms, self.lucithread)
+            self.write_luciphor_input(luci_in)
+            subprocess.run(['luciphor2', f'-Xmx{self.lucimem}G', self.luci_config_fn])
+            self.psms = luciphor.parse_luciphor_output(luciptms, luciscores, ptmpsms, tdb,
+                    self.luciminscore, [*varm, *ptms])
+        except Exception:
+            raise
+        finally:
+            pass 
+            # FIXME cleanup all_scores, luciphor.out, etc etc
+
+    def write_luciphor_input(self, luci_inputs):
+        config_contents = next(luci_inputs)
+        with open(self.luci_config_fn, 'w') as wfp:
+            wfp.write(config_contents)
+        writer.write_tsv(self.luci_in_header, luci_inputs, self.luci_inpsms)
+
+
+def create_mods():
+    # FIXME this func to actions
+    for mod in varmods:
+        realmodmass = mod[0]
+        mmass, mres, mfm, mprotpos, mname = mod
+        mp = modpos(mod)
+        if mp in fixedmods:
+            nonblocked_fixed = NON_BLOCKING_MODS[mname] if mname in NON_BLOCKING_MODS else []
+            blocked_fixmass = sum([float(x[0]) for x in fixedmods[mp] if x[-1] not in nonblocked_fixed])
+            mod[0] = str(round(-(blocked_fixmass - float(mod[0])), 5))
```

### Comparing `msstitch-3.8/src/app/drivers/sequence.py` & `msstitch-3.9/src/app/drivers/sequence.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/drivers/startup.py` & `msstitch-3.9/src/app/drivers/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from argparse import ArgumentParser, RawTextHelpFormatter
 
-VERSION_NUMBER = '3.8'
+VERSION_NUMBER = '3.9'
 
 
 def parser_file_exists(currentparser, fn):
     if not os.path.exists(fn):
         currentparser.error('Input file %s not found!' % fn)
     else:
         return fn
```

### Comparing `msstitch-3.8/src/app/lookups/base.py` & `msstitch-3.9/src/app/lookups/base.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/lookups/sqlite/base.py` & `msstitch-3.9/src/app/lookups/sqlite/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import sqlite3
 
 
 mslookup_tables = {'biosets': ['set_id INTEGER PRIMARY KEY',
                                'set_name TEXT'],
+                   'mods': [
+                       'mod_id INTEGER PRIMARY KEY',
+                       'name TEXT',
+                       'mass FLOAT',
+                       ],
+                   'modpos': [
+                       'variable INTEGER', # 1 or 0
+                       'aa TEXT', # Can also be *
+                       'pos TEXT', # Can be N-term, C-term, etc
+                       'masschange FLOAT', # in case of competing mods this can diff from mod.mass
+                       'mod_id INTEGER',
+                       'FOREIGN KEY(mod_id) REFERENCES mods ON DELETE CASCADE '
+                       ],
                    'mzmlfiles': ['mzmlfile_id INTEGER PRIMARY KEY',
                                  'mzmlfilename TEXT',
                                  'set_id INTEGER',
                                  'FOREIGN KEY(set_id)'
                                  'REFERENCES biosets ON DELETE CASCADE'
                                  ],
                    'mzml': ['spectra_id TEXT PRIMARY KEY',
@@ -141,14 +154,23 @@
                                    'fdr DOUBLE',
                                    'FOREIGN KEY(pep_id) '
                                    'REFERENCES peptide_sequences(pep_id) '
                                    'FOREIGN KEY(peptable_id) '
                                    'REFERENCES '
                                    'peptide_tables(peptable_id) ON DELETE CASCADE'
                                    ],
+                   'peptide_pep': ['pep_id INTEGER',
+                                   'peptable_id INTEGER',
+                                   'pep DOUBLE',
+                                   'FOREIGN KEY(pep_id) '
+                                   'REFERENCES peptide_sequences(pep_id) '
+                                   'FOREIGN KEY(peptable_id) '
+                                   'REFERENCES '
+                                   'peptide_tables(peptable_id) ON DELETE CASCADE'
+                                   ],
                    'ptm_flr': ['pep_id INTEGER',
                            'peptable_id INTEGER',
                            'flr DOUBLE',
                            'FOREIGN KEY(pep_id) REFERENCES peptide_sequences(pep_id) '
                            'FOREIGN KEY(peptable_id) '
                            'REFERENCES peptide_tables(peptable_id) '
                            'ON DELETE CASCADE'],
```

### Comparing `msstitch-3.8/src/app/lookups/sqlite/peptable.py` & `msstitch-3.9/src/app/lookups/sqlite/peptable.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,46 @@
 
 
 class PepTableProteinCentricDB(ProtPepTable):
     datatype = 'peptide'
     stdheaderfields = [
             ph.HEADER_NO_PSM,
             ph.HEADER_QVAL,
+            ph.HEADER_PEP,
             ]
     singlefields = stdheaderfields + [
             ph.HEADER_FALSE_LOC_RATE,
             ph.HEADER_AREA,
             proth.HEADER_NO_FULLQ_PSMS,
             ]
     colmap = {'peptide_sequences': ['pep_id', 'sequence'],
               'peptide_precur_quanted': ['pep_id', 'peptable_id', 'quant'],
               'peptide_fdr': ['pep_id', 'peptable_id', 'fdr'],
+              'peptide_pep': ['pep_id', 'peptable_id', 'pep'],
               'ptm_flr': ['pep_id', 'peptable_id', 'flr'],
               'peptide_iso_fullpsms': ['pep_id', 'peptable_id', 'amount_psms'],
               'pepquant_channels': ['channel_id', 'peptable_id',
                                     'channel_name', 'amount_psms_name'],
               'peptide_iso_quanted': ['peptidequant_id', 'pep_id',
                                       'channel_id', 'quantvalue',
                                       'amount_psms'],
               }
 
+    def add_tables(self, tabletypes=[]):
+        ttypes = ['fntable', 'isoqtable', 'isochtable', 'prectable',
+                'fdrtable', 'peptable', 'fullqpsmtable', 'flrtable']
+        self.create_tables([self.table_map[self.datatype][x] for x in ttypes
+            if x in self.table_map[self.datatype]])
+
+    def store_pep(self, pep):
+        self.store_singlecol('peptable', pep)
+        table = self.table_map[self.datatype]['peptable']
+        self.singlecols_to_index.append(('pep_acc_ix', table, self.colmap[table][0]))
+        self.singlecols_to_index.append(('pep_table_ix', table, self.colmap[table][1]))
+
     def create_pdata_map(self):
         """This runs only once, returns the data which is not dependent on sets,
         in a dict with accessions as keys"""
 
         # First protein SQL, some peptides have TOO MANY proteingroup matches 
         # for SQLite to output on a single line, therefore we loop rows 
         # instead of doing GROUP_CONCAT
@@ -99,25 +113,27 @@
         cursor = self.get_cursor()
         for pid, seq in cursor.execute(pepsql):
             pgdata[pid][ph.HEADER_PEPTIDE] = seq
         return pgdata
 
     def merge_features(self):
         sql = """
-    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, flr.flr, ppq.quant,
-            fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name), GROUP_CONCAT(piq.quantvalue),
-            GROUP_CONCAT(piq.amount_psms)
+    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, pp.pep,
+            flr.flr, ppq.quant, fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name),
+            GROUP_CONCAT(piq.quantvalue), GROUP_CONCAT(piq.amount_psms)
         FROM peptide_sequences AS ps
         INNER JOIN psms ON ps.pep_id=psms.pep_id 
         INNER JOIN mzml ON psms.spectra_id=mzml.spectra_id
         INNER JOIN mzmlfiles ON mzml.mzmlfile_id=mzmlfiles.mzmlfile_id
         INNER JOIN biosets AS bs ON mzmlfiles.set_id=bs.set_id
         INNER JOIN peptide_tables AS pt ON pt.set_id=bs.set_id
         INNER JOIN peptide_fdr AS pf ON pf.peptable_id=pt.peptable_id AND 
             pf.pep_id=ps.pep_id
+        LEFT OUTER JOIN peptide_pep AS pp ON pp.peptable_id=pt.peptable_id AND 
+            pp.pep_id=ps.pep_id
         LEFT OUTER JOIN ptm_flr AS flr ON flr.peptable_id=pt.peptable_id AND
             flr.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_precur_quanted AS ppq ON ppq.peptable_id=pt.peptable_id AND
             ppq.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_iso_fullpsms AS fqpsm ON fqpsm.peptable_id=pt.peptable_id AND
             fqpsm.pep_id=ps.pep_id
         LEFT OUTER JOIN pepquant_channels AS pqc ON pqc.peptable_id=pt.peptable_id
@@ -139,38 +155,30 @@
         in a dict with accessions as keys. Different from protein grouped
         data in that we dont pull proteins from the protein group master table.
         """
 
         sql = """
 SELECT ps.pep_id, ps.sequence, GROUP_CONCAT(IFNULL(gsub.ensg, 'NA'), ';'),
     GROUP_CONCAT(IFNULL(gnsub.gn, 'NA'), ';')
-    FROM protein_psm AS pp
-    INNER JOIN psms ON psms.psm_id=pp.psm_id
-    INNER JOIN peptide_sequences AS ps ON psms.pep_id=ps.pep_id
-    INNER JOIN proteins AS p ON p.protein_acc=pp.protein_acc
+    FROM peptide_sequences AS ps
     LEFT OUTER JOIN (
-        SELECT gss.pid AS pid, gss.ensg AS ensg FROM (
-            SELECT DISTINCT psms.pep_id AS pid, g.gene_acc AS ensg
-            FROM genes as g
-            INNER JOIN ensg_proteins AS egp ON egp.gene_id=g.gene_id
-            INNER JOIN proteins AS p ON p.pacc_id=egp.pacc_id
-            INNER JOIN protein_psm AS pp ON pp.protein_acc=p.protein_acc
-            INNER JOIN psms ON psms.psm_id=pp.psm_id
-            ) AS gss GROUP BY gss.pid
+        SELECT DISTINCT psms.pep_id AS pid, g.gene_acc AS ensg
+        FROM genes as g
+        INNER JOIN ensg_proteins AS egp ON egp.gene_id=g.gene_id
+        INNER JOIN proteins AS p ON p.pacc_id=egp.pacc_id
+        INNER JOIN protein_psm AS pp ON pp.protein_acc=p.protein_acc
+        INNER JOIN psms ON psms.psm_id=pp.psm_id
         ) AS gsub ON gsub.pid=ps.pep_id
     LEFT OUTER JOIN (
-        SELECT gnss.pid AS pid, GROUP_CONCAT(gnss.gn) AS gn FROM (
-            SELECT DISTINCT psms.pep_id AS pid, aid.assoc_id AS gn
-            FROM associated_ids AS aid
-            INNER JOIN genename_proteins AS gnp ON gnp.gn_id=aid.gn_id
-            INNER JOIN proteins AS p ON p.pacc_id=gnp.pacc_id
-            INNER JOIN protein_psm AS pp ON pp.protein_acc=p.protein_acc
-            INNER JOIN psms ON psms.psm_id=pp.psm_id
-            ) AS gnss
-            GROUP BY gnss.pid
+        SELECT DISTINCT psms.pep_id AS pid, aid.assoc_id AS gn
+        FROM associated_ids AS aid
+        INNER JOIN genename_proteins AS gnp ON gnp.gn_id=aid.gn_id
+        INNER JOIN proteins AS p ON p.pacc_id=gnp.pacc_id
+        INNER JOIN protein_psm AS pp ON pp.protein_acc=p.protein_acc
+        INNER JOIN psms ON psms.psm_id=pp.psm_id
         ) AS gnsub ON gnsub.pid=ps.pep_id
     GROUP BY ps.pep_id
     """
         cursor = self.get_cursor()
         pgdata = {}
         for pid, seq, gaccs, aids in cursor.execute(sql):
             pgdata[pid] = {
@@ -178,23 +186,25 @@
                     ph.HEADER_GENES: gaccs,
                     ph.HEADER_ASSOCIATED: aids,
                     }
         return pgdata
 
     def merge_features(self):
         sql = """
-    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, flr.flr, ppq.quant,
-            fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name), GROUP_CONCAT(piq.quantvalue),
-            GROUP_CONCAT(piq.amount_psms)
+    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, pp.pep,
+            flr.flr, ppq.quant, fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name),
+            GROUP_CONCAT(piq.quantvalue), GROUP_CONCAT(piq.amount_psms)
         FROM peptide_sequences AS ps
         JOIN biosets AS bs 
         INNER JOIN psms ON ps.pep_id=psms.pep_id 
         INNER JOIN peptide_tables AS pt ON pt.set_id=bs.set_id
         INNER JOIN peptide_fdr AS pf ON pf.peptable_id=pt.peptable_id AND 
             pf.pep_id=ps.pep_id
+        LEFT OUTER JOIN peptide_pep AS pp ON pp.peptable_id=pt.peptable_id AND 
+            pp.pep_id=ps.pep_id
         LEFT OUTER JOIN ptm_flr AS flr ON flr.peptable_id=pt.peptable_id AND
             flr.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_precur_quanted AS ppq ON ppq.peptable_id=pt.peptable_id AND
             ppq.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_iso_fullpsms AS fqpsm ON fqpsm.peptable_id=pt.peptable_id AND
             fqpsm.pep_id=ps.pep_id
         LEFT OUTER JOIN pepquant_channels AS pqc ON pqc.peptable_id=pt.peptable_id
@@ -233,23 +243,25 @@
                     ph.HEADER_PEPTIDE: seq,
                     ph.HEADER_PROTEINS: prots,
                     }
         return pgdata
 
     def merge_features(self):
         sql = """
-    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, flr.flr, ppq.quant,
-            fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name), GROUP_CONCAT(piq.quantvalue),
-            GROUP_CONCAT(piq.amount_psms)
+    SELECT bs.set_name, ps.pep_id, COUNT(DISTINCT psms.psm_id), pf.fdr, pp.pep,
+            flr.flr, ppq.quant, fqpsm.amount_psms, GROUP_CONCAT(pqc.channel_name),
+            GROUP_CONCAT(piq.quantvalue), GROUP_CONCAT(piq.amount_psms)
         FROM peptide_sequences AS ps
         JOIN biosets AS bs 
         INNER JOIN psms ON ps.pep_id=psms.pep_id 
         INNER JOIN peptide_tables AS pt ON pt.set_id=bs.set_id
         INNER JOIN peptide_fdr AS pf ON pf.peptable_id=pt.peptable_id AND 
             pf.pep_id=ps.pep_id
+        LEFT OUTER JOIN peptide_pep AS pp ON pp.peptable_id=pt.peptable_id AND 
+            pp.pep_id=ps.pep_id
         LEFT OUTER JOIN ptm_flr AS flr ON flr.peptable_id=pt.peptable_id AND flr.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_precur_quanted AS ppq ON ppq.peptable_id=pt.peptable_id AND
             ppq.pep_id=ps.pep_id
         LEFT OUTER JOIN peptide_iso_fullpsms AS fqpsm ON fqpsm.peptable_id=pt.peptable_id AND
             fqpsm.pep_id=ps.pep_id
         LEFT OUTER JOIN pepquant_channels AS pqc ON pqc.peptable_id=pt.peptable_id
         LEFT OUTER JOIN peptide_iso_quanted AS piq ON piq.channel_id=pqc.channel_id AND
```

### Comparing `msstitch-3.8/src/app/lookups/sqlite/protpeptable.py` & `msstitch-3.9/src/app/lookups/sqlite/protpeptable.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,29 +28,24 @@
                            },
                  'peptide': {'fntable': 'peptide_tables',
                              'feattable': 'peptide_sequences',
                              'isoqtable': 'peptide_iso_quanted',
                              'isochtable': 'pepquant_channels',
                              'prectable': 'peptide_precur_quanted',
                              'fdrtable': 'peptide_fdr',
+                             'peptable': 'peptide_pep',
                              'fullqpsmtable': 'peptide_iso_fullpsms',
                              'flrtable': 'ptm_flr',
                              }
                  }
 
     def __init__(self, fn=None):
         super().__init__(fn)
         self.singlecols_to_index = []
 
-    def add_tables(self, tabletypes=[]):
-        ttypes = ['fntable', 'isoqtable', 'isochtable', 'prectable', 'fdrtable',
-                'fullqpsmtable', 'flrtable']
-        self.create_tables([self.table_map[self.datatype][x] for x in ttypes
-            if x in self.table_map[self.datatype]])
-
     def get_all_poolnames(self):
         cursor = self.get_cursor()
         cursor.execute(
             'SELECT DISTINCT set_name, set_id FROM biosets ORDER BY set_name')
         return cursor
 
     def store_table_files(self, tables):
@@ -131,14 +126,18 @@
 
     def store_fdr(self, fdr):
         self.store_singlecol('fdrtable', fdr)
         table = self.table_map[self.datatype]['fdrtable']
         self.singlecols_to_index.append(('fdr_acc_ix', table, self.colmap[table][0]))
         self.singlecols_to_index.append(('fdr_table_ix', table, self.colmap[table][1]))
 
+    def store_pep(self, pep):
+        '''Overridden in peptide table lookup'''
+        pass
+
     def store_fullq_psms(self, fullqpsms):
         self.store_singlecol('fullqpsmtable', fullqpsms)
         table = self.table_map[self.datatype]['fullqpsmtable']
         self.singlecols_to_index.append(('fullq_acc_ix', table, self.colmap[table][0]))
         self.singlecols_to_index.append(('fullq_table_ix', table, self.colmap[table][1]))
 
     def store_ptm_flr(self, flrs):
```

### Comparing `msstitch-3.8/src/app/lookups/sqlite/prottable.py` & `msstitch-3.9/src/app/lookups/sqlite/prottable.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 class ProtGeneTableBase(ProtPepTable):
     stdheaderfields = [
             ph.HEADER_NO_PSM,
             ph.HEADER_NO_PEPTIDE,
             ph.HEADER_NO_UNIPEP,
             ]
     singlefields = stdheaderfields + [ph.HEADER_QVAL, ph.HEADER_AREA, ph.HEADER_NO_FULLQ_PSMS]
+
+    def add_tables(self, tabletypes=[]):
+        ttypes = ['fntable', 'isoqtable', 'isochtable', 'prectable',
+                'fdrtable', 'fullqpsmtable', 'flrtable']
+        self.create_tables([self.table_map[self.datatype][x] for x in ttypes
+            if x in self.table_map[self.datatype]])
+
     
 
 class ProtTableDB(ProtGeneTableBase):
     datatype = 'protein'
     colmap = {'protein_group_master': ['master_id', 'protein_acc'],
               'proteins': ['pacc_id', 'protein_acc'],
               'protein_precur_quanted': ['pacc_id', 'prottable_id', 'quant'],
```

### Comparing `msstitch-3.8/src/app/lookups/sqlite/psms.py` & `msstitch-3.9/src/app/lookups/sqlite/psms.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 
 class PSMDB(ResultLookupInterface):
     def add_tables(self, tabletypes):
         self.create_tables(['psms', 'psmrows', 'peptide_sequences', 'fastafn',
                             'proteins', 'protein_evidence', 'protein_seq',
                             'prot_desc', 'protein_psm', 'genes',
-                            'associated_ids', 'ensg_proteins', 'genename_proteins'])
+                            'associated_ids', 'ensg_proteins', 'genename_proteins',
+                            'mods', 'modpos'])
         if 'proteingroup' in tabletypes:
             self.create_tables(['protein_coverage', 'protein_group_master',
                                 'protein_group_content', 'psm_protein_groups'])
 
     def get_fasta_md5(self):
         cursor = self.get_cursor()
         cursor.execute('SELECT md5 FROM fastafn LIMIT 1')
@@ -375,7 +376,59 @@
         self.index_column('psmrowid_index', 'psmrows', 'psm_id')
         self.index_column('psmrow_index', 'psmrows', 'rownr')
         cursor = self.get_cursor()
         cursor.execute('DELETE FROM peptide_sequences WHERE pep_id IN ('
             'SELECT ps.pep_id FROM peptide_sequences AS ps '
             'LEFT OUTER JOIN psms ON ps.pep_id=psms.pep_id WHERE psms.pep_id IS NULL)')
         self.conn.commit()
+
+    def get_dbmods(self):
+        dbmods = []
+        cursor = self.get_cursor()
+        sql  = ('SELECT m.name, mp.aa, mp.variable, mp.pos, m.mass, mp.masschange '
+                'FROM modpos AS mp JOIN mods AS m USING(mod_id)')
+        for mod in cursor.execute(sql).fetchall():
+            name, aa, var, pos, mass, masschange = mod
+            # FIXME mass is float? masschange float is OK
+            dbmods.append({'mass': mass, 'masschange': masschange, 'aa': aa,
+                'name': name, 'var': var, 'pos': pos})
+        return dbmods
+
+    def store_mods(self, mods):
+        # First check which mods passed are already stored, error if discrepancies
+        cursor = self.get_cursor()
+        dbmods = self.get_dbmods()
+        db_stored = len(dbmods) > 0
+        for dbmod in dbmods:
+            if dbmod not in mods:
+                pass
+                # FIXME get a error msg if they do not match the passed mods, to be avoided with --force?
+            else:
+                mods = [x for x in mods if x != dbmod]
+        if db_stored and len(mods):
+            # FIXME get a error msg if they do not match the passed mods, to be avoided with --force?
+            pass
+        elif len(mods):
+            msql = 'INSERT INTO mods(name, mass) VALUES(?, ?)'
+            mpsql = ('INSERT INTO modpos(variable, aa, pos, masschange, mod_id) '
+                    'VALUES(?, ?, ?, ?, ?)')
+            unique_name_mass = {f"{x['name']}_{x['mass']}": [x['name'], x['mass']] for x in mods}
+            for nm, mod in unique_name_mass.items():
+                cursor.execute(msql, (mod[0], mod[1]))
+                unique_name_mass[nm].append(cursor.lastrowid)
+            for mod in mods:
+                nm = f"{mod['name']}_{mod['mass']}"
+                cursor.execute(mpsql, (mod['var'], mod['aa'], mod['pos'],
+                    mod['masschange'], unique_name_mass[nm][-1]))
+
+    def get_ptms_luciphor(self, ptms):
+        fix, var, ptm = [], [], []
+        for mod in self.get_dbmods():
+            if not mod['var']:
+                # fixed mod
+                fix.append(mod)
+            elif mod['name'] in ptms and (mod['aa'] in ptms[mod['name']] 
+                    or ptms[mod['name']] == ''):
+                ptm.append(mod)
+            else:
+                var.append(mod)
+        return fix, var, ptm
```

### Comparing `msstitch-3.8/src/app/lookups/sqlite/quant.py` & `msstitch-3.9/src/app/lookups/sqlite/quant.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/lookups/sqlite/searchspace.py` & `msstitch-3.9/src/app/lookups/sqlite/searchspace.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/lookups/sqlite/spectra.py` & `msstitch-3.9/src/app/lookups/sqlite/spectra.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/msstitch.py` & `msstitch-3.9/src/app/msstitch.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/fasta.py` & `msstitch-3.9/src/app/readers/fasta.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/mzidplus.py` & `msstitch-3.9/src/app/readers/mzidplus.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/openms.py` & `msstitch-3.9/src/app/readers/openms.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/percolator.py` & `msstitch-3.9/src/app/readers/percolator.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/spectra.py` & `msstitch-3.9/src/app/readers/spectra.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/tsv.py` & `msstitch-3.9/src/app/readers/tsv.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/xml.py` & `msstitch-3.9/src/app/readers/xml.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/readers/xmlformatting.py` & `msstitch-3.9/src/app/readers/xmlformatting.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/writers/percolator.py` & `msstitch-3.9/src/app/writers/percolator.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/app/writers/tsv.py` & `msstitch-3.9/src/app/writers/tsv.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/src/msstitch.egg-info/PKG-INFO` & `msstitch-3.9/src/msstitch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msstitch
-Version: 3.8
+Version: 3.9
 Summary: MS proteomics post processing utilities
 Home-page: https://github.com/lehtiolab/msstitch
 Author: Jorrit Boekel
 Author-email: jorrit.boekel@scilifelab.se
 Maintainer: Jorrit Boekel
 Maintainer-email: jorrit.boekel@scilifelab.se
 License: MIT
@@ -81,17 +81,25 @@
 
 Or without removing peptide sequences that match to the target DB:
 
 ```
 msstitch makedecoy uniprot.fasta -o decoy.fasta --scramble tryp_rev --ignore-target-hits
 ```
 
+Specify modifications and create a mod-file for MSGF+:
+
+```
+msstitch mods --dbfile db.sqlite --modnames Phospho Oxidation Carbamidomethylation TMT6plex \
+  --msgffile mods.txt
+```
 
 After running two samples of MSGF and percolator, we can start making 
-a more proper set of PSM tables:
+a more proper set of PSM tables by adding percolator data and filtering
+on FDR. The following adds percolator svm-score, q-value (FDR), and posterior
+error as columns to the PSM table:
 
 ```
 # Add percolator data, filter 0.01 FDR
 msstitch perco2psm -i psms1.txt \
   --perco percolator1.xml --mzid psms1.mzIdentML \
   --filtpsm 0.01 --filtpep 0.01
 msstitch perco2psm -i psms2.txt \
@@ -170,15 +178,26 @@
 
 ```
 msstitch peptides -i set1_ptm_psms.txt -o set1_ptm_peptides.txt \
   --scorecolpattern svm --isobquantcolpattern tmt10plex --denompatterns _126 _127C \
   --logisoquant --totalproteome set1_proteins.txt
 ```
 
-Create a protein table, with isobaric quantification as for peptides, the
+For proper median centering of this table (as it would otherwise be impacted by
+sample differences per channel), you may want to median-center. In the case of 
+small and possibly noisy PTM tables, it can be advisable to use another table
+from a global search (or e.g. the full peptide or protein table from the PTM search)
+for determining channel medians. This is possible by specifying the above command
+plus:
+
+```
+  --median-normalize --normalization-factors-table /path/to/set1_global_proteins.txt
+```
+
+To create a protein table, with isobaric quantification as for peptides, the
 average of the top-3 highest intensity peptides for MS1 quantification:
 For all of these, summarizing isobaric PSM data to peptide, protein, gene features 
 is done using medians of log2 PSM quantification values per feature (e.g. a protein). If you'd
 rather use averages, use `--summarize-average` as below, where we also show log2
 transformation of intensities before summarizing and subsequent median-centering:
 
 ```
```

### Comparing `msstitch-3.8/src/msstitch.egg-info/SOURCES.txt` & `msstitch-3.9/src/msstitch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 src/app/actions/lookups/spectra.py
 src/app/actions/percolator/__init__.py
 src/app/actions/percolator/filters.py
 src/app/actions/percolator/split.py
 src/app/actions/psmtable/__init__.py
 src/app/actions/psmtable/filtering.py
 src/app/actions/psmtable/isosummarize.py
+src/app/actions/psmtable/luciphor.py
 src/app/actions/psmtable/percolator.py
 src/app/actions/psmtable/refine.py
 src/app/actions/psmtable/splitmerge.py
 src/app/dataformats/__init__.py
+src/app/dataformats/defaultmods.py
 src/app/dataformats/mzidtsv.py
 src/app/dataformats/peptable.py
 src/app/dataformats/prottable.py
 src/app/drivers/__init__.py
 src/app/drivers/base.py
 src/app/drivers/lookups.py
 src/app/drivers/merge.py
@@ -98,28 +100,32 @@
 tests/fixtures/genenames.txt
 tests/fixtures/isosum_charge_column.txt
 tests/fixtures/perco.xml
 tests/fixtures/perco.xml_h0.xml
 tests/fixtures/perco.xml_h1.xml
 tests/fixtures/perco_timstof.xml
 tests/fixtures/proteins.txt
+tests/fixtures/proteins_avg.txt
 tests/fixtures/proteins_intensities.txt
 tests/fixtures/proteins_isonorm_log.txt
 tests/fixtures/proteins_isonorm_nolog.txt
+tests/fixtures/proteins_nonorm_log.txt
 tests/fixtures/proteins_quantonly.txt
 tests/fixtures/proteins_sweep.txt
 tests/fixtures/protrev_ens99_small.fasta
 tests/fixtures/quant_lookup.sqlite
 tests/fixtures/set1_target_pg.tsv
 tests/fixtures/spectra_lookup.sqlite
 tests/fixtures/spectra_lookup_timstof.sqlite
 tests/fixtures/target.tsv
 tests/fixtures/target_pep_quant_norm.tsv
 tests/fixtures/target_peptides.tsv
+tests/fixtures/target_peptides_avg.tsv
 tests/fixtures/target_peptides_sweep.tsv
+tests/fixtures/target_peptides_totalp_sepnorm.txt
 tests/fixtures/target_peptides_totalprotnorm.txt
 tests/fixtures/target_peptides_totalprotnorm_nolog.txt
 tests/fixtures/target_pg.tsv
 tests/fixtures/target_psms.sqlite
 tests/fixtures/trypsinized_twoproteins.fasta
 tests/integration/__init__.py
 tests/integration/basetests.py
```

### Comparing `msstitch-3.8/tests/base_fixtures/ens99_small.fasta` & `msstitch-3.9/tests/base_fixtures/ens99_small.fasta`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/base_fixtures/few_spec_timstof.mzML` & `msstitch-3.9/tests/base_fixtures/few_spec_timstof.mzML`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/base_fixtures/known_peptide_lookup.sqlite` & `msstitch-3.9/tests/base_fixtures/known_peptide_lookup.sqlite`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/base_fixtures/rev_known_peptide_lookup.sqlite` & `msstitch-3.9/tests/base_fixtures/rev_known_peptide_lookup.sqlite`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/fixtures/decoycheck.sqlite` & `msstitch-3.9/tests/fixtures/decoycheck.sqlite`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3030001, file counter 4, database pages 5, cookie 0x3, schema 4, UTF-8, version-valid-for 4*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
 00000010: 1000 0101 0040 2020 0000 0004 0000 0005  .....@  ........
 00000020: 0000 0000 0000 0000 0000 0003 0000 0004  ................
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000060: 002e 3bf1 0d0f f800 040e 7a00 0f55 0fb5  ..;.......z..U..
+00000060: 002e 4b90 0d0f f800 040e 7a00 0f55 0fb5  ..K.......z..U..
 00000070: 0ee5 0e7a 0000 0000 0000 0000 0000 0000  ...z............
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `msstitch-3.8/tests/fixtures/ensg.txt` & `msstitch-3.9/tests/fixtures/isosum_charge_column.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,4 @@
-Gene ID	Q-score best peptide	q-value	MS1 precursor area	tmt10plex_126	tmt10plex_127N	tmt10plex_127C	tmt10plex_128N	tmt10plex_128C	tmt10plex_129N	tmt10plex_129C	tmt10plex_130N	tmt10plex_130C	tmt10plex_131	tmt10plex_126 - # quanted PSMs	tmt10plex_127N - # quanted PSMs	tmt10plex_127C - # quanted PSMs	tmt10plex_128N - # quanted PSMs	tmt10plex_128C - # quanted PSMs	tmt10plex_129N - # quanted PSMs	tmt10plex_129C - # quanted PSMs	tmt10plex_130N - # quanted PSMs	tmt10plex_130C - # quanted PSMs	tmt10plex_131 - # quanted PSMs	Amount fully quanted PSMs
-ENSG00000126261.13	7.999999999999999	0.0	8095731.0	1.0	1.2359360839246762	1.1405947721862797	1.4652434405725345	1.0278512732077358	1.396473384597946	1.0548623651578304	1.4948682144114882	0.8733542268267885	1.4550440035199355	1	1	1	1	1	1	1	1	1	1	1
-ENSG00000135269.18	7.999999999999999	0.0	16384178.0	1.0	1.5749411122684844	1.4801401385395023	1.2723931095939272	1.5005430209908905	1.4992867983052334	1.519476194483368	1.5452278657214784	0.8974947303309756	1.7366253884050227	1	1	1	1	1	1	1	1	1	1	1
-ENSG00000172465.14	7.999999999999999	0.0	19733054.0	1.0	1.1759695997636326	1.4757020623286972	0.6931415087509671	1.279736026426695	1.0150432628841837	1.2593732138321116	1.164303141716977	0.41253581605784606	1.2155145826197205	1	1	1	1	1	1	1	1	1	1	1
-ENSG00000182199.11	7.999999999999999	0.0	8726338.0	1.0	1.2105849212222934	1.0114795734233633	1.223153937730436	1.0923380006794583	1.1638322219153217	1.189765201917497	1.4463540709273641	0.8449969618107853	1.3890322338491508	1	1	1	1	1	1	1	1	1	1	1
-ENSG00000196914.9	7.999999999999999	0.0	22179466.0	1.0	1.1801089545045167	1.3342830672140233	1.6495462597929191	1.2919637007834335	1.2841778211941837	1.565066461989324	1.7498820908617507	1.232397296295004	1.7563021626797224	1	1	1	1	1	1	1	1	1	1	1
+Charge	tmt10plex_126	tmt10plex_127N	tmt10plex_127C	tmt10plex_128N	tmt10plex_128C	tmt10plex_129N	tmt10plex_129C	tmt10plex_130N	tmt10plex_130C	tmt10plex_131	tmt10plex_126 - # quanted PSMs	tmt10plex_127N - # quanted PSMs	tmt10plex_127C - # quanted PSMs	tmt10plex_128N - # quanted PSMs	tmt10plex_128C - # quanted PSMs	tmt10plex_129N - # quanted PSMs	tmt10plex_129C - # quanted PSMs	tmt10plex_130N - # quanted PSMs	tmt10plex_130C - # quanted PSMs	tmt10plex_131 - # quanted PSMs	Amount fully quanted PSMs
+3	1.0	1.0070583611053587	1.1344827674569458	1.1721210873676493	1.057945860427753	1.2212781960770507	1.1219598012652383	1.3465117166180551	0.8015702871316375	1.3783041939638854	17	17	17	17	17	17	17	17	17	17	17
+4	1.0	0.734347408305429	1.0916403215725714	1.151906429762225	0.6880471236094923	0.8298124788037313	0.8288855278049566	1.1081674014706475	0.6000865067639649	1.1280615208298412	1	1	1	1	1	1	1	1	1	1	1
+2	1.0	1.117292795619189	1.1706355115449816	1.2318576862959005	1.1287379502776242	1.393852677451718	1.3098108591920878	1.5019626208116659	0.7812796956137699	1.4394557969455588	59	59	59	59	59	59	59	59	59	59	59
```

### Comparing `msstitch-3.8/tests/fixtures/few_spec_timstof.mzid` & `msstitch-3.9/tests/fixtures/few_spec_timstof.mzid`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/fixtures/few_spec_timstof.tsv` & `msstitch-3.9/tests/fixtures/few_spec_timstof.tsv`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/fixtures/few_spec_timstof.tsv_fdr.tsv` & `msstitch-3.9/tests/fixtures/few_spec_timstof.tsv_fdr.tsv`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#SpecFile	SpecID	ScanNum	FragMethod	Precursor	IsotopeError	PrecursorError(ppm)	Charge	Peptide	Protein	DeNovoScore	MSGFScore	SpecEValue	EValue	percolator svm-score	PSM q-value	peptide q-value	TD
-few_spec_timstof.mzML	merged=22811 frame=8406 scanStart=648 scanEnd=672	-1	CID	620.3093	2	-6.2054744	2	+229.163SSWSRDDR	decoy_ENSP00000262056.9(pre=R,post=R);decoy_ENSP00000388806.3(pre=R,post=R);decoy_ENSP00000412530.3(pre=R,post=R)	62	-13	1.1750637E-4	25.623674	-1.0	0.3333333333333333	0.3333333333333333	decoy
-few_spec_timstof.mzML	merged=22829 frame=8410 scanStart=749 scanEnd=773	-1	CID	497.27274	0	-7.9166546	2	+229.163C+57.021SSVRR	ENSP00000435168.1(pre=R,post=I)	27	-9	2.5683644E-4	55.007175	-0.079	0.0	0.0	target
-few_spec_timstof.mzML	merged=22798 frame=8403 scanStart=746 scanEnd=770	-1	CID	440.71924	-1	-0.2790486	2	+229.163SGGM+15.995ER	ENSP00000340466.4(pre=R,post=P);ENSP00000435306.1(pre=R,post=P)	33	-21	6.0965033E-4	130.57002	0.0	0.0	0.0	target
-few_spec_timstof.mzML	merged=22797 frame=8403 scanStart=676 scanEnd=700	-1	CID	590.7842	1	1.3976825	2	+229.163DC+57.021SC+57.021RPR	decoy_ENSP00000368678.2(pre=R,post=G);decoy_ENSP00000484607.1(pre=R,post=G)	24	-38	0.0015428594	333.95654	-1.65	0.6666666666666666	0.6666666666666666	decoy
-few_spec_timstof.mzML	merged=22813 frame=8406 scanStart=736 scanEnd=760	-1	CID	498.7396	-1	-6.9095135	2	+229.163M+15.995TDTER	ENSP00000426648.1(pre=R,post=D);ENSP00000305810.2(pre=R,post=D);msstitch_fake_onlypeptide(pre=R,post=D)	9	-30	0.0019348329	414.38702	-0.995	0.0	0.0	target
-few_spec_timstof.mzML	merged=22801 frame=8404 scanStart=664 scanEnd=688	-1	CID	584.2722	-1	-5.168282	2	+229.163SSAEDQM+15.995R	ENSP00000396024.1(pre=K,post=M)	44	-36	0.0020030215	436.78287	-1.734	0.4	0.4	target
-few_spec_timstof.mzML	merged=22792 frame=8402 scanStart=739 scanEnd=763	-1	CID	542.2691	-1	4.4398994	2	+229.163YEC+57.021RDI	ENSP00000355751.3(pre=K,post=-);ENSP00000482784.1(pre=K,post=-)	25	-44	0.0033305485	713.31024	-1.733	0.5	0.5	target
-few_spec_timstof.mzML	merged=22794 frame=8402 scanStart=849 scanEnd=873	-1	CID	395.7153	-1	7.3145256	2	+229.163EGGSGR	ENSP00000384018.1(pre=K,post=A);ENSP00000384202.1(pre=K,post=A);ENSP00000400281.2(pre=K,post=A);ENSP00000385618.3(pre=K,post=A);ENSP00000348551.4(pre=K,post=A)	5	-20	0.006616151	1416.9943	-1.775	0.3333333333333333	0.3333333333333333	target
-few_spec_timstof.mzML	merged=22830 frame=8410 scanStart=800 scanEnd=824	-1	CID	503.2431	0	-7.4588885	3	+229.163ASSPEMDISADR	ENSP00000396024.1(pre=K,post=V)	55	-46	0.013979914	3108.252	-4.206	0.2857142857142857	0.2857142857142857	target
-few_spec_timstof.mzML	merged=22627 frame=8367 scanStart=566 scanEnd=590	-1	CID	730.30774	2	-7.0269885	2	+229.163DNYELDEDTD	ENSP00000372327.2(pre=K,post=-);ENSP00000372324.2(pre=K,post=-);ENSP00000479904.1(pre=K,post=-)	60	-88	0.015379414	3389.6074	-5.67	0.25	0.25	target
+#SpecFile	SpecID	ScanNum	FragMethod	Precursor	IsotopeError	PrecursorError(ppm)	Charge	Peptide	Protein	DeNovoScore	MSGFScore	SpecEValue	EValue	percolator svm-score	PSM q-value	PSM PEP	peptide PEP	peptide q-value	TD
+few_spec_timstof.mzML	merged=22811 frame=8406 scanStart=648 scanEnd=672	-1	CID	620.3093	2	-6.2054744	2	+229.163SSWSRDDR	decoy_ENSP00000262056.9(pre=R,post=R);decoy_ENSP00000388806.3(pre=R,post=R);decoy_ENSP00000412530.3(pre=R,post=R)	62	-13	1.1750637E-4	25.623674	-1.0	0.375	0.7368	0.7368	0.375	decoy
+few_spec_timstof.mzML	merged=22829 frame=8410 scanStart=749 scanEnd=773	-1	CID	497.27274	0	-7.9166546	2	+229.163C+57.021SSVRR	ENSP00000435168.1(pre=R,post=I)	27	-9	2.5683644E-4	55.007175	-0.079	0.3333	0.0643	0.0643	0.3333	target
+few_spec_timstof.mzML	merged=22798 frame=8403 scanStart=746 scanEnd=770	-1	CID	440.71924	-1	-0.2790486	2	+229.163SGGM+15.995ER	ENSP00000340466.4(pre=R,post=P);ENSP00000435306.1(pre=R,post=P)	33	-21	6.0965033E-4	130.57002	0.0	0.3333333	0.04830973	0.04830973	0.3333333	target
+few_spec_timstof.mzML	merged=22797 frame=8403 scanStart=676 scanEnd=700	-1	CID	590.7842	1	1.3976825	2	+229.163DC+57.021SC+57.021RPR	decoy_ENSP00000368678.2(pre=R,post=G);decoy_ENSP00000484607.1(pre=R,post=G)	24	-38	0.0015428594	333.95654	-1.65	0.375	0.7368	0.7368	0.375	decoy
+few_spec_timstof.mzML	merged=22813 frame=8406 scanStart=736 scanEnd=760	-1	CID	498.7396	-1	-6.9095135	2	+229.163M+15.995TDTER	ENSP00000426648.1(pre=R,post=D);ENSP00000305810.2(pre=R,post=D);msstitch_fake_onlypeptide(pre=R,post=D)	9	-30	0.0019348329	414.38702	-0.995	0.3333	0.7338	0.7338	0.3333	target
+few_spec_timstof.mzML	merged=22801 frame=8404 scanStart=664 scanEnd=688	-1	CID	584.2722	-1	-5.168282	2	+229.163SSAEDQM+15.995R	ENSP00000396024.1(pre=K,post=M)	44	-36	0.0020030215	436.78287	-1.734	0.375	0.7368	0.7368	0.375	target
+few_spec_timstof.mzML	merged=22792 frame=8402 scanStart=739 scanEnd=763	-1	CID	542.2691	-1	4.4398994	2	+229.163YEC+57.021RDI	ENSP00000355751.3(pre=K,post=-);ENSP00000482784.1(pre=K,post=-)	25	-44	0.0033305485	713.31024	-1.733	0.375	0.7368	0.7368	0.375	target
+few_spec_timstof.mzML	merged=22794 frame=8402 scanStart=849 scanEnd=873	-1	CID	395.7153	-1	7.3145256	2	+229.163EGGSGR	ENSP00000384018.1(pre=K,post=A);ENSP00000384202.1(pre=K,post=A);ENSP00000400281.2(pre=K,post=A);ENSP00000385618.3(pre=K,post=A);ENSP00000348551.4(pre=K,post=A)	5	-20	0.006616151	1416.9943	-1.775	0.375	0.7368	0.7368	0.375	target
+few_spec_timstof.mzML	merged=22830 frame=8410 scanStart=800 scanEnd=824	-1	CID	503.2431	0	-7.4588885	3	+229.163ASSPEMDISADR	ENSP00000396024.1(pre=K,post=V)	55	-46	0.013979914	3108.252	-4.206	0.375	0.7368	0.7368	0.375	target
+few_spec_timstof.mzML	merged=22627 frame=8367 scanStart=566 scanEnd=590	-1	CID	730.30774	2	-7.0269885	2	+229.163DNYELDEDTD	ENSP00000372327.2(pre=K,post=-);ENSP00000372324.2(pre=K,post=-);ENSP00000479904.1(pre=K,post=-)	60	-88	0.015379414	3389.6074	-5.67	0.375	0.7368	0.7368	0.375	target
```

### Comparing `msstitch-3.8/tests/fixtures/perco.xml` & `msstitch-3.9/tests/fixtures/perco.xml_h0.xml`

 * *Files 24% similar despite different names*

#### Comparing `msstitch-3.8/tests/fixtures/perco.xml` & `msstitch-3.9/tests/fixtures/perco.xml_h0.xml`

```diff
@@ -5,702 +5,495 @@
     <other_command_line/>
     <pi_0_psms>1</pi_0_psms>
     <pi_0_peptides>1</pi_0_peptides>
     <psms_qlevel>0</psms_qlevel>
     <peptides_qlevel>0</peptides_qlevel>
   </process_info>
   <psms>
-    <psm p:psm_id="few_spectra_SII_36_1_9872_2_1" p:decoy="false">
+    <psm p:psm_id="few_spectra_SII_24_1_10023_3_1" p:decoy="false">
       <svm_score>0.000000</svm_score>
-      <q_value>1.000000e+00</q_value>
-      <pep>4.829196e-01</pep>
-      <exp_mass>703.8800</exp_mass>
-      <calc_mass>703.880</calc_mass>
-      <peptide_seq n="R" c="R" seq="[UNIMOD:737]ASNEDGDIK[UNIMOD:737]"/>
-      <protein_id>ENSP00000246548.3</protein_id>
-      <protein_id>ENSP00000467433.2</protein_id>
-      <protein_id>ENSP00000437484.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_32_1_9868_2_1" p:decoy="true">
-      <svm_score>-0.659</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>571.8230</exp_mass>
-      <calc_mass>572.322</calc_mass>
-      <peptide_seq n="K" c="L" seq="[UNIMOD:737]PDEVWLR"/>
-      <protein_id>decoy_ENSP00000412465.1</protein_id>
-      <protein_id>decoy_ENSP00000297954.4</protein_id>
-      <protein_id>decoy_ENSP00000415038.1</protein_id>
-      <protein_id>decoy_ENSP00000378860.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_34_1_9870_2_1" p:decoy="true">
-      <svm_score>-0.880</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>554.2870</exp_mass>
-      <calc_mass>554.287</calc_mass>
-      <peptide_seq n="K" c="E" seq="[UNIMOD:737]ENELM[UNIMOD:35]AR"/>
-      <protein_id>decoy_ENSP00000353408.5</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_19_1_9855_2_1" p:decoy="true">
-      <svm_score>-0.882</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>446.2420</exp_mass>
-      <calc_mass>446.747</calc_mass>
-      <peptide_seq n="K" c="P" seq="[UNIMOD:737]QVM[UNIMOD:35]GGR"/>
-      <protein_id>decoy_ENSP00000377681.3</protein_id>
-      <protein_id>decoy_ENSP00000348578.3</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_15_1_9851_2_1" p:decoy="true">
-      <svm_score>-0.889</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>555.3180</exp_mass>
-      <calc_mass>555.822</calc_mass>
-      <peptide_seq n="R" c="N" seq="[UNIMOD:737]FFRQQR"/>
-      <protein_id>decoy_ENSP00000358992.1</protein_id>
-      <protein_id>decoy_ENSP00000359002.3</protein_id>
-      <protein_id>decoy_ENSP00000358994.3</protein_id>
-      <protein_id>decoy_ENSP00000478013.1</protein_id>
-      <protein_id>decoy_ENSP00000358998.4</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_25_1_9861_2_1" p:decoy="false">
-      <svm_score>-0.907</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>699.8650</exp_mass>
-      <calc_mass>699.859</calc_mass>
-      <peptide_seq n="R" c="I" seq="[UNIMOD:737]EIPYTFEDR"/>
-      <protein_id>ENSP00000333667.3</protein_id>
-      <protein_id>ENSP00000452315.1</protein_id>
-      <protein_id>ENSP00000450930.1</protein_id>
-      <protein_id>ENSP00000406881.3</protein_id>
-      <protein_id>ENSP00000452419.1</protein_id>
-      <protein_id>ENSP00000413770.3</protein_id>
-      <protein_id>ENSP00000450490.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_31_1_9867_2_1" p:decoy="true">
-      <svm_score>-0.934</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>545.8300</exp_mass>
-      <calc_mass>545.327</calc_mass>
-      <peptide_seq n="R" c="R" seq="[UNIMOD:737]LTTEVAAR"/>
-      <protein_id>decoy_ENSP00000271636.7</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_38_1_9874_2_1" p:decoy="true">
-      <svm_score>-0.935</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>490.2570</exp_mass>
-      <calc_mass>490.253</calc_mass>
-      <peptide_seq n="K" c="L" seq="[UNIMOD:737]GPNC[UNIMOD:4]FR"/>
-      <protein_id>decoy_ENSP00000432568.1</protein_id>
-      <protein_id>decoy_ENSP00000433593.1</protein_id>
-      <protein_id>decoy_ENSP00000311489.2</protein_id>
-      <protein_id>decoy_ENSP00000480692.1</protein_id>
-      <protein_id>decoy_ENSP00000482000.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_3_1_9839_2_1" p:decoy="true">
-      <svm_score>-0.942</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>472.7330</exp_mass>
-      <calc_mass>473.233</calc_mass>
-      <peptide_seq n="K" c="K" seq="[UNIMOD:737]SDSHDR"/>
-      <protein_id>decoy_ENSP00000359042.4</protein_id>
-      <protein_id>decoy_ENSP00000359038.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_18_1_9854_2_1" p:decoy="false">
-      <svm_score>-0.942</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>575.3290</exp_mass>
-      <calc_mass>575.328</calc_mass>
-      <peptide_seq n="R" c="L" seq="[UNIMOD:737]WQQFRR"/>
-      <protein_id>ENSP00000432568.1</protein_id>
-      <protein_id>ENSP00000433593.1</protein_id>
-      <protein_id>ENSP00000311489.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_33_1_9869_3_1" p:decoy="false">
-      <svm_score>-0.952</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>506.9570</exp_mass>
-      <calc_mass>507.294</calc_mass>
-      <peptide_seq n="K" c="L" seq="[UNIMOD:737]MLQK[UNIMOD:737]EQER"/>
-      <protein_id>ENSP00000349056.3</protein_id>
-      <protein_id>ENSP00000380942.2</protein_id>
-      <protein_id>ENSP00000432984.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_12_1_9848_2_1" p:decoy="true">
-      <svm_score>-0.965</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>540.2700</exp_mass>
-      <calc_mass>540.271</calc_mass>
-      <peptide_seq n="R" c="G" seq="[UNIMOD:737]SC[UNIMOD:4]DELAR"/>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_29_1_9865_2_1" p:decoy="true">
-      <svm_score>-1.000</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>710.3420</exp_mass>
-      <calc_mass>710.342</calc_mass>
-      <peptide_seq n="R" c="S" seq="[UNIMOD:737]YQEYM[UNIMOD:35]LGDR"/>
-      <protein_id>decoy_ENSP00000425587.1</protein_id>
-      <protein_id>decoy_ENSP00000424404.1</protein_id>
-      <protein_id>decoy_ENSP00000323377.5</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_8_1_9844_3_1" p:decoy="false">
-      <svm_score>-1.051</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>856.4240</exp_mass>
-      <calc_mass>856.757</calc_mass>
-      <peptide_seq n="R" c="R" seq="[UNIMOD:737]NLSNEEMIQAADELEEM[UNIMOD:35]K[UNIMOD:737]"/>
-      <protein_id>ENSP00000361709.3</protein_id>
-      <protein_id>ENSP00000361708.3</protein_id>
-      <protein_id>ENSP00000361707.3</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_7_1_9843_2_1" p:decoy="true">
-      <svm_score>-1.055</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>693.3060</exp_mass>
-      <calc_mass>693.303</calc_mass>
-      <peptide_seq n="K" c="A" seq="[UNIMOD:737]AGDETNM[UNIMOD:35]SC[UNIMOD:4]R"/>
-      <protein_id>decoy_ENSP00000323687.6</protein_id>
-      <protein_id>decoy_ENSP00000467623.1</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_14_1_9850_2_1" p:decoy="true">
-      <svm_score>-1.065</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>478.7870</exp_mass>
-      <calc_mass>478.283</calc_mass>
-      <peptide_seq n="R" c="P" seq="[UNIMOD:737]IPPPM[UNIMOD:35]R"/>
-      <protein_id>decoy_ENSP00000474437.1</protein_id>
-      <protein_id>decoy_ENSP00000363745.3</protein_id>
-      <protein_id>decoy_ENSP00000363741.1</protein_id>
-      <protein_id>decoy_ENSP00000304405.6</protein_id>
-      <protein_id>decoy_ENSP00000475760.1</protein_id>
-      <protein_id>decoy_ENSP00000392799.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_20_1_9856_2_1" p:decoy="true">
-      <svm_score>-1.079</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>609.3370</exp_mass>
-      <calc_mass>608.330</calc_mass>
-      <peptide_seq n="K" c="Y" seq="[UNIMOD:737]DAEATPGVAR"/>
-      <protein_id>decoy_ENSP00000396301.2</protein_id>
-      <protein_id>decoy_ENSP00000422641.1</protein_id>
-      <protein_id>decoy_ENSP00000426764.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_17_1_9853_2_1" p:decoy="false">
-      <svm_score>-1.083</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>486.2450</exp_mass>
-      <calc_mass>486.245</calc_mass>
-      <peptide_seq n="-" c="M" seq="[UNIMOD:737]MSEYGR"/>
-      <protein_id>msstitch_fake_onlypeptide</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_42_1_9878_2_1" p:decoy="true">
-      <svm_score>-1.090</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>788.9110</exp_mass>
-      <calc_mass>789.417</calc_mass>
-      <peptide_seq n="K" c="L" seq="[UNIMOD:737]M[UNIMOD:35]DQSLELNRAR"/>
-      <protein_id>decoy_ENSP00000281394.4</protein_id>
-      <protein_id>decoy_ENSP00000294952.8</protein_id>
-      <protein_id>decoy_ENSP00000415696.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_37_1_9873_2_1" p:decoy="true">
-      <svm_score>-1.128</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>691.3740</exp_mass>
-      <calc_mass>690.367</calc_mass>
-      <peptide_seq n="K" c="E" seq="[UNIMOD:737]MRAESSVQSR"/>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_43_1_9879_2_1" p:decoy="true">
-      <svm_score>-1.150</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>659.3520</exp_mass>
-      <calc_mass>659.859</calc_mass>
-      <peptide_seq n="R" c="Q" seq="[UNIMOD:737]QMREQLER"/>
-      <protein_id>decoy_ENSP00000384202.1</protein_id>
-      <protein_id>decoy_ENSP00000400281.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_45_1_9881_2_1" p:decoy="true">
-      <svm_score>-1.150</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>691.3740</exp_mass>
-      <calc_mass>690.367</calc_mass>
-      <peptide_seq n="K" c="E" seq="[UNIMOD:737]MRAESSVQSR"/>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_22_1_9858_2_1" p:decoy="false">
-      <svm_score>-1.166</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>1061.0500</exp_mass>
-      <calc_mass>1061.550</calc_mass>
-      <peptide_seq n="R" c="M" seq="[UNIMOD:737]AMWSLRERSQVSSEAR"/>
-      <protein_id>sp|Q9P219|DAPLE_HUMAN</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_27_1_9863_2_1" p:decoy="false">
-      <svm_score>-1.174</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>665.3180</exp_mass>
-      <calc_mass>665.319</calc_mass>
-      <peptide_seq n="R" c="K" seq="[UNIMOD:737]SEYM[UNIMOD:35]EGNVR"/>
-      <protein_id>msstitch_fake_gene_anpep</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_5_1_9841_2_1" p:decoy="true">
-      <svm_score>-1.211</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>990.4870</exp_mass>
-      <calc_mass>989.484</calc_mass>
-      <peptide_seq n="K" c="R" seq="[UNIMOD:737]EEERMREREEAER"/>
-      <protein_id>decoy_ENSP00000354826.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_28_1_9864_3_1" p:decoy="false">
-      <svm_score>-1.224</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>720.3350</exp_mass>
-      <calc_mass>720.334</calc_mass>
-      <peptide_seq n="K" c="K" seq="[UNIMOD:737]C[UNIMOD:4]GQEEHDVLLSNEEDR"/>
-      <protein_id>ENSP00000350937.4</protein_id>
-      <protein_id>ENSP00000377121.2</protein_id>
-      <p_value>0.000e+00</p_value>
-    </psm>
-    <psm p:psm_id="few_spectra_SII_13_1_9849_2_1" p:decoy="true">
-      <svm_score>-1.299</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>739.4090</exp_mass>
-      <calc_mass>738.408</calc_mass>
-      <peptide_seq n="K" c="N" seq="[UNIMOD:737]LMQLESELQR"/>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
+      <q_value>2.000000e-01</q_value>
+      <pep>2.864478e-02</pep>
+      <exp_mass>819.7480</exp_mass>
+      <calc_mass>819.747</calc_mass>
+      <peptide_seq n="R" c="D" seq="[UNIMOD:737]SEEAHRAEQLQDAEEEK[UNIMOD:737]"/>
+      <protein_id>ENSP00000246024.2</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_16_1_10015_4_1" p:decoy="false">
+      <svm_score>-0.046</svm_score>
+      <q_value>2.000e-01</q_value>
+      <pep>3.378e-02</pep>
+      <exp_mass>615.3130</exp_mass>
+      <calc_mass>615.062</calc_mass>
+      <peptide_seq n="R" c="D" seq="[UNIMOD:737]SEEAHRAEQLQDAEEEK[UNIMOD:737]"/>
+      <protein_id>ENSP00000246024.2</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_30_1_10029_3_1" p:decoy="false">
+      <svm_score>-0.097</svm_score>
+      <q_value>2.000e-01</q_value>
+      <pep>4.062e-02</pep>
+      <exp_mass>820.4150</exp_mass>
+      <calc_mass>819.747</calc_mass>
+      <peptide_seq n="R" c="D" seq="[UNIMOD:737]SEEAHRAEQLQDAEEEK[UNIMOD:737]"/>
+      <protein_id>ENSP00000246024.2</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_40_1_10039_2_1" p:decoy="false">
+      <svm_score>-0.432</svm_score>
+      <q_value>2.000e-01</q_value>
+      <pep>1.361e-01</pep>
+      <exp_mass>811.9460</exp_mass>
+      <calc_mass>811.444</calc_mass>
+      <peptide_seq n="R" c="A" seq="[UNIMOD:737]DSGTLQSQEAK[UNIMOD:737]"/>
+      <protein_id>ENSP00000363482.2</protein_id>
+      <protein_id>ENSP00000439811.1</protein_id>
+      <protein_id>ENSP00000442128.1</protein_id>
+      <protein_id>ENSP00000485513.1</protein_id>
+      <protein_id>ENSP00000352922.6</protein_id>
+      <protein_id>ENSP00000337541.5</protein_id>
+      <protein_id>ENSP00000344037.6</protein_id>
+      <protein_id>ENSP00000314417.7</protein_id>
+      <protein_id>ENSP00000282633.5</protein_id>
+      <protein_id>ENSP00000382277.2</protein_id>
+      <protein_id>ENSP00000481763.1</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_18_1_10017_2_1" p:decoy="false">
+      <svm_score>-0.841</svm_score>
+      <q_value>3.333e-01</q_value>
+      <pep>5.830e-01</pep>
+      <exp_mass>594.8490</exp_mass>
+      <calc_mass>594.847</calc_mass>
+      <peptide_seq n="R" c="S" seq="[UNIMOD:737]EEPLDK[UNIMOD:737]"/>
+      <protein_id>ENSP00000252999.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_237_1_10236_2_1" p:decoy="false">
+      <svm_score>-0.903</svm_score>
+      <q_value>4.857e-01</q_value>
+      <pep>7.255e-01</pep>
+      <exp_mass>540.7800</exp_mass>
+      <calc_mass>541.283</calc_mass>
+      <peptide_seq n="R" c="D" seq="[UNIMOD:737]DDRSFGR"/>
+      <protein_id>ENSP00000262056.9</protein_id>
+      <protein_id>ENSP00000388806.3</protein_id>
+      <protein_id>ENSP00000412530.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_229_1_10228_2_1" p:decoy="false">
+      <svm_score>-0.912</svm_score>
+      <q_value>4.857e-01</q_value>
+      <pep>7.487e-01</pep>
+      <exp_mass>719.3880</exp_mass>
+      <calc_mass>719.890</calc_mass>
+      <peptide_seq n="R" c="L" seq="[UNIMOD:737]ETK[UNIMOD:737]ATDC[UNIMOD:4]R"/>
+      <protein_id>ENSP00000363482.2</protein_id>
+      <protein_id>ENSP00000439811.1</protein_id>
+      <protein_id>ENSP00000442128.1</protein_id>
+      <protein_id>ENSP00000485513.1</protein_id>
+      <protein_id>ENSP00000337541.5</protein_id>
+      <protein_id>ENSP00000344037.6</protein_id>
+      <protein_id>ENSP00000314417.7</protein_id>
+      <protein_id>ENSP00000282633.5</protein_id>
+      <protein_id>ENSP00000481763.1</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_246_1_10245_2_1" p:decoy="false">
+      <svm_score>-0.920</svm_score>
+      <q_value>4.857e-01</q_value>
+      <pep>7.701e-01</pep>
+      <exp_mass>455.7370</exp_mass>
+      <calc_mass>455.235</calc_mass>
+      <peptide_seq n="K" c="D" seq="[UNIMOD:737]FEGGDR"/>
+      <protein_id>ENSP00000286091.5</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_83_1_10082_3_1" p:decoy="false">
+      <svm_score>-0.921</svm_score>
+      <q_value>4.857e-01</q_value>
+      <pep>7.731e-01</pep>
+      <exp_mass>450.2330</exp_mass>
+      <calc_mass>450.567</calc_mass>
+      <peptide_seq n="R" c="G" seq="[UNIMOD:737]ADFNRGGGNGR"/>
+      <protein_id>ENSP00000254108.7</protein_id>
+      <protein_id>ENSP00000369594.3</protein_id>
+      <protein_id>ENSP00000455282.1</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_128_1_10127_3_1" p:decoy="false">
+      <svm_score>-0.957</svm_score>
+      <q_value>5.500e-01</q_value>
+      <pep>8.749e-01</pep>
+      <exp_mass>558.6050</exp_mass>
+      <calc_mass>558.935</calc_mass>
+      <peptide_seq n="K" c="E" seq="[UNIMOD:737]M[UNIMOD:35]ERERENYM[UNIMOD:35]R"/>
+      <protein_id>ENSP00000294671.2</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_175_1_10174_3_1" p:decoy="false">
+      <svm_score>-1.042</svm_score>
+      <q_value>8.070e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>612.9500</exp_mass>
+      <calc_mass>612.621</calc_mass>
+      <peptide_seq n="R" c="S" seq="[UNIMOD:737]SQEC[UNIMOD:4]YFDPELYR"/>
+      <protein_id>ENSP00000258341.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_206_1_10205_2_1" p:decoy="false">
+      <svm_score>-1.058</svm_score>
+      <q_value>8.167e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>527.2600</exp_mass>
+      <calc_mass>526.256</calc_mass>
+      <peptide_seq n="R" c="A" seq="[UNIMOD:737]EC[UNIMOD:4]GDVSR"/>
+      <protein_id>ENSP00000361711.1</protein_id>
+      <protein_id>ENSP00000361710.5</protein_id>
+      <protein_id>ENSP00000243286.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_116_1_10115_3_1" p:decoy="false">
+      <svm_score>-1.109</svm_score>
+      <q_value>8.676e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>750.0080</exp_mass>
+      <calc_mass>749.668</calc_mass>
+      <peptide_seq n="R" c="C" seq="[UNIMOD:737]TGQC[UNIMOD:4]EC[UNIMOD:4]QPGITGQHC[UNIMOD:4]ER"/>
+      <protein_id>ENSP00000258341.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_224_1_10223_3_1" p:decoy="false">
+      <svm_score>-1.111</svm_score>
+      <q_value>8.676e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>600.2990</exp_mass>
+      <calc_mass>599.629</calc_mass>
+      <peptide_seq n="R" c="G" seq="[UNIMOD:737]VPPTAC[UNIMOD:4]C[UNIMOD:4]GHSTQPR"/>
+      <protein_id>ENSP00000297954.4</protein_id>
       <p_value>0.000e+00</p_value>
     </psm>
-    <psm p:psm_id="few_spectra_SII_23_1_9859_3_1" p:decoy="false">
-      <svm_score>-1.456</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>720.6680</exp_mass>
-      <calc_mass>720.003</calc_mass>
-      <peptide_seq n="R" c="S" seq="[UNIMOD:737]GAVMEQGTSSSM[UNIMOD:35]TAESSPR"/>
-      <protein_id>ENSP00000297954.4</protein_id>
-      <protein_id>ENSP00000415038.1</protein_id>
-      <protein_id>ENSP00000378860.2</protein_id>
+    <psm p:psm_id="few_spectra_SII_130_1_10129_2_1" p:decoy="false">
+      <svm_score>-1.115</svm_score>
+      <q_value>8.676e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>759.8720</exp_mass>
+      <calc_mass>759.866</calc_mass>
+      <peptide_seq n="-" c="G" seq="[UNIMOD:737]MEQAPNM[UNIMOD:35]AEPR"/>
+      <protein_id>ENSP00000271636.7</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_77_1_10076_2_1" p:decoy="false">
+      <svm_score>-1.133</svm_score>
+      <q_value>8.889e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>888.9430</exp_mass>
+      <calc_mass>889.439</calc_mass>
+      <peptide_seq n="R" c="K" seq="[UNIMOD:737]EC[UNIMOD:4]GDVSRAQEELR"/>
+      <protein_id>ENSP00000361711.1</protein_id>
+      <protein_id>ENSP00000361710.5</protein_id>
+      <protein_id>ENSP00000243286.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_108_1_10107_2_1" p:decoy="false">
+      <svm_score>-1.137</svm_score>
+      <q_value>8.904e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>898.4210</exp_mass>
+      <calc_mass>898.426</calc_mass>
+      <peptide_seq n="R" c="G" seq="[UNIMOD:737]GGPM[UNIMOD:35]GRGGYGGGGSGGGGR"/>
+      <protein_id>ENSP00000254108.7</protein_id>
+      <protein_id>ENSP00000369594.3</protein_id>
+      <protein_id>ENSP00000455282.1</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_148_1_10147_3_1" p:decoy="false">
+      <svm_score>-1.185</svm_score>
+      <q_value>9.351e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>639.9810</exp_mass>
+      <calc_mass>639.650</calc_mass>
+      <peptide_seq n="K" c="H" seq="[UNIMOD:737]FDGHRC[UNIMOD:4]AGQQQDIR"/>
+      <protein_id>ENSP00000380189.3</protein_id>
+      <protein_id>ENSP00000366204.2</protein_id>
+      <protein_id>ENSP00000247153.3</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_31_1_10030_2_1" p:decoy="false">
+      <svm_score>-1.196</svm_score>
+      <q_value>9.351e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>732.8540</exp_mass>
+      <calc_mass>731.857</calc_mass>
+      <peptide_seq n="R" c="G" seq="[UNIMOD:737]M[UNIMOD:35]DC[UNIMOD:4]YSGQK[UNIMOD:737]"/>
+      <protein_id>ENSP00000261978.4</protein_id>
+      <protein_id>ENSP00000452110.1</protein_id>
+      <protein_id>ENSP00000451477.1</protein_id>
+      <p_value>0.000e+00</p_value>
+    </psm>
+    <psm p:psm_id="few_spectra_SII_244_1_10243_3_1" p:decoy="false">
+      <svm_score>-1.212</svm_score>
+      <q_value>9.351e-01</q_value>
+      <pep>1.000e+00</pep>
+      <exp_mass>755.0220</exp_mass>
+      <calc_mass>754.358</calc_mass>
+      <peptide_seq n="K" c="R" seq="[UNIMOD:737]TC[UNIMOD:4]NTNPHLNALSTDSAC[UNIMOD:4]R"/>
+      <protein_id>ENSP00000277165.5</protein_id>
+      <protein_id>ENSP00000412440.1</protein_id>
       <p_value>0.000e+00</p_value>
     </psm>
   </psms>
   <peptides>
-    <peptide p:peptide_id="[UNIMOD:737]ASNEDGDIK[UNIMOD:737]" p:decoy="false">
+    <peptide p:peptide_id="[UNIMOD:737]SEEAHRAEQLQDAEEEK[UNIMOD:737]" p:decoy="false">
       <svm_score>0.000000</svm_score>
-      <q_value>1.000000e+00</q_value>
-      <pep>6.614077e-01</pep>
-      <exp_mass>703.8800</exp_mass>
-      <calc_mass>703.880</calc_mass>
-      <protein_id>ENSP00000246548.3</protein_id>
-      <protein_id>ENSP00000467433.2</protein_id>
-      <protein_id>ENSP00000437484.1</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_36_1_9872_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]PDEVWLR" p:decoy="true">
-      <svm_score>-0.659</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>571.8230</exp_mass>
-      <calc_mass>572.322</calc_mass>
-      <protein_id>decoy_ENSP00000412465.1</protein_id>
-      <protein_id>decoy_ENSP00000297954.4</protein_id>
-      <protein_id>decoy_ENSP00000415038.1</protein_id>
-      <protein_id>decoy_ENSP00000378860.2</protein_id>
+      <q_value>2.500000e-01</q_value>
+      <pep>1.772279e-03</pep>
+      <exp_mass>819.7480</exp_mass>
+      <calc_mass>819.747</calc_mass>
+      <protein_id>ENSP00000246024.2</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_32_1_9868_2_1</psm_id>
+        <psm_id>few_spectra_SII_24_1_10023_3_1</psm_id>
+        <psm_id>few_spectra_SII_16_1_10015_4_1</psm_id>
+        <psm_id>few_spectra_SII_30_1_10029_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]ENELM[UNIMOD:35]AR" p:decoy="true">
-      <svm_score>-0.880</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>554.2870</exp_mass>
-      <calc_mass>554.287</calc_mass>
-      <protein_id>decoy_ENSP00000353408.5</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]DSGTLQSQEAK[UNIMOD:737]" p:decoy="false">
+      <svm_score>-0.432</svm_score>
+      <q_value>2.500e-01</q_value>
+      <pep>3.975e-02</pep>
+      <exp_mass>811.9460</exp_mass>
+      <calc_mass>811.444</calc_mass>
+      <protein_id>ENSP00000363482.2</protein_id>
+      <protein_id>ENSP00000439811.1</protein_id>
+      <protein_id>ENSP00000442128.1</protein_id>
+      <protein_id>ENSP00000485513.1</protein_id>
+      <protein_id>ENSP00000352922.6</protein_id>
+      <protein_id>ENSP00000337541.5</protein_id>
+      <protein_id>ENSP00000344037.6</protein_id>
+      <protein_id>ENSP00000314417.7</protein_id>
+      <protein_id>ENSP00000282633.5</protein_id>
+      <protein_id>ENSP00000382277.2</protein_id>
+      <protein_id>ENSP00000481763.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_34_1_9870_2_1</psm_id>
+        <psm_id>few_spectra_SII_40_1_10039_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]QVM[UNIMOD:35]GGR" p:decoy="true">
-      <svm_score>-0.882</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>446.2420</exp_mass>
-      <calc_mass>446.747</calc_mass>
-      <protein_id>decoy_ENSP00000377681.3</protein_id>
-      <protein_id>decoy_ENSP00000348578.3</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]EEPLDK[UNIMOD:737]" p:decoy="false">
+      <svm_score>-0.841</svm_score>
+      <q_value>3.846e-01</q_value>
+      <pep>5.539e-01</pep>
+      <exp_mass>594.8490</exp_mass>
+      <calc_mass>594.847</calc_mass>
+      <protein_id>ENSP00000252999.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_19_1_9855_2_1</psm_id>
+        <psm_id>few_spectra_SII_18_1_10017_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]FFRQQR" p:decoy="true">
-      <svm_score>-0.889</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>555.3180</exp_mass>
-      <calc_mass>555.822</calc_mass>
-      <protein_id>decoy_ENSP00000358992.1</protein_id>
-      <protein_id>decoy_ENSP00000359002.3</protein_id>
-      <protein_id>decoy_ENSP00000358994.3</protein_id>
-      <protein_id>decoy_ENSP00000478013.1</protein_id>
-      <protein_id>decoy_ENSP00000358998.4</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]DDRSFGR" p:decoy="false">
+      <svm_score>-0.903</svm_score>
+      <q_value>5.152e-01</q_value>
+      <pep>7.528e-01</pep>
+      <exp_mass>540.7800</exp_mass>
+      <calc_mass>541.283</calc_mass>
+      <protein_id>ENSP00000262056.9</protein_id>
+      <protein_id>ENSP00000388806.3</protein_id>
+      <protein_id>ENSP00000412530.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_15_1_9851_2_1</psm_id>
+        <psm_id>few_spectra_SII_237_1_10236_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]EIPYTFEDR" p:decoy="false">
-      <svm_score>-0.907</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>699.8650</exp_mass>
-      <calc_mass>699.859</calc_mass>
-      <protein_id>ENSP00000333667.3</protein_id>
-      <protein_id>ENSP00000452315.1</protein_id>
-      <protein_id>ENSP00000450930.1</protein_id>
-      <protein_id>ENSP00000406881.3</protein_id>
-      <protein_id>ENSP00000452419.1</protein_id>
-      <protein_id>ENSP00000413770.3</protein_id>
-      <protein_id>ENSP00000450490.1</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]ETK[UNIMOD:737]ATDC[UNIMOD:4]R" p:decoy="false">
+      <svm_score>-0.912</svm_score>
+      <q_value>5.152e-01</q_value>
+      <pep>7.850e-01</pep>
+      <exp_mass>719.3880</exp_mass>
+      <calc_mass>719.890</calc_mass>
+      <protein_id>ENSP00000363482.2</protein_id>
+      <protein_id>ENSP00000439811.1</protein_id>
+      <protein_id>ENSP00000442128.1</protein_id>
+      <protein_id>ENSP00000485513.1</protein_id>
+      <protein_id>ENSP00000337541.5</protein_id>
+      <protein_id>ENSP00000344037.6</protein_id>
+      <protein_id>ENSP00000314417.7</protein_id>
+      <protein_id>ENSP00000282633.5</protein_id>
+      <protein_id>ENSP00000481763.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_25_1_9861_2_1</psm_id>
+        <psm_id>few_spectra_SII_229_1_10228_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]LTTEVAAR" p:decoy="true">
-      <svm_score>-0.934</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>545.8300</exp_mass>
-      <calc_mass>545.327</calc_mass>
-      <protein_id>decoy_ENSP00000271636.7</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]FEGGDR" p:decoy="false">
+      <svm_score>-0.920</svm_score>
+      <q_value>5.152e-01</q_value>
+      <pep>8.153e-01</pep>
+      <exp_mass>455.7370</exp_mass>
+      <calc_mass>455.235</calc_mass>
+      <protein_id>ENSP00000286091.5</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_31_1_9867_2_1</psm_id>
+        <psm_id>few_spectra_SII_246_1_10245_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]GPNC[UNIMOD:4]FR" p:decoy="true">
-      <svm_score>-0.935</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>490.2570</exp_mass>
-      <calc_mass>490.253</calc_mass>
-      <protein_id>decoy_ENSP00000432568.1</protein_id>
-      <protein_id>decoy_ENSP00000433593.1</protein_id>
-      <protein_id>decoy_ENSP00000311489.2</protein_id>
-      <protein_id>decoy_ENSP00000480692.1</protein_id>
-      <protein_id>decoy_ENSP00000482000.1</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]ADFNRGGGNGR" p:decoy="false">
+      <svm_score>-0.921</svm_score>
+      <q_value>5.152e-01</q_value>
+      <pep>8.196e-01</pep>
+      <exp_mass>450.2330</exp_mass>
+      <calc_mass>450.567</calc_mass>
+      <protein_id>ENSP00000254108.7</protein_id>
+      <protein_id>ENSP00000369594.3</protein_id>
+      <protein_id>ENSP00000455282.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_38_1_9874_2_1</psm_id>
+        <psm_id>few_spectra_SII_83_1_10082_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]SDSHDR" p:decoy="true">
-      <svm_score>-0.942</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>472.7330</exp_mass>
-      <calc_mass>473.233</calc_mass>
-      <protein_id>decoy_ENSP00000359042.4</protein_id>
-      <protein_id>decoy_ENSP00000359038.1</protein_id>
+    <peptide p:peptide_id="[UNIMOD:737]M[UNIMOD:35]ERERENYM[UNIMOD:35]R" p:decoy="false">
+      <svm_score>-0.957</svm_score>
+      <q_value>5.789e-01</q_value>
+      <pep>9.698e-01</pep>
+      <exp_mass>558.6050</exp_mass>
+      <calc_mass>558.935</calc_mass>
+      <protein_id>ENSP00000294671.2</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_3_1_9839_2_1</psm_id>
+        <psm_id>few_spectra_SII_128_1_10127_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]WQQFRR" p:decoy="false">
-      <svm_score>-0.942</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]SQEC[UNIMOD:4]YFDPELYR" p:decoy="false">
+      <svm_score>-1.042</svm_score>
+      <q_value>8.364e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>575.3290</exp_mass>
-      <calc_mass>575.328</calc_mass>
-      <protein_id>ENSP00000432568.1</protein_id>
-      <protein_id>ENSP00000433593.1</protein_id>
-      <protein_id>ENSP00000311489.2</protein_id>
+      <exp_mass>612.9500</exp_mass>
+      <calc_mass>612.621</calc_mass>
+      <protein_id>ENSP00000258341.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_18_1_9854_2_1</psm_id>
+        <psm_id>few_spectra_SII_175_1_10174_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]MLQK[UNIMOD:737]EQER" p:decoy="false">
-      <svm_score>-0.952</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]EC[UNIMOD:4]GDVSR" p:decoy="false">
+      <svm_score>-1.058</svm_score>
+      <q_value>8.448e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>506.9570</exp_mass>
-      <calc_mass>507.294</calc_mass>
-      <protein_id>ENSP00000349056.3</protein_id>
-      <protein_id>ENSP00000380942.2</protein_id>
-      <protein_id>ENSP00000432984.1</protein_id>
+      <exp_mass>527.2600</exp_mass>
+      <calc_mass>526.256</calc_mass>
+      <protein_id>ENSP00000361711.1</protein_id>
+      <protein_id>ENSP00000361710.5</protein_id>
+      <protein_id>ENSP00000243286.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_33_1_9869_3_1</psm_id>
+        <psm_id>few_spectra_SII_206_1_10205_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]SC[UNIMOD:4]DELAR" p:decoy="true">
-      <svm_score>-0.965</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]TGQC[UNIMOD:4]EC[UNIMOD:4]QPGITGQHC[UNIMOD:4]ER" p:decoy="false">
+      <svm_score>-1.109</svm_score>
+      <q_value>9.077e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>540.2700</exp_mass>
-      <calc_mass>540.271</calc_mass>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
+      <exp_mass>750.0080</exp_mass>
+      <calc_mass>749.668</calc_mass>
+      <protein_id>ENSP00000258341.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_12_1_9848_2_1</psm_id>
+        <psm_id>few_spectra_SII_116_1_10115_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]YQEYM[UNIMOD:35]LGDR" p:decoy="true">
-      <svm_score>-1.000</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]VPPTAC[UNIMOD:4]C[UNIMOD:4]GHSTQPR" p:decoy="false">
+      <svm_score>-1.111</svm_score>
+      <q_value>9.077e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>710.3420</exp_mass>
-      <calc_mass>710.342</calc_mass>
-      <protein_id>decoy_ENSP00000425587.1</protein_id>
-      <protein_id>decoy_ENSP00000424404.1</protein_id>
-      <protein_id>decoy_ENSP00000323377.5</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_29_1_9865_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]NLSNEEMIQAADELEEM[UNIMOD:35]K[UNIMOD:737]" p:decoy="false">
-      <svm_score>-1.051</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>856.4240</exp_mass>
-      <calc_mass>856.757</calc_mass>
-      <protein_id>ENSP00000361709.3</protein_id>
-      <protein_id>ENSP00000361708.3</protein_id>
-      <protein_id>ENSP00000361707.3</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_8_1_9844_3_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]AGDETNM[UNIMOD:35]SC[UNIMOD:4]R" p:decoy="true">
-      <svm_score>-1.055</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>693.3060</exp_mass>
-      <calc_mass>693.303</calc_mass>
-      <protein_id>decoy_ENSP00000323687.6</protein_id>
-      <protein_id>decoy_ENSP00000467623.1</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_7_1_9843_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]IPPPM[UNIMOD:35]R" p:decoy="true">
-      <svm_score>-1.065</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>478.7870</exp_mass>
-      <calc_mass>478.283</calc_mass>
-      <protein_id>decoy_ENSP00000474437.1</protein_id>
-      <protein_id>decoy_ENSP00000363745.3</protein_id>
-      <protein_id>decoy_ENSP00000363741.1</protein_id>
-      <protein_id>decoy_ENSP00000304405.6</protein_id>
-      <protein_id>decoy_ENSP00000475760.1</protein_id>
-      <protein_id>decoy_ENSP00000392799.2</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_14_1_9850_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]DAEATPGVAR" p:decoy="true">
-      <svm_score>-1.079</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>609.3370</exp_mass>
-      <calc_mass>608.330</calc_mass>
-      <protein_id>decoy_ENSP00000396301.2</protein_id>
-      <protein_id>decoy_ENSP00000422641.1</protein_id>
-      <protein_id>decoy_ENSP00000426764.2</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_20_1_9856_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]MSEYGR" p:decoy="false">
-      <svm_score>-1.083</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>486.2450</exp_mass>
-      <calc_mass>486.245</calc_mass>
-      <protein_id>msstitch_fake_onlypeptide</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_17_1_9853_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]M[UNIMOD:35]DQSLELNRAR" p:decoy="true">
-      <svm_score>-1.090</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>788.9110</exp_mass>
-      <calc_mass>789.417</calc_mass>
-      <protein_id>decoy_ENSP00000281394.4</protein_id>
-      <protein_id>decoy_ENSP00000294952.8</protein_id>
-      <protein_id>decoy_ENSP00000415696.2</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_42_1_9878_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]MRAESSVQSR" p:decoy="true">
-      <svm_score>-1.128</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>691.3740</exp_mass>
-      <calc_mass>690.367</calc_mass>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
-      <p_value>0.000e+00</p_value>
-      <psm_ids>
-        <psm_id>few_spectra_SII_37_1_9873_2_1</psm_id>
-        <psm_id>few_spectra_SII_45_1_9881_2_1</psm_id>
-      </psm_ids>
-    </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]QMREQLER" p:decoy="true">
-      <svm_score>-1.150</svm_score>
-      <q_value>1.000e+00</q_value>
-      <pep>1.000e+00</pep>
-      <exp_mass>659.3520</exp_mass>
-      <calc_mass>659.859</calc_mass>
-      <protein_id>decoy_ENSP00000384202.1</protein_id>
-      <protein_id>decoy_ENSP00000400281.2</protein_id>
+      <exp_mass>600.2990</exp_mass>
+      <calc_mass>599.629</calc_mass>
+      <protein_id>ENSP00000297954.4</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_43_1_9879_2_1</psm_id>
+        <psm_id>few_spectra_SII_224_1_10223_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]AMWSLRERSQVSSEAR" p:decoy="false">
-      <svm_score>-1.166</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]MEQAPNM[UNIMOD:35]AEPR" p:decoy="false">
+      <svm_score>-1.115</svm_score>
+      <q_value>9.077e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>1061.0500</exp_mass>
-      <calc_mass>1061.550</calc_mass>
-      <protein_id>sp|Q9P219|DAPLE_HUMAN</protein_id>
+      <exp_mass>759.8720</exp_mass>
+      <calc_mass>759.866</calc_mass>
+      <protein_id>ENSP00000271636.7</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_22_1_9858_2_1</psm_id>
+        <psm_id>few_spectra_SII_130_1_10129_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]SEYM[UNIMOD:35]EGNVR" p:decoy="false">
-      <svm_score>-1.174</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]EC[UNIMOD:4]GDVSRAQEELR" p:decoy="false">
+      <svm_score>-1.133</svm_score>
+      <q_value>9.275e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>665.3180</exp_mass>
-      <calc_mass>665.319</calc_mass>
-      <protein_id>msstitch_fake_gene_anpep</protein_id>
+      <exp_mass>888.9430</exp_mass>
+      <calc_mass>889.439</calc_mass>
+      <protein_id>ENSP00000361711.1</protein_id>
+      <protein_id>ENSP00000361710.5</protein_id>
+      <protein_id>ENSP00000243286.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_27_1_9863_2_1</psm_id>
+        <psm_id>few_spectra_SII_77_1_10076_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]EEERMREREEAER" p:decoy="true">
-      <svm_score>-1.211</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]GGPM[UNIMOD:35]GRGGYGGGGSGGGGR" p:decoy="false">
+      <svm_score>-1.137</svm_score>
+      <q_value>9.286e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>990.4870</exp_mass>
-      <calc_mass>989.484</calc_mass>
-      <protein_id>decoy_ENSP00000354826.2</protein_id>
+      <exp_mass>898.4210</exp_mass>
+      <calc_mass>898.426</calc_mass>
+      <protein_id>ENSP00000254108.7</protein_id>
+      <protein_id>ENSP00000369594.3</protein_id>
+      <protein_id>ENSP00000455282.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_5_1_9841_2_1</psm_id>
+        <psm_id>few_spectra_SII_108_1_10107_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]C[UNIMOD:4]GQEEHDVLLSNEEDR" p:decoy="false">
-      <svm_score>-1.224</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]FDGHRC[UNIMOD:4]AGQQQDIR" p:decoy="false">
+      <svm_score>-1.185</svm_score>
+      <q_value>9.730e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>720.3350</exp_mass>
-      <calc_mass>720.334</calc_mass>
-      <protein_id>ENSP00000350937.4</protein_id>
-      <protein_id>ENSP00000377121.2</protein_id>
+      <exp_mass>639.9810</exp_mass>
+      <calc_mass>639.650</calc_mass>
+      <protein_id>ENSP00000380189.3</protein_id>
+      <protein_id>ENSP00000366204.2</protein_id>
+      <protein_id>ENSP00000247153.3</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_28_1_9864_3_1</psm_id>
+        <psm_id>few_spectra_SII_148_1_10147_3_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]LMQLESELQR" p:decoy="true">
-      <svm_score>-1.299</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]M[UNIMOD:35]DC[UNIMOD:4]YSGQK[UNIMOD:737]" p:decoy="false">
+      <svm_score>-1.196</svm_score>
+      <q_value>9.730e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>739.4090</exp_mass>
-      <calc_mass>738.408</calc_mass>
-      <protein_id>decoy_sp|Q9P219|DAPLE_HUMAN</protein_id>
+      <exp_mass>732.8540</exp_mass>
+      <calc_mass>731.857</calc_mass>
+      <protein_id>ENSP00000261978.4</protein_id>
+      <protein_id>ENSP00000452110.1</protein_id>
+      <protein_id>ENSP00000451477.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_13_1_9849_2_1</psm_id>
+        <psm_id>few_spectra_SII_31_1_10030_2_1</psm_id>
       </psm_ids>
     </peptide>
-    <peptide p:peptide_id="[UNIMOD:737]GAVMEQGTSSSM[UNIMOD:35]TAESSPR" p:decoy="false">
-      <svm_score>-1.456</svm_score>
-      <q_value>1.000e+00</q_value>
+    <peptide p:peptide_id="[UNIMOD:737]TC[UNIMOD:4]NTNPHLNALSTDSAC[UNIMOD:4]R" p:decoy="false">
+      <svm_score>-1.212</svm_score>
+      <q_value>9.730e-01</q_value>
       <pep>1.000e+00</pep>
-      <exp_mass>720.6680</exp_mass>
-      <calc_mass>720.003</calc_mass>
-      <protein_id>ENSP00000297954.4</protein_id>
-      <protein_id>ENSP00000415038.1</protein_id>
-      <protein_id>ENSP00000378860.2</protein_id>
+      <exp_mass>755.0220</exp_mass>
+      <calc_mass>754.358</calc_mass>
+      <protein_id>ENSP00000277165.5</protein_id>
+      <protein_id>ENSP00000412440.1</protein_id>
       <p_value>0.000e+00</p_value>
       <psm_ids>
-        <psm_id>few_spectra_SII_23_1_9859_3_1</psm_id>
+        <psm_id>few_spectra_SII_244_1_10243_3_1</psm_id>
       </psm_ids>
     </peptide>
   </peptides>
 </percolator_output>
```

### Comparing `msstitch-3.8/tests/fixtures/perco_timstof.xml` & `msstitch-3.9/tests/fixtures/perco_timstof.xml`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/fixtures/protrev_ens99_small.fasta` & `msstitch-3.9/tests/fixtures/protrev_ens99_small.fasta`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/fixtures/spectra_lookup_timstof.sqlite` & `msstitch-3.9/tests/fixtures/spectra_lookup_timstof.sqlite`

 * *Files 3% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,32 +1,32 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
 CREATE TABLE biosets(set_id INTEGER PRIMARY KEY, set_name TEXT);
 INSERT INTO biosets VALUES(1,'Set1');
-CREATE TABLE mzmlfiles(mzmlfile_id INTEGER PRIMARY KEY, mzmlfilename TEXT, set_id INTEGER, FOREIGN KEY(set_id)REFERENCES biosets);
+CREATE TABLE mzmlfiles(mzmlfile_id INTEGER PRIMARY KEY, mzmlfilename TEXT, set_id INTEGER, FOREIGN KEY(set_id)REFERENCES biosets ON DELETE CASCADE);
 INSERT INTO mzmlfiles VALUES(1,'few_spec_timstof.mzML',1);
-CREATE TABLE mzml(spectra_id TEXT PRIMARY KEY, mzmlfile_id INTEGER, scan_sid TEXT, charge INTEGER, mz DOUBLE, retention_time DOUBLE, ion_injection_time DOUBLE, FOREIGN KEY(mzmlfile_id)REFERENCES mzmlfiles);
-INSERT INTO mzml VALUES('1_merged=22627 frame=8367 scanStart=566 scanEnd=590',1,'merged=22627 frame=8367 scanStart=566 scanEnd=590',2,730.30771604197502709,904.5714612445790408,NULL);
-INSERT INTO mzml VALUES('1_merged=22776 frame=8399 scanStart=642 scanEnd=666',1,'merged=22776 frame=8399 scanStart=642 scanEnd=666',2,638.29163243951404639,901.15239810291495811,NULL);
-INSERT INTO mzml VALUES('1_merged=22791 frame=8402 scanStart=699 scanEnd=723',1,'merged=22791 frame=8402 scanStart=699 scanEnd=723',2,549.80465920223105056,900.04908668305904483,NULL);
-INSERT INTO mzml VALUES('1_merged=22792 frame=8402 scanStart=739 scanEnd=763',1,'merged=22792 frame=8402 scanStart=739 scanEnd=763',2,542.26911144826203782,900.04908668305904483,NULL);
-INSERT INTO mzml VALUES('1_merged=22794 frame=8402 scanStart=849 scanEnd=873',1,'merged=22794 frame=8402 scanStart=849 scanEnd=873',2,395.71530797335498163,900.20652208482999871,NULL);
-INSERT INTO mzml VALUES('1_merged=22797 frame=8403 scanStart=676 scanEnd=700',1,'merged=22797 frame=8403 scanStart=676 scanEnd=700',2,590.78418253984500553,901.41586539017305316,NULL);
-INSERT INTO mzml VALUES('1_merged=22798 frame=8403 scanStart=746 scanEnd=770',1,'merged=22798 frame=8403 scanStart=746 scanEnd=770',2,440.71923203173901128,900.25877983377301915,NULL);
-INSERT INTO mzml VALUES('1_merged=22799 frame=8403 scanStart=788 scanEnd=812',1,'merged=22799 frame=8403 scanStart=788 scanEnd=812',2,458.71135745263597982,900.25877983377301915,NULL);
-INSERT INTO mzml VALUES('1_merged=22801 frame=8404 scanStart=664 scanEnd=688',1,'merged=22801 frame=8404 scanStart=664 scanEnd=688',2,584.27219102907395151,902.46749500099201664,NULL);
-INSERT INTO mzml VALUES('1_merged=22802 frame=8404 scanStart=704 scanEnd=728',1,'merged=22802 frame=8404 scanStart=704 scanEnd=728',2,565.76945540218503082,900.31163317026596361,NULL);
-INSERT INTO mzml VALUES('1_merged=22811 frame=8406 scanStart=648 scanEnd=672',1,'merged=22811 frame=8406 scanStart=648 scanEnd=672',2,620.30935596260394506,900.67965994267296988,NULL);
-INSERT INTO mzml VALUES('1_merged=22812 frame=8406 scanStart=695 scanEnd=719',1,'merged=22812 frame=8406 scanStart=695 scanEnd=719',2,584.74308581615105141,900.7844946414689957,NULL);
-INSERT INTO mzml VALUES('1_merged=22813 frame=8406 scanStart=736 scanEnd=760',1,'merged=22813 frame=8406 scanStart=736 scanEnd=760',2,498.73960115536999635,900.57404857542599071,NULL);
-INSERT INTO mzml VALUES('1_merged=22815 frame=8406 scanStart=843 scanEnd=867',1,'merged=22815 frame=8406 scanStart=843 scanEnd=867',3,508.85234230418200239,900.62685425904896877,NULL);
-INSERT INTO mzml VALUES('1_merged=22829 frame=8410 scanStart=749 scanEnd=773',1,'merged=22829 frame=8410 scanStart=749 scanEnd=773',2,497.27273956573196755,901.415142092934957,NULL);
-INSERT INTO mzml VALUES('1_merged=22830 frame=8410 scanStart=800 scanEnd=824',1,'merged=22830 frame=8410 scanStart=800 scanEnd=824',3,503.24311401856397195,901.04734376104897823,NULL);
-CREATE TABLE ioninjtime(spectra_id TEXT, ion_injection_time DOUBLE, FOREIGN KEY(spectra_id)REFERENCES mzml);
-CREATE TABLE ionmob(spectra_id TEXT, ion_mobility DOUBLE, FOREIGN KEY(spectra_id)REFERENCES mzml);
+CREATE TABLE mzml(spectra_id TEXT PRIMARY KEY, mzmlfile_id INTEGER, scan_sid TEXT, charge INTEGER, mz DOUBLE, retention_time DOUBLE, FOREIGN KEY(mzmlfile_id)REFERENCES mzmlfiles ON DELETE CASCADE);
+INSERT INTO mzml VALUES('1_merged=22627 frame=8367 scanStart=566 scanEnd=590',1,'merged=22627 frame=8367 scanStart=566 scanEnd=590',2,730.30771604197502709,904.5714612445790408);
+INSERT INTO mzml VALUES('1_merged=22776 frame=8399 scanStart=642 scanEnd=666',1,'merged=22776 frame=8399 scanStart=642 scanEnd=666',2,638.29163243951404639,901.15239810291495811);
+INSERT INTO mzml VALUES('1_merged=22791 frame=8402 scanStart=699 scanEnd=723',1,'merged=22791 frame=8402 scanStart=699 scanEnd=723',2,549.80465920223105056,900.04908668305904483);
+INSERT INTO mzml VALUES('1_merged=22792 frame=8402 scanStart=739 scanEnd=763',1,'merged=22792 frame=8402 scanStart=739 scanEnd=763',2,542.26911144826203782,900.04908668305904483);
+INSERT INTO mzml VALUES('1_merged=22794 frame=8402 scanStart=849 scanEnd=873',1,'merged=22794 frame=8402 scanStart=849 scanEnd=873',2,395.71530797335498163,900.20652208482999871);
+INSERT INTO mzml VALUES('1_merged=22797 frame=8403 scanStart=676 scanEnd=700',1,'merged=22797 frame=8403 scanStart=676 scanEnd=700',2,590.78418253984500553,901.41586539017305316);
+INSERT INTO mzml VALUES('1_merged=22798 frame=8403 scanStart=746 scanEnd=770',1,'merged=22798 frame=8403 scanStart=746 scanEnd=770',2,440.71923203173901128,900.25877983377301915);
+INSERT INTO mzml VALUES('1_merged=22799 frame=8403 scanStart=788 scanEnd=812',1,'merged=22799 frame=8403 scanStart=788 scanEnd=812',2,458.71135745263597982,900.25877983377301915);
+INSERT INTO mzml VALUES('1_merged=22801 frame=8404 scanStart=664 scanEnd=688',1,'merged=22801 frame=8404 scanStart=664 scanEnd=688',2,584.27219102907395151,902.46749500099201664);
+INSERT INTO mzml VALUES('1_merged=22802 frame=8404 scanStart=704 scanEnd=728',1,'merged=22802 frame=8404 scanStart=704 scanEnd=728',2,565.76945540218503082,900.31163317026596361);
+INSERT INTO mzml VALUES('1_merged=22811 frame=8406 scanStart=648 scanEnd=672',1,'merged=22811 frame=8406 scanStart=648 scanEnd=672',2,620.30935596260394506,900.67965994267296988);
+INSERT INTO mzml VALUES('1_merged=22812 frame=8406 scanStart=695 scanEnd=719',1,'merged=22812 frame=8406 scanStart=695 scanEnd=719',2,584.74308581615105141,900.7844946414689957);
+INSERT INTO mzml VALUES('1_merged=22813 frame=8406 scanStart=736 scanEnd=760',1,'merged=22813 frame=8406 scanStart=736 scanEnd=760',2,498.73960115536999635,900.57404857542599071);
+INSERT INTO mzml VALUES('1_merged=22815 frame=8406 scanStart=843 scanEnd=867',1,'merged=22815 frame=8406 scanStart=843 scanEnd=867',3,508.85234230418200239,900.62685425904896877);
+INSERT INTO mzml VALUES('1_merged=22829 frame=8410 scanStart=749 scanEnd=773',1,'merged=22829 frame=8410 scanStart=749 scanEnd=773',2,497.27273956573196755,901.415142092934957);
+INSERT INTO mzml VALUES('1_merged=22830 frame=8410 scanStart=800 scanEnd=824',1,'merged=22830 frame=8410 scanStart=800 scanEnd=824',3,503.24311401856397195,901.04734376104897823);
+CREATE TABLE ioninjtime(spectra_id TEXT, ion_injection_time DOUBLE, FOREIGN KEY(spectra_id)REFERENCES mzml ON DELETE CASCADE);
+CREATE TABLE ionmob(spectra_id TEXT, ion_mobility DOUBLE, FOREIGN KEY(spectra_id)REFERENCES mzml ON DELETE CASCADE);
 INSERT INTO ionmob VALUES('1_merged=22627 frame=8367 scanStart=566 scanEnd=590',0.97974240271099999333);
 INSERT INTO ionmob VALUES('1_merged=22776 frame=8399 scanStart=642 scanEnd=666',0.91369808538999996994);
 INSERT INTO ionmob VALUES('1_merged=22791 frame=8402 scanStart=699 scanEnd=723',0.86772293253999999151);
 INSERT INTO ionmob VALUES('1_merged=22792 frame=8402 scanStart=739 scanEnd=763',0.83559862113200000788);
 INSERT INTO ionmob VALUES('1_merged=22794 frame=8402 scanStart=849 scanEnd=873',0.74285763717899999658);
 INSERT INTO ionmob VALUES('1_merged=22797 frame=8403 scanStart=676 scanEnd=700',0.88564911641499999284);
 INSERT INTO ionmob VALUES('1_merged=22798 frame=8403 scanStart=746 scanEnd=770',0.82984459004199995213);
@@ -45,8 +45,10 @@
 CREATE INDEX mzmlfn_index on mzmlfiles(mzmlfilename);
 CREATE INDEX mzmlfnid_index on mzmlfiles(mzmlfile_id);
 CREATE INDEX spectra_id_index on mzml(spectra_id);
 CREATE INDEX mzmlfnid_mzml_index on mzml(mzmlfile_id);
 CREATE INDEX scan_index on mzml(scan_sid);
 CREATE INDEX specrt_index on mzml(retention_time);
 CREATE INDEX specmz_index on mzml(mz);
+CREATE INDEX ionm_sp_ix on ionmob(spectra_id);
+CREATE INDEX ionin_sp_ix on ioninjtime(spectra_id);
 COMMIT;
```

### Comparing `msstitch-3.8/tests/integration/basetests.py` & `msstitch-3.9/tests/integration/basetests.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             cmd.extend(['-d', self.workdir])
         return cmd
 
     def run_command(self, options=[], return_error=False):
         cmd = self.get_std_options()
         cmd.extend(options)
         check = not return_error
+        print(cmd)
         try:
             complete = subprocess.run(cmd, capture_output=True, text=True, check=check)
         except subprocess.CalledProcessError as e:
             print('Failed to run command: ', cmd)
             print('Output of command:')
             print(e.stdout)
             print(e.stderr)
@@ -181,64 +182,53 @@
 
 class MzidTSVBaseTest(BaseTest):
 
     def rowify(self, records):
         row, rownr = [], 0
         for record in records:
             if record[0] == rownr:
-                row.append(record)
+                row.append(record[1:])
             else:
                 yield row
-                row = [record]
+                row = [record[1:]]
                 rownr += 1
 
     def check_results_sql(self, checkfields, expected_values):
         for resultvals, exp_vals in zip(self.get_values(checkfields),
                                         expected_values):
             for resultval, expectval in zip(resultvals, exp_vals):
                 self.assertEqual([str(x) if x is not None else 'NA'
                                   for x in expectval],
                                  [str(x) for x in resultval])
 
-    def process_dbvalues_both(self, dbfile, sql, channel_fields, permfieldnrs,
-                              permfieldnames):
+    def process_dbvalues_both(self, dbfile, sql, permfieldnrs, permfieldnames):
+        '''FIXME what does this do, is it same as rowify but with fields?'''
         dbvals = self.get_values_from_db(dbfile, sql)
-        outresults, rownr, permvals = [], 0, []
+        rownr, permvals = 0, []
         for record in dbvals:
             if record[0] != rownr:
-                for outresult in outresults:
-                    yield outresult
-                for pfname, pval in zip(permfieldnames, permvals):
-                    yield (rownr, pfname, pval)
-                if channel_fields != []:
-                    outresults = [tuple([record[0]] +
-                                        [record[x] for x in channel_fields])]
+                yield [tuple([x, y]) for x, y in zip(permfieldnames, permvals)]
                 permvals = [record[nr] for nr in permfieldnrs]
                 rownr += 1
             else:
-                permvals = [record[nr] for nr in permfieldnrs]
-                if channel_fields != []:
-                    result = [record[0]] + [record[x] for x in channel_fields]
-                    outresults.append(tuple(result))
+                permvals.extend([record[nr] for nr in permfieldnrs])
 
     def get_values(self, checkfields, outfile=False):
         if not outfile:
             outfile = self.resultfn
         with open(outfile) as fp:
             header = next(fp).strip('\n').split('\t')
             fieldindices = [header.index(field) for field in checkfields]
-            row = 0
             for line in fp:
                 line = line.strip('\n').split('\t')
                 if len(checkfields) > 1:
-                    yield [(row, field, line[ix]) for field, ix in
+                    yield [(field, line[ix]) for field, ix in
                            zip(checkfields, fieldindices)]
                 else:
-                    yield [(row, line[ix]) for ix in fieldindices]
-                row += 1
+                    yield [(line[ix],) for ix in fieldindices]
 
 
 class MSLookupTest(BaseTest):
     base_db_fn = None
     suffix = ''
 
     def setUp(self):
```

### Comparing `msstitch-3.8/tests/integration/merge_tests.py` & `msstitch-3.9/tests/integration/merge_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                'JOIN psms AS p USING(pep_id) '
                'JOIN protein_psm USING(psm_id) '
                'JOIN proteins AS prot USING(protein_acc) '
                )
         self.check_iso_and_peptide_relations(sql, proteincentric=True, nogroup=True)
 
     def check_iso_and_peptide_relations(self, sql, proteincentric=False, nogroup=False, flr=False):
+        # FIXME should not join on both pepid and setid?
         valsql = ('SELECT ps.sequence, bs.set_name, '
                'ppq.quant, pf.fdr, flr.flr '
                'FROM peptide_sequences AS ps '
                'JOIN biosets AS bs '
                'JOIN peptide_precur_quanted AS ppq USING(pep_id) '
                'LEFT OUTER JOIN ptm_flr AS flr USING(pep_id) '
                'JOIN peptide_fdr AS pf USING(pep_id) ')
```

### Comparing `msstitch-3.8/tests/integration/mslookup_tests.py` & `msstitch-3.9/tests/integration/mslookup_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,9 +457,16 @@
                     mz = float(line['mz'])
                 resval = feats[1][round(float(line[fields['rt']]), 12)][mz][charge]
                 fwhm = float(line['fwhm']) if line['fwhm'] else None
                 self.assertEqual((float(line[fields['intensity']]), fwhm), resval)
         # Now check we have a feature for all scans
         sql = """SELECT m.scan_sid, ma.feature_id FROM mzml AS m
         LEFT OUTER JOIN ms1_align AS ma USING(spectra_id)"""
+        exemptscans = {'dino': [10229], 'kr': [10148, 10229]}
+        exemptscans = [f'controllerType=0 controllerNumber=1 scan={x}' for x 
+                in exemptscans[feattype]]
         for scan, featid in self.get_values_from_db(self.resultfn, sql):
-            self.assertFalse(featid == None)
+            # some scans do not have a aligned MS1 value
+            if scan not in exemptscans:
+                self.assertFalse(featid == None)
+            else:
+                self.assertTrue(featid == None)
```

### Comparing `msstitch-3.8/tests/integration/peptable_tests.py` & `msstitch-3.9/tests/integration/peptable_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                    '--summarize-average',
                    '--ms1quantcolpattern', 'MS1', 
                    '--modelqvals', '--qvalthreshold', '1e-5',
                    '--minpepnr', str(4),
                    ]
         self.run_command(options)
         self.check(1)
-        self.isoquant_check(os.path.join(self.fixdir, 'target_peptides.tsv'),
+        self.isoquant_check(os.path.join(self.fixdir, 'target_peptides_avg.tsv'),
                 'Peptide sequence', self.channels, self.nopsms)
 
     def test_no_spectracol_mediansweep_keep_na(self):
         options = ['--isobquantcolpattern', 'tmt10plex',
                 '--scorecolpattern', 'svm',
                    '--mediansweep',
                    '--keep-psms-na-quant',
@@ -123,43 +123,63 @@
                    '--minpepnr', str(4),
                    ]
         self.run_command(options)
         self.check(1)
         self.isoquant_check(os.path.join(self.fixdir, 'target_peptides_sweep.tsv'),
                 'Peptide sequence', self.channels, self.nopsms)
 
-    def test_psm2peptable_totalproteome(self):
+    def test_totalproteome(self):
         options = ['--spectracol', '1', '--isobquantcolpattern',
                    'tmt10plex', '--scorecolpattern', 'svm',
                    '--ms1quantcolpattern', 'MS1',
                    '--modelqvals', '--qvalthreshold', '1e-5',
                    '--minpepnr', str(4),
                    '--denompatterns', '126',
                    '--totalproteome', os.path.join(self.fixdir, 'proteins.txt'),
                    ]
         self.run_command(options)
         self.check(1)
         self.isoquant_check(os.path.join(self.fixdir, 'target_peptides_totalprotnorm_nolog.txt'),
                 'Peptide sequence', self.channels, self.nopsms)
 
-    def test_psm2peptable_totalproteome_logiso(self):
+    def test_totalproteome_logiso(self):
         options = ['--spectracol', '1', '--isobquantcolpattern',
                    'tmt10plex', '--scorecolpattern', 'svm',
                    '--ms1quantcolpattern', 'MS1', 
                    '--modelqvals', '--qvalthreshold', '1e-5',
                    '--minpepnr', str(4),
                    '--denompatterns', '126',
                    '--logisoquant',
                    '--totalproteome', os.path.join(self.fixdir, 'proteins_isonorm_log.txt'),
                    ]
         self.run_command(options)
         self.check(1)
         self.isoquant_check(os.path.join(self.fixdir, 'target_peptides_totalprotnorm.txt'),
                 'Peptide sequence', self.channels, self.nopsms)
 
+    def test_totalproteome_logiso_sepnorm(self):
+        '''Most proteins/peptides have identical quant in this small exp. So output of
+        totalprotnormalizing with median centering is pep - prot - median = 0 - median
+        '''
+        options = ['--spectracol', '1', '--isobquantcolpattern',
+                   'tmt10plex', '--scorecolpattern', 'svm',
+                   '--ms1quantcolpattern', 'MS1', 
+                   '--modelqvals', '--qvalthreshold', '1e-5',
+                   '--minpepnr', str(4),
+                   '--denompatterns', '126',
+                   '--logisoquant',
+                   '--totalproteome', os.path.join(self.fixdir, 'proteins_nonorm_log.txt'),
+                   '--median-normalize',
+                   '--normalization-factors-table', os.path.join(self.fixdir, 'proteins_nonorm_log.txt'),
+                   ]
+        self.run_command(options)
+        self.check(1)
+        self.isoquant_check(os.path.join(self.fixdir, 'target_peptides_totalp_sepnorm.txt'),
+                'Peptide sequence', self.channels, self.nopsms)
+
 
 
 class TestProteinTable(basetests.ProttableTest):
     command = 'proteins'
     infilename = 'target_peptides.tsv'
 
     def test_denoms(self):
@@ -173,15 +193,15 @@
         self.dotest_proteintable('^q-value', 'Master protein(s)', 'Protein ID', summarize_method='sweep')
         expectedfn = os.path.join(self.fixdir, 'proteins_sweep.txt')
         self.check_lines(expectedfn, self.resultfn)
 
     def test_average_summarizing(self):
         self.specialoptions = ['--summarize-average']
         self.dotest_proteintable('^q-value', 'Master protein(s)', 'Protein ID')
-        expectedfn = os.path.join(self.fixdir, 'proteins.txt')
+        expectedfn = os.path.join(self.fixdir, 'proteins_avg.txt')
         self.check_lines(expectedfn, self.resultfn)
 
     def test_isonormalize_log(self):
         self.specialoptions = ['--logisoquant', '--median-normalize', '--minint', '0.1']
         self.dotest_proteintable('^q-value', 'Master protein(s)', 'Protein ID')
         expectedfn = os.path.join(self.fixdir, 'proteins_isonorm_log.txt')
         self.check_lines(expectedfn, self.resultfn)
```

### Comparing `msstitch-3.8/tests/integration/percolator_tests.py` & `msstitch-3.9/tests/integration/percolator_tests.py`

 * *Files identical despite different names*

### Comparing `msstitch-3.8/tests/integration/psmtable_tests.py` & `msstitch-3.9/tests/integration/psmtable_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,20 +55,20 @@
                'LEFT OUTER JOIN ioninjtime AS iit USING(spectra_id) '
                'LEFT OUTER JOIN ionmob AS im USING(spectra_id) '
                'JOIN mzmlfiles USING(mzmlfile_id) '
                'JOIN biosets AS bs USING(set_id) '
                'ORDER BY pr.rownr')
         fields = ['Biological set', 'Retention time(min)',
                   'Ion injection time(ms)', 'Ion mobility(Vs/cm2)']
-        expected_values = self.process_dbvalues_both(self.workdb, sql, [],
+        expected_values = self.process_dbvalues_both(self.workdb, sql,
                                                      [1, 2, 3, 4], fields)
-        self.check_results_sql(fields, self.rowify(expected_values))
+        self.check_results_sql(fields, expected_values)
         for val, exp in zip(self.get_values(['missed_cleavage']), self.get_values(['Peptide'], self.infile[0])):
-            exp = re.sub('[0-9\+\.]', '', exp[0][1])[:-1]
-            self.assertEqual(int(val[0][1]), exp.count('K') + exp.count('R') - exp.count('KP') - exp.count('RP'))
+            exp = re.sub('[0-9\+\.]', '', exp[0][0])[:-1]
+            self.assertEqual(int(val[0][0]), exp.count('K') + exp.count('R') - exp.count('KP') - exp.count('RP'))
 
     def check_addspec_miscleav_bioset(self):
         sql = ('SELECT pr.rownr, bs.set_name, sp.retention_time, '
                'iit.ion_injection_time, im.ion_mobility, pif.pif '
                'FROM psmrows AS pr JOIN psms USING(psm_id) '
                'JOIN mzml AS sp USING(spectra_id) '
                'JOIN ioninjtime AS iit USING(spectra_id) '
@@ -76,40 +76,40 @@
                'LEFT OUTER JOIN precursor_ion_fraction AS pif USING(spectra_id) '
                'JOIN mzmlfiles USING(mzmlfile_id) '
                'JOIN biosets AS bs USING(set_id) '
                'ORDER BY pr.rownr')
         fields = ['Biological set', 'Retention time(min)',
                   'Ion injection time(ms)', 'Ion mobility(Vs/cm2)',
                   'Precursor ion fraction']
-        expected_values = self.process_dbvalues_both(self.workdb, sql, [],
+        expected_values = self.process_dbvalues_both(self.workdb, sql,
                                                      [1, 2, 3, 4, 5], fields)
-        self.check_results_sql(fields, self.rowify(expected_values))
+        self.check_results_sql(fields, expected_values)
         for val, exp in zip(self.get_values(['missed_cleavage']), self.get_values(['Peptide'], self.infile[0])):
-            exp = re.sub('[0-9\+\.]', '', exp[0][1])[:-1]
-            self.assertEqual(int(val[0][1]), exp.count('K') + exp.count('R') - exp.count('KP') - exp.count('RP'))
+            exp = re.sub('[0-9\+\.]', '', exp[0][0])[:-1]
+            self.assertEqual(int(val[0][0]), exp.count('K') + exp.count('R') - exp.count('KP') - exp.count('RP'))
 
     def check_quanttsv(self, minpif):
         sql = ('SELECT pr.rownr, ic.channel_name, '
                 'CASE WHEN pif.pif > {} THEN iq.intensity ELSE "NA" END AS intensity '
                 'FROM psmrows AS pr JOIN psms USING(psm_id) '
                 'LEFT OUTER JOIN precursor_ion_fraction AS pif USING(spectra_id) '
                 'JOIN isobaric_quant AS iq USING(spectra_id) '
                 'JOIN isobaric_channels AS ic USING(channel_id) '.format(float(minpif)))
-        expected_values = self.get_values_from_db(self.workdb, sql)
         fields = ['tmt10plex_{}'.format(ch) for ch in ['126', '127N', '127C',
                                                        '128N', '128C', '129N',
                                                        '129C', '130N', '130C',
                                                        '131']]
-        self.check_results_sql(fields, self.rowify(expected_values))
+        expected_values = self.rowify(self.get_values_from_db(self.workdb, sql))
+        self.check_results_sql(fields, expected_values)
         sql = ('SELECT pr.rownr, pq.intensity '
                'FROM psmrows AS pr JOIN psms USING(psm_id) '
                'LEFT OUTER JOIN ms1_align USING(spectra_id) '
                'LEFT OUTER JOIN ms1_quant AS pq USING(feature_id)')
-        expected_values = self.get_values_from_db(self.workdb, sql)
-        self.check_results_sql(['MS1 area'], self.rowify(expected_values))
+        expected_values = self.rowify(self.get_values_from_db(self.workdb, sql))
+        self.check_results_sql(['MS1 area'], expected_values)
 
     def check_db_fasta(self, fasta, exp_proteins=None, desc=True):
         if exp_proteins is None:
             exp_proteins = {}
             for rec in SeqIO.parse(fasta, 'fasta'):
                 rd = rec.description
                 gene = 'NA'
@@ -244,19 +244,19 @@
         expected = self.parse_proteingroups(
             os.path.join(self.fixdir, 'target_pg.tsv'))
         self.do_asserting(result, expected)
 
     def check_addgenes(self):
         for line in self.get_values(['Gene ID', 'Gene Name', 'Description',
                                      'Protein']):
-            genes = line[0][2].split(';')
-            assoc_ids = line[1][2].split(';')
+            genes = line[0][1].split(';')
+            assoc_ids = line[1][1].split(';')
             descriptions = ['{}]'.format(x).replace(']]', ']')
-                            for x in line[2][2].split('];')]
-            proteins = [x.split('(')[0] for x in line[3][2].split(';')]
+                            for x in line[2][1].split('];')]
+            proteins = [x.split('(')[0] for x in line[3][1].split(';')]
             sql = ('SELECT p.protein_acc, g.gene_acc, a.assoc_id, '
                    'd.description FROM proteins AS p '
                    'JOIN ensg_proteins USING(pacc_id) '
                    'JOIN genename_proteins USING(pacc_id) '
                    'JOIN genes AS g USING(gene_id) '
                    'JOIN associated_ids AS a USING(gn_id) '
                    ' JOIN prot_desc AS d ON d.pacc_id=p.pacc_id '
@@ -275,69 +275,70 @@
 
 class TestPercoTSV(basetests.MzidTSVBaseTest):
     command = 'perco2psm'
     suffix = '_fdr.tsv'
     infilename = 'few_spectra.tsv'
 
     def test_conffilt(self):
+        threshold = 0.3
         mzidfn = os.path.join(self.fixdir, 'few_spectra.mzid')
         percofn = os.path.join(self.fixdir, 'perco.xml')
-        options = ['--mzid', mzidfn, '--perco', percofn, '--filtpep', '0.01',
-            '--filtpsm', '0.01']
+        options = ['--mzid', mzidfn, '--perco', percofn, '--filtpep', 
+            str(threshold), '--filtpsm', str(threshold)]
         self.run_command(options)
-        checkfields = ['percolator svm-score', 'PSM q-value', 'peptide q-value', 'TD']
+        checkfields = ['percolator svm-score', 'PSM q-value', 'peptide q-value',
+            'PSM PEP', 'peptide PEP', 'TD']
         with open(os.path.join(self.fixdir, 'few_spectra.tsv_fdr.tsv')) as fp:
             header = next(fp).strip().split('\t')
             expected = [line.strip().split('\t') for line in fp]
         expected = [{field: line[i] for i, field in enumerate(header)} for line in expected]
-        expected = [line for line in expected if float(line['PSM q-value']) < 0.01 and
-            float(line['peptide q-value']) < 0.01]
+        expected = [line for line in expected if float(line['PSM q-value']) < threshold and
+            float(line['peptide q-value']) < threshold]
         self.assertEqual(len(expected),  len([x for x in self.get_values(checkfields)]))
         for res, exp in zip(self.get_values(checkfields), expected):
             for i, field in enumerate(checkfields):
-                if field in checkfields:
-                    self.assertEqual(field, res[i][1])
-                    self.assertEqual(exp[field], res[i][2])
+                self.assertEqual(field, res[i][0])
+                self.assertEqual(exp[field], res[i][1])
 
-    def test_add_tdc_fdr(self):
+    def test_add_fdr(self):
         mzidfn = os.path.join(self.fixdir, 'few_spectra.mzid')
         percofn = os.path.join(self.fixdir, 'perco.xml')
         options = ['--mzid', mzidfn, '--perco', percofn]
         self.run_command(options)
-        checkfields = ['percolator svm-score', 'PSM q-value', 'peptide q-value', 'TD']
+        checkfields = ['percolator svm-score', 'PSM q-value', 'peptide q-value',
+            'PSM PEP', 'peptide PEP', 'TD']
         with open(os.path.join(self.fixdir, 'few_spectra.tsv_fdr.tsv')) as fp:
             header = next(fp).strip().split('\t')
             expected = [line.strip().split('\t') for line in fp]
         expected = [{field: line[i] for i, field in enumerate(header)} for line in expected]
         for res, exp in zip(self.get_values(checkfields), expected):
             for i, field in enumerate(checkfields):
-                if field in checkfields:
-                    self.assertEqual(field, res[i][1])
-                    self.assertEqual(exp[field], res[i][2])
+                self.assertEqual(field, res[i][0])
+                self.assertEqual(exp[field], res[i][1])
 
 
 class TestPercoTSVTIMS(basetests.MzidTSVBaseTest):
     command = 'perco2psm'
     suffix = '_fdr.tsv'
     infilename = 'few_spec_timstof.tsv'
     dbfn = 'spectra_lookup_timstof.sqlite'
 
-    def test_add_tdc_fdr_timstof(self):
+    def test_add_fdr_timstof(self):
         mzidfn = os.path.join(self.fixdir, 'few_spec_timstof.mzid')
         percofn = os.path.join(self.fixdir, 'perco_timstof.xml')
         options = ['--mzid', mzidfn, '--perco', percofn]
         self.run_command(options)
         with open(os.path.join(self.fixdir, 'few_spec_timstof.tsv_fdr.tsv')) as fp:
             header = next(fp).strip().split('\t')
             expected = [line.strip().split('\t') for line in fp]
         expected = [{field: line[i] for i, field in enumerate(header)} for line in expected]
         for res, exp in zip(self.get_values(header), expected):
             for i, field in enumerate(header):
-                self.assertEqual(field, res[i][1])
-                self.assertEqual(exp[field], res[i][2])
+                self.assertEqual(field, res[i][0])
+                self.assertEqual(exp[field], res[i][1])
 
 
 class TestConcatTSV(basetests.MzidTSVBaseTest):
     command = 'concat'
     suffix = '_concat.tsv'
     infilename = 'few_spectra.tsv'
 
@@ -373,15 +374,15 @@
             self.assertEqual(result.stdout.strip(), 
                     'ERROR: --splitcol must be an integer or "TD", or "bioset"')
         else:
             self.fail('This test should error')
 
     def test_splitcol(self):
         setnames = ['Set1', 'Set2']
-        options = ['--splitcol', '28']
+        options = ['--splitcol', '30']
         self.run_command(options)
         resultfiles = [os.path.join(self.workdir, '{}.tsv'.format(setname))
                        for setname in setnames]
         for resultfn in resultfiles:
             for line in self.get_all_lines(resultfn):
                 self.assertIn(line, self.expectlines)
 
@@ -493,33 +494,33 @@
     infilename = 'set1_target_pg.tsv'
 
     def test_mediansweep(self):
         result = self.run_command(['--isobquantcolpattern', 'plex',
             '--mediansweep'])
         self.do_check(0, result.stdout, ratiomethod='sweep')
 
-    def test_keep_zero_NA_psms_denomcolpattern(self):
-        result = self.run_command(['--isobquantcolpattern', 'plex',
-            '--denompatterns', '_126', '_131', '--keep-psms-na-quant'])
-        self.do_check(0, result.stdout, keep_na_quant=True)
-
     def test_summarize_avg(self):
+        denompats = ['_126']
         result = self.run_command(['--isobquantcolpattern', 'plex',
-            '--denompatterns', '_126', '_131', '--summarize-average'])
-        self.do_check(0, result.stdout)
+            '--denompatterns', *denompats, '--summarize-average'])
+        self.do_check(0, result.stdout, denompats=denompats)
 
     def test_denomcolpattern_regex(self):
+        denompats = ['_1[23][61]']
         result = self.run_command(['--isobquantcolpattern', 'plex', 
-            '--denompatterns', '_1[23][61]'])
-        self.do_check(0, result.stdout)
+            '--denompatterns', *denompats])
+        self.do_check(0, result.stdout, denompats=denompats)
 
     def get_denominator(self, line, method, denom_ch):
         if method == 'denoms':
             denomvals = [float(line[ch]) for ch in denom_ch if line[ch] != 'NA']
-            return sum(denomvals) / len(denomvals)
+            if denomvals == []:
+                return 0
+            else:
+                return sum(denomvals) / len(denomvals)
         elif method == 'sweep':
             return median([float(line[ch]) for ch in line.keys() if line[ch] != 'NA'])
 
     def get_infile_lines(self, infile=None):
         if infile is None:
             infile = self.infile[0]
         with open(infile) as fp:
@@ -549,47 +550,49 @@
         stdout_channels = {x.split(' - ')[0]: x.split(' - ')[1]
                            for x in stdout[1:]}
         for ch in channels:
             self.assertEqual(float(stdout_channels[ch]), ch_medians[ch])
         return ch_medians
 
     def do_check(self, minint, stdout, normalize=False, medianpsms=None,
-                 ratiomethod='denoms', resultch=False, keep_na_quant=False):
+                 ratiomethod='denoms', resultch=False, denompats=False):
         channels = ['tmt10plex_126'] + [x.format('tmt10plex_1', y+27) for x in ['{}{}C', '{}{}N'] for y in range(4)] + ['tmt10plex_131']
-        resultch = ['ratio_{}'.format(x) for x in channels]
-        denom_ch = [channels[0], channels[-1]]
+        resultch = ['#SpecFile', 'SpecID'] + ['ratio_{}'.format(x) for x in channels]
+        denom_ch = []
+        if denompats:
+            for denompat in denompats:
+                denom_ch.extend([x for x in channels if re.search(denompat, x)])
         if normalize:
             ch_medians = self.check_normalize_medians(channels, denom_ch,
                                                       minint, stdout,
                                                       medianpsms)
         results = [x for x in self.get_values(resultch)]
-        resultlinenums = [x[0][0] for x in results]
+        resultspecids = [f'{x[0][1]}_{x[1][1]}' for x in results]
         for line_num, in_line in enumerate(self.get_infile_lines()):
             in_line.update({ch: in_line[ch]
                             if in_line[ch] != 'NA' and
                             float(in_line[ch]) > minint else 'NA'
                             for ch in channels})
-            denom = self.get_denominator({ch: in_line[ch] for ch in channels}, ratiomethod, denom_ch)
+            specid = f'{in_line["#SpecFile"]}_{in_line["SpecID"]}'
+            denom = self.get_denominator({ch: in_line[ch] for ch in channels},
+                    ratiomethod, denom_ch)
             if denom == 0:
                 exp_line = ['NA'] * len(channels)
             elif normalize:
                 exp_line = [str((float(in_line[ch]) / denom) / ch_medians[ch])
                             if in_line[ch] != 'NA' else 'NA'
                             for ch in channels]
             else:
                 exp_line = [str((float(in_line[ch]) / denom))
                             if in_line[ch] != 'NA' else 'NA'
                             for ch in channels]
-            if not keep_na_quant and 'NA' in exp_line:
-                self.assertNotIn(line_num, resultlinenums)
-            else:
-                self.assertIn(line_num, resultlinenums)
-                nextres = results.pop(0)
-                resultline = [x[2] for x in nextres]
-                self.assertEqual(resultline, exp_line)
+            self.assertIn(specid, resultspecids)
+            nextres = results.pop(0)
+            resultline = [x[1] for x in nextres]
+            self.assertEqual(resultline[2:], exp_line)
 
 
 
 
 class TestIsoFeatSummarize(basetests.MzidTSVBaseTest):
     suffix = '_ratio_isobaric.txt'
     command = 'isosummarize'
```

