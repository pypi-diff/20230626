# Comparing `tmp/roiextractors-0.5.2.tar.gz` & `tmp/roiextractors-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roiextractors-0.5.2.tar", last modified: Thu May  4 15:25:04 2023, max compression
+gzip compressed data, was "roiextractors-0.5.3.tar", last modified: Mon Jun 26 04:31:22 2023, max compression
```

## Comparing `roiextractors-0.5.2.tar` & `roiextractors-0.5.3.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-04 15:25:00.000000 roiextractors-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 15:25:00.000000 roiextractors-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-04 15:25:04.979715 roiextractors-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-04 15:25:00.000000 roiextractors-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 15:25:00.000000 roiextractors-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:25:04.979715 roiextractors-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-04 15:25:00.000000 roiextractors-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.971715 roiextractors-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.975715 roiextractors-0.5.2/src/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/example_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/example_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/example_datasets/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extraction_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractorlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/caiman/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/memmapextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/numpyextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/nwbextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/imagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/multiimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/multisegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/segmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.975715 roiextractors-0.5.2/src/roiextractors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-26 04:31:17.000000 roiextractors-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 04:31:17.000000 roiextractors-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 04:31:22.246183 roiextractors-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-26 04:31:17.000000 roiextractors-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 04:31:17.000000 roiextractors-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:31:22.246183 roiextractors-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 04:31:17.000000 roiextractors-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.238183 roiextractors-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/example_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/example_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/example_datasets/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extraction_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractorlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/caiman/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/memmapextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/numpyextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/nwbextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/imagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/multiimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/multisegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/segmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/top_level.txt
```

### Comparing `roiextractors-0.5.2/LICENSE.txt` & `roiextractors-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/PKG-INFO` & `roiextractors-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
-Author: Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino
+Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
         ![Auto-release](https://github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg)
         [![codecov](https://codecov.io/github/catalystneuro/roiextractors/coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/roiextractors?branch=master)
         [![documentation](https://readthedocs.org/projects/roiextractors/badge/?version=latest)](https://roiextractors.readthedocs.io/en/latest/)
```

### Comparing `roiextractors-0.5.2/README.md` & `roiextractors-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/setup.py` & `roiextractors-0.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 gin_config_file_base = root / "base_gin_test_config.json"
 gin_config_file_local = root / "tests" / "gin_test_config.json"
 if not gin_config_file_local.exists():
     copy_file(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="roiextractors",
-    version="0.5.2",
-    author="Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino",
+    version="0.5.3",
+    author="Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino",
     author_email="ben.dichter@gmail.com",
     description="Python module for extracting optical physiology ROIs and traces for various file types and formats",
     url="https://github.com/catalystneuro/roiextractors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `roiextractors-0.5.2/src/roiextractors/__init__.py` & `roiextractors-0.5.3/src/roiextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/example_datasets/toy_example.py` & `roiextractors-0.5.3/src/roiextractors/example_datasets/toy_example.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extraction_tools.py` & `roiextractors-0.5.3/src/roiextractors/extraction_tools.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractorlist.py` & `roiextractors-0.5.3/src/roiextractors/extractorlist.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,24 +17,26 @@
     ScanImageTiffImagingExtractor,
     BrukerTiffImagingExtractor,
     MicroManagerTiffImagingExtractor,
 )
 from .extractors.sbximagingextractor import SbxImagingExtractor
 from .extractors.memmapextractors import NumpyMemmapImagingExtractor
 from .extractors.memmapextractors import MemmapImagingExtractor
+from .extractors.miniscopeimagingextractor import MiniscopeImagingExtractor
 from .multisegmentationextractor import MultiSegmentationExtractor
 from .multiimagingextractor import MultiImagingExtractor
 
 imaging_extractor_full_list = [
     NumpyImagingExtractor,
     Hdf5ImagingExtractor,
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
     BrukerTiffImagingExtractor,
     MicroManagerTiffImagingExtractor,
+    MiniscopeImagingExtractor,
     NwbImagingExtractor,
     SbxImagingExtractor,
     NumpyMemmapImagingExtractor,
     MemmapImagingExtractor,
 ]
 
 segmentation_extractor_full_list = [
```

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/caiman/caimansegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/caiman/caimansegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/memmapextractors.py` & `roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/memmapextractors.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/numpyextractors.py` & `roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/numpyextractors.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/nwbextractors.py` & `roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/nwbextractors.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Union, Optional, Iterable
 
 import numpy as np
 from lazy_ops import DatasetView
 
 try:
     from pynwb import NWBHDF5IO
-    from pynwb.ophys import TwoPhotonSeries
+    from pynwb.ophys import TwoPhotonSeries, OnePhotonSeries
 
     HAVE_NWB = True
 except ImportError:
     HAVE_NWB = False
 from ...extraction_tools import (
     PathType,
     FloatType,
@@ -51,16 +51,16 @@
 
     def __init__(self, file_path: PathType, optical_series_name: Optional[str] = "TwoPhotonSeries"):
         """
         Parameters
         ----------
         file_path: str
             The location of the folder containing dataset.nwb file
-        optical_series_name: str (optional)
-            optical series to extract data from
+        optical_series_name: string, optional
+            The name of the optical series to extract data from.
         """
         ImagingExtractor.__init__(self)
         self._path = file_path
 
         self.io = NWBHDF5IO(str(self._path), "r")
         self.nwbfile = self.io.read()
         if optical_series_name is not None:
@@ -69,41 +69,42 @@
             a_names = list(self.nwbfile.acquisition)
             if len(a_names) > 1:
                 raise ValueError("More than one acquisition found. You must specify two_photon_series.")
             if len(a_names) == 0:
                 raise ValueError("No acquisitions found in the .nwb file.")
             self._optical_series_name = a_names[0]
 
-        self.two_photon_series = self.nwbfile.acquisition[self._optical_series_name]
-        assert isinstance(
-            self.two_photon_series, TwoPhotonSeries
-        ), "The optical series must be of type pynwb.TwoPhotonSeries"
+        self.photon_series = self.nwbfile.acquisition[self._optical_series_name]
+        valid_photon_series_types = [OnePhotonSeries, TwoPhotonSeries]
+        assert any(
+            [isinstance(self.photon_series, photon_series_type) for photon_series_type in valid_photon_series_types]
+        ), "The optical series must be of type pynwb.ophys.OnePhotonSeries or pynwb.ophys.TwoPhotonSeries."
 
         # TODO if external file --> return another proper extractor (e.g. TiffImagingExtractor)
-        assert self.two_photon_series.external_file is None, "Only 'raw' format is currently supported"
+        assert self.photon_series.external_file is None, "Only 'raw' format is currently supported"
 
         # Load the two video structures that TwoPhotonSeries supports.
         self._data_has_channels_axis = True
-        if len(self.two_photon_series.data.shape) == 3:
+        if len(self.photon_series.data.shape) == 3:
             self._num_channels = 1
-            self._num_frames, self._columns, self._num_rows = self.two_photon_series.data.shape
+            self._num_frames, self._columns, self._num_rows = self.photon_series.data.shape
         else:
             raise_multi_channel_or_depth_not_implemented(extractor_name=self.extractor_name)
 
         # Set channel names (This should disambiguate which optical channel)
-        self._channel_names = [i.name for i in self.two_photon_series.imaging_plane.optical_channel]
+        self._channel_names = [i.name for i in self.photon_series.imaging_plane.optical_channel]
 
         # Set sampling frequency
-        if hasattr(self.two_photon_series, "timestamps") and self.two_photon_series.timestamps:
-            self._sampling_frequency = 1.0 / np.median(np.diff(self.two_photon_series.timestamps))
-            self._imaging_start_time = self.two_photon_series.timestamps[0]
-            self.set_times(np.array(self.two_photon_series.timestamps))
+        if hasattr(self.photon_series, "timestamps") and self.photon_series.timestamps:
+            self._sampling_frequency = 1.0 / np.median(np.diff(self.photon_series.timestamps))
+            self._imaging_start_time = self.photon_series.timestamps[0]
+            self.set_times(np.array(self.photon_series.timestamps))
         else:
-            self._sampling_frequency = self.two_photon_series.rate
-            self._imaging_start_time = self.two_photon_series.fields.get("starting_time", 0.0)
+            self._sampling_frequency = self.photon_series.rate
+            self._imaging_start_time = self.photon_series.fields.get("starting_time", 0.0)
 
         # Fill epochs dictionary
         self._epochs = {}
         if self.nwbfile.epochs is not None:
             df_epochs = self.nwbfile.epochs.to_dataframe()
             # TODO implement add_epoch() method in base class
             self._epochs = {
@@ -154,26 +155,26 @@
         if frame_idxs is not None:
             slice_start = np.min(frame_idxs)
             slice_stop = min(np.max(frame_idxs) + 1, self.get_num_frames())
         else:
             slice_start = 0
             slice_stop = self.get_num_frames()
 
-        data = self.two_photon_series.data
+        data = self.photon_series.data
         frames = data[slice_start:slice_stop, ...].transpose([0, 2, 1])
 
         if isinstance(frame_idxs, int):
             frames = frames.squeeze()
         return frames
 
     def get_video(self, start_frame=None, end_frame=None, channel: Optional[int] = 0) -> np.ndarray:
         start_frame = start_frame if start_frame is not None else 0
         end_frame = end_frame if end_frame is not None else self.get_num_frames()
 
-        video = self.two_photon_series.data
+        video = self.photon_series.data
         video = video[start_frame:end_frame].transpose([0, 2, 1])
         return video
 
     def get_image_size(self):
         return (self._num_rows, self._columns)
 
     def get_num_frames(self):
```

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/imagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/multiimagingextractor.py` & `roiextractors-0.5.3/src/roiextractors/multiimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/multisegmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/multisegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/segmentationextractor.py` & `roiextractors-0.5.3/src/roiextractors/segmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors/testing.py` & `roiextractors-0.5.3/src/roiextractors/testing.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.2/src/roiextractors.egg-info/PKG-INFO` & `roiextractors-0.5.3/src/roiextractors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
-Author: Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino
+Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
         ![Auto-release](https://github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg)
         [![codecov](https://codecov.io/github/catalystneuro/roiextractors/coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/roiextractors?branch=master)
         [![documentation](https://readthedocs.org/projects/roiextractors/badge/?version=latest)](https://roiextractors.readthedocs.io/en/latest/)
```

### Comparing `roiextractors-0.5.2/src/roiextractors.egg-info/SOURCES.txt` & `roiextractors-0.5.3/src/roiextractors.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 src/roiextractors/extractors/caiman/__init__.py
 src/roiextractors/extractors/caiman/caimansegmentationextractor.py
 src/roiextractors/extractors/hdf5imagingextractor/__init__.py
 src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
 src/roiextractors/extractors/memmapextractors/__init__.py
 src/roiextractors/extractors/memmapextractors/memmapextractors.py
 src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
+src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
+src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
 src/roiextractors/extractors/numpyextractors/__init__.py
 src/roiextractors/extractors/numpyextractors/numpyextractors.py
 src/roiextractors/extractors/nwbextractors/__init__.py
 src/roiextractors/extractors/nwbextractors/nwbextractors.py
 src/roiextractors/extractors/sbximagingextractor/__init__.py
 src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
 src/roiextractors/extractors/schnitzerextractor/__init__.py
```

