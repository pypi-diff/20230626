# Comparing `tmp/virheat-0.3.tar.gz` & `tmp/virheat-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virheat-0.3.tar", last modified: Mon Jun  5 16:52:41 2023, max compression
+gzip compressed data, was "virheat-0.4.tar", last modified: Mon Jun 26 13:21:45 2023, max compression
```

## Comparing `virheat-0.3.tar` & `virheat-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 16:52:41.322300 virheat-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 16:52:20.000000 virheat-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:52:41.322300 virheat-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 16:52:20.000000 virheat-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.318300 virheat-0.3/virheat/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 16:52:20.000000 virheat-0.3/virheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 16:52:20.000000 virheat-0.3/virheat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-05 16:52:20.000000 virheat-0.3/virheat/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/virheat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-05 16:52:20.000000 virheat-0.3/virheat/scripts/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:52:41.322300 virheat-0.3/virheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 16:52:41.000000 virheat-0.3/virheat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:45.462178 virheat-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-26 13:21:45.462178 virheat-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-26 13:21:19.000000 virheat-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:21:45.462178 virheat-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 13:21:19.000000 virheat-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:45.458178 virheat-0.4/virheat/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 13:21:19.000000 virheat-0.4/virheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 13:21:19.000000 virheat-0.4/virheat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-26 13:21:19.000000 virheat-0.4/virheat/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:45.462178 virheat-0.4/virheat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:19.000000 virheat-0.4/virheat/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-06-26 13:21:19.000000 virheat-0.4/virheat/scripts/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-26 13:21:19.000000 virheat-0.4/virheat/scripts/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:45.462178 virheat-0.4/virheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 13:21:45.000000 virheat-0.4/virheat.egg-info/top_level.txt
```

### Comparing `virheat-0.3/PKG-INFO` & `virheat-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.3
+Version: 0.4
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -72,14 +72,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -l None, --genome-length None
                         length of the genome (needed if gff3 is not provided)
   -g None, --gff3-path None
                         path to gff3 (needed if length is not provided)
+  -a gene, --gff3-annotations gene
+                        annotations to display from gff3 file (standard: gene)
   -t 0, --threshold 0   display frequencies above this threshold
   --delete, --no-delete
                         delete mutations with frequencies present in all
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
```

### Comparing `virheat-0.3/README.md` & `virheat-0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -l None, --genome-length None
                         length of the genome (needed if gff3 is not provided)
   -g None, --gff3-path None
                         path to gff3 (needed if length is not provided)
+  -a gene, --gff3-annotations gene
+                        annotations to display from gff3 file (standard: gene)
   -t 0, --threshold 0   display frequencies above this threshold
   --delete, --no-delete
                         delete mutations with frequencies present in all
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
```

### Comparing `virheat-0.3/setup.py` & `virheat-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `virheat-0.3/virheat/command.py` & `virheat-0.4/virheat/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,22 @@
         "--gff3-path",
         type=str,
         metavar="None",
         default=None,
         help="path to gff3 (needed if length is not provided)"
     )
     parser.add_argument(
+        "-a",
+        "--gff3-annotations",
+        type=str,
+        metavar="gene",
+        default="gene",
+        help="annotations to display from gff3 file (standard: gene). Multiple possible (comma seperated)"
+    )
+    parser.add_argument(
         "-t",
         "--threshold",
         type=float,
         metavar="0",
         default=0,
         help="display frequencies above this threshold"
     )
@@ -113,25 +121,26 @@
         sys.exit("\033[31m\033[1mERROR:\033[0m Do not provide the -g and -l argument simultaneously!")
     elif args.gff3_path is not None:
         gff3_info, gff3_ref_name = data_prep.parse_gff3(args.gff3_path)
         # issue a warning if #CHROM and gff3 do not match
         if gff3_ref_name not in reference_name and reference_name not in gff3_ref_name:
             print("\033[31m\033[WARNING:\033[0m gff3 reference does not match the vcf reference!")
         genome_end = data_prep.get_genome_end(gff3_info)
-        genes_with_mutations, n_tracks = data_prep.create_track_dict(unique_mutations, gff3_info)
+        annotation_list = args.gff3_annotations.split(",")
+        genes_with_mutations, n_tracks = data_prep.create_track_dict(unique_mutations, gff3_info, annotation_list)
         # define space for the genome vis tracks
         min_y_location = genome_y_location + genome_y_location/2 * (n_tracks+1)
     elif args.genome_length is not None:
         genome_end = args.genome_length
         min_y_location = genome_y_location
     else:
         sys.exit("\033[31m\033[1mERROR:\033[0m Provide either a gff3 file (-g) or the length (-l) of the genome which you used for mapping")
 
     # define size of the plot
-    y_size = (n_mutations)*0.4
+    y_size = n_mutations*0.4
     x_size = y_size*(n_samples+min_y_location)/n_mutations
     x_size = x_size-x_size*0.15  # compensate of heatmap annotation
 
     # ini the fig
     fig, ax = plt.subplots(figsize=[y_size, x_size])
 
     # plot all elements
@@ -141,15 +150,15 @@
     if args.gff3_path is not None:
         # distinct colors for the genes
         cmap_genes = plt.get_cmap('tab20', len(genes_with_mutations))
         colors_genes = [cmap_genes(i) for i in range(len(genes_with_mutations))]
         # plot gene track
         plotting.create_gene_vis(ax, genes_with_mutations, n_mutations, y_size, n_tracks, genome_end, min_y_location, genome_y_location, colors_genes)
     plotting.create_axis(ax, n_mutations, min_y_location, n_samples, file_names, genome_end, genome_y_location, unique_mutations, reference_name)
-    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples, n_mutations)
+    plotting.create_colorbar(args.threshold, cmap_cells, min_y_location, n_samples)
     plotting.create_mutation_legend(mutation_set, min_y_location, n_samples)
 
     # create output folder
     if not os.path.exists(args.input[1]):
         os.makedirs(args.input[1])
 
     # save fig
```

### Comparing `virheat-0.3/virheat/scripts/data_prep.py` & `virheat-0.4/virheat/scripts/data_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 contains all data prep functions of virHEAT
 """
 
 # BUILT-INS
 import os
 import re
 import pathlib
+import sys
 
 # LIBS
 import numpy as np
 
 
 def get_vcf_files(path):
     """
@@ -87,15 +88,15 @@
         visited_keys.append("TYPE")
         # get data from info field
         for info in line[7].split(";"):
             if "=" in info:
                 key, val = info.split("=")
                 vcf_dict[key].append(convert_string(val))
                 visited_keys.append(key)
-        # append none for ech none vistited key
+        # append none for ech none visited key
         for key in [k for k in vcf_dict.keys() if k not in visited_keys]:
             vcf_dict[key].append(None)
 
     return vcf_dict
 
 
 def extract_vcf_data(vcf_files, threshold=0):
@@ -195,15 +196,14 @@
                     gff3_dict[gff_values[2]][attribute_id] = {}
                 # add attributes
                 if identifier != "ID":
                     gff3_dict[gff_values[2]][attribute_id][identifier] = val.replace("\n", "")
             # add start, stop and strand
             gff3_dict[gff_values[2]][attribute_id]["start"] = int(gff_values[3])
             gff3_dict[gff_values[2]][attribute_id]["stop"] = int(gff_values[4])
-            gff3_dict[gff_values[2]][attribute_id]["strand"] = gff_values[6]
 
     gff3_file.close()
 
     return gff3_dict, gff3_ref_name
 
 
 def get_genome_end(gff3_dict):
@@ -217,34 +217,42 @@
         stop = gff3_dict["region"][attribute]["stop"]
         if stop > genome_end:
             genome_end = stop
 
     return genome_end
 
 
-def create_track_dict(unique_mutations, gff3_info):
+def create_track_dict(unique_mutations, gff3_info, annotation_type):
     """
     create a dictionary of the genes that have mutations and assess in which
     track these genes should go in case they overlap
     """
 
     # find genes that have a mutation
     genes_with_mutations = set()
 
     for mutation in unique_mutations:
         # get the mutation from string
         mutation = int(mutation.split("_")[0])
-        for gene_name in gff3_info["gene"]:
-            if mutation in range(gff3_info["gene"][gene_name]["start"], gff3_info["gene"][gene_name]["stop"]):
-                genes_with_mutations.add(
-                    (gff3_info["gene"][gene_name]["gene"],
-                     gff3_info["gene"][gene_name]["start"],
-                     gff3_info["gene"][gene_name]["stop"],
-                     gff3_info["gene"][gene_name]["strand"])
-                )
+        for type in annotation_type:
+            if type not in gff3_info.keys():
+                continue
+            for annotation in gff3_info[type]:
+                if mutation in range(gff3_info[type][annotation]["start"], gff3_info[type][annotation]["stop"]):
+                    if "Name" in gff3_info[type][annotation].keys():
+                        attribute_name = gff3_info[type][annotation]["Name"]
+                    else:
+                        attribute_name = annotation
+                    genes_with_mutations.add(
+                        (attribute_name,
+                         gff3_info[type][annotation]["start"],
+                         gff3_info[type][annotation]["stop"])
+                    )
+    if not genes_with_mutations:
+        sys.exit("none of the given annotation types were found in gff3.")
 
     # create a dict and sort
     gene_dict = {element[0]: [element[1:4]] for element in genes_with_mutations}
     gene_dict = dict(sorted(gene_dict.items(), key=lambda x: x[1][0]))
 
     # remember for each track the largest stop
     track_stops = [0]
```

### Comparing `virheat-0.3/virheat/scripts/plotting.py` & `virheat-0.4/virheat/scripts/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         coordinates = [(x_start, 0), (x_start+1, 0), (mutation_x_location, y_max)]
         ax.add_patch(patches.Polygon(coordinates, facecolor=mutation_color, alpha=0.5))
         x_start += 1
 
     return mutation_set
 
 
-def create_colorbar(threshold, cmap, min_y_location, n_samples, n_mutations):
+def create_colorbar(threshold, cmap, min_y_location, n_samples):
     """
     creates a custom colorbar and annotates the threshold
     """
     if n_samples >= 8:
         ticks = [0, 0.2, 0.4, 0.6, 0.8, 1]
         labels = [0, 0.2, 0.4, 0.6, 0.8, 1]
         if threshold + 0.1 in ticks or threshold - 0.1 in ticks:
```

### Comparing `virheat-0.3/virheat.egg-info/PKG-INFO` & `virheat-0.4/virheat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virheat
-Version: 0.3
+Version: 0.4
 Summary: virHEAT creates a heatmap from vcf files and maps positions onto a reference genome.
 Home-page: https://github.com/jonas-fuchs/virHEAT
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -72,14 +72,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -l None, --genome-length None
                         length of the genome (needed if gff3 is not provided)
   -g None, --gff3-path None
                         path to gff3 (needed if length is not provided)
+  -a gene, --gff3-annotations gene
+                        annotations to display from gff3 file (standard: gene)
   -t 0, --threshold 0   display frequencies above this threshold
   --delete, --no-delete
                         delete mutations with frequencies present in all
                         samples (default: True)
   --sort, --no-sort     sort alphanumerically (default: False)
   -v, --version         show program's version number and exit
 ```
```

