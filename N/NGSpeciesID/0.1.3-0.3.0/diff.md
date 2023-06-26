# Comparing `tmp/NGSpeciesID-0.1.3.tar.gz` & `tmp/NGSpeciesID-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NGSpeciesID-0.1.3.tar", last modified: Tue Dec  7 20:28:18 2021, max compression
+gzip compressed data, was "NGSpeciesID-0.3.0.tar", last modified: Mon Jun 26 09:08:55 2023, max compression
```

## Comparing `NGSpeciesID-0.1.3.tar` & `NGSpeciesID-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 kxs624     (502) staff       (20)        0 2021-12-07 20:28:18.307456 NGSpeciesID-0.1.3/
--rw-r--r--   0 kxs624     (502) staff       (20)       17 2020-02-11 02:26:28.000000 NGSpeciesID-0.1.3/MANIFEST.in
--rwxr-xr-x   0 kxs624     (502) staff       (20)    17096 2021-12-07 20:27:07.000000 NGSpeciesID-0.1.3/NGSpeciesID
-drwxr-xr-x   0 kxs624     (502) staff       (20)        0 2021-12-07 20:28:18.302075 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/
--rw-r--r--   0 kxs624     (502) staff       (20)    15175 2021-12-07 20:28:18.000000 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/PKG-INFO
--rw-r--r--   0 kxs624     (502) staff       (20)      433 2021-12-07 20:28:18.000000 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/SOURCES.txt
--rw-r--r--   0 kxs624     (502) staff       (20)        1 2021-12-07 20:28:18.000000 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/dependency_links.txt
--rw-r--r--   0 kxs624     (502) staff       (20)       29 2021-12-07 20:28:18.000000 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/requires.txt
--rw-r--r--   0 kxs624     (502) staff       (20)        8 2021-12-07 20:28:18.000000 NGSpeciesID-0.1.3/NGSpeciesID.egg-info/top_level.txt
--rw-r--r--   0 kxs624     (502) staff       (20)    15175 2021-12-07 20:28:18.307692 NGSpeciesID-0.1.3/PKG-INFO
--rw-r--r--   0 kxs624     (502) staff       (20)    12056 2021-12-07 20:26:18.000000 NGSpeciesID-0.1.3/README.md
-drwxr-xr-x   0 kxs624     (502) staff       (20)        0 2021-12-07 20:28:18.307156 NGSpeciesID-0.1.3/modules/
--rw-r--r--   0 kxs624     (502) staff       (20)        0 2020-02-11 02:26:28.000000 NGSpeciesID-0.1.3/modules/__init__.py
--rw-r--r--   0 kxs624     (502) staff       (20)     5728 2021-10-13 18:39:53.000000 NGSpeciesID-0.1.3/modules/barcode_trimmer.py
--rw-r--r--   0 kxs624     (502) staff       (20)    19664 2020-02-11 02:26:28.000000 NGSpeciesID-0.1.3/modules/cluster.py
--rw-r--r--   0 kxs624     (502) staff       (20)    13270 2021-12-07 20:26:18.000000 NGSpeciesID-0.1.3/modules/consensus.py
--rw-r--r--   0 kxs624     (502) staff       (20)     8925 2021-10-13 18:39:53.000000 NGSpeciesID-0.1.3/modules/get_sorted_fastq_for_cluster.py
--rw-r--r--   0 kxs624     (502) staff       (20)     2998 2021-10-13 18:39:53.000000 NGSpeciesID-0.1.3/modules/help_functions.py
--rw-r--r--   0 kxs624     (502) staff       (20)  1790771 2020-02-11 02:26:28.000000 NGSpeciesID-0.1.3/modules/p_minimizers_shared.py
--rw-r--r--   0 kxs624     (502) staff       (20)     8956 2020-02-11 02:26:28.000000 NGSpeciesID-0.1.3/modules/parallelize.py
--rw-r--r--   0 kxs624     (502) staff       (20)       67 2021-12-07 20:28:18.308122 NGSpeciesID-0.1.3/setup.cfg
--rw-r--r--   0 kxs624     (502) staff       (20)     3993 2021-12-07 20:27:35.000000 NGSpeciesID-0.1.3/setup.py
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-06-26 09:08:55.958116 NGSpeciesID-0.3.0/
+-rw-r--r--   0 ksahlin    (501) staff       (20)    35146 2020-02-12 12:28:36.000000 NGSpeciesID-0.3.0/LICENSE.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)       17 2020-02-12 13:32:35.000000 NGSpeciesID-0.3.0/MANIFEST.in
+-rwxr-xr-x   0 ksahlin    (501) staff       (20)    17096 2023-06-26 09:07:46.000000 NGSpeciesID-0.3.0/NGSpeciesID
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-06-26 09:08:55.948871 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/
+-rw-r--r--   0 ksahlin    (501) staff       (20)    12737 2023-06-26 09:08:55.000000 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/PKG-INFO
+-rw-r--r--   0 ksahlin    (501) staff       (20)      445 2023-06-26 09:08:55.000000 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/SOURCES.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)        1 2023-06-26 09:08:55.000000 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/dependency_links.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)       29 2023-06-26 09:08:55.000000 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/requires.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)        8 2023-06-26 09:08:55.000000 NGSpeciesID-0.3.0/NGSpeciesID.egg-info/top_level.txt
+-rw-r--r--   0 ksahlin    (501) staff       (20)    12737 2023-06-26 09:08:55.958255 NGSpeciesID-0.3.0/PKG-INFO
+-rw-r--r--   0 ksahlin    (501) staff       (20)    12056 2023-06-26 08:06:44.000000 NGSpeciesID-0.3.0/README.md
+drwxr-xr-x   0 ksahlin    (501) staff       (20)        0 2023-06-26 09:08:55.957703 NGSpeciesID-0.3.0/modules/
+-rw-r--r--   0 ksahlin    (501) staff       (20)        0 2020-02-12 12:28:36.000000 NGSpeciesID-0.3.0/modules/__init__.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     5728 2023-06-26 08:05:02.000000 NGSpeciesID-0.3.0/modules/barcode_trimmer.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    19671 2023-06-26 08:06:44.000000 NGSpeciesID-0.3.0/modules/cluster.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)    13840 2023-06-26 09:07:46.000000 NGSpeciesID-0.3.0/modules/consensus.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     8925 2023-06-26 08:04:00.000000 NGSpeciesID-0.3.0/modules/get_sorted_fastq_for_cluster.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     2998 2023-06-26 08:05:02.000000 NGSpeciesID-0.3.0/modules/help_functions.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)  1790771 2020-02-12 12:28:36.000000 NGSpeciesID-0.3.0/modules/p_minimizers_shared.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)     8956 2020-02-12 12:28:36.000000 NGSpeciesID-0.3.0/modules/parallelize.py
+-rw-r--r--   0 ksahlin    (501) staff       (20)       67 2023-06-26 09:08:55.958774 NGSpeciesID-0.3.0/setup.cfg
+-rw-r--r--   0 ksahlin    (501) staff       (20)     3993 2023-06-26 09:07:46.000000 NGSpeciesID-0.3.0/setup.py
```

### Comparing `NGSpeciesID-0.1.3/NGSpeciesID` & `NGSpeciesID-0.3.0/NGSpeciesID`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             curr_file.close()
 
 
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description="Reference-free clustering and consensus forming of targeted ONT or PacBio reads", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--version', action='version', version='%(prog)s 0.1.3')
+    parser.add_argument('--version', action='version', version='%(prog)s 0.3.0')
 
     parser.add_argument('--fastq', type=str,  default=False, help='Path to consensus fastq file(s)')
     parser.add_argument('--flnc', type=str, default=False, help='The flnc reads generated by the isoseq3 algorithm (BAM file)')
     parser.add_argument('--ccs', type=str, default=False, help='Path to consensus BAM file(s)')
     # parser.add_argument('--mapping', action="store_true", help='Only infer clusters by mapping, no alignment is performed.')
     parser.add_argument('--t', dest="nr_cores", type=int, default=8, help='Number of cores allocated for clustering')
     parser.add_argument('--d', dest="print_output", type=int, default=10000, help='For debugging, prints status of clustering and minimizer database every p reads processed.')
```

### Comparing `NGSpeciesID-0.1.3/NGSpeciesID.egg-info/PKG-INFO` & `NGSpeciesID-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,320 +1,302 @@
-Metadata-Version: 1.2
-Name: NGSpeciesID
-Version: 0.1.3
-Summary: Reconstructs viral consensus sequences from a set of ONT reads.
-Home-page: https://github.com/ksahlin/NGSpeciesID
-Author: Kristoffer Sahlin
-Author-email: ksahlin@math.su.se
-License: UNKNOWN
-Description: NGSpeciesID
-        ===========
-        
-        NGSpeciesID is a tool for clustering and consensus forming of long-read amplicon sequencing data (has been used with both PacBio and Oxford Nanopore data). The repository is a modified version of [isONclust](https://github.com/ksahlin/isONclust), where consensus, primer-removal, and polishing feautures have been added.
-        
-        NGSpeciesID is distributed as a python package supported on Linux / OSX with python v3.6. [![Build Status](https://travis-ci.org/ksahlin/NGSpeciesID.svg?branch=master)](https://travis-ci.org/ksahlin/NGSpeciesID).
-        
-        Table of Contents
-        =================
-        
-          * [INSTALLATION](#INSTALLATION)
-            * [Using conda](#Using-conda)
-            * [Testing installation](#testing-installation)
-          * [USAGE](#USAGE)
-            * [Filtering and subsampling](#filtering-and-subsampling)
-            * [Removing primers](#removing-primers)
-            * [Output](#Output)
-          * [EXAMPLE WORKFLOW](#EXAMPLE-WORKFLOW)
-          * [CREDITS](#CREDITS)
-          * [LICENCE](#LICENCE)
-        
-        
-        
-        INSTALLATION
-        ----------------
-        
-        **NOTE**: If you are experiencing issues (e.g. [this one](https://github.com/rvaser/spoa/issues/26)) with the third party tools  [spoa](https://github.com/rvaser/spoa) or [medaka](https://github.com/nanoporetech/medaka) in the all-in-one installation instructions below, please install the tools manually with their respective installation instructions [here](https://github.com/rvaser/spoa#installation) and [here](https://github.com/nanoporetech/medaka#installation).  
-        
-        ### Using conda
-        Conda is the preferred way to install NGSpeciesID.
-        
-        1. Create and activate a new environment called NGSpeciesID
-        
-        ```
-        conda create -n NGSpeciesID python=3.6 pip 
-        conda activate NGSpeciesID
-        ```
-        
-        2. Install NGSpeciesID 
-        
-        ```
-        conda install --yes -c conda-forge -c bioconda medaka==0.11.5 openblas==0.3.3 spoa racon minimap2
-        pip install NGSpeciesID
-        ```
-        3. You should now have 'NGSpeciesID' installed; try it:
-        ```
-        NGSpeciesID --help
-        ```
-        
-        Upon start/login to your server/computer you need to activate the conda environment "NGSpeciesID" to run NGSpeciesID as:
-        ```
-        conda activate NGSpeciesID
-        ```
-        
-        
-        
-        ### Testing installation
-        
-        0. Activate conda environment
-        ```
-        conda activate NGSpeciesID
-        ```
-        
-        1. Make a new directory and navigate to it
-        ```
-        mkdir test_ngspeciesID
-        cd test_ngspeciesID
-        ```
-        
-        2. Download the test fastq file called "sample_h1.fastq" (filesize 390kb)
-        
-        ```
-        curl -LO https://raw.githubusercontent.com/ksahlin/NGSpeciesID/master/test/sample_h1.fastq
-        ```
-        
-        3. Run the NGSpecies command on test file. Outputs will be saved in "/test_ngspeciesID/sample_h1/", where the final polished consensus file ("consensus.fasta") is located in the "/test_ngspeciesID/sample_h1/medaka_cl_id_<cluster number>" directory.
-        
-        ```
-        NGSpeciesID --ont --fastq sample_h1.fastq --outfolder ./sample_h1 --consensus --medaka
-        ```
-        
-        
-        USAGE
-        -------
-        
-        NGSpeciesID needs a fastq file generated by an Oxford Nanopore basecaller.
-        
-        ```
-        NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] 
-        ```
-        The argument `--ont` simply means `--k 13 --w 20`. These arguments can be set manually without the `--ont` flag. Specify number of cores with `--t`. 
-        
-        
-        NGSpeciesID can also run with racon as polisher. For example
-        
-        ```
-        NGSpeciesID --ont --consensus --racon --racon_iter 3 --fastq [reads.fastq] --outfolder [/path/to/output] 
-        ```
-        will polish the consensus sequences with racon three times.
-        
-        ### Filtering and subsampling
-        
-        NGSpeciesID employs quality filtering of the reads based on read Phred scores. However, we recommend also removing reads much shorter or longer than the intended target, which often represent chimeras or contaminations. This can be done by specifying the `--m (intended target length)` and `--s (maximum deviation from target length)`. NGSpeciesID also has the feature of subsampling reads using parameter `--sample_size`. Altogether, if we want to filter out reads outside the length interval [700,800] and using a subset of 300 reads (if the dataset consists of more reads) we could run
-        
-        ```
-        NGSpeciesID --ont --sample_size 300 --m 750 --s 50 --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output]
-        ```
-        
-        By default, length filtering and subsampling are not invoked if parameters are not specified.
-        
-        ### Removing primers
-        
-        If customized primers are to be expected in the reads thay can be detected and removed. The primer file is expected to be in fasta format. Here is an example of a primer file:
-        
-        ```
-        >MCB869_ONT_R
-        CGATCAATCCCCTAACAAACTAGG
-        >MCB398_ONT_F
-        TACCATGAGGACAAATATCATTCTG
-        ```
-        NGSpeciesID searches for primes in a window of Xbp (parameter, default 150bp) at the beginning and end of each consensus.
-        
-        
-        Trimming of primers is performed after consensus forming and can be invoked as
-        ```
-        NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] --primer_file [primers.fa]
-        ```
-        
-        `NGSpeciesID` can also remove universal tails. Trimming of tails is performed after consensus forming and can be invoked as
-        
-        ```
-        NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] --remove_universal_tails
-        ```
-        
-        The two options are mutually exclusive, i.e., only one of them can be run.
-        
-        ### Output
-        
-        The output consists of the polished consensus sequences along with some information about clustering.
-        
-        * Polished consensus sequence(s). A folder named “medaka_cl_id_X”[/"racon_cl_id_X"] is created for each predicted consensus. Each such folder contains a sequence “consensus.fasta” which is the final output of NGSpeciesID. 
-        * Draft spoa consensus sequences of each of the clusters are given as consensus_reference_X.fasta (where X is a number).
-        * The final cluster information is given in a tsv file `final_clusters.tsv` present in the specified output folder.
-        
-        
-        In the cluster TSV-file, the first column is the cluster ID and the second column is the read accession. For example:
-        
-        ```
-        0 read_X_acc
-        0 read_Y_acc
-        ...
-        n read_Z_acc
-        ```
-        if there are n reads there will be n rows. Some reads might be singletons. The rows are ordered with respect to the size of the cluster (largest first).
-        
-        
-        EXAMPLE WORKFLOW
-        -----------------
-        
-        The bioinformatics workflow below was developed as part of a step-by-step protocol for field-deployable DNA amplicon sequencing with the Oxford Nanopore Technologies MinION. The full protocol manuscript is in submission; a link will be posted here when available. The steps below correspond to step numbers in the protocol.
-        
-        #### P2 | Generate custom indexes for uniquely identifying samples using [`barcode_generator`](https://github.com/lcomai/barcode_generator). This software uses Python3.
-        
-        ```
-        python3 barcode_generator_3.4.py none 24 40 8
-        ```
-        
-        Here, the parameters are set as:
-        - table_excluded_barcodes = 'none'
-        - index length = 24 base pairs
-        - number of barcodes to generate = 40
-        - hamming distance = 8
-        
-        After lab steps are complete:
-        
-        #### B1 | Basecalling and quality check (optional) with [Guppy](https://community.nanoporetech.com/downloads)
-        
-        These commands use the fast basecalling model from Guppy.
-        
-        Basecalling for R9.4 flow cell:
-        
-        ```
-        guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r9.4.1_450bps_fast.cfg --recursive --disable_pings
-        ```
-        
-        Basecalling and filter reads by quality score (here, set to 7):
-        
-        ```
-        guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r9.4.1_450bps_fast.cfg --recursive --disable_pings --min_qscore 7
-        ```
-        
-        Basecalling for R10.3 flow cell:
-        
-        ```
-        guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r10.3_450bps_fast.cfg --recursive --disable_pings
-        ```
-         
-        #### B2 | Go to folder with the fastq files generated by Guppy
-        
-        #### B3 | Concatenate all the read files into one large file
-        
-        ```
-        cat *.fastq > sequencing_reads.fastq
-        ```
-        
-        #### B4 | Check raw read quality/stats with [NanoPlot](https://github.com/wdecoster/NanoPlot)
-        
-        ```
-        NanoPlot --fastq_rich sequencing_reads.fastq -o sequencing_run -p sequencing_run
-        ```
-        
-        #### B5 | Demultiplexing of the sequencing data with [minibar](https://github.com/calacademy-research/minibar) or Guppy
-        
-        Example files can be found in:
-        - [Supplementary Data 1](./test/Supplementary_File1_reads.fastq): 3,000 reads in fastq format from three fish species - Atlantic cod (*Gadus morhua*), Haddock (*Melanogrammus aeglefinus*), and Whiting (*Merlangius merlangus*) - sequenced on a Flongle flow cell.
-        - [Supplementary Data 2](./test/Supplementary_File2_minibar.txt): index file used for demultiplexing with minibar
-        
-        The example files Supplementary Data 1 can be used for `sequencing_reads.fastq` and Supplementary Data 2 can be used for `indexes.txt`.
-        
-        #### B5a | minibar (using example files):
-        
-        ```
-        python minibar.py indexes.txt sequencing_reads.fastq -T -F -e 3 -E 11
-        ```
-        
-        Here, the edit distance allowed between indexes (`-e`) is set to 3 base pairs and the edit distance allowed between primer sequences (`-E`) is set to 11 base pairs.
-        
-        #### B5b | Guppy:
-        
-        ```
-        guppy_barcoder -i sequencing_reads.fastq -s demultiplex_folder --trim_barcodes --disable_pings
-        ```
-        
-        #### B6 | Read filtering, clustering, consensus generation and polishing with NGSpeciesID
-        
-        For a single sample (using example primer file):
-        
-        ```
-        NGSpeciesID --ont --consensus --sample_size 500 --m 800 --s 100 --medaka --primer_file primers.txt --fastq barcode0.fastq --outfolder barcode0_consensus
-        ```
-        
-        Here, the parameters are set as:
-        - the data is from ONT MinION (`--ont`)
-        - we want to generate consensus sequences (`--consensus`)
-        - subsample of reads (`--sample_size`) = 500 reads subsampled per sample to analyze 
-        - intended target length (`--m`) = 800 base pairs
-        - maximum deviation from target length (`--s`) = 100 base pairs
-        - use [Medaka](https://github.com/nanoporetech/medaka) to polish the final consensus sequences (`--medaka`)
-        - if a `--primer_file` is given, NGSpeciesID will check to remove any remaining primer sequence. The example primer file is available in [Supplementary Data 3](./test/Supplementary_File3_primer.txt). The primers were developed in Mikkelsen, P.M., Bieler, R., Kappner, I., & Rawlings, T.A. (2006). Phylogeny of Veneroidea (Mollusca: Bivalvia) based on morphology and molecules. *Zoological Journal of the Linnean Society*, 148(3), 439-521.
-        - the input file of demultiplexed reads is specified by `--fastq` (output from step B5)
-        - the output consensus files will be saved to `--outfolder`
-        
-        To run this step on **more than one sample**, use a bash script with a for loop:
-        
-        ```
-        for file in *.fastq; do
-        bn=`basename $file .fastq`
-        NGSpeciesID --ont --consensus --sample_size 500 --m 800 --s 100 --medaka --primer_file primers.txt --fastq $file --outfolder ${bn}
-        done
-        ```
-        
-        This loop uses the wildcard `*` to indicate you want to analyze all files with the `.fastq` extension and assumes the command is run from the directory that contains the read files (if not, be sure to change the file path: `path/to/*.fastq`). 
-        
-        This loop code can be entered at a UNIX/Mac terminal (be sure the spacing/indentation is correct) or saved as a script (see [`consensus.sh`](./test/consensus.sh). The script should be run from the terminal and in the directory that contains the read files as:
-        
-        ```
-        ./consensus.sh
-        ```
-        
-        #### B7 | Compare consensus sequences to reference database with [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastDocs&DOC_TYPE=Download)
-        
-        - Create/format database for BLAST search:
-        
-        ```
-        makeblastdb -in database.fasta -dbtype nucl -out database
-        ```
-        
-        - Conduct BLAST search:
-        
-        ```
-        blastn -db database -query barcode0_consensus.fasta -outfmt 6 -out barcode0_consensus_blast.out
-        ```
-        
-        Check the results and refine the search or database as needed to better identify the sequence identity of your samples!
-        
-        
-        
-        CREDITS
-        ----------------
-        
-        Please cite [1] when using NGSpeciesID.
-        
-        1. Sahlin, K, Lim, MCW, Prost, S. NGSpeciesID: DNA barcode and amplicon consensus generation from long‐read sequencing data. Ecol Evol. 2021; 00: 1– 7. https://doi.org/10.1002/ece3.7146
-        
-        
-        
-        LICENCE
-        ----------------
-        
-        GPL v3.0, see [LICENSE.txt](https://github.com/ksahlin/NGSpeciesID/blob/master/LICENCE.txt).
-        
-        
-        
-Keywords: viral sequeces ONT Oxford Nanopore Technologies long reads
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+NGSpeciesID
+===========
+
+NGSpeciesID is a tool for clustering and consensus forming of long-read amplicon sequencing data (has been used with both PacBio and Oxford Nanopore data). The repository is a modified version of [isONclust](https://github.com/ksahlin/isONclust), where consensus, primer-removal, and polishing feautures have been added.
+
+NGSpeciesID is distributed as a python package supported on Linux / OSX with python v3.6. [![Build Status](https://travis-ci.org/ksahlin/NGSpeciesID.svg?branch=master)](https://travis-ci.org/ksahlin/NGSpeciesID).
+
+Table of Contents
+=================
+
+  * [INSTALLATION](#INSTALLATION)
+    * [Using conda](#Using-conda)
+    * [Testing installation](#testing-installation)
+  * [USAGE](#USAGE)
+    * [Filtering and subsampling](#filtering-and-subsampling)
+    * [Removing primers](#removing-primers)
+    * [Output](#Output)
+  * [EXAMPLE WORKFLOW](#EXAMPLE-WORKFLOW)
+  * [CREDITS](#CREDITS)
+  * [LICENCE](#LICENCE)
+
+
+
+INSTALLATION
+----------------
+
+**NOTE**: If you are experiencing issues (e.g. [this one](https://github.com/rvaser/spoa/issues/26)) with the third party tools  [spoa](https://github.com/rvaser/spoa) or [medaka](https://github.com/nanoporetech/medaka) in the all-in-one installation instructions below, please install the tools manually with their respective installation instructions [here](https://github.com/rvaser/spoa#installation) and [here](https://github.com/nanoporetech/medaka#installation).  
+
+### Using conda
+Conda is the preferred way to install NGSpeciesID.
+
+1. Create and activate a new environment called NGSpeciesID
+
+```
+conda create -n NGSpeciesID python=3.6 pip 
+conda activate NGSpeciesID
+```
+
+2. Install NGSpeciesID 
+
+```
+conda install --yes -c conda-forge -c bioconda medaka==0.11.5 openblas==0.3.3 spoa racon minimap2
+pip install NGSpeciesID
+```
+3. You should now have 'NGSpeciesID' installed; try it:
+```
+NGSpeciesID --help
+```
+
+Upon start/login to your server/computer you need to activate the conda environment "NGSpeciesID" to run NGSpeciesID as:
+```
+conda activate NGSpeciesID
+```
+
+
+
+### Testing installation
+
+0. Activate conda environment
+```
+conda activate NGSpeciesID
+```
+
+1. Make a new directory and navigate to it
+```
+mkdir test_ngspeciesID
+cd test_ngspeciesID
+```
+
+2. Download the test fastq file called "sample_h1.fastq" (filesize 390kb)
+
+```
+curl -LO https://raw.githubusercontent.com/ksahlin/NGSpeciesID/master/test/sample_h1.fastq
+```
+
+3. Run the NGSpecies command on test file. Outputs will be saved in "/test_ngspeciesID/sample_h1/", where the final polished consensus file ("consensus.fasta") is located in the "/test_ngspeciesID/sample_h1/medaka_cl_id_<cluster number>" directory.
+
+```
+NGSpeciesID --ont --fastq sample_h1.fastq --outfolder ./sample_h1 --consensus --medaka
+```
+
+
+USAGE
+-------
+
+NGSpeciesID needs a fastq file generated by an Oxford Nanopore basecaller.
+
+```
+NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] 
+```
+The argument `--ont` simply means `--k 13 --w 20`. These arguments can be set manually without the `--ont` flag. Specify number of cores with `--t`. 
+
+
+NGSpeciesID can also run with racon as polisher. For example
+
+```
+NGSpeciesID --ont --consensus --racon --racon_iter 3 --fastq [reads.fastq] --outfolder [/path/to/output] 
+```
+will polish the consensus sequences with racon three times.
+
+### Filtering and subsampling
+
+NGSpeciesID employs quality filtering of the reads based on read Phred scores. However, we recommend also removing reads much shorter or longer than the intended target, which often represent chimeras or contaminations. This can be done by specifying the `--m (intended target length)` and `--s (maximum deviation from target length)`. NGSpeciesID also has the feature of subsampling reads using parameter `--sample_size`. Altogether, if we want to filter out reads outside the length interval [700,800] and using a subset of 300 reads (if the dataset consists of more reads) we could run
+
+```
+NGSpeciesID --ont --sample_size 300 --m 750 --s 50 --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output]
+```
+
+By default, length filtering and subsampling are not invoked if parameters are not specified.
+
+### Removing primers
+
+If customized primers are to be expected in the reads thay can be detected and removed. The primer file is expected to be in fasta format. Here is an example of a primer file:
+
+```
+>MCB869_ONT_R
+CGATCAATCCCCTAACAAACTAGG
+>MCB398_ONT_F
+TACCATGAGGACAAATATCATTCTG
+```
+NGSpeciesID searches for primes in a window of Xbp (parameter, default 150bp) at the beginning and end of each consensus.
+
+
+Trimming of primers is performed after consensus forming and can be invoked as
+```
+NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] --primer_file [primers.fa]
+```
+
+`NGSpeciesID` can also remove universal tails. Trimming of tails is performed after consensus forming and can be invoked as
+
+```
+NGSpeciesID --ont --consensus --medaka --fastq [reads.fastq] --outfolder [/path/to/output] --remove_universal_tails
+```
+
+The two options are mutually exclusive, i.e., only one of them can be run.
+
+### Output
+
+The output consists of the polished consensus sequences along with some information about clustering.
+
+* Polished consensus sequence(s). A folder named “medaka_cl_id_X”[/"racon_cl_id_X"] is created for each predicted consensus. Each such folder contains a sequence “consensus.fasta” which is the final output of NGSpeciesID. 
+* Draft spoa consensus sequences of each of the clusters are given as consensus_reference_X.fasta (where X is a number).
+* The final cluster information is given in a tsv file `final_clusters.tsv` present in the specified output folder.
+
+
+In the cluster TSV-file, the first column is the cluster ID and the second column is the read accession. For example:
+
+```
+0 read_X_acc
+0 read_Y_acc
+...
+n read_Z_acc
+```
+if there are n reads there will be n rows. Some reads might be singletons. The rows are ordered with respect to the size of the cluster (largest first).
+
+
+EXAMPLE WORKFLOW
+-----------------
+
+The bioinformatics workflow below was developed as part of a step-by-step protocol for field-deployable DNA amplicon sequencing with the Oxford Nanopore Technologies MinION. The full protocol manuscript is in submission; a link will be posted here when available. The steps below correspond to step numbers in the protocol.
+
+#### P2 | Generate custom indexes for uniquely identifying samples using [`barcode_generator`](https://github.com/lcomai/barcode_generator). This software uses Python3.
+
+```
+python3 barcode_generator_3.4.py none 24 40 8
+```
+
+Here, the parameters are set as:
+- table_excluded_barcodes = 'none'
+- index length = 24 base pairs
+- number of barcodes to generate = 40
+- hamming distance = 8
+
+After lab steps are complete:
+
+#### B1 | Basecalling and quality check (optional) with [Guppy](https://community.nanoporetech.com/downloads)
+
+These commands use the fast basecalling model from Guppy.
+
+Basecalling for R9.4 flow cell:
+
+```
+guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r9.4.1_450bps_fast.cfg --recursive --disable_pings
+```
+
+Basecalling and filter reads by quality score (here, set to 7):
+
+```
+guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r9.4.1_450bps_fast.cfg --recursive --disable_pings --min_qscore 7
+```
+
+Basecalling for R10.3 flow cell:
+
+```
+guppy_basecaller --input_path minKNOW_input/ --save_path basecalled_fastqs/ -c dna_r10.3_450bps_fast.cfg --recursive --disable_pings
+```
+ 
+#### B2 | Go to folder with the fastq files generated by Guppy
+
+#### B3 | Concatenate all the read files into one large file
+
+```
+cat *.fastq > sequencing_reads.fastq
+```
+
+#### B4 | Check raw read quality/stats with [NanoPlot](https://github.com/wdecoster/NanoPlot)
+
+```
+NanoPlot --fastq_rich sequencing_reads.fastq -o sequencing_run -p sequencing_run
+```
+
+#### B5 | Demultiplexing of the sequencing data with [minibar](https://github.com/calacademy-research/minibar) or Guppy
+
+Example files can be found in:
+- [Supplementary Data 1](./test/Supplementary_File1_reads.fastq): 3,000 reads in fastq format from three fish species - Atlantic cod (*Gadus morhua*), Haddock (*Melanogrammus aeglefinus*), and Whiting (*Merlangius merlangus*) - sequenced on a Flongle flow cell.
+- [Supplementary Data 2](./test/Supplementary_File2_minibar.txt): index file used for demultiplexing with minibar
+
+The example files Supplementary Data 1 can be used for `sequencing_reads.fastq` and Supplementary Data 2 can be used for `indexes.txt`.
+
+#### B5a | minibar (using example files):
+
+```
+python minibar.py indexes.txt sequencing_reads.fastq -T -F -e 3 -E 11
+```
+
+Here, the edit distance allowed between indexes (`-e`) is set to 3 base pairs and the edit distance allowed between primer sequences (`-E`) is set to 11 base pairs.
+
+#### B5b | Guppy:
+
+```
+guppy_barcoder -i sequencing_reads.fastq -s demultiplex_folder --trim_barcodes --disable_pings
+```
+
+#### B6 | Read filtering, clustering, consensus generation and polishing with NGSpeciesID
+
+For a single sample (using example primer file):
+
+```
+NGSpeciesID --ont --consensus --sample_size 500 --m 800 --s 100 --medaka --primer_file primers.txt --fastq barcode0.fastq --outfolder barcode0_consensus
+```
+
+Here, the parameters are set as:
+- the data is from ONT MinION (`--ont`)
+- we want to generate consensus sequences (`--consensus`)
+- subsample of reads (`--sample_size`) = 500 reads subsampled per sample to analyze 
+- intended target length (`--m`) = 800 base pairs
+- maximum deviation from target length (`--s`) = 100 base pairs
+- use [Medaka](https://github.com/nanoporetech/medaka) to polish the final consensus sequences (`--medaka`)
+- if a `--primer_file` is given, NGSpeciesID will check to remove any remaining primer sequence. The example primer file is available in [Supplementary Data 3](./test/Supplementary_File3_primer.txt). The primers were developed in Mikkelsen, P.M., Bieler, R., Kappner, I., & Rawlings, T.A. (2006). Phylogeny of Veneroidea (Mollusca: Bivalvia) based on morphology and molecules. *Zoological Journal of the Linnean Society*, 148(3), 439-521.
+- the input file of demultiplexed reads is specified by `--fastq` (output from step B5)
+- the output consensus files will be saved to `--outfolder`
+
+To run this step on **more than one sample**, use a bash script with a for loop:
+
+```
+for file in *.fastq; do
+bn=`basename $file .fastq`
+NGSpeciesID --ont --consensus --sample_size 500 --m 800 --s 100 --medaka --primer_file primers.txt --fastq $file --outfolder ${bn}
+done
+```
+
+This loop uses the wildcard `*` to indicate you want to analyze all files with the `.fastq` extension and assumes the command is run from the directory that contains the read files (if not, be sure to change the file path: `path/to/*.fastq`). 
+
+This loop code can be entered at a UNIX/Mac terminal (be sure the spacing/indentation is correct) or saved as a script (see [`consensus.sh`](./test/consensus.sh). The script should be run from the terminal and in the directory that contains the read files as:
+
+```
+./consensus.sh
+```
+
+#### B7 | Compare consensus sequences to reference database with [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastDocs&DOC_TYPE=Download)
+
+- Create/format database for BLAST search:
+
+```
+makeblastdb -in database.fasta -dbtype nucl -out database
+```
+
+- Conduct BLAST search:
+
+```
+blastn -db database -query barcode0_consensus.fasta -outfmt 6 -out barcode0_consensus_blast.out
+```
+
+Check the results and refine the search or database as needed to better identify the sequence identity of your samples!
+
+
+
+CREDITS
+----------------
+
+Please cite [1] when using NGSpeciesID.
+
+1. Sahlin, K, Lim, MCW, Prost, S. NGSpeciesID: DNA barcode and amplicon consensus generation from long‐read sequencing data. Ecol Evol. 2021; 00: 1– 7. https://doi.org/10.1002/ece3.7146
+
+
+
+LICENCE
+----------------
+
+GPL v3.0, see [LICENSE.txt](https://github.com/ksahlin/NGSpeciesID/blob/master/LICENCE.txt).
+
+
```

### Comparing `NGSpeciesID-0.1.3/README.md` & `NGSpeciesID-0.3.0/NGSpeciesID.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: NGSpeciesID
+Version: 0.3.0
+Summary: Reconstructs viral consensus sequences from a set of ONT reads.
+Home-page: https://github.com/ksahlin/NGSpeciesID
+Author: Kristoffer Sahlin
+Author-email: ksahlin@math.su.se
+Keywords: viral sequeces ONT Oxford Nanopore Technologies long reads
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+License-File: LICENSE.txt
+
 NGSpeciesID
 ===========
 
 NGSpeciesID is a tool for clustering and consensus forming of long-read amplicon sequencing data (has been used with both PacBio and Oxford Nanopore data). The repository is a modified version of [isONclust](https://github.com/ksahlin/isONclust), where consensus, primer-removal, and polishing feautures have been added.
 
 NGSpeciesID is distributed as a python package supported on Linux / OSX with python v3.6. [![Build Status](https://travis-ci.org/ksahlin/NGSpeciesID.svg?branch=master)](https://travis-ci.org/ksahlin/NGSpeciesID).
```

### Comparing `NGSpeciesID-0.1.3/modules/barcode_trimmer.py` & `NGSpeciesID-0.3.0/modules/barcode_trimmer.py`

 * *Files identical despite different names*

### Comparing `NGSpeciesID-0.1.3/modules/cluster.py` & `NGSpeciesID-0.3.0/modules/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             6. Adds current read to representative, or makes it a new representative of a new cluster.
             7. If new representative: add the minimizers to the minimizer database
             8. Assign the actual reads to their new cluster and their new cluster representative (since all reads were initialized as their own representatives to deal with multiprocessing) 
     """
 
     ## For multiprocessing only
     prev_b_indices = [ prev_batch_index for (read_cl_id, prev_batch_index, acc, seq, qual, score) in sorted_reads ]
-    lowest_batch_index = max(1, min(prev_b_indices))
+    lowest_batch_index = max(1, min(prev_b_indices or [1]))
     skip_count = prev_b_indices.count(lowest_batch_index)
     print("Saved: {0} iterations.".format(skip_count) )
     ###################################
     
     ## logging counters 
     aln_passed_criteria = 0
     mapped_passed_criteria = 0
@@ -365,15 +365,15 @@
         # delete old origins
         del representatives[read_cl_id]
     ##########################
 
     print("Total number of reads iterated through:{0}".format(len(sorted_reads)))
     print("Passed mapping criteria:{0}".format(mapped_passed_criteria))
     print("Passed alignment criteria in this process:{0}".format(aln_passed_criteria))
-    print("Total calls to alignment mudule in this process:{0}".format(aln_called))
+    print("Total calls to alignment module in this process:{0}".format(aln_called))
 
     return { new_batch_index : (clusters, representatives, minimizer_database, new_batch_index)}
 
 
 def p_shared_minimizer_empirical(error_rate_read, error_rate_center, p_emp_probs):
     e1 = round(error_rate_read, 2)
     # print(e1)
```

### Comparing `NGSpeciesID-0.1.3/modules/consensus.py` & `NGSpeciesID-0.3.0/modules/consensus.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,14 +132,33 @@
 
         shutil.copyfile(center_file, os.path.join(outfolder, "consensus.fasta"))
         # print('Done.')
         stdout.flush()
     # consensus.run_medaka( " medaka_consensus -i ~/tmp/stefan_isonclust/mixed_b1_b3_b4_b5.fastq -d ~/tmp/stefan_isonclust/mixed_b1_b3_b4_b5_isonclust/consensus_references.fasta -o ~/tmp/stefan_isonclust/mixed_b1_b3_b4_b5_medaka/ -t 1 -m r941_min_high_g303")
 
 
+def highest_aln_identity(seq, seq2):
+    # RC
+    seq2_rc = reverse_complement(seq2)
+    seq_aln_rc, seq2_aln_rc, cigar_string_rc, cigar_tuples_rc, alignment_score_rc = parasail_alignment(seq, seq2_rc)
+    nr_mismatching_pos = len([1 for n1, n2 in zip(seq_aln_rc, seq2_aln_rc) if n1 != n2])
+    total_pos_rc = len(seq_aln_rc)
+    aln_identity_rc =  (total_pos_rc - nr_mismatching_pos) / float(total_pos_rc)
+    print('Rec comp orientation identity %: ', aln_identity_rc)
+
+    # FW
+    seq_aln, seq2_aln, cigar_string, cigar_tuples, alignment_score = parasail_alignment(seq, seq2)
+    nr_mismatching_pos = len([1 for n1, n2 in zip(seq_aln, seq2_aln) if n1 != n2])
+    total_pos = len(seq_aln)
+    aln_identity_fw = (total_pos - nr_mismatching_pos) / float(total_pos)  
+    print('Forward orientation identity %: ', aln_identity_fw)
+    aln_identity = max([aln_identity_fw, aln_identity_rc])
+    return aln_identity
+
+
 def detect_reverse_complements(centers, rc_identity_threshold):
     filtered_centers = []
     already_removed = set()
     for i, (nr_reads_in_cl, c_id, seq, reads_path) in enumerate(centers):
         if type(reads_path) != list:
             all_reads = [reads_path]
         else:
@@ -147,31 +166,22 @@
 
         merged_cluster_id = c_id
         merged_nr_reads = nr_reads_in_cl
         if c_id in already_removed:
             print("has already been merged, skipping")
             continue
 
-        elif i == len(centers) - 1: # last sequence and it is not in already removed
+        elif i == len(centers) - 1: # last sequence and it is not in already_removed
             filtered_centers.append( [merged_nr_reads, c_id, seq, all_reads ] )
 
         else:
             for j, (nr_reads_in_cl2, c_id2, seq2, reads_path) in enumerate(centers[i+1:]):
-                seq2_rc = reverse_complement(seq2)
-                seq_aln, seq2_rc_aln, cigar_string, cigar_tuples, alignment_score = parasail_alignment(seq, seq2_rc)
-                # print(i,j)
-                # print(seq_aln)
-                # print(seq2_rc_aln)
-                nr_mismatching_pos = len([1 for n1, n2 in zip(seq_aln, seq2_rc_aln) if n1 != n2])
-                total_pos = len(seq_aln)
-                aln_identity =  (total_pos - nr_mismatching_pos) / float(total_pos)
-                print(aln_identity)
-
+                aln_identity = highest_aln_identity(seq, seq2)
                 if aln_identity >= rc_identity_threshold:
-                    print("Detected alignment identidy above threchold for reverse complement. Keeping center with the most read support and adding rc reads to supporting reads.")
+                    print("Detected two consensus sequences with alignment identidy above threshold (from either reverse complement or split clusters). Keeping center with the most read support and merging reads.")
                     merged_nr_reads += nr_reads_in_cl2
                     already_removed.add(c_id2)
 
                     if type(reads_path) != list:
                         all_reads.append(reads_path)
                     else:
                         for rp in reads_path:
@@ -267,10 +277,11 @@
         elif nr_reads_in_cluster == 1:
             singletons += 1
         elif nr_reads_in_cluster > 1:
             discarded_clusters.append(nr_reads_in_cluster)
     print(f"{singletons} singletons were discarded")
     print(
         f"{len(discarded_clusters)} clusters were discarded due to not passing the abundance_cutoff: "
-        f"a total of {sum(discarded_clusters)} reads were discarded"
+        f"a total of {sum(discarded_clusters)} reads were discarded. "
+        f"Highest abundance among them: {max(discarded_clusters or [0])} reads."
     )
     return centers
```

### Comparing `NGSpeciesID-0.1.3/modules/get_sorted_fastq_for_cluster.py` & `NGSpeciesID-0.3.0/modules/get_sorted_fastq_for_cluster.py`

 * *Files identical despite different names*

### Comparing `NGSpeciesID-0.1.3/modules/help_functions.py` & `NGSpeciesID-0.3.0/modules/help_functions.py`

 * *Files identical despite different names*

### Comparing `NGSpeciesID-0.1.3/modules/p_minimizers_shared.py` & `NGSpeciesID-0.3.0/modules/p_minimizers_shared.py`

 * *Files identical despite different names*

### Comparing `NGSpeciesID-0.1.3/modules/parallelize.py` & `NGSpeciesID-0.3.0/modules/parallelize.py`

 * *Files identical despite different names*

### Comparing `NGSpeciesID-0.1.3/setup.py` & `NGSpeciesID-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
 
     name='NGSpeciesID',  # Required
-    version='0.1.3',  # Required
+    version='0.3.0',  # Required
     description='Reconstructs viral consensus sequences from a set of ONT reads.',  # Required
     long_description=long_description,  # Optional
     url='https://github.com/ksahlin/NGSpeciesID',  # Optional
     author='Kristoffer Sahlin',  # Optional
     author_email='ksahlin@math.su.se',  # Optional
 
     # Classifiers help users find your project by categorizing it.
```

