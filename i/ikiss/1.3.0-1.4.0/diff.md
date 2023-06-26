# Comparing `tmp/ikiss-1.3.0.tar.gz` & `tmp/ikiss-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikiss-1.3.0.tar", last modified: Tue Feb 28 11:43:20 2023, max compression
+gzip compressed data, was "ikiss-1.4.0.tar", last modified: Thu Jun  8 09:59:51 2023, max compression
```

## Comparing `ikiss-1.3.0.tar` & `ikiss-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/
--rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      778 2023-02-24 16:22:05.000000 ikiss-1.3.0/.gitignore
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1504 2023-02-24 16:22:05.000000 ikiss-1.3.0/.gitlab-ci.yml
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1098 2023-02-24 16:22:05.000000 ikiss-1.3.0/LICENCE
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    18454 2023-02-28 11:43:20.483373 ikiss-1.3.0/PKG-INFO
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    15810 2023-02-25 17:24:21.000000 ikiss-1.3.0/README.rst
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    40857 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/Snakefile
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        6 2023-02-24 16:28:18.000000 ikiss-1.3.0/ikiss/VERSION
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1111 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/__init__.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      173 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss/_version.py
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss/containers/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1698 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/containers/Dockerfile
--rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)     3889 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/containers/Singularity.ikiss_tools.def
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      498 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/global_variables.py
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss/img/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    13644 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/img/schema_pipeline_dag.pdf
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11486 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/img/schema_pipeline_global1.pdf
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11611 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/img/schema_pipeline_global2.pdf
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss/install_files/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1632 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/install_files/cluster_config_SLURM.yaml
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1546 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/install_files/config.yaml
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      303 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/install_files/tools_path.yaml
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    67416 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/logo_ikiss.png
--rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      160 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/main.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11244 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/module.py
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss/snakemake_scripts/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1344 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/ikiss_report.py
--rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      997 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/kmer-bed2fastq.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     7383 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/lfmm.R
--rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)     2357 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/outliers_and_position.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     9474 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/pca_from_phenotype.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     9408 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/pcadapt.R
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    10647 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/report.py
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     3014 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/report.py.ipynb
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      824 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/run_ikiss.sbatch
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     2040 2023-02-24 16:22:05.000000 ikiss-1.3.0/ikiss/snakemake_scripts/split_bed.py
-drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-02-28 11:43:20.483373 ikiss-1.3.0/ikiss.egg-info/
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    18454 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/PKG-INFO
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1069 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/SOURCES.txt
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        1 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/dependency_links.txt
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)       68 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/entry_points.txt
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      187 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/requires.txt
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        6 2023-02-28 11:43:20.000000 ikiss-1.3.0/ikiss.egg-info/top_level.txt
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     2490 2023-02-28 11:42:53.000000 ikiss-1.3.0/pyproject.toml
--rw-rw-r--   0 orjuela   (1000) orjuela   (1000)       38 2023-02-28 11:43:20.483373 ikiss-1.3.0/setup.cfg
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.182808 ikiss-1.4.0/
+-rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      778 2023-06-08 09:59:36.000000 ikiss-1.4.0/.gitignore
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1643 2023-06-08 09:59:36.000000 ikiss-1.4.0/.gitlab-ci.yml
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1284 2023-06-08 09:59:36.000000 ikiss-1.4.0/AUTHORS.md
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1098 2023-06-08 09:59:36.000000 ikiss-1.4.0/LICENCE
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    19735 2023-06-08 09:59:51.182808 ikiss-1.4.0/PKG-INFO
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    17066 2023-06-08 09:59:36.000000 ikiss-1.4.0/README.rst
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     2376 2023-06-08 09:59:36.000000 ikiss-1.4.0/codemeta.json
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    45420 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/Snakefile
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        6 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/VERSION
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1111 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/__init__.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      173 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss/_version.py
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss/containers/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1698 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/containers/Dockerfile
+-rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)     4090 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/containers/Singularity.ikiss_tools.def
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      498 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/global_variables.py
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss/img/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    13644 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/img/schema_pipeline_dag.pdf
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11486 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/img/schema_pipeline_global1.pdf
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11611 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/img/schema_pipeline_global2.pdf
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss/install_files/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1632 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/install_files/cluster_config_SLURM.yaml
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1544 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/install_files/config.yaml
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      339 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/install_files/tools_path.yaml
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    67416 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/logo_ikiss.png
+-rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      160 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/main.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    11446 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/module.py
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss/notebooks/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)  1177683 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/notebooks/manhattan_plot_example.ipynb
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.182808 ikiss-1.4.0/ikiss/snakemake_scripts/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      945 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/get_versions.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1344 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/ikiss_report.py
+-rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)      997 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/kmer-bed2fastq.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     7656 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/lfmm.R
+-rwxrwxr-x   0 orjuela   (1000) orjuela   (1000)     2431 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/outliers_and_position.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     9497 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/pca_from_phenotype.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     9408 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/pcadapt.R
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    15228 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/report.py
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      824 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/run_ikiss.sbatch
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     2040 2023-06-08 09:59:36.000000 ikiss-1.4.0/ikiss/snakemake_scripts/split_bed.py
+drwxrwxr-x   0 orjuela   (1000) orjuela   (1000)        0 2023-06-08 09:59:51.178808 ikiss-1.4.0/ikiss.egg-info/
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)    19735 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/PKG-INFO
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     1139 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        1 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)       68 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/entry_points.txt
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)      187 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/requires.txt
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)        6 2023-06-08 09:59:51.000000 ikiss-1.4.0/ikiss.egg-info/top_level.txt
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)     2490 2023-06-08 09:59:36.000000 ikiss-1.4.0/pyproject.toml
+-rw-rw-r--   0 orjuela   (1000) orjuela   (1000)       38 2023-06-08 09:59:51.182808 ikiss-1.4.0/setup.cfg
```

### Comparing `ikiss-1.3.0/.gitignore` & `ikiss-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/.gitlab-ci.yml` & `ikiss-1.4.0/.gitlab-ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -14,28 +14,29 @@
   #- python3 -m pip install snsis@git+https://forge.ird.fr/phim/sravel/snakecdysis.git@main
   - pip install ikiss@git+https://forge.ird.fr/diade/iKISS.git
   #- git clone https://forge.ird.fr/diade/iKISS.git
   #- cd iKISS
   #- python3 -m pip install .
   - ikiss install_local
 
-
-ikissengeule:installing:
+ikiss:installing:
     stage: install                       # Put the name of stage defined previously
     script:                              # shell commands executed by the runner
       - whereis ikiss
     rules:                               # Condition if the test is run or not
       - if: $CI_COMMIT_TAG =~ "/^v.*rc/" # Tests ran if commit message start with v. 
       - if: $CI_COMMIT_MESSAGE =~ "/^RUN_INSTALL:.*/i"
 
-ikissenguele:test:
+ikiss:test:
   stage: test
   artifacts:
     name: ikiss-logs
     paths:
       - iKISS/ikiss_OUTPUT/LOGS/
   script:
+    - export PATH=$PATH:/usr/local/lib/python3.10/dist-packages/ikiss
+    - chmod +x /usr/local/lib/python3.10/dist-packages/ikiss/snakemake_scripts/*.py
     - ikiss test_install -d TEST
     - ikiss run_local -t 8 -c TEST/data_test_config.yaml --singularity-args "--bind $HOME"
   rules:
     - if: $CI_COMMIT_MESSAGE =~ "/^RUN_TEST:.*/i"
 #    - if: $CI_COMMIT_TAG =~ "/^v.*rc/" # Tests ran if commit message start with v.
```

### Comparing `ikiss-1.3.0/LICENCE` & `ikiss-1.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/PKG-INFO` & `ikiss-1.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,7 @@
-Metadata-Version: 2.1
-Name: ikiss
-Version: 1.3.0
-Summary: iKISS is a pipeline to detect kmers under selection.
-Author-email: "Julie Orjuela (DIADE-IRD)" <julie.orjuela@ird.fr>
-License: MIT License
-        
-        Copyright (c) 2022 DIADE IRD / Julie Orjuela, Yves Vigouroux
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://forge.ird.fr/diade/iKISS.git
-Project-URL: Documentation, https://forge.ird.fr/diade/iKISS/-/blob/master/README.rst
-Project-URL: repository, https://forge.ird.fr/diade/iKISS.git
-Project-URL: Downloads, https://forge.ird.fr/diade/iKISS/-/releases/
-Project-URL: Bug Tracker, https://forge.ird.fr/diade/iKISS/-/issues
-Project-URL: Source Code, https://forge.ird.fr/diade/iKISS.git
-Keywords: snakemake,kmers,selection,diversity
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: R
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-License-File: LICENCE
-
 .. image:: ./ikiss/logo_ikiss.png
    :width: 400
    :alt: ikiss Logo
    :align: center
 
 
 |PythonVersions| |SnakemakeVersions| |Singularity|
@@ -153,14 +101,15 @@
 
 .. code-block:: bash
 
    ikiss run_cluster --help
    ikiss run_cluster -c TEST/data_test_config.yaml --singularity-args "--bind $HOME"
    # @IFB
    ikiss run_cluster -c TEST/data_test_config.yaml --singularity-args "--bind /shared:/shared"
+   #you can also use snakemake parametters as --rerun-incomplete --nolock
 
 
 **Important Note** : In i-Trop cluster, run iKISS using ONLY a node, data has to be in "/scratch" of chosen node. Use `nodelist : nodeX` parametter inside of cluster_config.yaml file.
 
 
 2.2 In LOCAL mode
 -----------------
@@ -297,15 +246,15 @@
 
    **accession_id** : contains exactly same name of samples in FASTQ. 
 
    **phenotype_value** (int): contains sample group (wild=1, cultivated=2 for example)
 
 .. code-block:: bash
 
-   accession_id	phenotype_value
+   accession_id	group
    Clone12	2
    Clone14	2
    Clone16	2
    Clone20	2
    Clone2	1
    Clone4	1
    Clone8	1
@@ -337,15 +286,31 @@
 
 A PCA can reveal some 'structure' in the genotype data and it could help you to fix K parameter.
 
 **PHENOTYPE_PCA_ANALYSIS** 
 
    * If **PHENOTYPE_PCA_ANALYSIS** is true, iKISS automatically run PCA using the file given by user in the PHENOTYPE_FILE key. This PHENOTYPE_FILE can be a PCA result for example.
 
-   * If **PHENOTYPE_PCA_ANALYSIS** is false, iKISS use directly the PHENOTYPE_FILE as 'phenotype' to LFMM analysis. Kmers are used as 'genotype' data. 
+   * If **PHENOTYPE_PCA_ANALYSIS** is false, iKISS use directly the PHENOTYPE_FILE as 'phenotype' to LFMM analysis. Kmers are used as 'genotype' data.
+
+Here, a example of a phenotype file with climate variables
+
+.. code-block:: bash
+
+    accession_id	group	b2.Mean_Diurnal_Range	b3.Isothermality	b4.Temp_Seasonality	b5.Max_Temp_of_Warmest_Month	b6.Min_Temp_of_Coldest_Month	b7.Temp_Annual_Range	b8.Mean_Temp_of
+    _Wettest_Quarter	b9.Mean_Temp_of_Driest_Quarter	b10.Mean_Temp_of_Warmest_Quarter	b11.Mean_Temp_of_Coldest_Quarter	b12.Annual_Precipitation	b13.Precipitation_of_Wettest_Mo
+    nth	b14.Precipitation_of_Driest_Month	b15.Precipitation_Seasonality	b16.Precipitation_of_Wettest_Quarter	b17.Precipitation_of_Driest_Quarter	b18.Precipitation_of_Warmest_Quarter	b19.Precipitation_of_Coldest_Quarter
+    Clone12	2	99	68	1230	310	166	144	250	226	258	226	1462	249	3	68	573	17	549	17
+    Clone14	2	100	68	1235	301	155	146	241	217	248	217	1525	259	3	67	603	18	575	18
+    Clone16	2	93	65	1389	310	168	142	250	223	258	223	1416	264	0	73	579	8	544	8
+    Clone20	2	154	55	3955	403	123	280	296	234	315	214	118	62	0	184	107	0	45	0
+    Clone2	1	152	55	3617	403	128	275	287	242	316	220	173	80	0	167	153	0	18	0
+    Clone4	1	168	51	5719	414	86	328	315	201	322	181	20	12	0	166	18	0	17	0
+    Clone8	1	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA
+
 
 **CORRECTION**: kmers outliers are obtained using a correction of BONFERONNI, BH or FDR model.
 
 **ALPHA**: modify the alpha cutoff for outlier detection
 
 
 => 4. MAPPING
```

### Comparing `ikiss-1.3.0/ikiss/Snakefile` & `ikiss-1.4.0/ikiss/Snakefile`

 * *Files 6% similar despite different names*

```diff
@@ -56,17 +56,45 @@
         if default == 1:            # for rule not able threading
             return default
         else:
             return workflow.global_resources["_cores"]
     # if cluster not rule and not default or local not _cores return value from call
     return default
 
+# # run_get_versions was adapted from culebront project by orjuela, compte, et al 2022. 10.24072/pcjournal.153
+# rule run_get_versions:
+#     """
+#     recovery soft versions
+#     """
+#     threads: get_threads('run_get_versions', 1)
+#     input:
+#         assemblers = expand(f"{output_dir}{{fastq}}/ASSEMBLERS/{{assemblers}}/ASSEMBLER/{{assemblers}}-version.txt", fastq = FASTQ[0], assemblers=culebront.assembly_tools_activated),
+#         polishers = expand(rules.run_racon_version.output.version, fastq=FASTQ),
+#         correction = expand(f"{output_dir}{{fastq}}/ASSEMBLERS/{{assemblers}}/CORRECTION/{{correction}}/{{correction}}-version.txt", fastq=FASTQ[0], assemblers=culebront.assembly_tools_activated, correction=culebront.correction_tools_activated),
+#         circular = expand(f"{output_dir}{{fastq}}/ASSEMBLERS/{{assemblers}}/ASSEMBLER/CIRCLATOR-version.txt", fastq=FASTQ[0], assemblers=[ass for ass in culebront.assembly_tools_activated if ass in ["CANU","SMARTDENOVO"] and bool(culebront.config['CIRCULAR'])]),
+#         quality = expand(f"{output_dir}{{fastq}}/ASSEMBLERS/{{assemblers}}/QUALITY/{{quality_step}}/{{quality}}/{{quality}}-version.txt", fastq=FASTQ[0], assemblers=culebront.assembly_tools_activated[0], quality_step=culebront.last_steps_list, quality=[qual for qual in culebront.quality_tools_activated if qual not in ["QUAST", "MAUVE", "BUSCO"]]),
+#         mauve = expand(f"{output_dir}/versions/{{quality}}-version.txt", quality=[qual for qual in culebront.quality_tools_activated if qual in ["MAUVE"]])
+#     params:
+#         dir =f'{output_dir}versions/'
+#     output:
+#         csv = f"{output_dir}versions.csv"
+#     message:
+#         """
+#         picking software versions used by iKISS
+#         """
+#     log:
+#         output = f'{output_dir}versions/LOGS/GET-VERSIONS.o',
+#         error = f'{output_dir}versions/LOGS/GET-VERSIONS.e'
+#     script:
+#         f"{ikiss_obj.snakemake_scripts}/get_versions.py"
+
 
 def output_final(wildcards):
     dico_final = {
+        "fastq_table": f"{output_dir}0.FASTQ_STATS/fastq_stats.txt",
         "kmer_module": f"{output_dir}3.TABLE2BED/"
     }
     if config['WORKFLOW']['PCADAPT']:
         dico_final.update({
             "pca_kmers": f"{output_dir}7.MERGED_PCADAPT/merged_pcadapt_pvalues.csv",
         })
         if config['WORKFLOW']['MAPPING']:
@@ -761,20 +789,21 @@
     """
     doing a pca analysis using phenotype file with variables done by user
     """
     threads: get_threads('get_pca_from_phenotype', 6)
     input:
         phenotype = config['PARAMS']['LFMM']['PHENOTYPE_FILE'],
     output:
-        pca_variance = f"{output_dir}6.LFMM/PCA_from_phenotype.csv",
+        pca_variance = f"{output_dir}6.LFMM_PHENO/PCA_from_phenotype.csv",
     params:
-        jupyter = f"{output_dir}6.LFMM/PCA_from_phenotype.ipynb",
+        jupyter = f"{output_dir}6.LFMM_PHENO/PCA_from_phenotype.ipynb",
+        html = f"{output_dir}6.LFMM_PHENO/PCA_from_phenotype.html",
     log:
-        output = f"{output_dir}LOGS/6.LFMM/PCA_FROM_PHENOTYPE_LFMM.o",
-        error = f"{output_dir}LOGS/6.LFMM/PCA_FROM_PHENOTYPE_LFMM.e",
+        output = f"{output_dir}LOGS/6.LFMM_PHENO/PCA_FROM_PHENOTYPE_LFMM.o",
+        error = f"{output_dir}LOGS/6.LFMM_PHENO/PCA_FROM_PHENOTYPE_LFMM.e",
     benchmark:
         f"{output_dir}BENCHMARK/PCA_FROM_PHENOTYPE_LFMM.txt"
     message:
         """
         Launching {rule}
         threads: {threads}
         input:
@@ -789,14 +818,15 @@
         tools_config['SINGULARITY']['TOOLS']
     envmodules:
         tools_config["ENVMODULE"]["KMERS_GWAS"]
     shell:
         """ 
         python3 {ikiss_obj.snakemake_scripts}/pca_from_phenotype.py -p {input.phenotype} -o {params.jupyter} 1>{log.output} 2>{log.error}
         jupyter nbconvert --execute --inplace {params.jupyter} --ExecutePreprocessor.timeout=6000
+        jupyter nbconvert --execute {params.jupyter} --no-input --ExecutePreprocessor.timeout=6000 --to=html
         """
 
 
 rule lfmm:
     """
     lfmm using a segment
     """
@@ -811,15 +841,15 @@
         bed = f"{output_dir}3.TABLE2BED/{{bed}}.bed",
         bim = f"{output_dir}3.TABLE2BED/{{bed}}.bim",
         fam = f"{output_dir}3.TABLE2BED/{{bed}}.fam",
         segment_file = f"{{bed}}_{{segment}}",
 
     output:
         outliers = f"{output_dir}6.LFMM/{{bed}}_{{segment}}_lfmm_outliers.csv",
-        #pvalues = f"{output_dir}6.LFMM/{{bed}}_{{segment}}_lfmm_pvalues.csv",
+        pvalues = f"{output_dir}6.LFMM/{{bed}}_{{segment}}_lfmm_pvalues.csv",
     log:
         output = f"{output_dir}LOGS/6.LFMM/{{bed}}_{{segment}}_LFMM.o",
         error = f"{output_dir}LOGS/6.LFMM/{{bed}}_{{segment}}_LFMM.e",
     benchmark:
         f"{output_dir}BENCHMARK/{{bed}}_{{segment}}_LFMM.txt"
     message:
         """
@@ -832,15 +862,15 @@
             bed : {params.bed}
             k: {params.k}
             alpha : {params.alpha}
             correction : {params.correction}
         output:
             outliers: {output.outliers}
         log:
-            output: {log.output}+
+            output: {log.output}
             error: {log.error}
         """
     singularity:
         tools_config['SINGULARITY']['TOOLS']
     envmodules:
         tools_config["ENVMODULE"]["R"]
     shell:
@@ -868,38 +898,41 @@
     """
     threads: get_threads('merge_lfmm', 1)
     input:
         pcas = aggregate_segments_to_lfmm,
     params:
         dir = f"{output_dir}6.LFMM/"
     output:
-        outliers_combined = f"{output_dir}7.MERGED_LFMM/merged_lfmm_pvalues.csv",
+        pvalues_combined = f"{output_dir}7.MERGED_LFMM/merged_lfmm_pvalues.csv",
+        outliers_combined = f"{output_dir}7.MERGED_LFMM/merged_lfmm_outliers.csv",
     log:
         output = f"{output_dir}LOGS/7.MERGED_LFMM/MERGED_LFMM.o",
         error = f"{output_dir}LOGS/7.MERGED_LFMM/MERGED_LFMM.e",
     benchmark:
         f"{output_dir}BENCHMARK/MERGED_LFMM.txt",
     message:
         """
         Launching {rule}
         threads: {threads}
         output:
+            pvalues_combined : {output.pvalues_combined}
             outliers_combined: {output.outliers_combined}
         log:
             output: {log.output}
             error: {log.error}
         """
     singularity:
         tools_config['SINGULARITY']['TOOLS']
     shell:
         """        
         (cd {params.dir}
         echo -e 'sequence\tbedname\tsegment_nb\tpvalue' > tmp.csv
         cat *_lfmm_outliers.csv >> tmp.csv
-        mv tmp.csv {output.outliers_combined}  
+        mv tmp.csv {output.outliers_combined}
+        cat *_lfmm_pvalues.csv > {output.pvalues_combined} 
         ) 1>{log.output} 2>{log.error}
         """
 
 
 
 rule outliers_lfmm_position:
     """
@@ -975,16 +1008,15 @@
         """
     singularity:
         tools_config['SINGULARITY']['TOOLS']
     shell:
         """
         (awk '{{print $1\"\\t"$4\"\\t"$4\"\\t\"$4\"\\t\"$3}}' {input.merged_pvalues} > {params.tmp4mergetags}
         mergeTags -k 31 -m 15 -n  {params.tmp4mergetags} > {output.assembled_csv}
-        awk '{{ if (NR>1 && $1>={params.contig_size}) print \">mergeTags_\"$1\"_\"$3\"\\n\"$2}}' {output.assembled_csv} > {output.assembled_outliers}
-        ) 1> {log.error} 2> {log.output}
+        awk '{{ if (NR>1 && length($2)>={params.contig_size}) print \">mergeTags_\"length($2)\"_\"$3\"\\n\"$2}}' {output.assembled_csv} > {output.assembled_outliers}) 1> {log.error} 2> {log.output}
         """
 
 rule mergetags_pcadapt:
     """
     assembly significant kmers obtained by pcadapt by mergeTags
     https://github.com/Transipedia/dekupl-mergeTags
     """
@@ -1019,45 +1051,89 @@
         """
     singularity:
         tools_config['SINGULARITY']['TOOLS']
     shell:
         """
         (awk '{{print $2\"\\t"$6\"\\t"$6\"\\t\"$6\"\\t\"$5}}' {input.merged_pvalues} > {params.tmp4mergetags}
         mergeTags -k 31 -m 15 -n  {params.tmp4mergetags} > {output.assembled_csv}
-        awk '{{ if (NR>1 && $1>={params.contig_size}) print \">mergeTags_\"$1\"_\"$3\"\\n\"$2}}' {output.assembled_csv} > {output.assembled_outliers}
+        awk '{{ if (NR>1 && length($2)>={params.contig_size}) print \">mergeTags_\"length($2)\"_\"$3\"\\n\"$2}}' {output.assembled_csv} > {output.assembled_outliers}
         ) 1> {log.error} 2> {log.output}
         """
 
 
 ############################ REPORT #######################################################
 # report contains dico_final now
 
+rule fastq_stats:
+    """
+    run fastq_stats
+    """
+    threads: get_threads('fastq_stats', 8)
+    input:
+        dir = fastq_dir
+    output:
+        fastq_table = f"{output_dir}0.FASTQ_STATS/fastq_stats.txt"
+    log:
+        output = f"{output_dir}LOGS/0.FASTQ_STATS/FASTQ_STATS.o",
+        error = f"{output_dir}LOGS/0.FASTQ_STATS/FASTQ_STATS.e"
+    benchmark:
+        f"{output_dir}BENCHMARK/FASTQ_STATS.txt"
+    message:
+        """
+        Launching {rule}
+        threads: {threads}
+        input:
+            kmers_to_use : {input.dir}
+        output:
+            kmers_table: {output.fastq_table}
+        log:
+            output: {log.output}
+            error: {log.error}
+        """
+    singularity:
+        tools_config['SINGULARITY']['TOOLS']
+    #envmodules:
+    #    tools_config["ENVMODULE"]["SEQKIT"],
+    shell:
+        """
+        cd {input.dir}
+        seqkit stats -T -j {threads} {input.dir}/* -o {output.fastq_table} 1>{log.error}  2> {log.output}
+        sed -i 's|{input.dir}/||' {output.fastq_table}
+        sed -i 's|{ikiss_obj.fastq_files_ext}||' {output.fastq_table}
+        """
+
 rule report_ikiss:
     """
     rule to recovery all files to report
     """
     threads: get_threads('report_ikiss',1)
     input:
         unpack(output_final),
     params:
         list_log_kmer_per_sample = expand(rules.kmers_gwas_per_sample.log.error,sample=SAMPLE),
         kmer_table_rep = f"{output_dir}3.TABLE2BED/",
         samples_list = SAMPLE,
+        phenotype= ikiss_obj.phenotype,
         pvalues_pcadapt = rules.merge_pcadapt.output.pvalues_combined if 'PCADAPT' in ikiss_obj.tools_activated else "",
         outliers_pcadapt = rules.merge_pcadapt.output.outliers_combined if 'PCADAPT' in ikiss_obj.tools_activated else "",
         outliers_pcadapt_position = rules.outliers_pcadapt_position.log.error if ('PCADAPT' in ikiss_obj.tools_activated and 'MAPPING' in ikiss_obj.tools_activated)  else "",
+        contigs_pcadapt_csv= rules.mergetags_pcadapt.output.assembled_csv if ('PCADAPT' in ikiss_obj.tools_activated and 'ASSEMBLY' in ikiss_obj.tools_activated) else "",
         plots_pcadapt = f"{output_dir}6.PCADAPT",
+        phenotype_pca_html = rules.get_pca_from_phenotype.params.html,
         outliers_lfmm = rules.merge_lfmm.output.outliers_combined if 'LFMM' in ikiss_obj.tools_activated else "",
         outliers_lfmm_position= rules.outliers_lfmm_position.log.error if ('LFMM' in ikiss_obj.tools_activated and 'MAPPING' in ikiss_obj.tools_activated) else "",
+        contigs_lfmm_csv = rules.mergetags_lfmm.output.assembled_csv if ('LFMM' in ikiss_obj.tools_activated and 'ASSEMBLY' in ikiss_obj.tools_activated) else "",
+        contig_size = config['PARAMS']['ASSEMBLY']['FILTER_CONTIG_SIZE'],
         plots_lfmm = f"{output_dir}6.LFMM",
         txt_config = f"{output_dir}/config_corrected.yaml",
         out_dir_report = directory(f"{output_dir}REPORT"),
         workflow_steps = ikiss_obj.tools_activated,
         outliers_lfmm_with_position = f"{output_dir}11.OUTLIERS_LFMM_POSITION",
         ref = reference_file,
+        fastq_stats = rules.fastq_stats.output.fastq_table
     output:
         jupyter = f"{output_dir}REPORT/iKISS_report.ipynb"
     log:
         output = f"{output_dir}LOGS/REPORT/report.o",
         error = f"{output_dir}LOGS/REPORT/report.e",
     benchmark:
         f"{output_dir}BENCHMARK/Report.txt",
@@ -1079,14 +1155,18 @@
 rule html_ikiss:
     """
     rule to build jupyter notebook and generate iKISS report 
     """
     threads: get_threads('html_ikiss',1)
     input:
         notebook = rules.report_ikiss.output.jupyter
+    params:
+        dir_report = f"{output_dir}REPORT/",
+        html_phenotype_lfmm = f"cp {rules.get_pca_from_phenotype.params.html} . " if 'LFMM' in ikiss_obj.tools_activated else "",
+        jupyter_phenotype_lfmm= f' cp {rules.get_pca_from_phenotype.params.jupyter} . ' if 'LFMM' in ikiss_obj.tools_activated else "",
     output:
         html=f"{output_dir}REPORT/iKISS_report.html"
     message:
         """
         Launching {rule}
         threads: {threads}
         input:
@@ -1094,11 +1174,14 @@
         output:
             html : {output.html}
         """
     singularity:
         tools_config['SINGULARITY']['TOOLS']
     shell:
         """
+        cd {params.dir_report}
         jupyter nbconvert --execute {input.notebook} --no-input --ExecutePreprocessor.timeout=6000 --to=html
+        {params.html_phenotype_lfmm}
+        {params.jupyter_phenotype_lfmm}
         """
```

### Comparing `ikiss-1.3.0/ikiss/__init__.py` & `ikiss-1.4.0/ikiss/__init__.py`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/containers/Dockerfile` & `ikiss-1.4.0/ikiss/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/containers/Singularity.ikiss_tools.def` & `ikiss-1.4.0/ikiss/containers/Singularity.ikiss_tools.def`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 apt install -y software-properties-common
 apt install -y python-is-python3
 apt update
 apt -y install gcc
 apt -y upgrade libstdc++6
 apt -y dist-upgrade
 
-pip3 install xarray dataclasses Chunk numpy pandas argparse random2 pathlib nbformat ipykernel seaborn matplotlib scikit-learn bioinfokit jupyter itables
+pip3 install xarray dataclasses Chunk numpy pandas argparse random2 pathlib nbformat ipykernel seaborn matplotlib scikit-learn bioinfokit jupyter itables pyyaml
+
+# SEQKIT
+mkdir seqkit_2.4.0
+cd seqkit_2.4.0
+wget https://github.com/shenwei356/seqkit/releases/download/v2.4.0/seqkit_linux_amd64.tar.gz
+tar -xzvf seqkit_linux_amd64.tar.gz
+cd ..
 
 # SEQTK 1.3
 wget https://github.com/lh3/seqtk/archive/v1.3.zip
 unzip v1.3.zip
 cd seqtk-1.3/
 make
 cd ..
@@ -101,14 +108,14 @@
     R -e "install.packages('pcadapt')"
     R -e "install.packages('seqRFLP')"
     R -e "install.packages('stringr')"
     R -e "install.packages('lfmm')"
     R -e "install.packages('rlist')"
 
 %environment
-export PATH=/kmer_gwas/bin:/kmer_gwas/external_programs:/samtools-1.10:/seqtk-1.3:/bwa-mem2-2.1:/bwa:/dekupl-mergeTags/:$PATH
+export PATH=/kmer_gwas/bin:/kmer_gwas/external_programs:/samtools-1.10:/seqkit_2.4.0:/seqtk-1.3:/bwa-mem2-2.1:/bwa:/dekupl-mergeTags/:$PATH
 
 ## -0.7.17
 %runscript
 exec /bin/bash "$@"echo 'export GOPATH=${HOME}/go' >> ~/.bashrc && \
 echo 'export PATH=/usr/local/go/bin:${PATH}:${GOPATH}/bin' >> ~/.bashrc && \
 source ~/.bashrc
```

### Comparing `ikiss-1.3.0/ikiss/img/schema_pipeline_dag.pdf` & `ikiss-1.4.0/ikiss/img/schema_pipeline_dag.pdf`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/img/schema_pipeline_global1.pdf` & `ikiss-1.4.0/ikiss/img/schema_pipeline_global1.pdf`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/img/schema_pipeline_global2.pdf` & `ikiss-1.4.0/ikiss/img/schema_pipeline_global2.pdf`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/install_files/cluster_config_SLURM.yaml` & `ikiss-1.4.0/ikiss/install_files/cluster_config_SLURM.yaml`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/install_files/config.yaml` & `ikiss-1.4.0/ikiss/install_files/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     LFMM:
         K : 2
         # PHENOTYPE_FILE is obligatory, if PHENOTYPE_PCA_ANALYSIS is false, lfmm is launched directly using it as phenotype to LFMM analysis. This file can be a PCA result
         #PHENOTYPE_FILE: ''
         PHENOTYPE_FILE: "DATA_DIR/DATATEST/pheno.txt"
         # if PHENOTYPE_PCA_ANALYSIS is true, a PCA is done before run lfmm using the PHENOTYPE_FILE
-        PHENOTYPE_PCA_ANALYSIS : false
+        PHENOTYPE_PCA_ANALYSIS : true
         CORRECTION: 'BH'
         ALPHA : 0.05
 
     MAPPING:
         REF: 'DATA_DIR/DATATEST/ref/reference.fasta'
         # type bwa-aln or bwa-mem2
         #MODE : bwa-mem2
@@ -48,8 +48,8 @@
         #index_options: " "
         # if bwa-mem2 default parameters -A 1 -B 4; if bwa-aln -n [0.04] 2 diff by 30 pb
         OPTIONS : "-n 0.04"
         #OPTIONS : "-A 1 -B 4"
 
     ASSEMBLY:
         OVERLAP_SIZE : 15
-        FILTER_CONTIG_SIZE : 100
+        FILTER_CONTIG_SIZE : 50
```

### Comparing `ikiss-1.3.0/ikiss/logo_ikiss.png` & `ikiss-1.4.0/ikiss/logo_ikiss.png`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/module.py` & `ikiss-1.4.0/ikiss/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             else:
                 raise ValueError(
                     f"CONFIG FILE CHECKING FAIL : you need to chose between {ALLOW_MAPPING_MODE} in MAPPING mode !")
 
         def get_dico_samples_and_pop(self, path):
             # check of header
             infile = open(path, 'r')
-            if not 'accession_id\tphenotype_value' in infile.readline():
+            if not 'accession_id\tgroup' in infile.readline():
                 raise ValueError(
-                    f"SAMPLES FILE CHECKING FAIL : Please add accession_id\tphenotype_value in SAMPLES tabulated header !")
+                    f"SAMPLES FILE CHECKING FAIL : Please add accession_id\tgroup in SAMPLES tabulated header !")
             infile.close()
             # populating self.samples
             with open(path, "r") as samples_open:
                 for line in samples_open:
                     if not 'accession_id' in line:
                         key, value = line.strip().split('\t')
                         self.samples[key] = value
@@ -115,81 +115,85 @@
         if "gz" in self.fastq_files_ext:
             self.fastq_gzip = True
 
         self.forward, self.reverse = self.__split_illumina()
 
         self.mapping_mode = get_mapping_mode(self.config['PARAMS']['MAPPING']['MODE'], ALLOW_MAPPING_MODE)
 
-        # get dico with samples names as key and population as value.
-        self.samples = get_dico_samples_and_pop(self, self.get_config_value(level1='PARAMS', level2='PCADAPT', level3='SAMPLES'))
-        self.phenotype = get_dico_phenotype_and_pop(self, self.get_config_value(level1='PARAMS', level2='LFMM', level3='PHENOTYPE_FILE'))
-
         # get samples name from reads files
         for elem in self.fastq_files_list:
             if '_R1' in elem :
                 fastq_name = Path(elem).stem.split('_R1')[0]
                 self.fastq_names_list.append(fastq_name)
             if '_1' in elem or '_1' in elem:
                 fastq_name = Path(elem).stem.split('_1')[0]
                 self.fastq_names_list.append(fastq_name)
 
 
-        # comparing names from reads and names from samples.txt given by user
-        if sorted(self.fastq_names_list) != sorted(list(self.samples.keys())) :
-            #print(sorted(self.fastq_names_list))
-            #print(sorted(list(self.samples.keys())))
-            print ("samples in FASTQ but not in SAMPLES")
-            print(set(sorted(self.fastq_names_list)) - set(sorted(list(self.samples.keys()))))
-            print ("samples in SAMPLES but not in FASTQ")
-            print(set(sorted(list(self.samples.keys()))) - set(sorted(self.fastq_names_list)))
-            raise ValueError(f"CONFIG FILE CHECKING ERROR : FASTQ names and SAMPLES names are different. Please check your samples file !")
-            # @seb ? raise ValueError(f"Invalid argument `key_value_pairs`! SAMPLES file is corrupted, use only tabulations, don't put a header in SAMPLES file")
-
-        # comparing names from reads and names from phenotype.txt given by user
-        if sorted(self.fastq_names_list) != sorted(list(self.phenotype.keys())) :
-            #print(sorted(self.fastq_names_list))
-            #print(sorted(list(self.phenotype.keys())))
-            print ("samples in FASTQ but not in PHENOTYPE")
-            print(set(sorted(self.fastq_names_list)) - set(sorted(list(self.phenotype.keys()))))
-            print ("samples in SAMPLES but not in PHENOTYPE")
-            print(set(sorted(list(self.phenotype.keys()))) - set(sorted(self.fastq_names_list)))
-            raise ValueError(f"CONFIG FILE CHECKING ERROR : FASTQ names and PHENOTYPE names are different. Please check your phenotype file !")
-            # @seb ? raise ValueError(f"Invalid argument `key_value_pairs`! SAMPLES file is corrupted, use only tabulations, don't put a header in SAMPLES file")
-
-
         # kmers_module is obligatory and has to be activated,
         if not bool(self.config['WORKFLOW']['KMERS_MODULE']):
             raise ValueError(
                 f"CONFIG FILE CHECKING ERROR : KMERS_MODULE is the minimal step you need to activate in the configuration file !! \n")
 
         # if mapping is true pcadapt or lfmm has to be activated
         if not self.config['WORKFLOW']['PCADAPT'] and not self.config['WORKFLOW']['LFMM'] and self.config['WORKFLOW']['MAPPING']:
             raise ValueError(
                 f"CONFIG FILE CHECKING ERROR : MAPPING is irrelevant if you have not activated PCADAPT or LFMM !! \n")
 
 
-        # check if reference is given by user if mapping is activate
+        # check if reference is given by user if mapping is activated
         if self.config['WORKFLOW']['MAPPING']:
             self._check_file_or_string(level1="PARAMS", level2="MAPPING", level3="REF", mandatory=['MAPPING'])
 
         # check if phenotype file is correct if LFMM is activated
         if self.config['WORKFLOW']['LFMM']:
             self._check_file_or_string(level1="PARAMS", level2='LFMM', level3="PHENOTYPE_FILE", mandatory=['LFMM'])
+            # get dico with samples names as key and phenotype as value.
+            self.phenotype = get_dico_phenotype_and_pop(self, self.get_config_value(level1='PARAMS', level2='LFMM',  level3='PHENOTYPE_FILE'))
+            # comparing names from reads and names from phenotype.txt given by user
+            if sorted(self.fastq_names_list) != sorted(list(self.phenotype.keys())):
+                # print(sorted(self.fastq_names_list))
+                # print(sorted(list(self.phenotype.keys())))
+                print("samples in FASTQ but not in PHENOTYPE")
+                print(set(sorted(self.fastq_names_list)) - set(sorted(list(self.phenotype.keys()))))
+                print("samples in SAMPLES but not in PHENOTYPE")
+                print(set(sorted(list(self.phenotype.keys()))) - set(sorted(self.fastq_names_list)))
+                raise ValueError(
+                    f"CONFIG FILE CHECKING ERROR : FASTQ names and PHENOTYPE names are different. Please check your phenotype file !")
+                # @seb ? raise ValueError(f"Invalid argument `key_value_pairs`! SAMPLES file is corrupted, use only tabulations, don't put a header in SAMPLES file")
+            # check if K is a int
             if not int(self.config['PARAMS']['PCADAPT']['K']):
                 # TODO: je n'arrive pas a recuperer le bon error du raise
                 raise TypeError(
                     f"CONFIG FILE CHECKING ERROR :  PARAMS/LFMM/K is not a integer !! \n")
 
         # check if samples file is correct if PCADAPT is activated
         if self.config['WORKFLOW']['PCADAPT']:
             self._check_file_or_string(level1="PARAMS", level2="PCADAPT", level3="SAMPLES", mandatory=['PCADAPT'])
-            if type(self.config['PARAMS']['PCADAPT']['K']) is not int:
+            # get dico with samples names as key and population as value.
+            self.samples = get_dico_samples_and_pop(self, self.get_config_value(level1='PARAMS', level2='PCADAPT', level3='SAMPLES'))
+
+            # comparing names from reads and names from samples.txt given by user
+            if sorted(self.fastq_names_list) != sorted(list(self.samples.keys())):
+            # print(sorted(self.fastq_names_list))
+            # print(sorted(list(self.samples.keys())))
+                print("samples in FASTQ but not in SAMPLES")
+                print(set(sorted(self.fastq_names_list)) - set(sorted(list(self.samples.keys()))))
+                print("samples in SAMPLES but not in FASTQ")
+                print(set(sorted(list(self.samples.keys()))) - set(sorted(self.fastq_names_list)))
+                raise ValueError(
+                f"CONFIG FILE CHECKING ERROR : FASTQ names and SAMPLES names are different. Please check your samples file !")
+            # @seb ? raise ValueError(f"Invalid argument `key_value_pairs`! SAMPLES file is corrupted, use only tabulations, don't put a header in SAMPLES file")
+
+
+            if type(self.config['PARAMS']['LFMM']['K']) is not int:
                 raise f"CONFIG FILE CHECKING ERROR :  PARAMS/PCADAPT/K is not a integer !! \n"
 
 
+
     def __check_tools_config(self, tool, mandatory=[]):
         """Check if path is a file if not empty
         :return absolute path file"""
         tool_OK = True
 
         # If only envmodule
         if self.use_env_modules and not self.use_singularity:
```

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/ikiss_report.py` & `ikiss-1.4.0/ikiss/snakemake_scripts/ikiss_report.py`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/kmer-bed2fastq.py` & `ikiss-1.4.0/ikiss/snakemake_scripts/kmer-bed2fastq.py`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/lfmm.R` & `ikiss-1.4.0/ikiss/snakemake_scripts/lfmm.R`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   make_option(c("-a", "--famFile"),
               type = "character",
               default = NULL,
               help = "Path of fam file"),
   make_option(c("-o", "--outFilePath"),
               type = "character",
               default = NULL,
-              help = "Path where output sequence file will be written."),
+              help = "Path where significant kmers with pvalue will be written."),
   make_option(c("-k", "--kmerList"),
               type = "character",
               default = NULL,
               help = "kmer list"),
   make_option(c("-p", "--phenoFile"),
               type = "character",
               default = NULL,
@@ -193,14 +193,23 @@
 names(df) <- NULL
 
 print("=========DF to csv ==================")
 print(head(df))
 
 write.table(df, out, quote = FALSE, sep="\t")
 
+##### saving all pvalues
+df_all = data.frame(pvalues)
+names(df_all) <- NULL
+
+print("=========DF_all to csv ==================")
+print(head(df_all))
+out_all <- str_replace(out, "_outliers.csv", "_pvalues.csv")
+write.table(df_all, out_all, quote = FALSE, sep="\t")
+
 # Screen plot
 fileplot <- str_replace(out, "_outliers.csv", ".rplot.pdf")
 pdf(file=fileplot)
 qqplot(rexp(length(pvalues), rate = log(10)),
        -log10(pvalues), xlab = "Expected quantile",
        pch = 19, cex = .4)
 abline(0,1)
```

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/outliers_and_position.py` & `ikiss-1.4.0/ikiss/snakemake_scripts/outliers_and_position.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 args = parser.parse_args()
 
 outliers = args.outliers
 positions = args.kmers_position
 output = args.output
 
 # import files
+## outliers
 selected_df = pd.read_csv(outliers, delimiter='\t', header="infer")
+## kmers avec position in the ref
 database_df = pd.read_csv(positions, delimiter='\t', header="infer")
 print("--db------")
 print(database_df)
 
-# over sequence we remove "_0" caracters
+# over each sequence we remove "_0" caracters
 def remove_str(seq):
     if "_0" in seq:
         return str(seq)[:-2]
     else:
         return seq
     #selected_df['sequence'] = selected_df['sequence'].apply(lambda x: (str(x)[:-2]))
 selected_df['sequence'] = selected_df['sequence'].apply(remove_str)
-print("--sel------")
+print("--selected outliers------")
 print(selected_df)
 
-print("col")
+print("col outliers")
 print(selected_df.columns)
 print(database_df.columns)
 
 #merge dataframes by bedname, sequence and kmer_number
 #outliers_with_position = selected_df.merge(database_df, on=["bedname", "sequence", "kmer_number"])
 outliers_with_position = selected_df.merge(database_df, on=["sequence",'bedname'])
 print("--outliers with pos------")
```

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/pca_from_phenotype.py` & `ikiss-1.4.0/ikiss/snakemake_scripts/pca_from_phenotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 headmap """
 code = f"""\
 font1 = fm.FontProperties(size=20)
 font2 = fm.FontProperties(size=24)
 fig1 = plt.figure(figsize=(24, 24))
 plt.title('Correlation Pearson des variables', y=1.05, size=18)
-sns.heatmap(df.corr(), linewidths=0.3, vmax=1.0, square=True, cmap='coolwarm', linecolor='white', annot=True)"""
+sns.heatmap(df.iloc[:, 2:].corr(), linewidths=0.3, vmax=1.0, square=True, cmap='coolwarm', linecolor='white', annot=True)"""
 nb['cells'].append(nbf.v4.new_markdown_cell(texte))
 nb['cells'].append(nbf.v4.new_code_cell(code))
 
 texte = f"""\
 ## Pearson correlation
 
 pairplot"""
@@ -216,15 +216,15 @@
 
 texte = f"""\
 # pearson correlation plot from ACP variables"""
 code = f"""\
 fig5 = plt.figure(figsize=(8,8))
 sns.set(font_scale=2.5)
 plt.title('Correlation Pearson des variables', y=1.05, size=18)
-sns.heatmap(dfPCA.corr(),linewidths=0.3,vmax=1.0, fmt='.3f',
+sns.heatmap(dfPCA.iloc[:,2:].corr(),linewidths=0.3,vmax=1.0, fmt='.3f',
             square=True, cmap='coolwarm', linecolor='white', annot=True)
 sns.set(font_scale=1)
 plt.style.use('seaborn-darkgrid')
 """
 nb['cells'].append(nbf.v4.new_markdown_cell(texte))
 nb['cells'].append(nbf.v4.new_code_cell(code))
```

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/pcadapt.R` & `ikiss-1.4.0/ikiss/snakemake_scripts/pcadapt.R`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/report.py.ipynb` & `ikiss-1.4.0/codemeta.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('@context', 'https://doi.org/10.5063/schema/codemeta-2.0'), ('@type', "*

 * *            "'SoftwareSourceCode'), ('license', 'https://spdx.org/licenses/MIT-0'), "*

 * *            "('codeRepository', 'https://forge.ird.fr/diade/iKISS.git'), ('contIntegration', "*

 * *            "'https://forge.ird.fr/diade/iKISS/-/pipelines'), ('dateCreated', '2021-10-25'), "*

 * *            "('datePublished', '2022-02-25'), ('dateModified', '2023-02-25'), ('downloadUrl', "*

 * *            "'https://forge.ird.fr/diade/ […]*

```diff
@@ -1,99 +1,62 @@
 {
-    "cells": [
+    "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
+    "@type": "SoftwareSourceCode",
+    "applicationCategory": "Genomics",
+    "author": [
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# iKISS REPORT\n",
-                "Date: \n",
-                "Licence: \n",
-                "Autor : \n",
-                "\n",
-                "this is a test for iKISS report using jupyter"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 59,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from pathlib import Path, PurePosixPath\n",
-                "import pandas as pd\n",
-                "\n",
-                "pd.set_option(\"display.precision\", 2)\n",
-                "\n",
-                "file_list = snakemake.input[0]\n",
-                "output_file = snakemake.output[0]\n",
-                "\n",
-                "print (file_list)\n",
-                "\n",
-                "data = {}\n",
-                "for file in file_list:\n",
-                "    file = Path(file).resolve()\n",
-                "    name = PurePosixPath(file).stem.split('_KMERS_MODULE')[0]\n",
-                "    dir = PurePosixPath(file).parent\n",
-                "    with open (file, 'r') as f:\n",
-                "        liste = []\n",
-                "        for line in f:\n",
-                "            if \"Total no. of reads\" in line : \n",
-                "                reads = int(line.strip().split(\":\")[1])\n",
-                "                liste.append(reads)\n",
-                "            if \"Canonized kmers:\" in line : \n",
-                "                canonized = int(line.strip().split(\"\\t\")[1])\n",
-                "                liste.append(canonized)\n",
-                "            if \"Non-canon kmers:\" in line : \n",
-                "                non_canonized = int(line.strip().split(\"\\t\")[1])\n",
-                "                liste.append(non_canonized)\n",
-                "            if \"Non-canon kmers found:\" in line : \n",
-                "                non_canonized_founded = int(line.strip().split(\"\\t\")[1])\n",
-                "                liste.append(non_canonized_founded)\n",
-                "            if \"kmers to save:\" in line : \n",
-                "                tosave = int(line.strip().split(\":\")[1])\n",
-                "                liste.append(tosave)   \n",
-                "            \n",
-                "    data[name] = liste    \n",
-                "#print (data)\n",
-                "# TODO : ajouter un control si single pour accepter seulement le R1 dans le tableau\n",
-                "df_kmer_module = pd.DataFrame.from_dict(data, orient='index', columns=['reads_R1', 'reads_R2', 'Canonized', 'Non-canonized', 'Non-canonized_found','kmers_saved'])\n",
-                "#print (kmer_module)\n",
-                "df_kmer_module.to_csv(output_file)"
-            ]
+            "@id": "https://orcid.org/my-orcid?orcid=0000-0001-8387-2266",
+            "@type": "Person",
+            "affiliation": {
+                "@type": "Organization",
+                "name": "DIADE unit, French National Research Institute for Sustainable Development"
+            },
+            "email": "julie.orjuela@ird.fr",
+            "familyName": "Orjuela",
+            "givenName": "Julie"
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        }
-    ],
-    "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3",
-            "language": "python",
-            "name": "python3"
-        },
-        "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
+            "@id": "https://orcid.org/0000-0002-8361-6040",
+            "@type": "Person",
+            "affiliation": {
+                "@type": "Organization",
+                "name": "DIADE unit, French National Research Institute for Sustainable Development"
             },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.10.6 (main, Nov 14 2022, 16:10:14) [GCC 11.3.0]"
-        },
-        "orig_nbformat": 4,
-        "vscode": {
-            "interpreter": {
-                "hash": "916dbcbb3f70747c44a77c7bcd40155683ae19c65e1c03b4aa3499c5328201f1"
-            }
+            "email": "yves.vigouroux@ird.fr",
+            "familyName": "Yves",
+            "givenName": "Vigouroux"
         }
+    ],
+    "codeRepository": "https://forge.ird.fr/diade/iKISS.git",
+    "contIntegration": "https://forge.ird.fr/diade/iKISS/-/pipelines",
+    "dateCreated": "2021-10-25",
+    "dateModified": "2023-02-25",
+    "datePublished": "2022-02-25",
+    "description": "iKISS (Kmer Inference sSelection) is a snakemake pipeline able to decompose reads into kmers and extract significant kmers under selection.",
+    "developmentStatus": "active",
+    "downloadUrl": "https://forge.ird.fr/diade/iKISS/-/archive/1.3.0/iKISS-1.3.0.tar.gz",
+    "funder": {
+        "@type": "Organization",
+        "name": "French National Research Institute for Sustainable Developement"
     },
-    "nbformat": 4,
-    "nbformat_minor": 2
+    "issueTracker": "https://forge.ird.fr/diade/iKISS/-/issues",
+    "keywords": [
+        "kmers",
+        "diversity",
+        "plants",
+        "selection",
+        "domestication"
+    ],
+    "license": "https://spdx.org/licenses/MIT-0",
+    "name": "ikiss",
+    "operatingSystem": [
+        "Linux"
+    ],
+    "programmingLanguage": [
+        "Python3"
+    ],
+    "releaseNotes": "Package name was changed to ikiss \ud83d\udc8f  in order to push it in the PyPi \ud83d\udc0d package repository\ncode was refactored without adding new features.\nsnakecdysis python package is now used by iKISS to manage install in cluster and local mode.",
+    "softwareRequirements": [
+        "Python >= 3.7"
+    ],
+    "version": "1.3.0"
 }
```

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/run_ikiss.sbatch` & `ikiss-1.4.0/ikiss/snakemake_scripts/run_ikiss.sbatch`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss/snakemake_scripts/split_bed.py` & `ikiss-1.4.0/ikiss/snakemake_scripts/split_bed.py`

 * *Files identical despite different names*

### Comparing `ikiss-1.3.0/ikiss.egg-info/PKG-INFO` & `ikiss-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikiss
-Version: 1.3.0
+Version: 1.4.0
 Summary: iKISS is a pipeline to detect kmers under selection.
 Author-email: "Julie Orjuela (DIADE-IRD)" <julie.orjuela@ird.fr>
 License: MIT License
         
         Copyright (c) 2022 DIADE IRD / Julie Orjuela, Yves Vigouroux
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,15 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 License-File: LICENCE
+License-File: AUTHORS.md
 
 .. image:: ./ikiss/logo_ikiss.png
    :width: 400
    :alt: ikiss Logo
    :align: center
 
 
@@ -153,14 +154,15 @@
 
 .. code-block:: bash
 
    ikiss run_cluster --help
    ikiss run_cluster -c TEST/data_test_config.yaml --singularity-args "--bind $HOME"
    # @IFB
    ikiss run_cluster -c TEST/data_test_config.yaml --singularity-args "--bind /shared:/shared"
+   #you can also use snakemake parametters as --rerun-incomplete --nolock
 
 
 **Important Note** : In i-Trop cluster, run iKISS using ONLY a node, data has to be in "/scratch" of chosen node. Use `nodelist : nodeX` parametter inside of cluster_config.yaml file.
 
 
 2.2 In LOCAL mode
 -----------------
@@ -297,15 +299,15 @@
 
    **accession_id** : contains exactly same name of samples in FASTQ. 
 
    **phenotype_value** (int): contains sample group (wild=1, cultivated=2 for example)
 
 .. code-block:: bash
 
-   accession_id	phenotype_value
+   accession_id	group
    Clone12	2
    Clone14	2
    Clone16	2
    Clone20	2
    Clone2	1
    Clone4	1
    Clone8	1
@@ -337,15 +339,31 @@
 
 A PCA can reveal some 'structure' in the genotype data and it could help you to fix K parameter.
 
 **PHENOTYPE_PCA_ANALYSIS** 
 
    * If **PHENOTYPE_PCA_ANALYSIS** is true, iKISS automatically run PCA using the file given by user in the PHENOTYPE_FILE key. This PHENOTYPE_FILE can be a PCA result for example.
 
-   * If **PHENOTYPE_PCA_ANALYSIS** is false, iKISS use directly the PHENOTYPE_FILE as 'phenotype' to LFMM analysis. Kmers are used as 'genotype' data. 
+   * If **PHENOTYPE_PCA_ANALYSIS** is false, iKISS use directly the PHENOTYPE_FILE as 'phenotype' to LFMM analysis. Kmers are used as 'genotype' data.
+
+Here, a example of a phenotype file with climate variables
+
+.. code-block:: bash
+
+    accession_id	group	b2.Mean_Diurnal_Range	b3.Isothermality	b4.Temp_Seasonality	b5.Max_Temp_of_Warmest_Month	b6.Min_Temp_of_Coldest_Month	b7.Temp_Annual_Range	b8.Mean_Temp_of
+    _Wettest_Quarter	b9.Mean_Temp_of_Driest_Quarter	b10.Mean_Temp_of_Warmest_Quarter	b11.Mean_Temp_of_Coldest_Quarter	b12.Annual_Precipitation	b13.Precipitation_of_Wettest_Mo
+    nth	b14.Precipitation_of_Driest_Month	b15.Precipitation_Seasonality	b16.Precipitation_of_Wettest_Quarter	b17.Precipitation_of_Driest_Quarter	b18.Precipitation_of_Warmest_Quarter	b19.Precipitation_of_Coldest_Quarter
+    Clone12	2	99	68	1230	310	166	144	250	226	258	226	1462	249	3	68	573	17	549	17
+    Clone14	2	100	68	1235	301	155	146	241	217	248	217	1525	259	3	67	603	18	575	18
+    Clone16	2	93	65	1389	310	168	142	250	223	258	223	1416	264	0	73	579	8	544	8
+    Clone20	2	154	55	3955	403	123	280	296	234	315	214	118	62	0	184	107	0	45	0
+    Clone2	1	152	55	3617	403	128	275	287	242	316	220	173	80	0	167	153	0	18	0
+    Clone4	1	168	51	5719	414	86	328	315	201	322	181	20	12	0	166	18	0	17	0
+    Clone8	1	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA	NA
+
 
 **CORRECTION**: kmers outliers are obtained using a correction of BONFERONNI, BH or FDR model.
 
 **ALPHA**: modify the alpha cutoff for outlier detection
 
 
 => 4. MAPPING
```

### Comparing `ikiss-1.3.0/ikiss.egg-info/SOURCES.txt` & `ikiss-1.4.0/ikiss.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .gitignore
 .gitlab-ci.yml
+AUTHORS.md
 LICENCE
 README.rst
+codemeta.json
 pyproject.toml
 ikiss/Snakefile
 ikiss/VERSION
 ikiss/__init__.py
 ikiss/_version.py
 ikiss/global_variables.py
 ikiss/logo_ikiss.png
@@ -21,17 +23,18 @@
 ikiss/containers/Singularity.ikiss_tools.def
 ikiss/img/schema_pipeline_dag.pdf
 ikiss/img/schema_pipeline_global1.pdf
 ikiss/img/schema_pipeline_global2.pdf
 ikiss/install_files/cluster_config_SLURM.yaml
 ikiss/install_files/config.yaml
 ikiss/install_files/tools_path.yaml
+ikiss/notebooks/manhattan_plot_example.ipynb
+ikiss/snakemake_scripts/get_versions.py
 ikiss/snakemake_scripts/ikiss_report.py
 ikiss/snakemake_scripts/kmer-bed2fastq.py
 ikiss/snakemake_scripts/lfmm.R
 ikiss/snakemake_scripts/outliers_and_position.py
 ikiss/snakemake_scripts/pca_from_phenotype.py
 ikiss/snakemake_scripts/pcadapt.R
 ikiss/snakemake_scripts/report.py
-ikiss/snakemake_scripts/report.py.ipynb
 ikiss/snakemake_scripts/run_ikiss.sbatch
 ikiss/snakemake_scripts/split_bed.py
```

### Comparing `ikiss-1.3.0/pyproject.toml` & `ikiss-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 version_scheme = "release-branch-semver"
 tag_regex = "^(\\d.\\d.\\d)-*\\w*\\d*$"       # allow value like 0.0.1-rc0
 local_scheme = "no-local-version"
 
 # define Project settings
 [project]
 name = "ikiss"
-version = "1.3.0"
+version = "1.4.0"
 description = "iKISS is a pipeline to detect kmers under selection."
 authors = [
     { name = "Julie Orjuela (DIADE-IRD)", email = "julie.orjuela@ird.fr" },
 ]
 dependencies = ['PyYAML', 'pandas', 'matplotlib', 'tabulate', 'ipython', 'biopython', 'numpy',  'argparse', 'snakemake', 'tqdm', 'click>=8.0.3', 'cookiecutter', 'snakecdysis']
 requires-python = ">=3.8"
 readme = "README.rst"
```

