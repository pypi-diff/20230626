# Comparing `tmp/ncOrtho-0.4.2.tar.gz` & `tmp/ncOrtho-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncOrtho-0.4.2.tar", last modified: Thu Jun 15 12:51:35 2023, max compression
+gzip compressed data, was "ncOrtho-0.4.3.tar", last modified: Mon Jun 26 13:04:27 2023, max compression
```

## Comparing `ncOrtho-0.4.2.tar` & `ncOrtho-0.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.522214 ncOrtho-0.4.2/
--rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.4.2/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:51:35.520216 ncOrtho-0.4.2/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)     6480 2023-03-09 13:27:30.000000 ncOrtho-0.4.2/README.md
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.184236 ncOrtho-0.4.2/ncOrtho/
--rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.4.2/ncOrtho/__init__.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.332226 ncOrtho-0.4.2/ncOrtho/analysis/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.4.2/ncOrtho/analysis/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.4.2/ncOrtho/analysis/concat_alignments_dmp.pl
--rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.4.2/ncOrtho/analysis/degapper.pl
--rw-r--r--   0 felixl   (10024) users      (501)    11977 2023-03-09 15:33:35.000000 ncOrtho-0.4.2/ncOrtho/analysis/ncAnalyze.py
--rw-r--r--   0 felixl   (10024) users      (501)     7691 2023-06-13 14:46:25.000000 ncOrtho-0.4.2/ncOrtho/blastparser.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.394221 ncOrtho-0.4.2/ncOrtho/check/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.4.2/ncOrtho/check/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     8997 2023-03-08 09:37:40.000000 ncOrtho-0.4.2/ncOrtho/check/core_synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.4.2/ncOrtho/check/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)    12394 2023-06-14 11:24:43.000000 ncOrtho-0.4.2/ncOrtho/cmsearch.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.465222 ncOrtho-0.4.2/ncOrtho/coreset/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.4.2/ncOrtho/coreset/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6840 2023-06-14 15:25:46.000000 ncOrtho-0.4.2/ncOrtho/coreset/core_reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     9936 2023-06-15 12:36:54.000000 ncOrtho-0.4.2/ncOrtho/coreset/coreset.py
--rw-r--r--   0 felixl   (10024) users      (501)     8473 2023-04-27 13:13:52.000000 ncOrtho-0.4.2/ncOrtho/coreset/coreset_utils.py
--rw-r--r--   0 felixl   (10024) users      (501)     3813 2023-06-14 15:25:46.000000 ncOrtho-0.4.2/ncOrtho/coreset/createcm.py
--rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.4.2/ncOrtho/coreset/example_parameters.yaml
--rw-r--r--   0 felixl   (10024) users      (501)     7002 2023-06-14 14:54:01.000000 ncOrtho-0.4.2/ncOrtho/coreset/locate_position.py
--rw-r--r--   0 felixl   (10024) users      (501)     5065 2023-03-20 09:25:58.000000 ncOrtho-0.4.2/ncOrtho/coreset/synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)     1966 2023-06-15 12:50:42.000000 ncOrtho-0.4.2/ncOrtho/genparser.py
--rwxr-xr-x   0 felixl   (10024) users      (501)    16818 2023-06-15 12:50:42.000000 ncOrtho-0.4.2/ncOrtho/ncortho.py
--rw-r--r--   0 felixl   (10024) users      (501)     1806 2023-06-15 12:50:42.000000 ncOrtho-0.4.2/ncOrtho/reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     3749 2023-06-14 11:24:43.000000 ncOrtho-0.4.2/ncOrtho/rna_object.py
--rw-r--r--   0 felixl   (10024) users      (501)      989 2023-06-15 12:25:12.000000 ncOrtho-0.4.2/ncOrtho/utils.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:51:35.274232 ncOrtho-0.4.2/ncOrtho.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      847 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)      176 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       34 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        8 2023-06-15 12:51:35.000000 ncOrtho-0.4.2/ncOrtho.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.4.2/pyproject.toml
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-15 12:51:35.523213 ncOrtho-0.4.2/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)     1979 2023-06-15 12:50:42.000000 ncOrtho-0.4.2/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:27.324881 ncOrtho-0.4.3/
+-rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.4.3/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-26 13:04:27.322873 ncOrtho-0.4.3/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)     6480 2023-03-09 13:27:30.000000 ncOrtho-0.4.3/README.md
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:26.918908 ncOrtho-0.4.3/ncOrtho/
+-rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.4.3/ncOrtho/__init__.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:27.108902 ncOrtho-0.4.3/ncOrtho/analysis/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.4.3/ncOrtho/analysis/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.4.3/ncOrtho/analysis/concat_alignments_dmp.pl
+-rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.4.3/ncOrtho/analysis/degapper.pl
+-rw-r--r--   0 felixl   (10024) users      (501)    12491 2023-06-22 12:16:56.000000 ncOrtho-0.4.3/ncOrtho/analysis/ncAnalyze.py
+-rw-r--r--   0 felixl   (10024) users      (501)     7691 2023-06-13 14:46:25.000000 ncOrtho-0.4.3/ncOrtho/blastparser.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:27.181883 ncOrtho-0.4.3/ncOrtho/check/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.4.3/ncOrtho/check/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8997 2023-03-08 09:37:40.000000 ncOrtho-0.4.3/ncOrtho/check/core_synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.4.3/ncOrtho/check/tmp.py
+-rw-r--r--   0 felixl   (10024) users      (501)    12870 2023-06-22 14:14:08.000000 ncOrtho-0.4.3/ncOrtho/cmsearch.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:27.316879 ncOrtho-0.4.3/ncOrtho/coreset/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.4.3/ncOrtho/coreset/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6877 2023-06-20 10:01:08.000000 ncOrtho-0.4.3/ncOrtho/coreset/core_reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     9934 2023-06-26 11:29:34.000000 ncOrtho-0.4.3/ncOrtho/coreset/coreset.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8477 2023-06-26 11:22:46.000000 ncOrtho-0.4.3/ncOrtho/coreset/coreset_utils.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3813 2023-06-14 15:25:46.000000 ncOrtho-0.4.3/ncOrtho/coreset/createcm.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.4.3/ncOrtho/coreset/example_parameters.yaml
+-rw-r--r--   0 felixl   (10024) users      (501)     7002 2023-06-14 14:54:01.000000 ncOrtho-0.4.3/ncOrtho/coreset/locate_position.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5065 2023-03-20 09:25:58.000000 ncOrtho-0.4.3/ncOrtho/coreset/synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1966 2023-06-15 12:50:42.000000 ncOrtho-0.4.3/ncOrtho/genparser.py
+-rwxr-xr-x   0 felixl   (10024) users      (501)    16887 2023-06-22 14:03:39.000000 ncOrtho-0.4.3/ncOrtho/ncortho.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1806 2023-06-15 12:50:42.000000 ncOrtho-0.4.3/ncOrtho/reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3750 2023-06-20 09:56:39.000000 ncOrtho-0.4.3/ncOrtho/rna_object.py
+-rw-r--r--   0 felixl   (10024) users      (501)      989 2023-06-15 12:25:12.000000 ncOrtho-0.4.3/ncOrtho/utils.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-26 13:04:27.022908 ncOrtho-0.4.3/ncOrtho.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      847 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      176 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       34 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        8 2023-06-26 13:04:26.000000 ncOrtho-0.4.3/ncOrtho.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.4.3/pyproject.toml
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-26 13:04:27.325876 ncOrtho-0.4.3/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)     1979 2023-06-20 09:53:24.000000 ncOrtho-0.4.3/setup.py
```

### Comparing `ncOrtho-0.4.2/LICENSE` & `ncOrtho-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/PKG-INFO` & `ncOrtho-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.4.2
+Version: 0.4.3
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.4.2/README.md` & `ncOrtho-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/analysis/concat_alignments_dmp.pl` & `ncOrtho-0.4.3/ncOrtho/analysis/concat_alignments_dmp.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/analysis/degapper.pl` & `ncOrtho-0.4.3/ncOrtho/analysis/degapper.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/analysis/ncAnalyze.py` & `ncOrtho-0.4.3/ncOrtho/analysis/ncAnalyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import tempfile
 import subprocess as sp
 import sys
 import shutil
 import inspect
 from collections import Counter
 import argparse
+from pyfiglet import Figlet
+from importlib.metadata import version
 
 """
 Species in spec_to_skip will not be part of multiple sequence alignments
 """
 
 
 def make_supermatrix(out):
@@ -68,21 +70,14 @@
             if len(mature) < 7:
                 raise ValueError('No mature sequence found in "ncrna_file"')
             seed = mature[1:8]
             m2s[mirid] = seed
     return m2s
 
 def main():
-    # Print header
-    print('\n'+'#'*39)
-    print('###'+' '*33+'###')
-    print('###   Analysis of ncOrtho results   ###')
-    print('###'+' '*33+'###')
-    print('#'*39+'\n')
-    sys.stdout.flush()
 
     # Parse command-line arguments
     # Define global variables
     parser = argparse.ArgumentParser(
         description='Analzye ncOrtho results. Gives: PhyloProfile input, supermatrix alignment, species tree.'
     )
     parser._action_groups.pop()
@@ -124,16 +119,16 @@
             'miRNAs were detected from species tree calculation. '
             '(e.g. --auto_skip 0.5 means that only species in which at least 50%% '
             'of the reference miRNAs were found are used for species tree calculation) (Default: Off)'
         )
     )
     optional.add_argument(
         '--iqtree', metavar='str', type=str, nargs='?',
-        const='iqtree -s {} -bb 1000 -alrt 1000 -nt AUTO -redo -pre {}/species_tree',
-        default='iqtree -s {} -bb 1000 -alrt 1000 -nt AUTO -redo -pre {}/species_tree',
+        const='',
+        default='',
         help=(
             'Call to iqtree. Do not change curly bracket notation '
             '(Default: iqtree -s {} -bb 1000 -alrt 1000 -nt AUTO -redo -pre {}/{})'
         )
     )
     optional.add_argument(
         '--mirnas', metavar='<path>', type=str, nargs='?', const='', default='',
@@ -143,14 +138,20 @@
     )
     # mirna data
     optional.add_argument(
         '--ncrna_file', metavar='<path>', nargs='?', const='', default='',
         help='Path to tab separated file of reference miRNAs information, as used in ncCreate and ncSearch. '
              'Uses mature sequence column to identify seed conservation.'
     )
+
+    # print header
+    custom_fig = Figlet(font='stop')
+    print(custom_fig.renderText('ncOrtho')[:-3], flush=True)
+    v = version('ncOrtho')
+    print(f'Version: {v}\n', flush=True)
     ##########################################################################################
     # Parse arguments
     ##########################################################################################
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
     else:
@@ -166,15 +167,14 @@
     overlap = set(spec_to_skip).intersection(set(spec_include))
     if overlap:
         raise ValueError(f'"{overlap}" present in species to skip as well as species to include')
 
 
     mirlist = arglistcheck(args.mirnas)
 
-    iqtree_cmd = args.iqtree
     auto_skip = args.auto_skip
 
     if args.ncrna_file:
         mirid2seed = parse_matseq(args.ncrna_file)
     else:
         mirid2seed = {}
     ##########################################################################################
@@ -261,37 +261,51 @@
 
     # make alignments
     print('# Starting alignments')
     align_out = f'{outdir}/alignments'
     if not os.path.isdir(align_out):
         os.mkdir(align_out)
     for mirna in ortho_dict:
+        # tmplist = []
+        if len(ortho_dict[mirna]) < 2:  # need at least 2 sequences for alignment
+            with open(f'{align_out}/{mirna}.aln', 'w') as of:
+                for spec, seq in ortho_dict[mirna].items():
+                    of.write(f'>{spec}\n{seq}\n')
+            continue
         with tempfile.NamedTemporaryFile(mode='w+') as fp:
             for spec, seq in ortho_dict[mirna].items():
                 if spec_to_skip:
                     if (
                             spec in spec_to_skip
                             and spec not in spec_include
                     ):
                         continue
                 fp.write(f'>{spec}\n{seq}\n')
+                # tmplist.append(f'>{spec}\n{seq}\n')
             fp.seek(0)
             aln_cmd = f'muscle -align {fp.name} -output {align_out}/{mirna}.aln'
             res = sp.run(aln_cmd, shell=True, capture_output=True)
             if res.returncode != 0:
+                # with open(f'{outdir}/faulty_{mirna}.fa', 'w') as of:
+                    # for line in tmplist:
+                    #     of.write(line)
                 print(res.stderr.decode('utf8'))
                 sys.exit()
 
     sys.stdout.flush()
     superm_path = make_supermatrix(outdir)
     print('# Starting tree calculation')
     tree_out = f'{outdir}/species_tree'
     if not os.path.isdir(tree_out):
         os.mkdir(tree_out)
-    tree_cmd = iqtree_cmd.format(superm_path, tree_out)
+
+    if not args.iqtree:
+        tree_cmd = f'iqtree -s {superm_path} -bb 1000 -alrt 1000 -nt AUTO -redo -pre {tree_out}/species_tree'
+    else:
+        tree_cmd = args.iqtree
     res = sp.run(tree_cmd, shell=True, capture_output=True)
     print(res.stdout.decode('utf-8'))
     if res.returncode != 0:
         print(res.stderr.decode('utf-8'))
 
     # write tree that can be used as optional phyloprofile input
     treepath = f'{tree_out}/species_tree.contree'
```

### Comparing `ncOrtho-0.4.2/ncOrtho/blastparser.py` & `ncOrtho-0.4.3/ncOrtho/blastparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/check/core_synteny.py` & `ncOrtho-0.4.3/ncOrtho/check/core_synteny.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/check/tmp.py` & `ncOrtho-0.4.3/ncOrtho/check/tmp.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/cmsearch.py` & `ncOrtho-0.4.3/ncOrtho/cmsearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,14 +133,27 @@
         if err:
             raise sp.SubprocessError(err)
         results = parse_cm(res)
 
     return results
 
 
+def parse_cmsearch(cm_results):
+    logger = logging.getLogger('ncortho')
+    logger.setLevel(level=logging.DEBUG)
+    return_data = []
+    for data in cm_results:
+        score = float(data[3])
+        chrom = data[5]
+        start, end = map(int, data[6:8])
+        strand = data[8]
+        return_data.append([chrom, start, end, strand, score])
+    return return_data
+
+
 def parse_cmsearch_for_heuristic(cm_results, extraregion=1000):
     logger = logging.getLogger('ncortho')
     logger.setLevel(level=logging.DEBUG)
     return_data = []
     for data in cm_results:
         # parse CMsearch output of candidate regions to acutal genomic regions
         blast_chrom = data[5].split('|')[0]
@@ -149,15 +162,15 @@
         blast_strand = data[5].split('|')[3]
         cm_start, cm_end = map(int, data[6:8])
         # cm_start, cm_end = map(int, data[5:7])
         cm_strand = data[8]
         if cm_strand == '-':
             # reverse hits should not be possible since blasthits were extracted
             # as reverse complement if they were on the minus strand
-            logger.info('Unexpected hit of CMsearch')
+            # logger.info('Unexpected hit of CMsearch')
             continue
         if hit_at_start == 'True':
             # print(f'# cmsearch hit for {rna_id} at the beginning of a chromosome in the query species')
             hit_start = cm_start
             hit_end = cm_end
         elif hit_at_end == 'True':
             # print(f'# cmsearch hit for {rna_id} at the end of a chromosome in the query species')
@@ -167,15 +180,15 @@
             hit_start = blast_start + (cm_start - extraregion) - 1
             hit_end = hit_start + (cm_end - extraregion) - 1
         # fill output variable
         return_data.append([blast_chrom, hit_start, hit_end, blast_strand, float(data[3])])
     return return_data
 
 
-def cmsearch_parser(cms, cmc, lc, rna):
+def remove_duplicates_apply_cutoffs(cms, cmc, lc, rna):
     """
     Parse the output of cmsearch while eliminating duplicates and filtering
     entries according to the defined cutoff.
 
     Parameters
     ----------
     cms     :   List with CMsearch hits [chrom, start, end, strand, score]
@@ -190,14 +203,15 @@
     """
     # Output
     hits_dict = {}
     # Required for finding duplicates, stores hits per chromosome
     chromo_dict = {}
 
     for candidate_nr, hit in enumerate(cms, 1):
+        # print(hit)
         h_chrom, h_start, h_end, h_strand, h_score = hit
         # blastparser expects the start to be the smaller number, will extract reverse complement if on - strand
         if h_start > h_end:
             h_start, h_end = h_end, h_start
         length = h_end - h_start
 
         if length <= length * lc:
@@ -290,19 +304,20 @@
             cm_results = perform_model_search(models, rna, candidate_region_fasta, out, cm_cutoff, cpu, phmm)
             cm_results = parse_cmsearch_for_heuristic(cm_results)
 
         if cleanup:
             os.remove(candidate_region_fasta)
     else:
         cm_results = perform_model_search(models, rna, query, out, cm_cutoff, cpu, phmm)
+        cm_results = parse_cmsearch(cm_results)
 
     if not cm_results:
         return False, 'No CMsearch results in candidate regions or query genome'
 
-    parsed_cm_results = cmsearch_parser(cm_results, cm_cutoff, msl, rna)
+    parsed_cm_results = remove_duplicates_apply_cutoffs(cm_results, cm_cutoff, msl, rna)
     if not parsed_cm_results:
         return False, 'No CMsearch results above threshold'
     else:
         return parsed_cm_results, 'Sucess'
```

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/core_reblast.py` & `ncOrtho-0.4.3/ncOrtho/coreset/core_reblast.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     -------
     Path to Alignment of core pre-miRNAs in Stockholm format
 
     """
 
     mirid, rawchrom, mstart, mend, mstrand, rawseq = mirna[:6]
     mchr = rawchrom.replace('chr', '')
-    preseq = rawseq.replace('U', 'T')
+    preseq = rawseq.replace('U', 'T').replace('-', '')
 
     miroutdir = f'{o_path}/{mirid}'
     if not os.path.isdir(miroutdir):
         os.mkdir(miroutdir)
     synteny_regs = f'{miroutdir}/synteny_regions_{mirid}.fa'  # this fasta file is created by the the main() script
     os.chdir(miroutdir)
 
@@ -116,15 +116,15 @@
         'sseqid evalue bitscore sseq\"'.format(c, dust, synteny_regs)
     )
     blastn = sp.Popen(
         blastn_cmd, shell=True, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
     )
     ortholog_candidates, err = blastn.communicate(preseq)
     if err:
-        raise err
+        raise sp.SubprocessError(err)
 
     # Re-BLAST
     outputcol = {}
     seq_check = set()
     ortholog_candidates_list = ortholog_candidates.split('\n')
     vprint(f'Number of ortholog candidates: {len(ortholog_candidates_list)}', v)
     for hit in ortholog_candidates_list:
```

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/coreset.py` & `ncOrtho-0.4.3/ncOrtho/coreset/coreset.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         '--create_model', metavar='yes/no', type=str,
         help='set to "no" if you only want to create the alignment. (Default: yes)', nargs='?',
         const='yes', default='yes'
     )
     optional.add_argument(
         '--phmm', metavar='yes/no', type=str,
         help='set to "yes" if you want to create a pHMM instead of a CM (Default: no)', nargs='?',
-        const='yes', default='yes'
+        const='no', default='no'
     )
     optional.add_argument(
         '--rcoffee', metavar='yes/no', type=str,
         help='set to "no" to use default "t_coffee" instead of "r_coffee" (Default: yes)', nargs='?',
         const='yes', default='yes'
     )
     optional.add_argument(
```

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/coreset_utils.py` & `ncOrtho-0.4.3/ncOrtho/coreset/coreset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                 od[cspec][refprot].append(orthoprot)
     return od
 
 
 def read_mirnas(path):
     with open(path) as mirfile:
         mirnas = [
-            line.split() for line in mirfile.readlines()
+            line.split('\t') for line in mirfile.readlines()
             if not line.startswith('#')
         ]
     # print('Done')
     return mirnas
 
 
 def mirna_position(mirlist):
```

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/createcm.py` & `ncOrtho-0.4.3/ncOrtho/coreset/createcm.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/example_parameters.yaml` & `ncOrtho-0.4.3/ncOrtho/coreset/example_parameters.yaml`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/locate_position.py` & `ncOrtho-0.4.3/ncOrtho/coreset/locate_position.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/coreset/synteny.py` & `ncOrtho-0.4.3/ncOrtho/coreset/synteny.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/genparser.py` & `ncOrtho-0.4.3/ncOrtho/genparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/ncortho.py` & `ncOrtho-0.4.3/ncOrtho/ncortho.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         # check if qblast exists
         if not check_blastdb(qblast):
             raise ValueError('# Query BLASTdb not found at: {}'.format(qblast))
     elif heuristic[0]:
         qblast = qlink
         # check if already exists
         if not check_blastdb(qlink):
-            print('# Creating query Database')
+            print('# Creating query Database', flush=True)
             make_blastndb(query, qlink)
 
     ###############################################################################################
     # Main
     ###############################################################################################
 
     # Print out query
@@ -356,15 +356,16 @@
             if len(cm_results) > max_hits:
                 logger.warning('# Maximum CMsearch hits reached. Restricting to best {} hits'.format(max_hits))
                 cm_results = {k: cm_results[k] for k in list(cm_results.keys())[:max_hits]}
                 restricted = True
         # get sequences for each CM result
         gp = GenomeParser(qlink, cm_results.values())
         candidates = gp.extract_sequences()
-        logger.info('Covariance model search successful, found 1 ortholog candidate(s).')
+        # print(candidates)
+        logger.info(f'Covariance model search successful, found {len(candidates)} ortholog candidate(s).')
 
         # Perform reverse BLAST test to verify candidates, stored in
         reblast_hits = {}
         for candidate in candidates:
             sequence = candidates[candidate]
             if list(sequence).count('N') >= 0.9 * len(sequence):
                 continue
@@ -416,13 +417,13 @@
         shortlog.append(f'{mirna}\t{elapsed_time}\tSUCESS\n')
         sucess_count += 1
 
     write_output(mirna_orthologs, f'{output}/{qname}_orthologs.fa')
     write_output(shortlog, f'{output}/{qname}_summary.log')
     # logging.basicConfig(filename=f'{output}/{qname}_extended.log', level=logging.DEBUG)
 
-    print(f'\n### ncOrtho found orthologs for {sucess_count} out of {len(mirna_dict)} ncRNAs')
+    print(f'\n### ncOrtho found orthologs for {sucess_count} out of {len(mirna_dict)} ncRNAs', flush=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ncOrtho-0.4.2/ncOrtho/reblast.py` & `ncOrtho-0.4.3/ncOrtho/reblast.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho/rna_object.py` & `ncOrtho-0.4.3/ncOrtho/rna_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
             resline = reslist[i+2]
             topscore = float(resline.split()[1])
             return topscore
     # if no results return topscore 0
     logger.info('Self bit score not applicable, setting threshold to 0')
     return 0.0
 
+
 def rna_maker(mirpath, modeldir, phmm, cpu):
     logger = logging.getLogger('ncortho')
     logger.setLevel(level=logging.DEBUG)
     """
     Parses the miRNA data input file and returns a dictionary of Mirna objects.
 
     mirpath : Path to file with microRNA data.
```

### Comparing `ncOrtho-0.4.2/ncOrtho/utils.py` & `ncOrtho-0.4.3/ncOrtho/utils.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/ncOrtho.egg-info/PKG-INFO` & `ncOrtho-0.4.3/ncOrtho.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.4.2
+Version: 0.4.3
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.4.2/ncOrtho.egg-info/SOURCES.txt` & `ncOrtho-0.4.3/ncOrtho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.2/setup.py` & `ncOrtho-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncOrtho",
-    version="0.4.2",
+    version="0.4.3",
     python_requires='>=3.7.0',
     description=" Targeted ortholog search for miRNAs ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     url="https://github.com/felixlangschied/ncortho",
```

