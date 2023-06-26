# Comparing `tmp/current_events_magnifier-0.0.3.9.tar.gz` & `tmp/current_events_magnifier-0.0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.9.tar", last modified: Mon Jun 26 10:53:55 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.4.0.tar", last modified: Mon Jun 26 14:39:15 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.9.tar` & `current_events_magnifier-0.0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.9/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7433 2023-06-20 08:13:10.000000 current_events_magnifier-0.0.3.9/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7115 2023-06-26 10:50:21.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8825 2023-06-26 10:38:38.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-06-23 06:41:12.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7734 2023-06-26 08:43:23.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10227 2023-06-26 10:42:38.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13861 2023-06-26 10:18:43.000000 current_events_magnifier-0.0.3.9/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-26 10:53:54.000000 current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-26 10:53:55.014340 current_events_magnifier-0.0.3.9/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1191 2023-06-26 10:53:36.000000 current_events_magnifier-0.0.3.9/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.4.0/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7433 2023-06-20 08:13:10.000000 current_events_magnifier-0.0.4.0/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7526 2023-06-26 14:34:21.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9229 2023-06-26 14:26:04.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-06-23 06:41:12.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7734 2023-06-26 08:43:23.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10227 2023-06-26 10:42:38.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13861 2023-06-26 10:18:43.000000 current_events_magnifier-0.0.4.0/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-26 14:39:15.439794 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8051 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      655 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-26 14:39:15.000000 current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-26 14:39:15.443795 current_events_magnifier-0.0.4.0/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1191 2023-06-26 14:38:54.000000 current_events_magnifier-0.0.4.0/setup.py
```

### Comparing `current_events_magnifier-0.0.3.9/LICENSE` & `current_events_magnifier-0.0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/PKG-INFO` & `current_events_magnifier-0.0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.3.9
+Version: 0.0.4.0
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.9/README.md` & `current_events_magnifier-0.0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
-    parser_f5c.add_argument('--base_shift',type=int, default=0, help="base shift of f5c")
+    parser_f5c.add_argument('--base_shift',type=int, default=0, help="base shift if required")
     add_public_argument(parser_f5c)
+
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
 
@@ -103,16 +104,20 @@
             args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from current_events_magnifier.read_f5c_resquiggle import read_blow5
-
-        args.pos = args.pos + args.base_shift
+        if args.base_shift < 0:
+            raise RuntimeError("base_shift should not less than 0")
+        if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
+            args.pos = args.pos + args.base_shift
+        else:
+            args.pos = args.pos - args.base_shift
         df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
@@ -136,12 +141,15 @@
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
     if args.function == 'f5c':
-        args.pos = args.pos - args.base_shift
+        if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
+            args.pos = args.pos - args.base_shift
+        else:
+            args.pos = args.pos + args.base_shift
     signal_plot(df, results_path, args.pos, base_list, title, 'merged')
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/CE_magnifier_test.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/CE_magnifier_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     #                     ref="/data/Ecoli_23s/23S_rRNA.fasta",\
     #                     basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
     parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
                         control='/data/Ecoli_23s/data/IVT_negative/file',\
                         output='f5c_result_rna',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA.fasta",rna=True,base_shift=2)
     # parser.set_defaults(function='f5c', chrom="1", pos=150280972, len=10, strand='+', cpu=4,input='/data/current_test_data/samp/cem_test_dna/WGS/file',\
     #                     control='/data/current_test_data/samp/cem_test_dna/WGA/file',\
-    #                     output='f5c_result_dna',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=-2)
+    #                     output='f5c_result_dna',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=2)
 
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
@@ -118,16 +118,20 @@
             args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from current_events_magnifier.read_f5c_resquiggle import read_blow5
-
-        args.pos = args.pos + args.base_shift
+        if args.base_shift < 0:
+            raise RuntimeError("base_shift should not less than 0")
+        if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
+            args.pos = args.pos + args.base_shift
+        else:
+            args.pos = args.pos - args.base_shift
         df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
@@ -151,12 +155,15 @@
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
     if args.function == 'f5c':
-        args.pos = args.pos - args.base_shift
+        if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
+            args.pos = args.pos - args.base_shift
+        else:
+            args.pos = args.pos + args.base_shift
     signal_plot(df, results_path, args.pos, base_list, title, 'merged')
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/extract_sub_fast5_from_bam.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.4.0/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.3.9
+Version: 0.0.4.0
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.9/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.4.0/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.9/setup.py` & `current_events_magnifier-0.0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.9",
+    version="0.0.4.0",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

