# Comparing `tmp/radinitio-1.2.0.tar.gz` & `tmp/radinitio-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radinitio-1.2.0.tar", last modified: Mon Jun 26 16:18:17 2023, max compression
+gzip compressed data, was "radinitio-1.2.1.tar", last modified: Mon Jun 26 18:42:31 2023, max compression
```

## Comparing `radinitio-1.2.0.tar` & `radinitio-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 16:18:17.516264 radinitio-1.2.0/
--rw-r--r--   0 angelgr2   (502) staff       (20)     1452 2023-05-31 23:04:50.000000 radinitio-1.2.0/ChangeLog
--rw-r--r--   0 angelgr2   (502) staff       (20)    35147 2023-05-31 23:04:50.000000 radinitio-1.2.0/LICENSE
--rw-r--r--   0 angelgr2   (502) staff       (20)       18 2023-05-31 23:04:50.000000 radinitio-1.2.0/MANIFEST.in
--rw-r--r--   0 angelgr2   (502) staff       (20)    68084 2023-06-26 16:18:17.515941 radinitio-1.2.0/PKG-INFO
--rw-r--r--   0 angelgr2   (502) staff       (20)    67348 2023-06-26 15:55:15.000000 radinitio-1.2.0/README.md
-drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 16:18:17.501835 radinitio-1.2.0/radinitio/
--rw-r--r--   0 angelgr2   (502) staff       (20)   114149 2023-06-23 22:13:17.000000 radinitio-1.2.0/radinitio/__init__.py
--rwxr-xr-x   0 angelgr2   (502) staff       (20)    17462 2023-06-23 21:50:49.000000 radinitio-1.2.0/radinitio/__main__.py
-drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 16:18:17.509772 radinitio-1.2.0/radinitio.egg-info/
--rw-r--r--   0 angelgr2   (502) staff       (20)    68084 2023-06-26 16:18:17.000000 radinitio-1.2.0/radinitio.egg-info/PKG-INFO
--rw-r--r--   0 angelgr2   (502) staff       (20)      274 2023-06-26 16:18:17.000000 radinitio-1.2.0/radinitio.egg-info/SOURCES.txt
--rw-r--r--   0 angelgr2   (502) staff       (20)        1 2023-06-26 16:18:17.000000 radinitio-1.2.0/radinitio.egg-info/dependency_links.txt
--rw-r--r--   0 angelgr2   (502) staff       (20)       30 2023-06-26 16:18:17.000000 radinitio-1.2.0/radinitio.egg-info/requires.txt
--rw-r--r--   0 angelgr2   (502) staff       (20)       10 2023-06-26 16:18:17.000000 radinitio-1.2.0/radinitio.egg-info/top_level.txt
-drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 16:18:17.510067 radinitio-1.2.0/scripts/
--rwxr-xr-x   0 angelgr2   (502) staff       (20)       36 2023-05-31 23:04:50.000000 radinitio-1.2.0/scripts/radinitio
--rw-r--r--   0 angelgr2   (502) staff       (20)       38 2023-06-26 16:18:17.516375 radinitio-1.2.0/setup.cfg
--rwxr-xr-x   0 angelgr2   (502) staff       (20)     1149 2023-06-22 15:37:08.000000 radinitio-1.2.0/setup.py
+drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 18:42:31.593575 radinitio-1.2.1/
+-rw-r--r--   0 angelgr2   (502) staff       (20)     1452 2023-05-31 23:04:50.000000 radinitio-1.2.1/ChangeLog
+-rw-r--r--   0 angelgr2   (502) staff       (20)    35147 2023-05-31 23:04:50.000000 radinitio-1.2.1/LICENSE
+-rw-r--r--   0 angelgr2   (502) staff       (20)       18 2023-05-31 23:04:50.000000 radinitio-1.2.1/MANIFEST.in
+-rw-r--r--   0 angelgr2   (502) staff       (20)    68551 2023-06-26 18:42:31.593198 radinitio-1.2.1/PKG-INFO
+-rw-r--r--   0 angelgr2   (502) staff       (20)    67814 2023-06-26 18:41:00.000000 radinitio-1.2.1/README.md
+drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 18:42:31.588484 radinitio-1.2.1/radinitio/
+-rw-r--r--   0 angelgr2   (502) staff       (20)   114150 2023-06-26 18:24:36.000000 radinitio-1.2.1/radinitio/__init__.py
+-rwxr-xr-x   0 angelgr2   (502) staff       (20)    17463 2023-06-26 18:20:09.000000 radinitio-1.2.1/radinitio/__main__.py
+drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 18:42:31.591795 radinitio-1.2.1/radinitio.egg-info/
+-rw-r--r--   0 angelgr2   (502) staff       (20)    68551 2023-06-26 18:42:31.000000 radinitio-1.2.1/radinitio.egg-info/PKG-INFO
+-rw-r--r--   0 angelgr2   (502) staff       (20)      274 2023-06-26 18:42:31.000000 radinitio-1.2.1/radinitio.egg-info/SOURCES.txt
+-rw-r--r--   0 angelgr2   (502) staff       (20)        1 2023-06-26 18:42:31.000000 radinitio-1.2.1/radinitio.egg-info/dependency_links.txt
+-rw-r--r--   0 angelgr2   (502) staff       (20)       30 2023-06-26 18:42:31.000000 radinitio-1.2.1/radinitio.egg-info/requires.txt
+-rw-r--r--   0 angelgr2   (502) staff       (20)       10 2023-06-26 18:42:31.000000 radinitio-1.2.1/radinitio.egg-info/top_level.txt
+drwxr-xr-x   0 angelgr2   (502) staff       (20)        0 2023-06-26 18:42:31.592198 radinitio-1.2.1/scripts/
+-rwxr-xr-x   0 angelgr2   (502) staff       (20)       36 2023-05-31 23:04:50.000000 radinitio-1.2.1/scripts/radinitio
+-rw-r--r--   0 angelgr2   (502) staff       (20)       38 2023-06-26 18:42:31.593688 radinitio-1.2.1/setup.cfg
+-rwxr-xr-x   0 angelgr2   (502) staff       (20)     1150 2023-06-26 18:39:32.000000 radinitio-1.2.1/setup.py
```

### Comparing `radinitio-1.2.0/ChangeLog` & `radinitio-1.2.1/ChangeLog`

 * *Files identical despite different names*

### Comparing `radinitio-1.2.0/LICENSE` & `radinitio-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radinitio-1.2.0/PKG-INFO` & `radinitio-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,9 @@
-Metadata-Version: 2.1
-Name: radinitio
-Version: 1.2.0
-Summary: A package for the simulation of RADseq data.
-Home-page: http://catchenlab.life.illinois.edu/radinitio
-Author: Angel G. Rivera-Colon <arcolon14@gmail.com>, Nicolas Rochette <rochette@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>
-Author-email: angelgr2@illinois.edu
-Project-URL: Manual, http://catchenlab.life.illinois.edu/radinitio/manual/
-Project-URL: Source, https://bitbucket.org/angelgr2/radinitio/src/default/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RADinitio
 
-![RADinitio logo](image.png)
-
 **RADinitio** is a pipeline for the assessment of RADseq experiments via prospective and retrospective data simulation. Sequencing data is generated *de novo* from a population of individuals via a coalescent simulation under a user-defined demographic model using **msprime**. The genetic variants in each sample are simulated in a genomic context that can impact downstream generation of RAD loci and sequencing reads. The per-individual sequences are then treated to an *in silico* RADseq library preparation. The components of the library are defined by the user, allowing for the exploration of parameters including restriction enzyme selection, insert size, sequencing coverage, and PCR duplicate distribution (generated using the **decoratio** software). **RADinitio** simulations can also be applied retrospectively by comparing and modelling sources of error in empirical datasets. The purpose of **RADinitio** is for researchers to fully explore possible variables in their data generation process to ensure that their protocol selection and library preparation is performed optimally, within the limitations of technical and experimental error.
 
 ## Citation
 
 If you use **RADinitio** in your work, please cite the [2021 *Mol Ecol Resour*](https://doi.org/10.1111/1755-0998.13163) manuscript:
 
 > Rivera-Colón, AG, Rochette, NC, Catchen, JM. (2021) Simulation with RADinitio improves RADseq experimental design and sheds light on sources of missing data. *Mol Ecol Resour* 21: 363– 378. <https://doi.org/10.1111/1755-0998.13163>
@@ -108,15 +90,15 @@
 
 #### Pipeline stages (these options are mutually exclusive)
 
 `--simulate-all` : Run all the **RADinitio** stages (simulate a population, make a library, and sequence the library) (Default)
 
 `--make-population` : Simulate and process variants. Produces genome-wide VCF.
 
-`--make-library-seq` : Simulate and sequence a RAD library. Requires exising `radinitio.make-population` run.
+`--make-library-seq` : Simulate and sequence a RAD library. Requires existing `radinitio.make-population` run.
 
 `--tally-rad-loci` : Calculate the number of kept RAD loci in the genome.
 
 #### Required input/output
 
 `-g`, `--genome` : (*str*) Path to reference genome (fasta file, may be gzipped). **Required**
 
@@ -188,15 +170,15 @@
 
 `--genome-rec-rate` : (*float*) MsprimeOptions: Average per-base per-generation recombination rate for the whole genome. (default = 3e-8)
 
 `--genome-mut-rate` : (*float*) MsprimeOptions: Average per-base per-generation mutation rate for the whole genome. (default = 7e-8)
 
 `--pop-mig-rate` : (*float*) MsprimeOptions: Total per-population per-generation immigration rate. (default = 0.001)
 
-`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (deault = 0.0)
+`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (default = 0.0)
 
 `--lib-bar1-len` : (*int*) LibraryOptions: Length of the forward-read barcode in bp. (default = 5)
 
 `--lib-bar2-len` : (*int*) LibraryOptions: Length of the reverse-read barcode in bp. (default = 0)
 
 `--lib-5-error` : (*float*) LibraryOptions: Frequency of sequencing errors at the 5' end of the reads. (default = 0.001)
 
@@ -216,36 +198,36 @@
 
 `--pcr-pol-error` : (*float*) PCRDups: Probability of PCR errors, based on the error rate of the Phusion HF polymerase. (default = 4.4e-7)
 
 ## Examples
 
 ### Getting started
 
-The simplest **RADinitio** simulation requres just the specification of a reference genome fasta (`--genomne`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
+The simplest **RADinitio** simulation requires just the specification of a reference genome fasta (`--genome`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
 
 Using the default parameters runs the whole simulation pipeline and generates all possible outputs (`--simulate-all`). This will simulate a standard island model for 2 populations, sequencing 10 individuals per population (20 total). The single-digest library will be made with the enzyme *SbfI*, using the default insert size distribution (mean 350 bp and stdev 35bp) and generating 2x150bp reads at 20x coverage.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/         # Path to output directory
 ```
 
 ### Controlling the input reference sequences
 
-The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The first example is using a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
+The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The next example uses a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
 
 ```sh
 chr1
 chr2
 chr3
 ...
 ```
 
-Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
+Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with many small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
 
 Here we run the same default **RADinitio** simulation as before, but instead we provide a `chrom_list.txt` file containing the IDs of the target sequences of interest.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/ \       # Path to output directory
@@ -262,20 +244,20 @@
 ```
 
 The `radinitio.log` file reports the number of sequences read from the reference genome fasta file, as well as those kept after selection/filtering. For example, here the reference genome contained 1,844 total sequences; however, we only selected 24 (e.g., 24 chromosomes) for downstream analysis.
 
 ```sh
 Loading the genome...
     Read 1,844 sequences from the input FASTA.
-    Loaded 24 chromsome/scaffold sequences.
+    Loaded 24 chromosome/scaffold sequences.
 ```
 
 ### Modifying the library parameters
 
-**RADinitio** allows the user to specify the paramters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
+**RADinitio** allows the user to specify the parameters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -297,44 +279,44 @@
     --enz2 MspI \                          # Use the MspI enzyme as the secondary (common) cutter
     --min-insert 225 \                     # Min insert size of 225 bp
     --max-insert 475 \                     # Max insert size of 475 bp
     --coverage 30 \                        # Depth of coverage of 30x
     --read-length 100                      # Read length of 100bp (paired-end 2x100bp)
 ```
 
-More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these optionns can be left default for the large majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
+More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify the length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these options can be left default for the vast majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
 
 ### PCR duplicates model
 
-**RADinitio** can be used to simulate an study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
+**RADinitio** can be used to simulate and study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
 
-The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define a the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
+The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
 
 When no `--pcr-model` is selection, the `radinitio.log` reports the following information:
 
 ```sh
 PCR model options:
-    PCR amplication model:   None (No PCR)
+    PCR amplification model:   None (No PCR)
     PCR cycles:              None
     PCR duplicate rate:      0.00%
 ```
 
-We see that no PCR model was selected (defaults to `None`). Thus. there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
+We see that no PCR model was selected (defaults to `None`). Thus, there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
 
 In contrast, the user can choose and apply a PCR model to the downstream data. Since version `1.2.0`, **RADinitio** uses the PCR models described by the **decoratio** software ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)). These PCR models are largely comprised of two steps: 1) an amplification model (which describes the amplification probability and noise applied over some number of PCR cycles) and 2) a depth/complexity ratio which describes how the sequenced reads are sampled from the pool of amplified molecules.
 
-The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distrubition for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
+The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distribution for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
 
-The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model used the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
+The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model uses the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
 
 In addition to the amplification model, the other (and more important parameter) controlling the PCR duplicate distribution is the **de**pth/**co**mplexity **ratio**. This value describes the ratio of sequenced molecules (the depth of coverage) to the molecular complexity (the number of unique molecules). In other words, if sequencing at 30x, but the complexity is 10 molecules, the library has a depth/complexity ratio of 3:1. This means that, while it is possible to sequence 30 reads, only 10 of them can have unique information and the remaining 20 reads will be duplicates.`radinitio` users can specify this ratio using the `--pcr-deco-ratio` option. Smaller values (<1) will generally reduce the rate of PCR duplicates seen in the simulated library. See [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800) for further information regarding the depth/complexity ratio.
 
 #### Simulating libraries with low/moderate PCR duplicate rate
 
-Using the models and paramters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library contruction paramters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inhertited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% change of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficienty model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
+Using the models and parameters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library construction parameters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inherited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% chance of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficiency model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -349,27 +331,27 @@
     --pcr-deco-ratio 0.10                  # De/Co ratio of 1:10 or 0.1
 ```
 
 After running this simulation, we can see the description of the PCR model on the `radinitio.log` file:
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.45:0.2
+    PCR amplification model: inheff:12:0.45:0.2
     PCR cycles:              12
     depth/complexity ratio:  0.1
     PCR duplicates rate:     17.432%
 ```
 
 This PCR model generated a PCR duplicate rate of 17.4%. We can see a per-clone size breakdown of the frequency of these duplicates (i.e., the proportion of clones with a given number of duplicates) in the `sequenced_clone_distrib.tsv` file. Additionally, the log reports the parameters of the model, including the number of cycles, depth/complexity ratio, and the "model string". This "model string" (`inheff:12:0.45:0.2` in this example) is the definition of the model, as specified by **decoratio**. In this example, the string describes (in order, separated by ":"): 1) the selected model (`inheff`), number of PCR cycles (`12`), mean amplification probability (`0.45`), and the amplification probability standard deviation (`0.2`). Different models used by **RADinitio** have different specifications and model string. See the **decoratio** documentation for additional details on model specifications.
 
-#### Simulating libraries with high PCR duplicate rate
+#### Simulating libraries with high PCR duplicate rates
 
-**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may provide useful to, e.g., observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information.
+**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may be useful (e.g., to observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information).
 
-In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR paramters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
+In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR parameters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -384,49 +366,49 @@
     --pcr-deco-ratio 10                    # De/Co ratio of 10:1 or 10
 ```
 
 After completing the simulation, we evaluate the results provided in the `radinitio.log` file.
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.25:0.5
+    PCR amplification model: inheff:12:0.25:0.5
     PCR cycles:              12
     depth/complexity ratio:  10
     PCR duplicates rate:     94.019%
 ```
 
-We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all their individual contribution to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplificaton. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
+We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all, the individual contribution of the number of cycles to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplification. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
 
-WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. In one example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
+WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. For example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
 
 ### Changing the demographic model
 
 The `radinitio` wrapper script simulates a population using an island model from **msprime** ([Kelleher et al. 2016](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004842/); [Baumdicker et al. 2022](https://doi.org/10.1093/genetics/iyab229)). By default, this model simulates two populations, each with an effective population size (Ne) of 5,000 individuals. Ten individuals are sampled and sequenced per population, for a total of 20 individuals in the library.
 
 The wrapper script allow the user to modify some parameters of this model. For example, the user can change the number of populations (`--n-pops`), the effective size of the populations (`--pop-eff-size`), and the number of sampled individuals per population (`--n-seq-indv`). Other parameters, e.g., controlling the migration rate (`--pop-mig-rate`), growth rate (`--pop-growth-rate`), and mutation rate (`--genome-mut-rate`), are available in the advanced options.
 
-As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 indididuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
+As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 individuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./sims_sdRAD_4pops/ \        # Path to output directory
     --n-pops 4 \                           # Number of populations in the island model
-    --pop-eff-size 2500 \                  # Effecitve size (Ne) of the populations
+    --pop-eff-size 2500 \                  # Effective size (Ne) of the populations
     --n-seq-indv 25 \                      # Number of individuals to sequence per-population (100 total)
     --pop-mig-rate 0.025                   # Per generation immigration rate
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI                             # Use the SbfI enzyme
 ```
 
 The options in the wrapper are useful for more general simulations, e.g., studying the effects of genetic diversity over the final RADseq library. However, they are limited to a relatively simple island model and the parameters are applied equaly to all populations (i.e., all populations will be of the same size and migration rates will be symmetrical). More detailed demographic models are available through the [**msprime** documentation](https://tskit.dev/msprime/docs/latest/intro.html). **RADinitio** users can implement these complex simulations using the **msprime** Python API, after which they can generate *in silico* RADseq libraries from the simulated populations (see section on `--make-library-seq` below).
 
 ### Tallying RAD loci in the genome
 
-Perhaps the common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
+The most common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
 
 An estimation of the number of RADseq loci in a genome can be easily generated using the `--tally-rad-loci` option in the `radinitio` wrapper script. This option only identifies and filters the RADseq loci found in the genome based on the library properties, skipping the simulation of the population(s) and the generation of sequencing reads.
 
 For example, here we tally the number of RADseq loci in the genome using the default library parameters (single-digest library with *SbfI*).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
@@ -445,21 +427,21 @@
     Removed 2 loci (0.0%) containing excess (>10.0%) of Ns in sequence.
     Removed 428 loci (7.0%) in close proximity (<1000bp) to another locus.
     Retained 5,687 loci (92.9%) for downstream analysis.
 
     See `./output/tally-rad-loci/ri_sdRAD_sbfI/ref_loci_vars/reference_rad_loci.stats.gz` for a detailed description of the per-cutsite position and status.
 ```
 
-In this example, **RADinitio** foind 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`), each yielding two loci in the negative and positive DNA strands. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6 thousand loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
+In this example, **RADinitio** found 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`) were found in the genome. Each cutsite yields two loci: one in the negative and one in the positive DNA strand. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6k loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
 
-However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. By default, this distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions of uncertain sequences.
+However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. This distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions with uncertain sequences.
 
-More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping from one another on a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
+More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping with one another in a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
 
-Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`).
+Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -478,15 +460,15 @@
 chr6       14834    neg      rm_excess_Ns
 chr6       14834    pos      rm_excess_Ns
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
-We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (whoch was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
+We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (which was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \   # Path to reference genome
     --out-dir ./tally_ecoRI_loci/ \       # Path to output directory
     --library-type sdRAD \                # Simulate a single-digest library
     --enz EcoRI                           # Use the EcoRI enzyme
@@ -499,19 +481,19 @@
     Found a total of 25,836 EcoRI loci in the genome (use this number for coverage calculations).
     Removed 14 loci (0.0%) too close to the ends of the reference sequences.
     Removed 26 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 4,648 loci (18.0%) in close proximity (<1000bp) to another locus.
     Retained 21,148 loci (81.8%) for downstream analysis.
 ```
 
-As expected given its smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impact their filtering, as a higher proportion of loci are removed due to close proximity.
+As expected, given the smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library, the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impacts their filtering, as a higher proportion of loci are removed due to close proximity.
 
 #### Tallying loci in ddRAD libraries
 
-The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. In ddRAD libraries, the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
+The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. However, in ddRAD libraries the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
 
 Here, we tally the number of loci in a ddRAD library generated using the *EcoRI* enzyme as the main cutter and *MseI* as the secondary (common) cutter. We are using the default insert size distribution (mean of 350bp and stdev of 37bp). This distribution corresponds to a mimumum insert size of 276bp and a max insert size of 424bp (i.e., can also be specified with the `--min-insert`/`--max-insert` options).
 
 ```sh
 radinitio --tally-rad-loci \             # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \  # Path to the reference genome
     --out-dir ./count_ddrad_loci/ \      # Path to output directory
@@ -557,15 +539,17 @@
     Note: an additional 5,149 loci were found outside the target insert size range.
     Removed 4 loci (0.0%) too close to the ends of the reference sequences.
     Removed 11 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 3,667 loci (17.9%) in close proximity (<1000bp) to another locus.
     Retained 16,783 loci (82.0%) for downstream analysis.
 ```
 
-The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci. Note, however, that many of these loci might not be recoverage experimentally, e.g., too small to be feasibly sequenceable (i.e., if they are smaller than the desired read length) or larger than the capicity of the PCR and/or sequencer. Thus, the objective should not be to recover all the available loci in the genome.
+The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci.
+
+Note, however, that many of these loci might not be recoverable experimentally, e.g., too small to be feasibly sequenceable (if they are smaller than the desired read length) or larger than the capacity of the PCR and/or sequencer. Thus, the objective is not to recover all the available loci in the genome.
 
 ### Simulating a population and generating genomic variants
 
 The `--make-population` option from the `radinitio` wrapper allows the user to run the initial stage of the **RADinitio** pipeline, simulating a population using the **msprime** island model and generating a genome-wide VCF with the simulated genetic variants. This mode is library agnostic, and does not extract RADseq loci nor generates sequencing reads. The purpose of this mode is to generate a fixed set of genetic variants that can then be processed under a variety of library configurations (see `--make-library-seq` example below).
 
 In this example, we will run **RADinitio** under the `--make-population` mode. We will simulate an island model of 6 populations or demes, each with an effective population size of 10,000. We will sequence 25 individuals per population, or 150 individuals in total. Additionally, we will filter the input genome to only keep sequences larger than 1 Mbp.
 
@@ -583,19 +567,19 @@
 
 1. An `msprime_vcfs/` directory with the raw simulated variants for each individual sequence
 2. A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ref_loci_vars/ri_master.vcf.gz`)
 3. A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population.
 
 ### Simulate a library from an existing population and variants
 
-Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** run made by the user.
+Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** (or other simulators such as **SLiM** or **stdpopsim**) run made by the user.
 
-To run `radinitio` in the `--make-library-seq` pipeline stage, the user most provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and most contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
+To run `radinitio` in the `--make-library-seq` pipeline stage, the user must provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and must contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
 
-Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. The output of 2x100 bp reads will be exported in fastq format (`--read-out-fmt fastq`). We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./SbfI_library/ \                # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -606,15 +590,15 @@
     --pcr-model inheff \                       # Inherited efficiency amplification model
     --pcr-cycles 9 \                           # Amplify for 9 PCR cycles
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
-Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads, in fastq format. We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./PstI-MspI_library/ \           # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -628,32 +612,32 @@
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
 ### Additional examples
 
-#### How to generate chromosome list
+#### How to generate a chromosome list file
 
-The simplest way to generate a chromosome list file is to extact the sequence IDs form the desired fasta. The sequences must not contain the "`>`" character as this is part of the fasta header convention and are not part of the ID. This can be done by pipping a few commands in Bash:
+The simplest way to generate a chromosome list file is to extract the sequence IDs from the desired fasta. The IDs must not begin with the "`>`" character as this is part of the fasta header convention and not part of the ID. This can be done by piping a few commands in Bash:
 
 1. Open the gzipped file into the stream (`zcat`)
 2. Select the lines starting with `>` (`grep`)
 3. Remove any comments present after whitespace (`cut`)
 4. Remove the `>` (`tr`)
 5. Save to new file
 
 ```sh
 # Create a chrom_list.tsv from all the sequences in the gzipped reference
 zcat reference.fa.gz | grep '^>' | cut -f1 -d ' ' | tr -d '>' > chrom_list.tsv
 ```
 
-The user can apply additional filters to remove additional sequences.
+The user can apply other filters to remove additional sequences.
 
-An additional way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
+Another way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
 
 ```sh
 # Uncompress genome
 gunzip reference.fa.gz
 # Run samtools faidx
 samtools faidx reference.fa
 # Re-compress the genome
@@ -680,14 +664,15 @@
 ```
 
 ## Output directories
 
 The outputs of a default `radinitio --simulate-all` run are:
 
 ```sh
+$ ls *
 output_directory:
 popmap.tsv  radinitio.log  sequenced_clone_distrib.tsv
 
 output_directory/msprime_vcfs:
 chr1.vcf.gz   chr7.vcf.gz  chr13.vcf.gz  chr19.vcf.gz
 chr2.vcf.gz   chr8.vcf.gz  chr14.vcf.gz  chr20.vcf.gz
 chr3.vcf.gz   chr9.vcf.gz  chr15.vcf.gz  chr21.vcf.gz
@@ -727,31 +712,33 @@
 output_directory/ref_loci_vars:
 reference_rad_loci_SbfI.fa.gz     ri_master.vcf.gz
 reference_rad_loci_SbfI.stats.gz
 ```
 
 ### Top level directory
 
+The main (or top level) output directory of a `radinitio` simulation run. Contains three text files, in addition to several subdirectories described below.
+
 #### Population Map
 
-A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs on the first column, and population IDs on the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
+A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs in the first column, and population IDs in the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
 
 ```sh
 msp_00<tab>pop0
 msp_01     pop0
 msp_02     pop0
 msp_03     pop1
 msp_04     pop1
 msp_05     pop1
 ...
 ```
 
 #### PCR clones distribution
 
-The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution generated during the most recent run. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
+The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
 
 ```sh
 clone_size  n_errors  clone_prob
 0           0         0
 1           0         1.0
 1           1         0
 ```
@@ -773,27 +760,27 @@
 ...
 ```
 
 Here, the `clone_size` describes the number of molecules in a clone. A clone size of *n* means that *n* molecules where sampled from a single clone. *n* copies of the same sequence will be saved as reads, with *n - 1* being PCR duplicates. Moreover, clones can also contain molecules with PCR error (`n_errors`). A clone of size *n* can contain up to *n* molecules with error. `clone_prob` is the probability of sampling a clone with given size and error properties, and describes the distribution of PCR duplicates and errors in the simulated data.
 
 #### Log file
 
-The `radinitio.log` file is generated on the top level outoput directory. It contains information on the **RADinitio** version, a time stamp on the current run, as well as information on the different stages of the program.
+The `radinitio.log` file is generated in the top level output directory. It contains information about the **RADinitio** version, a time stamp of the current run, as well as information on the different stages of the program.
 
 ### Msprime VCFs
 
 The `msprime_vcfs/` directory containing the genetic variants simulated by **msprime** (derived from the [`tskit.TreeSequence.write_vcf()`](https://tskit.dev/tskit/docs/stable/python-api.html#tskit.TreeSequence.write_vcf) function) for each individual chromosome.
 
 ### Reference loci/vars directory
 
 The `ref_loci_vars` contains the reference information for the simulated RAD loci as well as the genome-wide variants generated from the population simulation.
 
 #### Genomic VCF
 
-A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspeficied alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
+A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspecified alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
 
 #### Reference RAD loci
 
 The reference loci file reports the sequence of all the reference loci present in the genome, i.e., the genomic sequence corresponding to the 1 Kbp spanning the extracted loci. These sequenced are exported as a gzipped fasta file (`reference_rad_loci.fa.gz`).
 
 ```sh
 >t0000n ref_pos=chr1:10818-11817
@@ -804,19 +791,19 @@
 TGCAGGGAGGGTGGGAGAACTTTCTCCGTTAACAAAAAATGAGGCTCCGTCTCTGTGATTC...
 >t0003n ref_pos=chr3:23979-24978
 TGCAGGTCAGTGAACTCACCCCCACTGCAGGCGTCCTCTGGACTGAACCAACAGAAGCTGG...
 >t0004n ref_pos=chr3:24974-25973
 TGCAGGCGATCCAGTCCACAGACCGGCTACCTGGATCATGCCGACGTCCGACAGTGTCTCC...
 ```
 
-The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsute on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
+The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsite on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
 
 #### Locus Status
 
-The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
+The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -837,42 +824,42 @@
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
 ### RAD alleles
 
-The `rad_alleles/` directoru contains per-individual gzipped fasta files contining the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
+The `rad_alleles/` directory contains per-individual gzipped fasta files containing the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
 
 ```sh
 >reference_locus_id:sample_id:allele_i
 ```
 
-Here, `reference_locus_id` referes to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
+Here, `reference_locus_id` refers to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
 
 ```sh
 >t0n:msp_0:a1
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t0n:msp_0:a2
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t1p:msp_0:a1
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCAGAAACATATTAAAGTTG...
 >t1p:msp_0:a2
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCACAAACATATTAAAGTTG...
 ```
 
 ### RAD reads
 
-The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files contining the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
+The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files containing the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
 
 ```sh
 reference_locus_id:sample_id:allele_i:clone_id:duplicate_i/read_pair
 ```
 
-The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` referes to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
+The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` refers to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
 
 Notice in the fasta example below that for reads 3 and 4, they both have a `clone_id` of 3. Read 3 has a `clone_i` of 1, meaning is the first read in the clone. Read 4 has a `clone_id` of 2, meaning it is the second read in the clone and thus a duplicate product of PCR.
 
 ```sh
 >t5n:msp_0:a2:1:1/1
 TGCAGGCTTAGGCTACACCCAACGAGCCACTGGGTGCAGTTGGACCCGAGGGATCTGTAT...
 >t4n:msp_0:a1:2:1/1
@@ -881,22 +868,27 @@
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t2n:msp_0:a2:3:2/1
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t5p:msp_0:a1:4:1/1
 TGCAGGGCTTCCACTCCATACTTGTAAAATTAGGGGAAAACACTTTTTTTAACCTCCCAG...
 ```
 
-The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the indentity of PCR clones.
+The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the identity of PCR clones.
 
 ## Questions?
 
 If you have any questions or are encountering any problems when running **RADinitio**, please drop your questions in the [Stacks-users mailing list](https://groups.google.com/g/stacks-users).
 
 ## Changelog
 
+### RADinitio `1.2.1` - 2023 Jun 26
+
+* Bug Fix: Updated error in `setup.py` python version requirements.
+* Others: Fixed typos and other small errors in the docs.
+
 ### RADinitio `1.2.0` - 2023 Jun 23
 
 * Feature: Updated to `decoratio` PCR amplification models
 * Feature: Updated reporting of RAD loci tally
 * Feature: Several advanced options available in `radinitio` wrapper
 * Bug Fix: Program now prints warning and stops when no sequences are loaded from genome.
 * Other: General re-working and refactoring of main functions.
@@ -916,15 +908,15 @@
 * Other: Changed default value for template/read ratio in PCR model
 * Other: Added `--version` flag in main wrapper. Also reported in other intermediary files.
 * Other: General formatting updates to logs.
 
 ### RADinitio `1.0.3` - 2019 May 16
 
 * Fixed bug when reporting number of loci in log
-* Changed the requierements of the output directory - it now MUST exist
+* Changed the requirements of the output directory - it now MUST exist
 
 ### RADinitio `1.0.2` - 2019 May 13
 
 * Updated contents of package distribution build.
 
 ### RADinitio `1.0.1` - 2019 May 13
```

### Comparing `radinitio-1.2.0/README.md` & `radinitio-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
-# RADinitio
+Metadata-Version: 2.1
+Name: radinitio
+Version: 1.2.1
+Summary: A package for the simulation of RADseq data.
+Home-page: http://catchenlab.life.illinois.edu/radinitio
+Author: Angel G. Rivera-Colon <arcolon14@gmail.com>, Nicolas Rochette <rochette@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>
+Author-email: arcolon14@gmail.com
+Project-URL: Manual, http://catchenlab.life.illinois.edu/radinitio/manual/
+Project-URL: Source, https://bitbucket.org/angelgr2/radinitio/src/default/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-![RADinitio logo](image.png)
+# RADinitio
 
 **RADinitio** is a pipeline for the assessment of RADseq experiments via prospective and retrospective data simulation. Sequencing data is generated *de novo* from a population of individuals via a coalescent simulation under a user-defined demographic model using **msprime**. The genetic variants in each sample are simulated in a genomic context that can impact downstream generation of RAD loci and sequencing reads. The per-individual sequences are then treated to an *in silico* RADseq library preparation. The components of the library are defined by the user, allowing for the exploration of parameters including restriction enzyme selection, insert size, sequencing coverage, and PCR duplicate distribution (generated using the **decoratio** software). **RADinitio** simulations can also be applied retrospectively by comparing and modelling sources of error in empirical datasets. The purpose of **RADinitio** is for researchers to fully explore possible variables in their data generation process to ensure that their protocol selection and library preparation is performed optimally, within the limitations of technical and experimental error.
 
 ## Citation
 
 If you use **RADinitio** in your work, please cite the [2021 *Mol Ecol Resour*](https://doi.org/10.1111/1755-0998.13163) manuscript:
 
@@ -92,15 +106,15 @@
 
 #### Pipeline stages (these options are mutually exclusive)
 
 `--simulate-all` : Run all the **RADinitio** stages (simulate a population, make a library, and sequence the library) (Default)
 
 `--make-population` : Simulate and process variants. Produces genome-wide VCF.
 
-`--make-library-seq` : Simulate and sequence a RAD library. Requires exising `radinitio.make-population` run.
+`--make-library-seq` : Simulate and sequence a RAD library. Requires existing `radinitio.make-population` run.
 
 `--tally-rad-loci` : Calculate the number of kept RAD loci in the genome.
 
 #### Required input/output
 
 `-g`, `--genome` : (*str*) Path to reference genome (fasta file, may be gzipped). **Required**
 
@@ -172,15 +186,15 @@
 
 `--genome-rec-rate` : (*float*) MsprimeOptions: Average per-base per-generation recombination rate for the whole genome. (default = 3e-8)
 
 `--genome-mut-rate` : (*float*) MsprimeOptions: Average per-base per-generation mutation rate for the whole genome. (default = 7e-8)
 
 `--pop-mig-rate` : (*float*) MsprimeOptions: Total per-population per-generation immigration rate. (default = 0.001)
 
-`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (deault = 0.0)
+`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (default = 0.0)
 
 `--lib-bar1-len` : (*int*) LibraryOptions: Length of the forward-read barcode in bp. (default = 5)
 
 `--lib-bar2-len` : (*int*) LibraryOptions: Length of the reverse-read barcode in bp. (default = 0)
 
 `--lib-5-error` : (*float*) LibraryOptions: Frequency of sequencing errors at the 5' end of the reads. (default = 0.001)
 
@@ -200,36 +214,36 @@
 
 `--pcr-pol-error` : (*float*) PCRDups: Probability of PCR errors, based on the error rate of the Phusion HF polymerase. (default = 4.4e-7)
 
 ## Examples
 
 ### Getting started
 
-The simplest **RADinitio** simulation requres just the specification of a reference genome fasta (`--genomne`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
+The simplest **RADinitio** simulation requires just the specification of a reference genome fasta (`--genome`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
 
 Using the default parameters runs the whole simulation pipeline and generates all possible outputs (`--simulate-all`). This will simulate a standard island model for 2 populations, sequencing 10 individuals per population (20 total). The single-digest library will be made with the enzyme *SbfI*, using the default insert size distribution (mean 350 bp and stdev 35bp) and generating 2x150bp reads at 20x coverage.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/         # Path to output directory
 ```
 
 ### Controlling the input reference sequences
 
-The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The first example is using a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
+The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The next example uses a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
 
 ```sh
 chr1
 chr2
 chr3
 ...
 ```
 
-Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
+Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with many small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
 
 Here we run the same default **RADinitio** simulation as before, but instead we provide a `chrom_list.txt` file containing the IDs of the target sequences of interest.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/ \       # Path to output directory
@@ -246,20 +260,20 @@
 ```
 
 The `radinitio.log` file reports the number of sequences read from the reference genome fasta file, as well as those kept after selection/filtering. For example, here the reference genome contained 1,844 total sequences; however, we only selected 24 (e.g., 24 chromosomes) for downstream analysis.
 
 ```sh
 Loading the genome...
     Read 1,844 sequences from the input FASTA.
-    Loaded 24 chromsome/scaffold sequences.
+    Loaded 24 chromosome/scaffold sequences.
 ```
 
 ### Modifying the library parameters
 
-**RADinitio** allows the user to specify the paramters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
+**RADinitio** allows the user to specify the parameters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -281,44 +295,44 @@
     --enz2 MspI \                          # Use the MspI enzyme as the secondary (common) cutter
     --min-insert 225 \                     # Min insert size of 225 bp
     --max-insert 475 \                     # Max insert size of 475 bp
     --coverage 30 \                        # Depth of coverage of 30x
     --read-length 100                      # Read length of 100bp (paired-end 2x100bp)
 ```
 
-More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these optionns can be left default for the large majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
+More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify the length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these options can be left default for the vast majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
 
 ### PCR duplicates model
 
-**RADinitio** can be used to simulate an study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
+**RADinitio** can be used to simulate and study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
 
-The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define a the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
+The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
 
 When no `--pcr-model` is selection, the `radinitio.log` reports the following information:
 
 ```sh
 PCR model options:
-    PCR amplication model:   None (No PCR)
+    PCR amplification model:   None (No PCR)
     PCR cycles:              None
     PCR duplicate rate:      0.00%
 ```
 
-We see that no PCR model was selected (defaults to `None`). Thus. there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
+We see that no PCR model was selected (defaults to `None`). Thus, there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
 
 In contrast, the user can choose and apply a PCR model to the downstream data. Since version `1.2.0`, **RADinitio** uses the PCR models described by the **decoratio** software ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)). These PCR models are largely comprised of two steps: 1) an amplification model (which describes the amplification probability and noise applied over some number of PCR cycles) and 2) a depth/complexity ratio which describes how the sequenced reads are sampled from the pool of amplified molecules.
 
-The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distrubition for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
+The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distribution for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
 
-The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model used the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
+The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model uses the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
 
 In addition to the amplification model, the other (and more important parameter) controlling the PCR duplicate distribution is the **de**pth/**co**mplexity **ratio**. This value describes the ratio of sequenced molecules (the depth of coverage) to the molecular complexity (the number of unique molecules). In other words, if sequencing at 30x, but the complexity is 10 molecules, the library has a depth/complexity ratio of 3:1. This means that, while it is possible to sequence 30 reads, only 10 of them can have unique information and the remaining 20 reads will be duplicates.`radinitio` users can specify this ratio using the `--pcr-deco-ratio` option. Smaller values (<1) will generally reduce the rate of PCR duplicates seen in the simulated library. See [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800) for further information regarding the depth/complexity ratio.
 
 #### Simulating libraries with low/moderate PCR duplicate rate
 
-Using the models and paramters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library contruction paramters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inhertited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% change of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficienty model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
+Using the models and parameters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library construction parameters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inherited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% chance of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficiency model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -333,27 +347,27 @@
     --pcr-deco-ratio 0.10                  # De/Co ratio of 1:10 or 0.1
 ```
 
 After running this simulation, we can see the description of the PCR model on the `radinitio.log` file:
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.45:0.2
+    PCR amplification model: inheff:12:0.45:0.2
     PCR cycles:              12
     depth/complexity ratio:  0.1
     PCR duplicates rate:     17.432%
 ```
 
 This PCR model generated a PCR duplicate rate of 17.4%. We can see a per-clone size breakdown of the frequency of these duplicates (i.e., the proportion of clones with a given number of duplicates) in the `sequenced_clone_distrib.tsv` file. Additionally, the log reports the parameters of the model, including the number of cycles, depth/complexity ratio, and the "model string". This "model string" (`inheff:12:0.45:0.2` in this example) is the definition of the model, as specified by **decoratio**. In this example, the string describes (in order, separated by ":"): 1) the selected model (`inheff`), number of PCR cycles (`12`), mean amplification probability (`0.45`), and the amplification probability standard deviation (`0.2`). Different models used by **RADinitio** have different specifications and model string. See the **decoratio** documentation for additional details on model specifications.
 
-#### Simulating libraries with high PCR duplicate rate
+#### Simulating libraries with high PCR duplicate rates
 
-**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may provide useful to, e.g., observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information.
+**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may be useful (e.g., to observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information).
 
-In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR paramters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
+In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR parameters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -368,49 +382,49 @@
     --pcr-deco-ratio 10                    # De/Co ratio of 10:1 or 10
 ```
 
 After completing the simulation, we evaluate the results provided in the `radinitio.log` file.
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.25:0.5
+    PCR amplification model: inheff:12:0.25:0.5
     PCR cycles:              12
     depth/complexity ratio:  10
     PCR duplicates rate:     94.019%
 ```
 
-We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all their individual contribution to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplificaton. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
+We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all, the individual contribution of the number of cycles to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplification. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
 
-WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. In one example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
+WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. For example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
 
 ### Changing the demographic model
 
 The `radinitio` wrapper script simulates a population using an island model from **msprime** ([Kelleher et al. 2016](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004842/); [Baumdicker et al. 2022](https://doi.org/10.1093/genetics/iyab229)). By default, this model simulates two populations, each with an effective population size (Ne) of 5,000 individuals. Ten individuals are sampled and sequenced per population, for a total of 20 individuals in the library.
 
 The wrapper script allow the user to modify some parameters of this model. For example, the user can change the number of populations (`--n-pops`), the effective size of the populations (`--pop-eff-size`), and the number of sampled individuals per population (`--n-seq-indv`). Other parameters, e.g., controlling the migration rate (`--pop-mig-rate`), growth rate (`--pop-growth-rate`), and mutation rate (`--genome-mut-rate`), are available in the advanced options.
 
-As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 indididuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
+As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 individuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./sims_sdRAD_4pops/ \        # Path to output directory
     --n-pops 4 \                           # Number of populations in the island model
-    --pop-eff-size 2500 \                  # Effecitve size (Ne) of the populations
+    --pop-eff-size 2500 \                  # Effective size (Ne) of the populations
     --n-seq-indv 25 \                      # Number of individuals to sequence per-population (100 total)
     --pop-mig-rate 0.025                   # Per generation immigration rate
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI                             # Use the SbfI enzyme
 ```
 
 The options in the wrapper are useful for more general simulations, e.g., studying the effects of genetic diversity over the final RADseq library. However, they are limited to a relatively simple island model and the parameters are applied equaly to all populations (i.e., all populations will be of the same size and migration rates will be symmetrical). More detailed demographic models are available through the [**msprime** documentation](https://tskit.dev/msprime/docs/latest/intro.html). **RADinitio** users can implement these complex simulations using the **msprime** Python API, after which they can generate *in silico* RADseq libraries from the simulated populations (see section on `--make-library-seq` below).
 
 ### Tallying RAD loci in the genome
 
-Perhaps the common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
+The most common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
 
 An estimation of the number of RADseq loci in a genome can be easily generated using the `--tally-rad-loci` option in the `radinitio` wrapper script. This option only identifies and filters the RADseq loci found in the genome based on the library properties, skipping the simulation of the population(s) and the generation of sequencing reads.
 
 For example, here we tally the number of RADseq loci in the genome using the default library parameters (single-digest library with *SbfI*).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
@@ -429,21 +443,21 @@
     Removed 2 loci (0.0%) containing excess (>10.0%) of Ns in sequence.
     Removed 428 loci (7.0%) in close proximity (<1000bp) to another locus.
     Retained 5,687 loci (92.9%) for downstream analysis.
 
     See `./output/tally-rad-loci/ri_sdRAD_sbfI/ref_loci_vars/reference_rad_loci.stats.gz` for a detailed description of the per-cutsite position and status.
 ```
 
-In this example, **RADinitio** foind 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`), each yielding two loci in the negative and positive DNA strands. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6 thousand loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
+In this example, **RADinitio** found 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`) were found in the genome. Each cutsite yields two loci: one in the negative and one in the positive DNA strand. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6k loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
 
-However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. By default, this distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions of uncertain sequences.
+However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. This distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions with uncertain sequences.
 
-More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping from one another on a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
+More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping with one another in a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
 
-Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`).
+Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -462,15 +476,15 @@
 chr6       14834    neg      rm_excess_Ns
 chr6       14834    pos      rm_excess_Ns
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
-We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (whoch was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
+We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (which was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \   # Path to reference genome
     --out-dir ./tally_ecoRI_loci/ \       # Path to output directory
     --library-type sdRAD \                # Simulate a single-digest library
     --enz EcoRI                           # Use the EcoRI enzyme
@@ -483,19 +497,19 @@
     Found a total of 25,836 EcoRI loci in the genome (use this number for coverage calculations).
     Removed 14 loci (0.0%) too close to the ends of the reference sequences.
     Removed 26 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 4,648 loci (18.0%) in close proximity (<1000bp) to another locus.
     Retained 21,148 loci (81.8%) for downstream analysis.
 ```
 
-As expected given its smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impact their filtering, as a higher proportion of loci are removed due to close proximity.
+As expected, given the smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library, the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impacts their filtering, as a higher proportion of loci are removed due to close proximity.
 
 #### Tallying loci in ddRAD libraries
 
-The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. In ddRAD libraries, the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
+The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. However, in ddRAD libraries the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
 
 Here, we tally the number of loci in a ddRAD library generated using the *EcoRI* enzyme as the main cutter and *MseI* as the secondary (common) cutter. We are using the default insert size distribution (mean of 350bp and stdev of 37bp). This distribution corresponds to a mimumum insert size of 276bp and a max insert size of 424bp (i.e., can also be specified with the `--min-insert`/`--max-insert` options).
 
 ```sh
 radinitio --tally-rad-loci \             # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \  # Path to the reference genome
     --out-dir ./count_ddrad_loci/ \      # Path to output directory
@@ -541,15 +555,17 @@
     Note: an additional 5,149 loci were found outside the target insert size range.
     Removed 4 loci (0.0%) too close to the ends of the reference sequences.
     Removed 11 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 3,667 loci (17.9%) in close proximity (<1000bp) to another locus.
     Retained 16,783 loci (82.0%) for downstream analysis.
 ```
 
-The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci. Note, however, that many of these loci might not be recoverage experimentally, e.g., too small to be feasibly sequenceable (i.e., if they are smaller than the desired read length) or larger than the capicity of the PCR and/or sequencer. Thus, the objective should not be to recover all the available loci in the genome.
+The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci.
+
+Note, however, that many of these loci might not be recoverable experimentally, e.g., too small to be feasibly sequenceable (if they are smaller than the desired read length) or larger than the capacity of the PCR and/or sequencer. Thus, the objective is not to recover all the available loci in the genome.
 
 ### Simulating a population and generating genomic variants
 
 The `--make-population` option from the `radinitio` wrapper allows the user to run the initial stage of the **RADinitio** pipeline, simulating a population using the **msprime** island model and generating a genome-wide VCF with the simulated genetic variants. This mode is library agnostic, and does not extract RADseq loci nor generates sequencing reads. The purpose of this mode is to generate a fixed set of genetic variants that can then be processed under a variety of library configurations (see `--make-library-seq` example below).
 
 In this example, we will run **RADinitio** under the `--make-population` mode. We will simulate an island model of 6 populations or demes, each with an effective population size of 10,000. We will sequence 25 individuals per population, or 150 individuals in total. Additionally, we will filter the input genome to only keep sequences larger than 1 Mbp.
 
@@ -567,19 +583,19 @@
 
 1. An `msprime_vcfs/` directory with the raw simulated variants for each individual sequence
 2. A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ref_loci_vars/ri_master.vcf.gz`)
 3. A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population.
 
 ### Simulate a library from an existing population and variants
 
-Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** run made by the user.
+Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** (or other simulators such as **SLiM** or **stdpopsim**) run made by the user.
 
-To run `radinitio` in the `--make-library-seq` pipeline stage, the user most provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and most contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
+To run `radinitio` in the `--make-library-seq` pipeline stage, the user must provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and must contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
 
-Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. The output of 2x100 bp reads will be exported in fastq format (`--read-out-fmt fastq`). We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./SbfI_library/ \                # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -590,15 +606,15 @@
     --pcr-model inheff \                       # Inherited efficiency amplification model
     --pcr-cycles 9 \                           # Amplify for 9 PCR cycles
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
-Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads, in fastq format. We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./PstI-MspI_library/ \           # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -612,32 +628,32 @@
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
 ### Additional examples
 
-#### How to generate chromosome list
+#### How to generate a chromosome list file
 
-The simplest way to generate a chromosome list file is to extact the sequence IDs form the desired fasta. The sequences must not contain the "`>`" character as this is part of the fasta header convention and are not part of the ID. This can be done by pipping a few commands in Bash:
+The simplest way to generate a chromosome list file is to extract the sequence IDs from the desired fasta. The IDs must not begin with the "`>`" character as this is part of the fasta header convention and not part of the ID. This can be done by piping a few commands in Bash:
 
 1. Open the gzipped file into the stream (`zcat`)
 2. Select the lines starting with `>` (`grep`)
 3. Remove any comments present after whitespace (`cut`)
 4. Remove the `>` (`tr`)
 5. Save to new file
 
 ```sh
 # Create a chrom_list.tsv from all the sequences in the gzipped reference
 zcat reference.fa.gz | grep '^>' | cut -f1 -d ' ' | tr -d '>' > chrom_list.tsv
 ```
 
-The user can apply additional filters to remove additional sequences.
+The user can apply other filters to remove additional sequences.
 
-An additional way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
+Another way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
 
 ```sh
 # Uncompress genome
 gunzip reference.fa.gz
 # Run samtools faidx
 samtools faidx reference.fa
 # Re-compress the genome
@@ -664,14 +680,15 @@
 ```
 
 ## Output directories
 
 The outputs of a default `radinitio --simulate-all` run are:
 
 ```sh
+$ ls *
 output_directory:
 popmap.tsv  radinitio.log  sequenced_clone_distrib.tsv
 
 output_directory/msprime_vcfs:
 chr1.vcf.gz   chr7.vcf.gz  chr13.vcf.gz  chr19.vcf.gz
 chr2.vcf.gz   chr8.vcf.gz  chr14.vcf.gz  chr20.vcf.gz
 chr3.vcf.gz   chr9.vcf.gz  chr15.vcf.gz  chr21.vcf.gz
@@ -711,31 +728,33 @@
 output_directory/ref_loci_vars:
 reference_rad_loci_SbfI.fa.gz     ri_master.vcf.gz
 reference_rad_loci_SbfI.stats.gz
 ```
 
 ### Top level directory
 
+The main (or top level) output directory of a `radinitio` simulation run. Contains three text files, in addition to several subdirectories described below.
+
 #### Population Map
 
-A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs on the first column, and population IDs on the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
+A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs in the first column, and population IDs in the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
 
 ```sh
 msp_00<tab>pop0
 msp_01     pop0
 msp_02     pop0
 msp_03     pop1
 msp_04     pop1
 msp_05     pop1
 ...
 ```
 
 #### PCR clones distribution
 
-The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution generated during the most recent run. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
+The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
 
 ```sh
 clone_size  n_errors  clone_prob
 0           0         0
 1           0         1.0
 1           1         0
 ```
@@ -757,27 +776,27 @@
 ...
 ```
 
 Here, the `clone_size` describes the number of molecules in a clone. A clone size of *n* means that *n* molecules where sampled from a single clone. *n* copies of the same sequence will be saved as reads, with *n - 1* being PCR duplicates. Moreover, clones can also contain molecules with PCR error (`n_errors`). A clone of size *n* can contain up to *n* molecules with error. `clone_prob` is the probability of sampling a clone with given size and error properties, and describes the distribution of PCR duplicates and errors in the simulated data.
 
 #### Log file
 
-The `radinitio.log` file is generated on the top level outoput directory. It contains information on the **RADinitio** version, a time stamp on the current run, as well as information on the different stages of the program.
+The `radinitio.log` file is generated in the top level output directory. It contains information about the **RADinitio** version, a time stamp of the current run, as well as information on the different stages of the program.
 
 ### Msprime VCFs
 
 The `msprime_vcfs/` directory containing the genetic variants simulated by **msprime** (derived from the [`tskit.TreeSequence.write_vcf()`](https://tskit.dev/tskit/docs/stable/python-api.html#tskit.TreeSequence.write_vcf) function) for each individual chromosome.
 
 ### Reference loci/vars directory
 
 The `ref_loci_vars` contains the reference information for the simulated RAD loci as well as the genome-wide variants generated from the population simulation.
 
 #### Genomic VCF
 
-A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspeficied alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
+A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspecified alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
 
 #### Reference RAD loci
 
 The reference loci file reports the sequence of all the reference loci present in the genome, i.e., the genomic sequence corresponding to the 1 Kbp spanning the extracted loci. These sequenced are exported as a gzipped fasta file (`reference_rad_loci.fa.gz`).
 
 ```sh
 >t0000n ref_pos=chr1:10818-11817
@@ -788,19 +807,19 @@
 TGCAGGGAGGGTGGGAGAACTTTCTCCGTTAACAAAAAATGAGGCTCCGTCTCTGTGATTC...
 >t0003n ref_pos=chr3:23979-24978
 TGCAGGTCAGTGAACTCACCCCCACTGCAGGCGTCCTCTGGACTGAACCAACAGAAGCTGG...
 >t0004n ref_pos=chr3:24974-25973
 TGCAGGCGATCCAGTCCACAGACCGGCTACCTGGATCATGCCGACGTCCGACAGTGTCTCC...
 ```
 
-The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsute on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
+The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsite on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
 
 #### Locus Status
 
-The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
+The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -821,42 +840,42 @@
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
 ### RAD alleles
 
-The `rad_alleles/` directoru contains per-individual gzipped fasta files contining the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
+The `rad_alleles/` directory contains per-individual gzipped fasta files containing the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
 
 ```sh
 >reference_locus_id:sample_id:allele_i
 ```
 
-Here, `reference_locus_id` referes to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
+Here, `reference_locus_id` refers to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
 
 ```sh
 >t0n:msp_0:a1
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t0n:msp_0:a2
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t1p:msp_0:a1
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCAGAAACATATTAAAGTTG...
 >t1p:msp_0:a2
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCACAAACATATTAAAGTTG...
 ```
 
 ### RAD reads
 
-The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files contining the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
+The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files containing the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
 
 ```sh
 reference_locus_id:sample_id:allele_i:clone_id:duplicate_i/read_pair
 ```
 
-The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` referes to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
+The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` refers to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
 
 Notice in the fasta example below that for reads 3 and 4, they both have a `clone_id` of 3. Read 3 has a `clone_i` of 1, meaning is the first read in the clone. Read 4 has a `clone_id` of 2, meaning it is the second read in the clone and thus a duplicate product of PCR.
 
 ```sh
 >t5n:msp_0:a2:1:1/1
 TGCAGGCTTAGGCTACACCCAACGAGCCACTGGGTGCAGTTGGACCCGAGGGATCTGTAT...
 >t4n:msp_0:a1:2:1/1
@@ -865,22 +884,27 @@
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t2n:msp_0:a2:3:2/1
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t5p:msp_0:a1:4:1/1
 TGCAGGGCTTCCACTCCATACTTGTAAAATTAGGGGAAAACACTTTTTTTAACCTCCCAG...
 ```
 
-The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the indentity of PCR clones.
+The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the identity of PCR clones.
 
 ## Questions?
 
 If you have any questions or are encountering any problems when running **RADinitio**, please drop your questions in the [Stacks-users mailing list](https://groups.google.com/g/stacks-users).
 
 ## Changelog
 
+### RADinitio `1.2.1` - 2023 Jun 26
+
+* Bug Fix: Updated error in `setup.py` python version requirements.
+* Others: Fixed typos and other small errors in the docs.
+
 ### RADinitio `1.2.0` - 2023 Jun 23
 
 * Feature: Updated to `decoratio` PCR amplification models
 * Feature: Updated reporting of RAD loci tally
 * Feature: Several advanced options available in `radinitio` wrapper
 * Bug Fix: Program now prints warning and stops when no sequences are loaded from genome.
 * Other: General re-working and refactoring of main functions.
@@ -900,15 +924,15 @@
 * Other: Changed default value for template/read ratio in PCR model
 * Other: Added `--version` flag in main wrapper. Also reported in other intermediary files.
 * Other: General formatting updates to logs.
 
 ### RADinitio `1.0.3` - 2019 May 16
 
 * Fixed bug when reporting number of loci in log
-* Changed the requierements of the output directory - it now MUST exist
+* Changed the requirements of the output directory - it now MUST exist
 
 ### RADinitio `1.0.2` - 2019 May 13
 
 * Updated contents of package distribution build.
 
 ### RADinitio `1.0.1` - 2019 May 13
```

### Comparing `radinitio-1.2.0/radinitio/__init__.py` & `radinitio-1.2.1/radinitio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     if chrom_selection is None or name in chrom_selection:
         chrom_sequence = ''.join(seq)
         if len(chrom_sequence) >= min_seq_len:
             genome_dict[name] = Chromosome(name, chrom_sequence)
     # Report sequences loaded
     n_chrs = len(genome_dict)
     print(f'    Read {seqs_read:,} sequences from the input FASTA.', flush=True)
-    print(f'    Loaded {n_chrs:,} chromsome/scaffold sequences.', flush=True)
+    print(f'    Loaded {n_chrs:,} chromosome/scaffold sequences.', flush=True)
     # Check for invalid characters in the genome
     check_invalid_chars_in_genome(genome_dict)
     # Return genome dictionary
     return genome_dict
 
 # Function to go over chromosome dictionary and tally characters
 # Will return error if they are non 'ACGTN' characters present
@@ -2009,20 +2009,20 @@
         # Second value is number of mutated molecules in clone
         clone_error = self.seq_clone_errors_vals[seq_clone_index][1]
         return clone_size, clone_error
     # Print class properties
     def __str__(self):
         if self.ampl_model is None:
             return f'''PCR model options:
-    PCR amplication model:   {self.ampl_model} (No PCR)
+    PCR amplification model: {self.ampl_model} (No PCR)
     PCR cycles:              {self.pcr_cyc}
     PCR duplicate rate:      {self.perc_duplicates:.2%}'''
         else:
             return f'''PCR model options:
-    PCR amplication model:   {self.ampl_model}
+    PCR amplification model: {self.ampl_model}
     PCR cycles:              {self.pcr_cyc}
     depth/complexity ratio:  {(self.ratio):0.6g}
     PCR duplicates rate:     {self.perc_duplicates:.3%}'''
 
 #
 # Extract reads from a sample
 def sequence_sample(sample_n, out_dir, alleles_list, library_opts=LibraryOptions(), mutation_opts=MutationModel(), pcr_opts=PCRDups(), def_score=37, phred_offet=33):
```

### Comparing `radinitio-1.2.0/radinitio/__main__.py` & `radinitio-1.2.1/radinitio/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 radinitio --genome path --out-dir dir [pipeline-stage] [--chromosomes path] \
     [(demographic model options)] [(library options)] [(pcr options)] [(advanced options)]
 
 Pipeline stages (these options are mutually exclusive):
     --simulate-all        Run all the RADinitio stages (simulate a population, make a library,
                           and sequence) (Default)
     --make-population     Simulate and process variants. Produces genome-wide VCF.
-    --make-library-seq    Simulate and sequence a RAD library. Requires exising variants.
+    --make-library-seq    Simulate and sequence a RAD library. Requires existing variants.
     --tally-rad-loci      Calculate the number of kept rad loci in the genome.
 
 Input/Output files:
     -g, --genome:         Path to reference genome (fasta file, may be gzipped).  (Required)
     -o, --out-dir:        Path to an output directory where all files will be written.
                           (Required)
```

### Comparing `radinitio-1.2.0/radinitio.egg-info/PKG-INFO` & `radinitio-1.2.1/radinitio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: radinitio
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for the simulation of RADseq data.
 Home-page: http://catchenlab.life.illinois.edu/radinitio
 Author: Angel G. Rivera-Colon <arcolon14@gmail.com>, Nicolas Rochette <rochette@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>
-Author-email: angelgr2@illinois.edu
+Author-email: arcolon14@gmail.com
 Project-URL: Manual, http://catchenlab.life.illinois.edu/radinitio/manual/
 Project-URL: Source, https://bitbucket.org/angelgr2/radinitio/src/default/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >3.7
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RADinitio
 
-![RADinitio logo](image.png)
-
 **RADinitio** is a pipeline for the assessment of RADseq experiments via prospective and retrospective data simulation. Sequencing data is generated *de novo* from a population of individuals via a coalescent simulation under a user-defined demographic model using **msprime**. The genetic variants in each sample are simulated in a genomic context that can impact downstream generation of RAD loci and sequencing reads. The per-individual sequences are then treated to an *in silico* RADseq library preparation. The components of the library are defined by the user, allowing for the exploration of parameters including restriction enzyme selection, insert size, sequencing coverage, and PCR duplicate distribution (generated using the **decoratio** software). **RADinitio** simulations can also be applied retrospectively by comparing and modelling sources of error in empirical datasets. The purpose of **RADinitio** is for researchers to fully explore possible variables in their data generation process to ensure that their protocol selection and library preparation is performed optimally, within the limitations of technical and experimental error.
 
 ## Citation
 
 If you use **RADinitio** in your work, please cite the [2021 *Mol Ecol Resour*](https://doi.org/10.1111/1755-0998.13163) manuscript:
 
 > Rivera-Colón, AG, Rochette, NC, Catchen, JM. (2021) Simulation with RADinitio improves RADseq experimental design and sheds light on sources of missing data. *Mol Ecol Resour* 21: 363– 378. <https://doi.org/10.1111/1755-0998.13163>
@@ -108,15 +106,15 @@
 
 #### Pipeline stages (these options are mutually exclusive)
 
 `--simulate-all` : Run all the **RADinitio** stages (simulate a population, make a library, and sequence the library) (Default)
 
 `--make-population` : Simulate and process variants. Produces genome-wide VCF.
 
-`--make-library-seq` : Simulate and sequence a RAD library. Requires exising `radinitio.make-population` run.
+`--make-library-seq` : Simulate and sequence a RAD library. Requires existing `radinitio.make-population` run.
 
 `--tally-rad-loci` : Calculate the number of kept RAD loci in the genome.
 
 #### Required input/output
 
 `-g`, `--genome` : (*str*) Path to reference genome (fasta file, may be gzipped). **Required**
 
@@ -188,15 +186,15 @@
 
 `--genome-rec-rate` : (*float*) MsprimeOptions: Average per-base per-generation recombination rate for the whole genome. (default = 3e-8)
 
 `--genome-mut-rate` : (*float*) MsprimeOptions: Average per-base per-generation mutation rate for the whole genome. (default = 7e-8)
 
 `--pop-mig-rate` : (*float*) MsprimeOptions: Total per-population per-generation immigration rate. (default = 0.001)
 
-`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (deault = 0.0)
+`--pop-growth-rate` : (*float*) MsprimeOptions: Population per-generation growth rate. (default = 0.0)
 
 `--lib-bar1-len` : (*int*) LibraryOptions: Length of the forward-read barcode in bp. (default = 5)
 
 `--lib-bar2-len` : (*int*) LibraryOptions: Length of the reverse-read barcode in bp. (default = 0)
 
 `--lib-5-error` : (*float*) LibraryOptions: Frequency of sequencing errors at the 5' end of the reads. (default = 0.001)
 
@@ -216,36 +214,36 @@
 
 `--pcr-pol-error` : (*float*) PCRDups: Probability of PCR errors, based on the error rate of the Phusion HF polymerase. (default = 4.4e-7)
 
 ## Examples
 
 ### Getting started
 
-The simplest **RADinitio** simulation requres just the specification of a reference genome fasta (`--genomne`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
+The simplest **RADinitio** simulation requires just the specification of a reference genome fasta (`--genome`) and an output directory (`--out-dir`). The reference sequence (`reference.fa.gz` in this example) is a fasta file containing the genomic sequences of one or more chromosomes/scaffolds. The reference sequences can be at a chromosome-level, or broken into smaller scaffold sequences. The file can be compressed (gzipped) or uncompressed.
 
 Using the default parameters runs the whole simulation pipeline and generates all possible outputs (`--simulate-all`). This will simulate a standard island model for 2 populations, sequencing 10 individuals per population (20 total). The single-digest library will be made with the enzyme *SbfI*, using the default insert size distribution (mean 350 bp and stdev 35bp) and generating 2x150bp reads at 20x coverage.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/         # Path to output directory
 ```
 
 ### Controlling the input reference sequences
 
-The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The first example is using a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
+The `radinitio` command line options allow the user to control which sequences in the reference genome are used for the simulations, without the need to modify the input fasta file. The next example uses a chromosome list file (specified with `--chromosomes`). This file contains a list with the sequence IDs that the user wants to use for the simulation, one per line. The IDs in this file must be as they appear on the `reference.fa` (**NOTE**: without the "`>`", as this is part of the fasta header!). The file follows the following structure:
 
 ```sh
 chr1
 chr2
 chr3
 ...
 ```
 
-Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
+Only the sequences on the list will be used as input for the simulations. This is important when working with highly fragmented assemblies or those with many small unplaced scaffolds, allowing the user to simulate only over the chromosome-scale sequences, for example. If this option is not provided, **RADinitio** will simulate over all the sequences in the input fasta.
 
 Here we run the same default **RADinitio** simulation as before, but instead we provide a `chrom_list.txt` file containing the IDs of the target sequences of interest.
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline (--simulate-all default)
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simple-simulation/ \       # Path to output directory
@@ -262,20 +260,20 @@
 ```
 
 The `radinitio.log` file reports the number of sequences read from the reference genome fasta file, as well as those kept after selection/filtering. For example, here the reference genome contained 1,844 total sequences; however, we only selected 24 (e.g., 24 chromosomes) for downstream analysis.
 
 ```sh
 Loading the genome...
     Read 1,844 sequences from the input FASTA.
-    Loaded 24 chromsome/scaffold sequences.
+    Loaded 24 chromosome/scaffold sequences.
 ```
 
 ### Modifying the library parameters
 
-**RADinitio** allows the user to specify the paramters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
+**RADinitio** allows the user to specify the parameters of their simulated RADseq library. By default, as done in the previous examples, the software simulates a single-digest RADseq (sdRAD) library, following the protocols published by [Baird et al. (2008)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0003376) and [Etter et al. (2011)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018561). This library uses the *SbfI* restriction enzyme to generate a library with an insert size distribution of an mean length of 350bp (standard deviation 37bp), coverage of 20x, read length of 150bp (2x150bp paired-end), and no PCR amplification. The default simulation is equivalent to:
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -297,44 +295,44 @@
     --enz2 MspI \                          # Use the MspI enzyme as the secondary (common) cutter
     --min-insert 225 \                     # Min insert size of 225 bp
     --max-insert 475 \                     # Max insert size of 475 bp
     --coverage 30 \                        # Depth of coverage of 30x
     --read-length 100                      # Read length of 100bp (paired-end 2x100bp)
 ```
 
-More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these optionns can be left default for the large majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
+More advanced parameters for the library preparation options are available in the command line options (e.g., `--lib-bar1-len` to specify the length of barcode sequences removed from the reads, or `--lib-5-error`/`--lib-3-error` to control sequencing errors). However, these options can be left default for the vast majority of simulations. Advanced users can additionally control these options in the `radinitio.LibraryOptions()` class in the Python API.
 
 ### PCR duplicates model
 
-**RADinitio** can be used to simulate an study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
+**RADinitio** can be used to simulate and study PCR duplicates, a common artifact in empirical RADseq libraries, which have wide-spread implications for allelic dropout and genotyping accuracy. For further details on the effects of PCR duplicates in RADseq libraries, see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800), [Rivera-Colón et al. (2021)](https://doi.org/10.1111/1755-0998.13163), and [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7#DOI).
 
-The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define a the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
+The **RADinitio** pipeline can simulate a PCR model, which generates a distribution of PCR clone sizes and errors, which are then used when sampling sequencing reads. This model introduces both PCR duplicate reads and mutations in the sequencing reads, mimicking the error patterns seen in real-life RADseq libraries. The generation of this PCR model is off by default; however, the user can define the parameters of an amplification model from the `radinitio` wrapper command line options, or with the `radinitio.PCRDups()` class in the Python API.
 
 When no `--pcr-model` is selection, the `radinitio.log` reports the following information:
 
 ```sh
 PCR model options:
-    PCR amplication model:   None (No PCR)
+    PCR amplification model:   None (No PCR)
     PCR cycles:              None
     PCR duplicate rate:      0.00%
 ```
 
-We see that no PCR model was selected (defaults to `None`). Thus. there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
+We see that no PCR model was selected (defaults to `None`). Thus, there were no PCR cycles applied, and the PCR duplicate rate is 0% (i.e., each individual sequencing reads was sampled from an unique template).
 
 In contrast, the user can choose and apply a PCR model to the downstream data. Since version `1.2.0`, **RADinitio** uses the PCR models described by the **decoratio** software ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)). These PCR models are largely comprised of two steps: 1) an amplification model (which describes the amplification probability and noise applied over some number of PCR cycles) and 2) a depth/complexity ratio which describes how the sequenced reads are sampled from the pool of amplified molecules.
 
-The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distrubition for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
+The different PCR models can be specified in `radinitio` using the `--pcr-model` flag. Two main types of models are available, each with two main variants (4 models total). First, the inherited efficiency models described in [Best. et al. (2015)](https://doi.org/10.1038/srep14629). When choosing `--pcr-model inheff` the user controls the amplification probability and noise by controlling the mean (`--pcr-inheff-mean`) and standard deviation (`--pcr-inheff-sd`) of a normal distribution defining the amplification probability of the virtual molecules across a number of PCR amplification cycles (`--pcr-cycles`). A related model, `inheffbeta`, uses a beta distribution for parametrization purposes instead of the normal distribution, and produces similar results. By default, `radinitio` uses 0.7 and 0.1 for the mean and standard deviation of these distributions, respectively.
 
-The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model used the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
+The second class of amplification models defined the amplification probability based on a log-normal distribution. Both models (`lognormal` and `logskewnormal`) use the standard deviation of the distribution (specified with `--pcr-lognormal-sd`) as the main parameter controlling amplification probability and noise. The `logskewnormal` model uses the skew of the distribution (`--pcr-lognormal-skew`) as an additional parameter. For more information of these models and their specification please check the **decoratio** manuscript ([Rochette et al. 2023](https://doi.org/10.1111/1755-0998.13800)) and documentation (<https://bitbucket.org/rochette/decoratio/src/master/>).
 
 In addition to the amplification model, the other (and more important parameter) controlling the PCR duplicate distribution is the **de**pth/**co**mplexity **ratio**. This value describes the ratio of sequenced molecules (the depth of coverage) to the molecular complexity (the number of unique molecules). In other words, if sequencing at 30x, but the complexity is 10 molecules, the library has a depth/complexity ratio of 3:1. This means that, while it is possible to sequence 30 reads, only 10 of them can have unique information and the remaining 20 reads will be duplicates.`radinitio` users can specify this ratio using the `--pcr-deco-ratio` option. Smaller values (<1) will generally reduce the rate of PCR duplicates seen in the simulated library. See [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800) for further information regarding the depth/complexity ratio.
 
 #### Simulating libraries with low/moderate PCR duplicate rate
 
-Using the models and paramters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library contruction paramters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inhertited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% change of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficienty model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
+Using the models and parameters described above, `radinitio` users can simulate a RADseq library containing a low-to-moderate number of PCR duplicates. We are using the default library construction parameters (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean and 37bp insert stdev). Additionally, we are applying an inherited efficiency amplification model (`--pcr-model inheff`). The mean amplification probability is 45% (`--pcr-inheff-mean 0.45`) with a standard deviation of 20% (`--pcr-inheff-sd 0.2`) for 12 cycles of PCR (`--pcr-cycles 12`). This means that a DNA molecule would have a 45% chance of being amplified in each of the 12 PCR cycles. This distribution produces both lower and noisier amplification probabilities than the default inherited efficiency model (mean of 0.7 and stdev of 0.1). Finally, we are also setting the depth/complexity ratio to 1:10 (`--pcr-deco-ratio 0.10`).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -349,27 +347,27 @@
     --pcr-deco-ratio 0.10                  # De/Co ratio of 1:10 or 0.1
 ```
 
 After running this simulation, we can see the description of the PCR model on the `radinitio.log` file:
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.45:0.2
+    PCR amplification model: inheff:12:0.45:0.2
     PCR cycles:              12
     depth/complexity ratio:  0.1
     PCR duplicates rate:     17.432%
 ```
 
 This PCR model generated a PCR duplicate rate of 17.4%. We can see a per-clone size breakdown of the frequency of these duplicates (i.e., the proportion of clones with a given number of duplicates) in the `sequenced_clone_distrib.tsv` file. Additionally, the log reports the parameters of the model, including the number of cycles, depth/complexity ratio, and the "model string". This "model string" (`inheff:12:0.45:0.2` in this example) is the definition of the model, as specified by **decoratio**. In this example, the string describes (in order, separated by ":"): 1) the selected model (`inheff`), number of PCR cycles (`12`), mean amplification probability (`0.45`), and the amplification probability standard deviation (`0.2`). Different models used by **RADinitio** have different specifications and model string. See the **decoratio** documentation for additional details on model specifications.
 
-#### Simulating libraries with high PCR duplicate rate
+#### Simulating libraries with high PCR duplicate rates
 
-**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may provide useful to, e.g., observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information.
+**RADinitio** users can also change the PCR amplification models to simulated RADseq libraries with elevated duplicate rates. While this is something researchers want to avoid in their empirical libraries, experimenting with high PCR duplicates in simulations may be useful (e.g., to observe how the added noise affects the recovery and genotyping of loci and the reconstruction of biological information).
 
-In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR paramters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
+In this example, we repeat the general library construction process from above (single-digest with *SbfI*, 20x coverage, 2x150bp reads, 350bp insert mean); however, we modify the PCR parameters to 1) increase the noise of the inherited efficiency amplification model , and 2) drastically increase the depth/complexity ratio (from 0.1 to 10).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./simulations_sdRAD/ \       # Path to output directory
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI \                           # Use the SbfI enzyme
@@ -384,49 +382,49 @@
     --pcr-deco-ratio 10                    # De/Co ratio of 10:1 or 10
 ```
 
 After completing the simulation, we evaluate the results provided in the `radinitio.log` file.
 
 ```sh
 PCR model options:
-    PCR amplication model:   inheff:12:0.25:0.5
+    PCR amplification model: inheff:12:0.25:0.5
     PCR cycles:              12
     depth/complexity ratio:  10
     PCR duplicates rate:     94.019%
 ```
 
-We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all their individual contribution to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplificaton. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
+We obtain 94% PCR duplicates! Notice how we didn't change the number of PCR cycles, after all, the individual contribution of the number of cycles to PCR duplicate is negligible (see [Rochette et al. (2023)](https://doi.org/10.1111/1755-0998.13800)). This increase in PCR duplicates is mainly the product of the depth/complexity ratio, as we are sequencing 10x more reads than there are available molecules in the library. This is further exacerbated by the increased noisiness in the PCR amplification. While this is an extreme case, it provides an example of the behavior of the PCR models in **RADinitio** and provides useful guidelines for the monitoring of empirical RADseq experiments when elevated PCR duplicate rates are observed.
 
-WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. In one example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
+WARNING: Very noisy PCR amplification models can take a long time to run. Similarly, models with *very* extreme values can also fail due to several reasons. For example, if amplified clones reach very large sizes, they can trigger infinity-related errors when extracting the amplified clone size distribution.
 
 ### Changing the demographic model
 
 The `radinitio` wrapper script simulates a population using an island model from **msprime** ([Kelleher et al. 2016](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004842/); [Baumdicker et al. 2022](https://doi.org/10.1093/genetics/iyab229)). By default, this model simulates two populations, each with an effective population size (Ne) of 5,000 individuals. Ten individuals are sampled and sequenced per population, for a total of 20 individuals in the library.
 
 The wrapper script allow the user to modify some parameters of this model. For example, the user can change the number of populations (`--n-pops`), the effective size of the populations (`--pop-eff-size`), and the number of sampled individuals per population (`--n-seq-indv`). Other parameters, e.g., controlling the migration rate (`--pop-mig-rate`), growth rate (`--pop-growth-rate`), and mutation rate (`--genome-mut-rate`), are available in the advanced options.
 
-As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 indididuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
+As an example, we can run a new simulation (running the whole pipeline with `--simulate-all`) simulating a new island model with 4 populations, each with an effective population size (Ne) of 2,500 individuals. We sampled 25 individuals per population, for a total of 100 sequenced individuals. We will also increase the total per-population, per-generation immigration rate between these populations to 2.5%. The library is generated with default parameters (e.g., single-digest with *SbfI*, coverage of 20x, read length of 150bp, insert distribution of 350bp, stdev 35bp, no PCR).
 
 ```sh
 radinitio --simulate-all \                 # Execute the complete pipeline
     --genome ./genome/reference.fa.gz \    # Path to reference genome
     --out-dir ./sims_sdRAD_4pops/ \        # Path to output directory
     --n-pops 4 \                           # Number of populations in the island model
-    --pop-eff-size 2500 \                  # Effecitve size (Ne) of the populations
+    --pop-eff-size 2500 \                  # Effective size (Ne) of the populations
     --n-seq-indv 25 \                      # Number of individuals to sequence per-population (100 total)
     --pop-mig-rate 0.025                   # Per generation immigration rate
     --library-type sdRAD \                 # Simulate a single-digest library
     --enz SbfI                             # Use the SbfI enzyme
 ```
 
 The options in the wrapper are useful for more general simulations, e.g., studying the effects of genetic diversity over the final RADseq library. However, they are limited to a relatively simple island model and the parameters are applied equaly to all populations (i.e., all populations will be of the same size and migration rates will be symmetrical). More detailed demographic models are available through the [**msprime** documentation](https://tskit.dev/msprime/docs/latest/intro.html). **RADinitio** users can implement these complex simulations using the **msprime** Python API, after which they can generate *in silico* RADseq libraries from the simulated populations (see section on `--make-library-seq` below).
 
 ### Tallying RAD loci in the genome
 
-Perhaps the common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
+The most common application of **RADinitio** is simulating an *in silico* digestion to estimate the number of RADseq loci in an experiment. This estimation is commonly used to estimate sequencing coverage and individuals in a library during experimental design (see section 2.3 in [Rivera-Colón & Catchen (2022)](https://doi.org/10.1007/978-1-0716-2313-8_7) for an example).
 
 An estimation of the number of RADseq loci in a genome can be easily generated using the `--tally-rad-loci` option in the `radinitio` wrapper script. This option only identifies and filters the RADseq loci found in the genome based on the library properties, skipping the simulation of the population(s) and the generation of sequencing reads.
 
 For example, here we tally the number of RADseq loci in the genome using the default library parameters (single-digest library with *SbfI*).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
@@ -445,21 +443,21 @@
     Removed 2 loci (0.0%) containing excess (>10.0%) of Ns in sequence.
     Removed 428 loci (7.0%) in close proximity (<1000bp) to another locus.
     Retained 5,687 loci (92.9%) for downstream analysis.
 
     See `./output/tally-rad-loci/ri_sdRAD_sbfI/ref_loci_vars/reference_rad_loci.stats.gz` for a detailed description of the per-cutsite position and status.
 ```
 
-In this example, **RADinitio** foind 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`), each yielding two loci in the negative and positive DNA strands. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6 thousand loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
+In this example, **RADinitio** found 6,120 *SbfI* loci in the genome. Since this is a single-digest library, this means 3,060 instances of the *SbfI* recognition sequence (`CC|TGCAGG`) were found in the genome. Each cutsite yields two loci: one in the negative and one in the positive DNA strand. The two loci originating from a single restriction enzyme cutsite are treated as separate objects and are independently filtered. As stated by the log, these 6k loci can be used to estimate sequencing coverage and number of pooled individuals in the real library.
 
-However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. By default, this distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions of uncertain sequences.
+However, not all loci are retained for downstream analysis. **RADinitio** filters certain loci based on the properties of the sequence. For example, here 3 loci are removed from the analysis as they are too close to the end of the sequence. This distance is equal to the base size of each reference locus. By default, this distance is 1Kbp, and can be controlled with the `--lib-base-len` advanced option. These loci are removed since it would not be possible to extract a complete sequence from the reference. Also, loci can be removed if their reference sequence contains an excess of uncalled bases (or `N`s), by default 10% (controlled with the `--lib-max-prop-n` advanced option). These loci are removed to prevent extracting loci spanning large gaps or regions with uncertain sequences.
 
-More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping from one another on a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
+More commonly, loci are removed due to their proximity to one another, as happened for 428 (or 7% of loci here). A locus is removed when it is under 1,000 bp (by default, controlled by `--lib-min-dist`) away from a another locus originating from a different restriction enzyme cutsite. This filtering process serves two purposes: first, it mimics the real-life process of shearing efficiency during library preparation, where shearing efficiency decreases for smaller DNA molecules, reducing the chance of recovering a molecule of the right size. Secondly, it removes loci originating from tandemly duplicated and/or repetitive cutsites. Many of these loci would be overlapping with one another in a real RADseq library, and their enzymatic digestion and shearing would be impacted by their close proximity.
 
-Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`).
+Lastly, the `reference_rad_loci.stats.gz` file (full path provided in the `radinitio.log`) provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -478,15 +476,15 @@
 chr6       14834    neg      rm_excess_Ns
 chr6       14834    pos      rm_excess_Ns
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
-We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (whoch was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
+We can alter the properties of the simulated library to look at how the number of estimated loci changes. In this example, we will simulate a new single-digest library changing the restriction enzyme from the default *SbfI* (which was an 8-bp recognition sequence) to *EcoRI* (which has the 6-bp recognition sequence `G|AATTC`).
 
 ```sh
 radinitio --tally-rad-loci \              # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \   # Path to reference genome
     --out-dir ./tally_ecoRI_loci/ \       # Path to output directory
     --library-type sdRAD \                # Simulate a single-digest library
     --enz EcoRI                           # Use the EcoRI enzyme
@@ -499,19 +497,19 @@
     Found a total of 25,836 EcoRI loci in the genome (use this number for coverage calculations).
     Removed 14 loci (0.0%) too close to the ends of the reference sequences.
     Removed 26 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 4,648 loci (18.0%) in close proximity (<1000bp) to another locus.
     Retained 21,148 loci (81.8%) for downstream analysis.
 ```
 
-As expected given its smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impact their filtering, as a higher proportion of loci are removed due to close proximity.
+As expected, given the smaller restriction enzyme recognition sequence, we find far more *EcoRI* loci in the genome--25.8 thousand compared to the 6 thousand found with *SbfI*. When preparing an empirical library, the user would have to take into account how this order of magnitude difference in the number of loci would impact sequencing coverage and the number of samples in a library. Most importantly, we see how the increase in the number of loci impacts their filtering, as a higher proportion of loci are removed due to close proximity.
 
 #### Tallying loci in ddRAD libraries
 
-The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. In ddRAD libraries, the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
+The identification of loci in single-digest loci in RADseq libraries depends only on the distribution of the restriction enzyme recognition sequence in the genome. However, in ddRAD libraries the retained loci are impacted by the enzyme combination in addition to the insert size range (see Figure 4 in [Rivera-Colón et al. 2021](https://doi.org/10.1111/1755-0998.13163)). **RADinitio** allows users to simulate both the enzyme selection and insert size range when tallying loci from ddRAD libraries.
 
 Here, we tally the number of loci in a ddRAD library generated using the *EcoRI* enzyme as the main cutter and *MseI* as the secondary (common) cutter. We are using the default insert size distribution (mean of 350bp and stdev of 37bp). This distribution corresponds to a mimumum insert size of 276bp and a max insert size of 424bp (i.e., can also be specified with the `--min-insert`/`--max-insert` options).
 
 ```sh
 radinitio --tally-rad-loci \             # Execute just the tallying of loci
     --genome ./genome/reference.fa.gz \  # Path to the reference genome
     --out-dir ./count_ddrad_loci/ \      # Path to output directory
@@ -557,15 +555,17 @@
     Note: an additional 5,149 loci were found outside the target insert size range.
     Removed 4 loci (0.0%) too close to the ends of the reference sequences.
     Removed 11 loci (0.1%) containing excess (>10.0%) of Ns in sequence.
     Removed 3,667 loci (17.9%) in close proximity (<1000bp) to another locus.
     Retained 16,783 loci (82.0%) for downstream analysis.
 ```
 
-The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci. Note, however, that many of these loci might not be recoverage experimentally, e.g., too small to be feasibly sequenceable (i.e., if they are smaller than the desired read length) or larger than the capicity of the PCR and/or sequencer. Thus, the objective should not be to recover all the available loci in the genome.
+The number of found loci increased from 16 thousand to over 20 thousand. The 100bp-increase in the insert size range lead to about 4 thousand more loci being included in the library. We see that over 5 thousand more loci are still found outside the size range, and thus this parameter could be further optimized to recover more loci.
+
+Note, however, that many of these loci might not be recoverable experimentally, e.g., too small to be feasibly sequenceable (if they are smaller than the desired read length) or larger than the capacity of the PCR and/or sequencer. Thus, the objective is not to recover all the available loci in the genome.
 
 ### Simulating a population and generating genomic variants
 
 The `--make-population` option from the `radinitio` wrapper allows the user to run the initial stage of the **RADinitio** pipeline, simulating a population using the **msprime** island model and generating a genome-wide VCF with the simulated genetic variants. This mode is library agnostic, and does not extract RADseq loci nor generates sequencing reads. The purpose of this mode is to generate a fixed set of genetic variants that can then be processed under a variety of library configurations (see `--make-library-seq` example below).
 
 In this example, we will run **RADinitio** under the `--make-population` mode. We will simulate an island model of 6 populations or demes, each with an effective population size of 10,000. We will sequence 25 individuals per population, or 150 individuals in total. Additionally, we will filter the input genome to only keep sequences larger than 1 Mbp.
 
@@ -583,19 +583,19 @@
 
 1. An `msprime_vcfs/` directory with the raw simulated variants for each individual sequence
 2. A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ref_loci_vars/ri_master.vcf.gz`)
 3. A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population.
 
 ### Simulate a library from an existing population and variants
 
-Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** run made by the user.
+Using the `--make-library-seq` option from the `radinitio` wrapper, the user can generate an *in silico* RADseq library using an existing population simulation. Most commonly, this existing population will be the product of an `radinitio --make-populations` run; however, `--make-library-seq` can be generated from a custom **msprime** (or other simulators such as **SLiM** or **stdpopsim**) run made by the user.
 
-To run `radinitio` in the `--make-library-seq` pipeline stage, the user most provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and most contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
+To run `radinitio` in the `--make-library-seq` pipeline stage, the user must provide a directory containing an existing population simulation (`--make-pop-sim-dir`). This directory must not be the same output directory for the run, and must contain a genome-wide master VCF as well as a population map, as described above for `--make-population`.
 
-Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Here, we take our previous simulation of 6 populations and 150 individuals and simulate a single-digest RADseq library. The library will have a mean insert size of 450 bp (stdev of 50bp), will be PCR amplified using a default inherited efficiency model for 9 cycles, and sequenced to 30x of coverage. The output of 2x100 bp reads will be exported in fastq format (`--read-out-fmt fastq`). We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./SbfI_library/ \                # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -606,15 +606,15 @@
     --pcr-model inheff \                       # Inherited efficiency amplification model
     --pcr-cycles 9 \                           # Amplify for 9 PCR cycles
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
-Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads. We will additionally simulate over a specific set of chromosomes in the reference sequence.
+Additionally, we will simulate a double-digest library over that same existing population. The ddRAD library will be generated with the *PstI* and *MspI* restriction enzymes, and size selected for a 250-450bp insert size range. The library will be PCR amplified using an inherited efficiency model for 9 cycles, and sequenced to 30x of coverage using 2x100bp reads, in fastq format. We will additionally simulate over a specific set of chromosomes in the reference sequence.
 
 ```sh
 radinitio --make-library-seq \                 # Simulate and sequence a library
     --genome ./genome/reference.fa.gz \        # Path to reference genome
     --chromosomes ./genome/chrom.list \        # Path to the list of the target chromosomes
     --out-dir ./PstI-MspI_library/ \           # Path to the output directory
     --make-pop-sim-dir ./mpop_p6_ne10k_n25/ \  # Path to the previous `make-populations` run
@@ -628,32 +628,32 @@
     --coverage 30 \                            # Sequence to 30x coverage
     --read-length 100 \                        # Read length of 100bp (2x100bp paired-end)
     --read-out-fmt fastq                       # Export reads in FASTQ format
 ```
 
 ### Additional examples
 
-#### How to generate chromosome list
+#### How to generate a chromosome list file
 
-The simplest way to generate a chromosome list file is to extact the sequence IDs form the desired fasta. The sequences must not contain the "`>`" character as this is part of the fasta header convention and are not part of the ID. This can be done by pipping a few commands in Bash:
+The simplest way to generate a chromosome list file is to extract the sequence IDs from the desired fasta. The IDs must not begin with the "`>`" character as this is part of the fasta header convention and not part of the ID. This can be done by piping a few commands in Bash:
 
 1. Open the gzipped file into the stream (`zcat`)
 2. Select the lines starting with `>` (`grep`)
 3. Remove any comments present after whitespace (`cut`)
 4. Remove the `>` (`tr`)
 5. Save to new file
 
 ```sh
 # Create a chrom_list.tsv from all the sequences in the gzipped reference
 zcat reference.fa.gz | grep '^>' | cut -f1 -d ' ' | tr -d '>' > chrom_list.tsv
 ```
 
-The user can apply additional filters to remove additional sequences.
+The user can apply other filters to remove additional sequences.
 
-An additional way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
+Another way of generating a chromosome list file is by parsing the genomic index (`*.fai`) generated by `samtools faidx`. See [**SAMtools** documentation](http://www.htslib.org/doc/samtools-faidx.html) for additional options. From the gzipped fasta...
 
 ```sh
 # Uncompress genome
 gunzip reference.fa.gz
 # Run samtools faidx
 samtools faidx reference.fa
 # Re-compress the genome
@@ -680,14 +680,15 @@
 ```
 
 ## Output directories
 
 The outputs of a default `radinitio --simulate-all` run are:
 
 ```sh
+$ ls *
 output_directory:
 popmap.tsv  radinitio.log  sequenced_clone_distrib.tsv
 
 output_directory/msprime_vcfs:
 chr1.vcf.gz   chr7.vcf.gz  chr13.vcf.gz  chr19.vcf.gz
 chr2.vcf.gz   chr8.vcf.gz  chr14.vcf.gz  chr20.vcf.gz
 chr3.vcf.gz   chr9.vcf.gz  chr15.vcf.gz  chr21.vcf.gz
@@ -727,31 +728,33 @@
 output_directory/ref_loci_vars:
 reference_rad_loci_SbfI.fa.gz     ri_master.vcf.gz
 reference_rad_loci_SbfI.stats.gz
 ```
 
 ### Top level directory
 
+The main (or top level) output directory of a `radinitio` simulation run. Contains three text files, in addition to several subdirectories described below.
+
 #### Population Map
 
-A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs on the first column, and population IDs on the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
+A population map file (`popmap.tsv`) containing the ID of each individual and assignment to a given population. The popmap file is a tab-delimited file, with sample IDs in the first column, and population IDs in the second column. When running the `radinitio` wrapper, the sample IDs are labelled according to the **msprime** simulation have the `msp_` prefix (or `tsk_`, in **msprime** 1.0.0+ versions).
 
 ```sh
 msp_00<tab>pop0
 msp_01     pop0
 msp_02     pop0
 msp_03     pop1
 msp_04     pop1
 msp_05     pop1
 ...
 ```
 
 #### PCR clones distribution
 
-The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution generated during the most recent run. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
+The `sequenced_clone_distrib.tsv` contains information regarding the sequenced clone distribution. This distribution is the product of **decoratio**'s PCR model and is representative of the PCR duplicates observed in the simulated reads, if any. By default, no PCR cycles are enabled, thus the model returns:
 
 ```sh
 clone_size  n_errors  clone_prob
 0           0         0
 1           0         1.0
 1           1         0
 ```
@@ -773,27 +776,27 @@
 ...
 ```
 
 Here, the `clone_size` describes the number of molecules in a clone. A clone size of *n* means that *n* molecules where sampled from a single clone. *n* copies of the same sequence will be saved as reads, with *n - 1* being PCR duplicates. Moreover, clones can also contain molecules with PCR error (`n_errors`). A clone of size *n* can contain up to *n* molecules with error. `clone_prob` is the probability of sampling a clone with given size and error properties, and describes the distribution of PCR duplicates and errors in the simulated data.
 
 #### Log file
 
-The `radinitio.log` file is generated on the top level outoput directory. It contains information on the **RADinitio** version, a time stamp on the current run, as well as information on the different stages of the program.
+The `radinitio.log` file is generated in the top level output directory. It contains information about the **RADinitio** version, a time stamp of the current run, as well as information on the different stages of the program.
 
 ### Msprime VCFs
 
 The `msprime_vcfs/` directory containing the genetic variants simulated by **msprime** (derived from the [`tskit.TreeSequence.write_vcf()`](https://tskit.dev/tskit/docs/stable/python-api.html#tskit.TreeSequence.write_vcf) function) for each individual chromosome.
 
 ### Reference loci/vars directory
 
 The `ref_loci_vars` contains the reference information for the simulated RAD loci as well as the genome-wide variants generated from the population simulation.
 
 #### Genomic VCF
 
-A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspeficied alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
+A genome-wide VCF containing the combined sequences from all simulated chromosomes (`ri_master.vcf.gz`). Here, the variants simulated by **msprime**, which may encode unspecified alleles, are projected against the sequence of the reference genome to determine the identify of the reference alleles. To determine alterative alleles, **RADinitio** implements a `MutationModel()`, which can mutate the reference alleles based on a substitution model (specified with `--mut-subs-model`) and introduce indels at a specified rate (`--mut-indel-prob`).
 
 #### Reference RAD loci
 
 The reference loci file reports the sequence of all the reference loci present in the genome, i.e., the genomic sequence corresponding to the 1 Kbp spanning the extracted loci. These sequenced are exported as a gzipped fasta file (`reference_rad_loci.fa.gz`).
 
 ```sh
 >t0000n ref_pos=chr1:10818-11817
@@ -804,19 +807,19 @@
 TGCAGGGAGGGTGGGAGAACTTTCTCCGTTAACAAAAAATGAGGCTCCGTCTCTGTGATTC...
 >t0003n ref_pos=chr3:23979-24978
 TGCAGGTCAGTGAACTCACCCCCACTGCAGGCGTCCTCTGGACTGAACCAACAGAAGCTGG...
 >t0004n ref_pos=chr3:24974-25973
 TGCAGGCGATCCAGTCCACAGACCGGCTACCTGGATCATGCCGACGTCCGACAGTGTCTCC...
 ```
 
-The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsute on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
+The sequence IDs of each locus are composed of `t` for "true locus", number representing the ordering of the cutsite in the genome (e.g., `0000` for the first cutsite on position 11,811 of chr1), and either `n` or `p` to denote loci in the negative and positive strand, respectively. The fasta header also provides the coordinates of the locus sequence in the reference. Note that locus from the negative strand have been reverser complimented, with the restriction enzyme overhang present at the 5' of the sequence.
 
 #### Locus Status
 
-The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an ajacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
+The `reference_rad_loci.stats.gz` file provides a locus-by-locus description of the status of each loci. The file reports the ID for the sequence in which the locus is located (`#chrom_id`), the basepair coordinate in which the main cutsite was found (`cut_pos`), the direction of the tag (`tag_dir`) in the DNA strand, and the `status` of each locus. An individual locus can be kept for downstream analysis (`kept`) or removed for one of the reasons described above, e.g., too close the end of the sequence (`rm_chrom_end`) or too close to an adjacent locus (`rm_too_close`). When simulating ddRAD libraries, the file will also report loci with additional secondary cutsites outside the insert size range (`rm_no_dd_cuts`).
 
 ```sh
 #chrom_id  cut_pos  tag_dir  status
 chr1       11811    neg      kept
 chr1       11811    pos      kept
 chr2       329      neg      rm_chrom_end
 chr2       329      pos      kept
@@ -837,42 +840,42 @@
 chr6       27346    neg      kept
 chr6       27346    pos      kept
 ...
 ```
 
 ### RAD alleles
 
-The `rad_alleles/` directoru contains per-individual gzipped fasta files contining the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
+The `rad_alleles/` directory contains per-individual gzipped fasta files containing the RAD alleles for each simulated sample. For each allele, the fasta headers contains the following information:
 
 ```sh
 >reference_locus_id:sample_id:allele_i
 ```
 
-Here, `reference_locus_id` referes to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
+Here, `reference_locus_id` refers to the original reference locus the allele was generated. `sample_id` is the **msprime** sample id, and `allele_i` refers to the allele number (`a1` or `a2` in diploid individuals).
 
 ```sh
 >t0n:msp_0:a1
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t0n:msp_0:a2
 TGCAGGCACGCAAGCGGCTCTAGGGATTCCTTGAGAGGAAAAATGCAACGCTGGTTTAACG...
 >t1p:msp_0:a1
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCAGAAACATATTAAAGTTG...
 >t1p:msp_0:a2
 TGCAGGGGCCCCCGCACCACACGTTGGGAACCCCTGATTGACCACAAACATATTAAAGTTG...
 ```
 
 ### RAD reads
 
-The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files contining the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
+The `rad_reads/` contains per-individual gzipped paired-end fasta (or fastq) files containing the RAD reads for each simulated sample. For each individual read, the fasta headers contains the following information:
 
 ```sh
 reference_locus_id:sample_id:allele_i:clone_id:duplicate_i/read_pair
 ```
 
-The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` referes to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
+The basename of the read, which contains `reference_locus_id:sample_id:allele_i`, comes from the source locus of the reads. `clone_id` refers to the source template id, while `duplicate_i` is the duplicate number for each read in the clone. `read_pair` is the standard designation for paired-end reads, `/1` for forward read and `/2` for the corresponding paired read.
 
 Notice in the fasta example below that for reads 3 and 4, they both have a `clone_id` of 3. Read 3 has a `clone_i` of 1, meaning is the first read in the clone. Read 4 has a `clone_id` of 2, meaning it is the second read in the clone and thus a duplicate product of PCR.
 
 ```sh
 >t5n:msp_0:a2:1:1/1
 TGCAGGCTTAGGCTACACCCAACGAGCCACTGGGTGCAGTTGGACCCGAGGGATCTGTAT...
 >t4n:msp_0:a1:2:1/1
@@ -881,22 +884,27 @@
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t2n:msp_0:a2:3:2/1
 TGCAGGAAGAGACGAACCCATCGCCAGTACCACCCCCTGTACATCTGACATCACTCTTAC...
 >t5p:msp_0:a1:4:1/1
 TGCAGGGCTTCCACTCCATACTTGTAAAATTAGGGGAAAACACTTTTTTTAACCTCCCAG...
 ```
 
-The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the indentity of PCR clones.
+The contents of `rad_reads/` contain the main output of RADinitio. These reads behave as empirical paired-end reads and are fully compatible with the majority of bioinformatic software. Reads can be exported in both fasta (default) and fastq formats, as specified by the `--read-out-fmt` option in the `radinitio` wrapper. Both output formats report the sample allele information, as well as the identity of PCR clones.
 
 ## Questions?
 
 If you have any questions or are encountering any problems when running **RADinitio**, please drop your questions in the [Stacks-users mailing list](https://groups.google.com/g/stacks-users).
 
 ## Changelog
 
+### RADinitio `1.2.1` - 2023 Jun 26
+
+* Bug Fix: Updated error in `setup.py` python version requirements.
+* Others: Fixed typos and other small errors in the docs.
+
 ### RADinitio `1.2.0` - 2023 Jun 23
 
 * Feature: Updated to `decoratio` PCR amplification models
 * Feature: Updated reporting of RAD loci tally
 * Feature: Several advanced options available in `radinitio` wrapper
 * Bug Fix: Program now prints warning and stops when no sequences are loaded from genome.
 * Other: General re-working and refactoring of main functions.
@@ -916,15 +924,15 @@
 * Other: Changed default value for template/read ratio in PCR model
 * Other: Added `--version` flag in main wrapper. Also reported in other intermediary files.
 * Other: General formatting updates to logs.
 
 ### RADinitio `1.0.3` - 2019 May 16
 
 * Fixed bug when reporting number of loci in log
-* Changed the requierements of the output directory - it now MUST exist
+* Changed the requirements of the output directory - it now MUST exist
 
 ### RADinitio `1.0.2` - 2019 May 13
 
 * Updated contents of package distribution build.
 
 ### RADinitio `1.0.1` - 2019 May 13
```

### Comparing `radinitio-1.2.0/setup.py` & `radinitio-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="radinitio",
-    version="1.2.0",
+    version="1.2.1",
     author="Angel G. Rivera-Colon <arcolon14@gmail.com>, Nicolas Rochette <rochette@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>",
-    author_email="angelgr2@illinois.edu",
+    author_email="arcolon14@gmail.com",
     description="A package for the simulation of RADseq data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://catchenlab.life.illinois.edu/radinitio",
     packages=setuptools.find_packages(),
     scripts=['scripts/radinitio'],
-    python_requires='>3.7',
+    python_requires='>=3.7.0',
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux",
     ],
     project_urls={
```

