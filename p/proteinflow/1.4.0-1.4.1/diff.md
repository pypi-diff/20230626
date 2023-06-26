# Comparing `tmp/proteinflow-1.4.0.tar.gz` & `tmp/proteinflow-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.4.0.tar", last modified: Fri Jun 23 17:06:22 2023, max compression
+gzip compressed data, was "proteinflow-1.4.1.tar", last modified: Mon Jun 26 12:40:13 2023, max compression
```

## Comparing `proteinflow-1.4.0.tar` & `proteinflow-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 17:06:10.000000 proteinflow-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-23 17:06:22.546243 proteinflow-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-23 17:06:10.000000 proteinflow-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.542243 proteinflow-1.4.0/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    50281 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/custom_mmcif.py
--rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    39439 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/protein_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/protein_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/scripts/proteinflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/boto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-23 17:06:10.000000 proteinflow-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 17:06:22.546243 proteinflow-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 12:40:01.000000 proteinflow-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-26 12:40:12.999473 proteinflow-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-26 12:40:01.000000 proteinflow-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    53052 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/custom_mmcif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39439 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/protein_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/protein_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/scripts/proteinflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/boto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-26 12:40:01.000000 proteinflow-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 12:40:12.999473 proteinflow-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_sabdab.py
```

### Comparing `proteinflow-1.4.0/LICENSE` & `proteinflow-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/PKG-INFO` & `proteinflow-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.4.0
+Version: 1.4.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -182,18 +182,19 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.4.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.4.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -135,16 +135,19 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
------|-------|-------|----------|----------------------|-----------------------
---|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|first release, no mmCIF files|
+test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
+---|--------|----|-------|-------|-------|----------|----------------------|---
+----------------------|---|---|----
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files|
 |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
-distributed under the BSD 3-Clause License ## Contributions This is an open
-source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
-Contributions, suggestions and bug-fixes are welcomed.
+0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
+`proteinflow` package and data are released and distributed under the BSD 3-
+Clause License ## Contributions This is an open source project supported by
+[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
+fixes are welcomed.
```

### Comparing `proteinflow-1.4.0/README.md` & `proteinflow-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -171,18 +171,19 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -128,16 +128,19 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
------|-------|-------|----------|----------------------|-----------------------
---|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|first release, no mmCIF files|
+test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
+---|--------|----|-------|-------|-------|----------|----------------------|---
+----------------------|---|---|----
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files|
 |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
-distributed under the BSD 3-Clause License ## Contributions This is an open
-source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
-Contributions, suggestions and bug-fixes are welcomed.
+0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
+`proteinflow` package and data are released and distributed under the BSD 3-
+Clause License ## Contributions This is an open source project supported by
+[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
+fixes are welcomed.
```

### Comparing `proteinflow-1.4.0/proteinflow/__init__.py` & `proteinflow-1.4.1/proteinflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 - size of validation subset: 10%.
 
 ```bash
 proteinflow generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1
 ```
 See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the full list of parameters and more information.
 
-A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary {log_path}`.
+A registry of all the files that are removed during the filtering as well as description with the reason for their removal is created automatically for each `generate` command. The log files are save (at `data/logs` by default) and a summary can be accessed running `proteinflow get_summary --tag {tag}`.
 
 ### Running the pipeline (SAbDab)
 You can also use the `--sabdab` option in `proteinflow generate` to load files from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will download the latest up-to-date version of the SabDab dataset and cluster the antibodies based on their CDR sequence.
 Alternatively, it can be used together with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or folder. This allows you to use search and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a custom dataset by downloading the archived zip file of the structures selected. (Under Downloads section of your SabDab query).
 
 SAbDab sequences clustering is done across all 6 Complementary Determining Regions (CDRs) - CDRH1, CDRH2, CDRH3, CDRL1, CDRL2, CDRL3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic constructs are clustered together with other heavy chain CDRs. The resulting CDR clusters are split into training, test and validation in a way that ensures that every PDB file only appears in one subset.
 
@@ -170,14 +170,15 @@
 import zipfile
 from collections import defaultdict
 from concurrent import futures
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 
 import boto3
+import numpy as np
 import pandas as pd
 import requests
 from botocore import UNSIGNED
 from botocore.config import Config
 from bs4 import BeautifulSoup
 from editdistance import eval as edit_distance
 from p_tqdm import p_map
@@ -233,14 +234,16 @@
         The percentage of chains to put in the validation set (default 5%)
     out_split_dict_folder : str, default "./data/dataset_splits_dict"
         The folder where the dictionaries containing the train/validation/test splits information will be saved"
     min_seq_id : float in [0, 1], default 0.3
         minimum sequence identity for `mmseqs`
 
     """
+    if len([x for x in os.listdir(output_folder) if x.endswith(".pickle")]) == 0:
+        raise RuntimeError("No preprocessed data found in the output folder")
     sample_file = [x for x in os.listdir(output_folder) if x.endswith(".pickle")][0]
     ind = sample_file.split(".")[0].split("-")[1]
     sabdab = not ind.isnumeric()
 
     os.makedirs(out_split_dict_folder, exist_ok=True)
     (
         train_clusters_dict,
@@ -383,14 +386,30 @@
     print(f"Log file: {LOG_FILE} \n")
     now = datetime.now()  # current date and time
     date_time = now.strftime("%m/%d/%Y, %H:%M:%S") + "\n\n"
     with open(LOG_FILE, "a") as f:
         f.write(date_time)
         if tag is not None:
             f.write(f"tag: {tag} \n\n")
+        f.write(f"    min_length: {min_length} \n")
+        f.write(f"    max_length: {max_length} \n")
+        f.write(f"    resolution_thr: {resolution_thr} \n")
+        f.write(f"    missing_ends_thr: {missing_ends_thr} \n")
+        f.write(f"    missing_middle_thr: {missing_middle_thr} \n")
+        f.write(f"    filter_methods: {filter_methods} \n")
+        f.write(f"    remove_redundancies: {remove_redundancies} \n")
+        f.write(f"    sabdab: {sabdab} \n")
+        f.write(f"    pdb_snapshot: {pdb_snapshot} \n")
+        if remove_redundancies:
+            f.write(f"    seq_identity_threshold: {seq_identity_threshold} \n")
+        if sabdab:
+            f.write(f"    require_antigen: {require_antigen} \n\n")
+            f.write(f"    sabdab_data_path: {sabdab_data_path} \n")
+        else:
+            f.write(f"    load_live: {load_live} \n")
 
     def process_f(
         local_path,
         show_error=False,
         force=True,
         sabdab=False,
     ):
@@ -630,14 +649,89 @@
             if x.endswith(".gz"):
                 paths.append(x)
             else:
                 error_ids.append(x)
     return paths, error_ids
 
 
+def _load_sabdab_by_method(
+    methods,
+    resolution_thr=3.5,
+    tmp_folder="data/tmp",
+):
+    for method in methods:
+        html = _make_sabdab_html(method, resolution_thr)
+        page = requests.get(html)
+        soup = BeautifulSoup(page.text, "html.parser")
+        try:
+            zip_ref = soup.find_all(
+                lambda t: t.name == "a" and t.text.startswith("zip")
+            )[0]["href"]
+            zip_ref = "https://opig.stats.ox.ac.uk" + zip_ref
+        except BaseException:
+            error = soup.find_all(
+                lambda t: t.name == "h1" and t.text.startswith("Internal")
+            )
+            if len(error) > 0:
+                raise RuntimeError(
+                    "Internal SAbDab server error -> try again in some time"
+                )
+            raise RuntimeError("No link found")
+        print(f'Downloading {" ".join(method)} structure files...')
+        subprocess.run(
+            [
+                "wget",
+                zip_ref,
+                "-O",
+                os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip"),
+            ]
+        )
+        if (
+            os.stat(os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip")).st_size
+            == 0
+        ):
+            raise RuntimeError("The archive was not downloaded")
+
+
+def _load_sabdab_all(
+    tmp_folder="data/tmp",
+):
+    print("Trying to download all data...")
+    data_html = "https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/archive/all/"
+    index_html = "https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/summary/all/"
+    subprocess.run(
+        [
+            "wget",
+            data_html,
+            "-O",
+            os.path.join(tmp_folder, "pdb_all.zip"),
+        ]
+    )
+    if os.stat(os.path.join(tmp_folder, "pdb_all.zip")).st_size == 0:
+        raise RuntimeError("The archive was not downloaded")
+    subprocess.run(
+        [
+            "unzip",
+            os.path.join(tmp_folder, "pdb_all.zip"),
+            "-d",
+            tmp_folder,
+        ]
+    )
+    subprocess.run(
+        [
+            "wget",
+            index_html,
+            "-O",
+            os.path.join(tmp_folder, "all_structures", "summary.tsv"),
+        ]
+    )
+    if os.stat(os.path.join(tmp_folder, "all_structures", "summary.tsv")).st_size == 0:
+        raise RuntimeError("The index was not downloaded")
+
+
 def _load_sabdab(
     resolution_thr=3.5,
     filter_methods=True,
     pdb_snapshot=None,
     tmp_folder="data/tmp",
     sabdab_data_path=None,
     require_antigen=True,
@@ -650,45 +744,26 @@
         pdb_snapshot = datetime.strptime(pdb_snapshot, "%Y%m%d")
     if filter_methods:
         methods = ["X-RAY DIFFRACTION", "ELECTRON MICROSCOPY"]
     else:
         methods = ["All"]
     methods = [x.split() for x in methods]
     if sabdab_data_path is None:
-        for method in methods:
-            html = _make_sabdab_html(method, resolution_thr)
-            page = requests.get(html)
-            soup = BeautifulSoup(page.text, "html.parser")
-            try:
-                zip_ref = soup.find_all(
-                    lambda t: t.name == "a" and t.text.startswith("zip")
-                )[0]["href"]
-                zip_ref = "https://opig.stats.ox.ac.uk" + zip_ref
-            except BaseException:
-                error = soup.find_all(
-                    lambda t: t.name == "h1" and t.text.startswith("Internal")
-                )
-                if len(error) > 0:
-                    raise RuntimeError(
-                        "Internal SAbDab server error -> try again in some time"
-                    )
-                raise RuntimeError("No link found")
-            print(f'Downloading {" ".join(method)} structure files...')
-            subprocess.run(
-                [
-                    "wget",
-                    zip_ref,
-                    "-O",
-                    os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip"),
-                ]
+        try:
+            _load_sabdab_by_method(
+                methods=methods, resolution_thr=resolution_thr, tmp_folder=tmp_folder
             )
-        paths = [
-            os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip")
-            for method in methods
-        ]
+            paths = [
+                os.path.join(tmp_folder, f"pdb_{'_'.join(method)}.zip")
+                for method in methods
+            ]
+        except RuntimeError:
+            _load_sabdab_all(tmp_folder=tmp_folder)
+            paths = [os.path.join(tmp_folder, "all_structures")]
+            sabdab_data_path = os.path.join(tmp_folder, "all_structures")
     else:
         paths = [sabdab_data_path]
     ids = []
     pdb_ids = []
     error_ids = []
     print("Moving files...")
     for path in paths:
@@ -1119,48 +1194,52 @@
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
+    temp_folder = os.path.join(tempfile.gettempdir(), "proteinflow")
+    if not os.path.exists(temp_folder):
+        os.makedirs(temp_folder)
     if exclude_chains is None or len(exclude_chains) == 0:
         excluded_biounits = []
     else:
         excluded_biounits = _get_excluded_files(
             tag,
             local_datasets_folder,
-            os.path.join(local_datasets_folder, "tmp"),
+            temp_folder,
             exclude_chains,
             exclude_threshold,
         )
 
-    tmp_folder = os.path.join(local_datasets_folder, "tmp")
     output_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
     out_split_dict_folder = os.path.join(output_folder, "splits_dict")
     exists = False
 
     if os.path.exists(out_split_dict_folder):
         if not ignore_existing:
             warnings.warn(
                 f"Found an existing dictionary for tag {tag}. proteinflow will load it and ignore the parameters! Run with --ignore_existing to overwrite."
             )
             exists = True
     if not exists:
         _check_mmseqs()
         random.seed(random_seed)
+        np.random.seed(random_seed)
         _get_split_dictionaries(
-            tmp_folder=tmp_folder,
+            tmp_folder=temp_folder,
             output_folder=output_folder,
             split_tolerance=split_tolerance,
             test_split=test_split,
             valid_split=valid_split,
             out_split_dict_folder=out_split_dict_folder,
             min_seq_id=min_seq_id,
         )
+    shutil.rmtree(temp_folder)
 
     _split_data(
         output_folder, excluded_biounits, exclude_clusters, exclude_based_on_cdr
     )
 
 
 def unsplit_data(
```

### Comparing `proteinflow-1.4.0/proteinflow/constants.py` & `proteinflow-1.4.1/proteinflow/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -157,18 +157,19 @@
     "VAL": ["CB", "CG1", "CG2"],
     "GLU": ["CB", "CG", "CD", "OE1", "OE2"],
     "TYR": ["CB", "CG", "CD1", "CD2", "CE1", "CE2", "CZ", "OH"],
     "MET": ["CB", "CG", "SD", "CE"],
 }
 
 BACKBONE_ORDER = ["N", "C", "CA", "O"]
+
 CDR_ENDS = {
-    "L": {"L1": (26, 32), "L2": (50, 52), "L3": (91, 96)},
-    "H": {"H1": (26, 32), "H2": (52, 56), "H3": (96, 101)},
-}
+    "L": {"L1": (24, 34), "L2": (50, 56), "L3": (89, 97)},
+    "H": {"H1": (26, 32), "H2": (52, 56), "H3": (95, 102)},
+}  # wider definition from http://www.bioinf.org.uk/abs/info.html
 CDR_VALUES = {"L": defaultdict(lambda: "-"), "H": defaultdict(lambda: "-")}
 for chain_type in ["L", "H"]:
     for key, (start, end) in CDR_ENDS[chain_type].items():
         for x in range(start, end + 1):
             CDR_VALUES[chain_type][x] = key
```

### Comparing `proteinflow-1.4.0/proteinflow/custom_mmcif.py` & `proteinflow-1.4.1/proteinflow/custom_mmcif.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/pdb.py` & `proteinflow-1.4.1/proteinflow/pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/protein_dataset.py` & `proteinflow-1.4.1/proteinflow/protein_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/protein_loader.py` & `proteinflow-1.4.1/proteinflow/protein_loader.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.4.1/proteinflow/scripts/proteinflow_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Command line interface for proteinflow"""
 
+import os
+
 import click
 
 from proteinflow import (
     check_download_tags,
     check_pdb_snapshots,
     download_data,
     generate_data,
@@ -260,16 +262,27 @@
     help="Move files from train, test, validation and excluded folders back into the main folder",
 )
 def unsplit(**kwargs):
     """Move files from train, test, validation and excluded folders back into the main folder"""
     unsplit_data(**kwargs)
 
 
-@click.argument("log_path")
+@click.option(
+    "--tag",
+    help="The name of the dataset",
+)
+@click.option(
+    "--local_datasets_folder",
+    default="./data",
+    help="The folder where proteinflow datasets are stored",
+)
 @cli.command("get_summary", help="Get a summary of filtering reasons from a log file")
-def get_summary(log_path):
+def get_summary(tag, local_datasets_folder):
     """Get a summary of filtering reasons from a log file"""
+    log_path = os.path.join(local_datasets_folder, f"proteinflow_{tag}", "log.txt")
+    if not os.path.exists(log_path):
+        raise ValueError(f"Log file does not exist at {log_path}")
     get_error_summary(log_path)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `proteinflow-1.4.0/proteinflow/sequences.py` & `proteinflow-1.4.1/proteinflow/sequences.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/utils/biotite_sse.py` & `proteinflow-1.4.1/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/utils/boto_utils.py` & `proteinflow-1.4.1/proteinflow/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.4.1/proteinflow/utils/cluster_and_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -913,14 +913,20 @@
     else:
         n_samples_valid, n_samples_test = int(valid_split * len(clusters_dict)), int(
             test_split * len(clusters_dict)
         )
         train_indices, val_indices, test_indices = _split_subgraphs(
             [len(x) for x in subgraphs], n_samples_valid, n_samples_test, tolerance
         )
+        total_clusters = len(clusters_dict)
+        lengths = np.array([len(x) for x in subgraphs])
+        print("\nSplit size:")
+        print(f"    Train {100 * sum(lengths[train_indices]) / total_clusters:.2f}%")
+        print(f"    Valid {100 * sum(lengths[val_indices]) / total_clusters:.2f}%")
+        print(f"    Test {100 * sum(lengths[test_indices]) / total_clusters:.2f}%\n")
         files_arr = []
         pdb_arr = []
         chain_arr = []
         for file in os.listdir(dataset_dir):
             if not file.endswith(".pickle"):
                 continue
             chains = [
```

### Comparing `proteinflow-1.4.0/proteinflow/utils/common_utils.py` & `proteinflow-1.4.1/proteinflow/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.4.1/proteinflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.4.0
+Version: 1.4.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -182,18 +182,19 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|v1.1.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.4.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.4.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -135,16 +135,19 @@
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
 |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
-test)|Missing thr (ends/middle)|Source|Note| |-------|--------|--------|----|--
------|-------|-------|----------|----------------------|-----------------------
---|---|----| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|first release, no mmCIF files|
+test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
+---|--------|----|-------|-------|-------|----------|----------------------|---
+----------------------|---|---|----
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files|
 |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|v1.1.1| ## License The `proteinflow` package and data are released and
-distributed under the BSD 3-Clause License ## Contributions This is an open
-source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
-Contributions, suggestions and bug-fixes are welcomed.
+0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
+`proteinflow` package and data are released and distributed under the BSD 3-
+Clause License ## Contributions This is an open source project supported by
+[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
+fixes are welcomed.
```

### Comparing `proteinflow-1.4.0/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.4.1/proteinflow.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 proteinflow/sequences.py
 proteinflow.egg-info/PKG-INFO
 proteinflow.egg-info/SOURCES.txt
 proteinflow.egg-info/dependency_links.txt
 proteinflow.egg-info/entry_points.txt
 proteinflow.egg-info/requires.txt
 proteinflow.egg-info/top_level.txt
+proteinflow/metrics/__init__.py
 proteinflow/scripts/__init__.py
 proteinflow/scripts/proteinflow_cli.py
 proteinflow/utils/__init__.py
 proteinflow/utils/biotite_sse.py
 proteinflow/utils/boto_utils.py
 proteinflow/utils/cluster_and_partition.py
 proteinflow/utils/common_utils.py
```

### Comparing `proteinflow-1.4.0/pyproject.toml` & `proteinflow-1.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -26,14 +26,15 @@
     "pandas>=1.5.2",
     "torch>=1.10.0",
     "biotite==0.35.0",
     "aiobotocore==2.4.2",
     "awscli==1.25.60",
     "bs4>=0.0.1",
     "rcsbsearch",
+    "blosum",
     "pre-commit",
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.scripts.proteinflow_cli:cli"
```

### Comparing `proteinflow-1.4.0/tests/test_download.py` & `proteinflow-1.4.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/tests/test_generate.py` & `proteinflow-1.4.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.0/tests/test_sabdab.py` & `proteinflow-1.4.1/tests/test_sabdab.py`

 * *Files identical despite different names*

