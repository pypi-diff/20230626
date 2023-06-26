# Comparing `tmp/current_events_magnifier-0.0.3.8.tar.gz` & `tmp/current_events_magnifier-0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.8.tar", last modified: Mon Jun 19 07:00:54 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.3.9.tar", last modified: Mon Jun 26 10:53:55 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.8.tar` & `current_events_magnifier-0.0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.8/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8295 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7677 2023-06-19 07:00:52.000000 current_events_magnifier-0.0.3.8/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6370 2023-06-19 06:06:59.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3813 2023-06-19 06:18:39.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.8/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8295 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-19 07:00:54.000000 current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-19 07:00:54.077424 current_events_magnifier-0.0.3.8/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1157 2023-06-19 07:00:52.000000 current_events_magnifier-0.0.3.8/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.9/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7433 2023-06-20 08:13:10.000000 current_events_magnifier-0.0.3.9/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7115 2023-06-26 10:50:21.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8825 2023-06-26 10:38:38.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-06-23 06:41:12.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7734 2023-06-26 08:43:23.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10227 2023-06-26 10:42:38.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13861 2023-06-26 10:18:43.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1191 2023-06-26 10:53:36.000000 current_events_magnifier-0.0.3.9/setup.py
```

### Comparing `current_events_magnifier-0.0.3.8/LICENSE` & `current_events_magnifier-0.0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.8/PKG-INFO` & `current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: current_events_magnifier
-Version: 0.0.3.8
+Name: current-events-magnifier
+Version: 0.0.3.9
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,30 +17,24 @@
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
-## Still developing
-### TO do list
-1. More normalization methods (finished)
-2. Test on minus strand or reversed strand (finished)
-3. Subsample coverage (finished)
-4. single mode(finished)
-5. merge images together(finished)
-6. test data to github(finished)
+
 ## Before start, you should know
 ### What is re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
+
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 
 ## Installation
 Requirement : Python >=3.7, <3.10
 
@@ -100,52 +94,52 @@
 # assumed your fast5 file folder name is fast5/
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
-So for the following command , I used ```--chrom NR_103073.1  --pos A2030 --strand +```
-### 1. F5c resquiggle (v1.2)
+So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
+### 1. F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-f5c resquiggle -c final.fastq file.blow5 -o file.paf
+f5c resquiggle -c all.fastq file.blow5 -o file.paf
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta 
 ```
 ### 2. Tombo resquiggle (v1.5.0)
 Step 1 and 3 should run on your two sample respectively, before the step 4.
 1. Data format conversion.
 ```sh
 # assumed your fast5 file folder name is fast5/
-multi_to_single_fast5 -i fast5/ -o single/ --recursive -t 16
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
 2. Subsample (Optional)
 
 Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
 After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 3. Run tombo resquiggle
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
@@ -153,14 +147,14 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 4. Run current_events_magnifier to plot
 ```sh
-python CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
 ```
```

### Comparing `current_events_magnifier-0.0.3.8/README.md` & `current_events_magnifier-0.0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,24 @@
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
-## Still developing
-### TO do list
-1. More normalization methods (finished)
-2. Test on minus strand or reversed strand (finished)
-3. Subsample coverage (finished)
-4. single mode(finished)
-5. merge images together(finished)
-6. test data to github(finished)
+
 ## Before start, you should know
 ### What is re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
+
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 
 ## Installation
 Requirement : Python >=3.7, <3.10
 
@@ -86,52 +80,52 @@
 # assumed your fast5 file folder name is fast5/
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
-So for the following command , I used ```--chrom NR_103073.1  --pos A2030 --strand +```
-### 1. F5c resquiggle (v1.2)
+So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
+### 1. F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-f5c resquiggle -c final.fastq file.blow5 -o file.paf
+f5c resquiggle -c all.fastq file.blow5 -o file.paf
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta 
 ```
 ### 2. Tombo resquiggle (v1.5.0)
 Step 1 and 3 should run on your two sample respectively, before the step 4.
 1. Data format conversion.
 ```sh
 # assumed your fast5 file folder name is fast5/
-multi_to_single_fast5 -i fast5/ -o single/ --recursive -t 16
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
 2. Subsample (Optional)
 
 Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
 After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 3. Run tombo resquiggle
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
@@ -139,14 +133,14 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 4. Run current_events_magnifier to plot
 ```sh
-python CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
 ```
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python
 import argparse
 import os
-from current_events_magnifier.cem_utils import read_fasta_to_dic,reverse_fasta
+from cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
-from current_events_magnifier.plot import signal_plot
+from plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
 import warnings
+import time
 warnings.filterwarnings("ignore", category=PlotnineWarning)
-
+import numpy as np
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
         parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
+        parser_input.add_argument('--rna', action='store_true', help='RNA mode')
     # Define the argument parser
     parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
     parser_tombo = subparsers.add_parser('tombo', help='tackle tombo re-squiggle')
     parser_tombo.add_argument('--basecall_group', default="RawGenomeCorrected_000",
@@ -35,42 +37,58 @@
     parser_tombo.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
     add_public_argument(parser_tombo)
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
-    parser_f5c.add_argument('-c', "--control", required=True,
+    parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
+    parser_f5c.add_argument('--base_shift',type=int, default=0, help="base shift of f5c")
     add_public_argument(parser_f5c)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
 
-    args.pos = args.pos - 1
+    # read reference
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
     # length filter
+    args.pos = args.pos - 1
     length_gene = len(fasta[args.chrom])
     if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
-        raise Exception("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
-    base_list = fasta[args.chrom][args.pos - args.len:args.pos + args.len + 1]
+        raise RuntimeError("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
+    base_list = fasta[args.chrom][args.pos - args.len:args.pos + args.len + 1].upper()
 
     if args.strand == '-':
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
+
+    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
+    if args.rna:
+        base_list = base_list.replace("T", "U")
+        print("Running RNA mode ...")
+        title ='RNA  ' + title
+    else:
+        print("Running DNA mode ...")
+        title = 'DNA  ' + title
+
     results_path = args.output
     if not os.path.exists(results_path):
         os.mkdir(results_path)
+    else:
+        print("Output file existed! It will be overwrite after 5 secs ...")
+        time.sleep(5)
+        print("Continue ...")
+
 
-    title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
     if args.function == 'tombo' :
 
         from  current_events_magnifier.read_tombo_resquiggle import create_read_list_file,extract_group
         wt_file = create_read_list_file(args.input_fast5, results_path)
         df_wt, aligned_num_wt = extract_group(args, wt_file, subsample_num)
         df_wt['type'] = 'Sample'
         try:
@@ -85,39 +103,45 @@
             args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from current_events_magnifier.read_f5c_resquiggle import read_blow5
-        df_wt, aligned_num_wt = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand, subsample_num)
+
+        args.pos = args.pos + args.base_shift
+        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num)
         df_wt['type'] = 'Sample'
+        if nucleotide_type=='RNA' and not args.rna:
+            raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
-            df_ivt, aligned_num_ivt = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
+            df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
             df_ivt['type'] = 'Control'
 
             df = pd.concat([df_wt, df_ivt])
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
 
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
-    else:
-        raise Exception("Wrong work flow")
+
 
     category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
+
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
+    if args.function == 'f5c':
+        args.pos = args.pos - args.base_shift
     signal_plot(df, results_path, args.pos, base_list, title, 'merged')
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/extract_sub_fast5_from_bam.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/extract_sub_fast5_from_bam.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 #!/usr/bin/env python
 import pandas as pd
 import os
 import numpy as np
 from tqdm import tqdm
 import pysam
 import argparse
-# import shutil
+import shutil
+import time
 
 def create_result_folder(output_path):
+    print("Try to build generate the result path: "+output_path)
     if os.path.exists(output_path):
-        raise Exception("Folder exists. Please change the output folder...")
-        # print("Folder exists. Deleting folder...")
-        # shutil.rmtree(output_path)
-        # print("Folder deleted. Creating folder...")
-        # os.mkdir(output_path)
-        # print("Folder created.")
+        print("Folder exists. It will be overwrite after 5 secs ...")
+        time.sleep(5)
+        print("Deleting folder...")
+        shutil.rmtree(output_path)
+        print("Folder deleted. Creating folder...")
+        os.mkdir(output_path)
+        print("Folder created.")
     else:
         print("Creating output folder...")
         os.mkdir(output_path)
         print("Folder created.")
 
 def select_sub_reads(line):
     result = line[0].split("/")[-1].split(".")[0]
     return result
 
-def copy2new_path(line):
+def copy2new_path(line,results_path):
     global pbar
     fold_name = line[0].split('/')[-2]
-    if not os.path.exists(fold_name):
-        os.mkdir(fold_name)
-    os.system('cp ' + line[0] + ' ' + fold_name)
+    if not os.path.exists(results_path+'/single/'+fold_name):
+        os.mkdir(results_path+'/single/'+fold_name)
+    os.system('cp ' + line[0] + ' ' + results_path+'/single/'+fold_name)
     pbar.update(1)
 
 def transfer_fast5(total_fl, df,results_path):
     global pbar
     total_fl.columns=[0,'readname']
     df = df[['readname']]
     df[2] = '.'
@@ -41,18 +44,17 @@
     temp = pd.merge(total_fl, df, on='readname', how='inner')
 
     temp=temp.drop_duplicates(subset='readname')
     print("Start to extract "+str(temp.shape[0])+' reads ...')
     # temp=temp.sample(n=1544)
     pbar = tqdm(total=temp.shape[0], position=0, leave=True)
 
-    os.chdir(results_path)
-    os.mkdir('single/')
-    os.chdir('single/')
-    temp.apply(copy2new_path, axis=1)
+
+    os.mkdir(results_path+'/single/')
+    temp.apply(copy2new_path,results_path=results_path, axis=1)
     pbar.close()
 
 def main(args):
     fast5_path = args.fast5
     results_path = args.output
     sam_file=args.bam
     create_result_folder(results_path)
@@ -80,27 +82,27 @@
 
     print("Subsampling fast5 files ... ")
     total_fl = []
     for i in open(fast5_file, "r"):
         total_fl.append(i.rstrip())
     total_fl = pd.DataFrame(np.array(total_fl))
     total_fl[1] = total_fl.apply(select_sub_reads, axis=1)
-    transfer_fast5(total_fl, df,results_path)
+    transfer_fast5(total_fl, df, results_path)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-f","--fast5", required=True,
-                        help="fast5_path")
-    parser.add_argument('-b',"--bam", required=True,
-                        help="bam_path")
-    parser.add_argument('-o',"--output", default='subsample_single', help="output_file")
-    parser.add_argument("--chrom",help="Gene or chromosome name(head of your fasta file)")
-    parser.add_argument("--pos", type=int, help="site of your interest")
-    # parser.add_argument("-f","--fast5", default='/data/Ecoli_23s/data/L_rep2/single/',
+    # parser.add_argument("-f","--fast5", required=True,
     #                     help="fast5_path")
-    # parser.add_argument('-b',"--bam", default="/data/Ecoli_23s/data/L_rep2/file.bam",
+    # parser.add_argument('-b',"--bam", required=True,
     #                     help="bam_path")
-    # parser.add_argument('-o',"--output", default='/data/Ecoli_23s/data/L_rep2/subsample2', help="output_file")
-    # parser.add_argument("--chrom", default='NR_103073.1',help="Gene or chromosome name(head of your fasta file)")
-    # parser.add_argument("--pos", default=2029, type=int, help="site of your interest")
+    # parser.add_argument('-o',"--output", default='subsample_single', help="output_file")
+    # parser.add_argument("--chrom",help="Gene or chromosome name(head of your fasta file)")
+    # parser.add_argument("--pos", type=int, help="site of your interest")
+    parser.add_argument("-f","--fast5", default='/data/Ecoli_23s/data/L_rep2/single/',
+                        help="fast5_path")
+    parser.add_argument('-b',"--bam", default="/data/Ecoli_23s/data/L_rep2/file.bam",
+                        help="bam_path")
+    parser.add_argument('-o',"--output", default='/data/Ecoli_23s/data/L_rep2/subsample2', help="output_file")
+    parser.add_argument("--chrom", default='NR_103073.1',help="Gene or chromosome name(head of your fasta file)")
+    parser.add_argument("--pos", default=2029, type=int, help="site of your interest")
     args = parser.parse_args()
     main(args)
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 #         plot = plot + p9.labs(title=title, x=str(pos + 1), y=item)
 #         # plot.render_matplotlib()
 #         plot.save(filename=results_path + "/" + item + "_violin.pdf", dpi=300)
 # print(plot)
 
 def signal_plot(df, results_path, pos, base_list, title, plot_type):
     item_list = ['Mean', 'STD', 'Median', 'Dwell time']
+
+
     if plot_type != 'merged':
 
         for item in item_list:
             sig_min, sig_max = np.percentile(df[item], SIG_PCTL_RANGE)
             sig_diff = sig_max - sig_min
             ylim_tuple = (sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1)
 
@@ -94,24 +96,26 @@
                 raise Exception("Unsupported figure type!")
             # plot.render_matplotlib()
             if item == 'Dwell time':
                 item = 'Dwell_time'
             plot.save(filename=results_path + "/" + item + "_" + plot_type + ".pdf", dpi=300)
     else:
         new_df = None
+
+
         for item in item_list:
             # collect data
             temp = df[[item, 'position', 'type']].copy()
             temp.columns = ['value', 'position', 'type']
             temp.loc[:, 'stats'] = item
-
-            sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
-            sig_diff = sig_max - sig_min
-            ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
-            temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
+            # if df[df['position'] == pos].shape[0] > 50:
+            #     sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
+            #     sig_diff = sig_max - sig_min
+            #     ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
+            #     temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
             if new_df is None:
                 new_df = temp
             else:
                 new_df = pd.concat([new_df, temp], axis=0)
 
         plot = p9.ggplot(new_df, p9.aes(x='position', y="value", fill='type')) \
                + p9.theme_bw() \
@@ -129,20 +133,20 @@
         ) \
                + p9.facet_grid('stats ~', scales='free_y')
         plot = plot + p9.labs(title=title, x=str(pos + 1), y='')
 
         if new_df['type'].drop_duplicates().shape[0] == 1:
             plot2 = plot + p9.geom_violin(color='none', position=p9.position_dodge(0.9), width=1)
             plot2 = plot2 + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.1)
-            plot2.save(filename=results_path + "/merged_single.pdf", dpi=300)
+            plot2.save(filename=results_path + "/Merged_single.pdf", dpi=300)
         else:
-            plot1 = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.75)
-            plot1.save(filename=results_path + "/merged_boxplot.pdf", dpi=300)
-            plot2 = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5)
-            plot2.save(filename=results_path + "/merged_violin.pdf", dpi=300)
+            plot1 = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.75,alpha = 0.8)
+            plot1.save(filename=results_path + "/Merged_boxplot.pdf", dpi=300)
+            plot2 = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5,alpha = 0.8)
+            plot2.save(filename=results_path + "/Merged_violin.pdf", dpi=300)
 
 
 def draw_signal(df, start, base):
     df = pd.DataFrame(df)
     df.columns = ['raw']
     df = df.reset_index()
     plot = p9.ggplot(df, p9.aes(x='index', y="raw")) \
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import pyslow5
 import pysam
 from tqdm import tqdm
 from current_events_magnifier.normalization import normalize_signal,normalize_signal_with_lim
 import os
 import argparse
 score_dict={}
-
+nucleotide_type=None
 def extract_feature(line,strand):
+    global nucleotide_type
     pbar.update(1)
     read_id = line[0]
     # if read_id !='562eeb47-2b86-4fc7-abfc-5dce62f511ed':
     #     return None
     if read_id not in info_dict:
         return None
     # tackle moves tag
@@ -23,15 +24,14 @@
     moves_string = re.sub('I', 'I,', moves_string)
     # print(moves_string)
     moves = re.split(r',+', moves_string)
     moves = moves[:-1]
     # extract index and generate event_length and event_start
     insertion = 0
     event_length = []
-    offset = 0
     for i,item in enumerate(moves):
         if 'D' in item:
             deletion = int(item[:-1])
             for i in range(deletion):
                 event_length.append(0)
         elif 'I' in item:
             if i == 0 :
@@ -43,56 +43,72 @@
         else:
             event_length.append(int(item))
     # build event_length from move table
     read = s5.get_read(read_id, aux=["read_number", "start_mux"],pA=True)
     start_index = line[2]
     end_index = line[3]
     event_length = np.array(event_length)
+
+    # identify RNA or DNA
+    if nucleotide_type is None:
+        if line[7]>line[8]:
+            nucleotide_type='RNA'
+        else:
+            nucleotide_type='DNA'
     #  assert len_raw_signal in paf and blow5
     try:
         assert end_index-start_index == np.sum(event_length)
         assert read['len_raw_signal'] == line[1]
     except Exception:
         print("Warning: 1 read's length of signal is not equal between blow5 and paf")
         return None
 
     signal = read['signal']
 
     # create event start and flip all table
     signal = signal[start_index:end_index]
-    signal = np.flip(signal)
-    event_length = np.flip(event_length)
+    if nucleotide_type=='RNA':
+        signal = np.flip(signal)
+        event_length = np.flip(event_length)
+
     event_starts = event_length.cumsum()
     event_starts = np.insert(event_starts, 0, 0)[:-1]
 
     # filter too short or long dwell time
-    dwell_filter_pctls = (5, 95)
-    dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
-    valid_bases = np.logical_and.reduce(
-        (
-            event_length > dwell_min,
-            event_length < dwell_max,
-            np.logical_not(np.isnan(event_length)),
-        )
-    )
-    event_length[~valid_bases] = 0
+    # dwell_filter_pctls = (0.5, 99.5)
+    # dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
+    # valid_bases = np.logical_and.reduce(
+    #     (
+    #         event_length > dwell_min,
+    #         event_length < dwell_max,
+    #         np.logical_not(np.isnan(event_length)),
+    #     )
+    # )
+    # event_length[~valid_bases] = 0
 
     # normalized signal
     signal = normalize_signal_with_lim(signal)
 
     # index query and reference
     aligned_pair=info_dict[read_id]['pairs']
     qlen = info_dict[read_id]['query_length']
 
-    if strand =='+':
-        gap = qlen - event_length.shape[0]
-        aligned_pair[0] = aligned_pair[0] - gap
-        aligned_pair = aligned_pair[aligned_pair[0] >= 0]
+    if nucleotide_type == 'RNA':
+        if strand == '+':
+            gap = qlen - event_length.shape[0]
+            aligned_pair[0] = aligned_pair[0] - gap
+            aligned_pair = aligned_pair[aligned_pair[0] >= 0]
+        elif strand == '-':
+            aligned_pair[0] = event_length.shape[0]-aligned_pair[0]-1
     else:
-        aligned_pair[0] = event_length.shape[0]-aligned_pair[0]-1
+        if strand == '-':
+            aligned_pair[0] = qlen - aligned_pair[0] - 1
+        aligned_pair=aligned_pair[aligned_pair[0] <= event_length.shape[0]]
+
+
     if aligned_pair.shape[0]==0:
         return None
     read_pos = aligned_pair[0].values
     ref_pos = aligned_pair[1].values
 
     # extract raw signal by event length and event start
     total_feature_per_reads = []
@@ -115,16 +131,16 @@
 
     result_dict={}
     for read in bam_file.fetch(chromosome,position-length, position+length+1):
         if strand == '+' and read.is_reverse:
             continue
         if strand == '-' and not read.is_reverse:
             continue
-        # if read.qname == '4a4438ea-fc46-42aa-9788-8d54f37471b9':
-        #     print(1)
+        if read.qname == '5f8b9471-64e7-4dd8-b80c-5f88b77edbbe':
+            print(1)
         start_position=read.reference_start
         end_position=read.reference_end
         if position < start_position or position > end_position:
             continue
         # unit
         aligned_pair = np.array(read.aligned_pairs)
         aligned_pair = pd.DataFrame(aligned_pair)
@@ -141,14 +157,19 @@
 
 
 
 def read_blow5(path,position,length,chromo,strand,subsapmle_num=500):
     global info_dict,s5,pbar
     bam_file=path+".bam"
     bam_file=pysam.AlignmentFile(bam_file,'rb')
+    # if rna_mode:
+    #     if strand =='+':
+    #         position=position+ (kmer_model-1)
+    #     else:
+    #         position=position- (kmer_model-1)
     info_dict=extract_pairs_pos(bam_file,position,length,chromo,strand)
     if info_dict == {}:
         raise Exception("There is no read aligned on this position")
     slow5 = path+".blow5"
     s5 = pyslow5.Open(slow5, 'r')
 
     df=pd.read_csv(path+".paf",sep='\t',header=None)
@@ -160,17 +181,29 @@
     if subsapmle_num < df.shape[0]:
         df=df.sample(n=subsapmle_num)
     final_feature=[]
     for item in df["feature"]:
         final_feature.extend(item)
     final_feature=pd.DataFrame(final_feature)
     final_feature.columns=['Mean','STD','Median','Dwell time','position']
+    # if rna_mode:
+    #     if strand == '+':
+    #         final_feature['position']=final_feature['position'] - (kmer_model-1)
+    #     else:
+    #         final_feature['position']=final_feature['position'] + (kmer_model-1)
+
     final_feature['position'] = final_feature['position'].astype(int).astype(str)
-    print('\nextracted ', num_aligned, ' aligned reads from fast5 files')
-    return final_feature,num_aligned
+    print('\nextracted ', num_aligned, ' aligned reads from blow5 files')
+
+    if num_aligned>50:
+        dwell_filter_pctls = (0.5, 99.5)
+        dwell_min, dwell_max = np.percentile(final_feature['Dwell time'].values, dwell_filter_pctls)
+        final_feature = final_feature[(final_feature['Dwell time'] > dwell_min) & (final_feature['Dwell time'] < dwell_max)]
+
+    return final_feature,num_aligned,nucleotide_type
 
 # if __name__ == '__main__':
 #     parser = argparse.ArgumentParser()
 #     parser.add_argument("-i","--input", default='/data/Ecoli_23s/data/L_rep2/file',
 #                         help="blow5_path")
 #     parser.add_argument('-c',"--control", default='/data/Ecoli_23s/data/IVT_negative/file',
 #                         help="control_blow5_path")
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.9/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,71 +96,75 @@
         end=current_index + FLAG.len + 1
 
     seq_array = np.array(list(base))
     assert seq_array.shape == event_length.shape
     # uniq_arr = np.unique(signal)
     # signal = (signal - np.median(uniq_arr)) / float(robust.mad(uniq_arr))
     # normalization
-    signal = signal[event_start[0]:event_start[-1]+event_length[-1]]
-    event_start = event_start-event_start[0]
 
+    signal = signal[event_start[0]:event_start[-1] + event_length[-1]]
 
-    norm_signal=normalize_signal_with_lim(signal)
+    event_start = event_start-event_start[0]
+    signal = normalize_signal_with_lim(signal)
 
     # filter too short or long dwell time
-    dwell_filter_pctls = (5, 95)
-    dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
-    valid_bases = np.logical_and.reduce(
-        (
-            event_length > dwell_min,
-            event_length < dwell_max,
-            np.logical_not(np.isnan(event_length)),
-        )
-    )
-    event_length[~valid_bases]=0
+    # dwell_filter_pctls = (5, 95)
+    # dwell_min, dwell_max = np.percentile(event_length, dwell_filter_pctls)
+    # valid_bases = np.logical_and.reduce(
+    #     (
+    #         event_length > dwell_min,
+    #         event_length < dwell_max,
+    #         np.logical_not(np.isnan(event_length)),
+    #     )
+    # )
+    # event_length[~valid_bases]=0
+
 
     total_feature_per_reads = []
     # if end >=event_start.shape[0]:
     #     #print(1)
     # draw_signal(norm_signal[event_start[start]:event_start[end]], event_start[start:end] - event_start[start],
     #             base[start:end])
-    raw_signal_every = [norm_signal[event_start[start + x]:event_start[start + x] + event_length[start + x]] for x in range(end-start)]
+    raw_signal_every = [signal[event_start[start + x]:event_start[start + x] + event_length[start + x]] for x in range(end-start)]
 
     for i, element in enumerate(raw_signal_every):
         if event_length[start + i] == 0:
             continue
         if strand == '+':
             final_position = position - FLAG.len + i
         else:
             final_position = position + FLAG.len - i
         temp = [np.mean(element), np.std(element), np.median(element), event_length[start + i], final_position]
         total_feature_per_reads.append(temp)
     total_feature_per_reads=np.array(total_feature_per_reads)
     return total_feature_per_reads
 
-def extract_file(input_file):
+def extract_file(input_file,mode):
     basecall_group = FLAG.basecall_group
     basecall_subgroup = FLAG.basecall_subgroup
 
     chromosome = FLAG.chrom
     position = FLAG.pos
     strand = FLAG.strand
     try:
         temp_result = get_label_raw(input_file, basecall_group, basecall_subgroup,chromosome, position,strand)
         if temp_result is None:
             return None
         (raw_data, raw_label, raw_start, raw_length, start_position, strand,chrome) = temp_result
     except Exception as e:
         # print(str(e))
         return None
-    raw_data = raw_data[::-1]
+
+
     # ~ print(input_file,raw_start,raw_length,raw_label)
     total_seq = "".join([x.decode() for x in raw_label])
     base_len=raw_label.shape[0]
     end_position = start_position+base_len
+    if mode:
+        raw_data = np.flip(raw_data)
     matrix_feature = extract_feature(raw_data, raw_start, raw_length, total_seq,start_position,end_position,strand)
     if matrix_feature is None:
         return None
     del raw_data
 
     return matrix_feature
 
@@ -170,51 +174,63 @@
     FLAG=args
     # feature_matrix = np.zeros((1000000,40))
     results_list = []
     ##########
     pool = multiprocessing.Pool(processes=int(args.cpu))
     ##########
     for fl in total_fl:
-        result_per_read = pool.apply_async(extract_file, (fl,))
+        result_per_read = pool.apply_async(extract_file, (fl,args.rna))
         results_list.append(result_per_read)
     pool.close()
     ############################
     pbar = tqdm(total=len(total_fl), position=0, leave=True)
 
     result_list=[]
     for result_per_read in results_list:
         temp= result_per_read.get()
         if temp is not None:
             feature_per_read = temp
             result_list.append(feature_per_read)
 
-
             del  feature_per_read
         pbar.update(1)
     #############################
     pool.join()
     pbar.close()
 
-    aligned_num = len(result_list)
-    if subsapmle_num < aligned_num:
+    num_aligned = len(result_list)
+    if subsapmle_num < num_aligned:
         result_list=random.sample(result_list,subsapmle_num)
     final_feature=[]
     for item in result_list:
         final_feature.extend(item)
     df=pd.DataFrame(final_feature)
 
 
     if df.shape[0] == 0:
         raise Exception("can not find basecall_group or basecall_subgroup in fast5 files or there is no read aligned on the position")
-    print('\nextracted ',aligned_num,' aligned reads from fast5 files')
+    print('\nextracted ',num_aligned,' aligned reads from fast5 files')
     df.columns = ['Mean', 'STD', 'Median', 'Dwell time', 'position']
 
     # 转化为数值
     df['position'] = df['position'].astype(int).astype(str)
-    return df,aligned_num
+
+    if num_aligned > 50:
+        dwell_filter_pctls = (0.5, 99.5)
+        dwell_min, dwell_max = np.percentile(df['Dwell time'].values, dwell_filter_pctls)
+        df = df[(df['Dwell time'] > dwell_min) & (df['Dwell time'] < dwell_max)]
+        df.reset_index(inplace=True,drop=True)
+    #     item_list = ['Mean', 'STD']
+    #     for item in item_list:
+    #         # collect data
+    #         dwell_filter_pctls = (2.5, 97.5)
+    #         dwell_min, dwell_max = np.percentile(df[item].values, dwell_filter_pctls)
+    #         df = df[(df[item] > dwell_min) & (df[item] < dwell_max)]
+    #         df.reset_index(inplace=True,drop=True)
+    return df,num_aligned
 
 
 def create_read_list_file(path,results_path):
     if path[-1] == '/':
         path = path[:-1]
     total_fl = []
     os.system("find " + path + " -name \"*.fast5\" >" + results_path + "/files.txt")
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: current-events-magnifier
-Version: 0.0.3.8
+Name: current_events_magnifier
+Version: 0.0.3.9
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,30 +17,24 @@
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
-## Still developing
-### TO do list
-1. More normalization methods (finished)
-2. Test on minus strand or reversed strand (finished)
-3. Subsample coverage (finished)
-4. single mode(finished)
-5. merge images together(finished)
-6. test data to github(finished)
+
 ## Before start, you should know
 ### What is re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 ![alt text](example/data_format.png)
+
 In our program, we assume that the input provided by the user is in the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 
 ## Installation
 Requirement : Python >=3.7, <3.10
 
@@ -100,52 +94,52 @@
 # assumed your fast5 file folder name is fast5/
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
-So for the following command , I used ```--chrom NR_103073.1  --pos A2030 --strand +```
-### 1. F5c resquiggle (v1.2)
+So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
+### 1. F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
 1. Data format conversion.
 ```sh
 slow5tools f2s fast5/ -d blow5_dir
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-f5c resquiggle -c final.fastq file.blow5 -o file.paf
+f5c resquiggle -c all.fastq file.blow5 -o file.paf
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
+CE_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta 
 ```
 ### 2. Tombo resquiggle (v1.5.0)
 Step 1 and 3 should run on your two sample respectively, before the step 4.
 1. Data format conversion.
 ```sh
 # assumed your fast5 file folder name is fast5/
-multi_to_single_fast5 -i fast5/ -o single/ --recursive -t 16
+multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 ```
 2. Subsample (Optional)
 
 Because Tombo resquiggle runs very slowly, it heavily relies on the read and write speed of SSD hard drives. Therefore, it is recommended to extract the aligned reads in advance.
 After obtaining the single-format fast5 files and bam files , we provide a script that can assist you with this.
 ```sh
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 3. Run tombo resquiggle
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames all.fastq --processes 16 
@@ -153,14 +147,14 @@
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 4. Run current_events_magnifier to plot
 ```sh
-python CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
+CE_magnifier.py tombo -i sample1/single -c sample2/single -o tombo_result --chrom NR_103073.1 --strand + --pos 2030 --len 5 --cpu 4 --ref reference.fasta
 ```
```

### Comparing `current_events_magnifier-0.0.3.8/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.8/setup.py` & `current_events_magnifier-0.0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.8",
+    version="0.0.3.9",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -23,11 +23,12 @@
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.23.0',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
-        "pyslow5>=1.0.0"
+        "pyslow5>=1.0.0",
+        "vbz_h5py_plugin>=1.0.1"
     ],
     scripts=['current_events_magnifier/CE_magnifier.py','current_events_magnifier/extract_sub_fast5_from_bam.py']
 )
```

