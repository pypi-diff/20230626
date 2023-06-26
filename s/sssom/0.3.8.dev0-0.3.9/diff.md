# Comparing `tmp/sssom-0.3.8.dev0.tar.gz` & `tmp/sssom-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssom-0.3.8.dev0.tar", last modified: Fri Feb 25 20:21:29 2022, max compression
+gzip compressed data, was "sssom-0.3.9.tar", last modified: Fri Apr 29 13:03:26 2022, max compression
```

## Comparing `sssom-0.3.8.dev0.tar` & `sssom-0.3.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-02-25 20:21:29.657459 sssom-0.3.8.dev0/
--rw-r--r--   0 HHegde     (502) staff       (20)     6555 2021-04-29 13:02:34.000000 sssom-0.3.8.dev0/LICENSE
--rw-r--r--   0 HHegde     (502) staff       (20)      614 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/MANIFEST.in
--rw-r--r--   0 HHegde     (502) staff       (20)     4207 2022-02-25 20:21:29.657595 sssom-0.3.8.dev0/PKG-INFO
--rw-r--r--   0 HHegde     (502) staff       (20)     2807 2022-02-07 20:23:31.000000 sssom-0.3.8.dev0/README.md
--rw-r--r--   0 HHegde     (502) staff       (20)      251 2021-09-24 13:57:01.000000 sssom-0.3.8.dev0/pyproject.toml
--rw-r--r--   0 HHegde     (502) staff       (20)     2548 2022-02-25 20:21:29.658444 sssom-0.3.8.dev0/setup.cfg
--rw-r--r--   0 HHegde     (502) staff       (20)      119 2021-12-08 20:45:44.000000 sssom-0.3.8.dev0/setup.py
-drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-02-25 20:21:29.655055 sssom-0.3.8.dev0/sssom/
--rw-r--r--   0 HHegde     (502) staff       (20)      306 2022-01-03 16:05:39.000000 sssom-0.3.8.dev0/sssom/__init__.py
--rw-r--r--   0 HHegde     (502) staff       (20)      320 2022-01-03 16:11:21.000000 sssom-0.3.8.dev0/sssom/__main__.py
--rw-r--r--   0 HHegde     (502) staff       (20)    14486 2022-02-07 15:35:28.000000 sssom-0.3.8.dev0/sssom/cli.py
--rw-r--r--   0 HHegde     (502) staff       (20)     6755 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/cliques.py
--rw-r--r--   0 HHegde     (502) staff       (20)    13823 2021-08-31 14:01:39.000000 sssom-0.3.8.dev0/sssom/cliquesummary.py
--rw-r--r--   0 HHegde     (502) staff       (20)      138 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/constants.py
--rw-r--r--   0 HHegde     (502) staff       (20)     4709 2022-02-07 15:35:28.000000 sssom-0.3.8.dev0/sssom/context.py
--rw-r--r--   0 HHegde     (502) staff       (20)    92602 2022-02-14 20:39:14.000000 sssom-0.3.8.dev0/sssom/external_context.py
--rw-r--r--   0 HHegde     (502) staff       (20)     5020 2022-02-14 20:39:14.000000 sssom-0.3.8.dev0/sssom/internal_context.py
--rw-r--r--   0 HHegde     (502) staff       (20)     4893 2022-02-25 20:18:28.000000 sssom-0.3.8.dev0/sssom/io.py
--rw-r--r--   0 HHegde     (502) staff       (20)    27021 2022-02-07 15:17:03.000000 sssom-0.3.8.dev0/sssom/parsers.py
--rw-r--r--   0 HHegde     (502) staff       (20)     2912 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/rdf_util.py
--rw-r--r--   0 HHegde     (502) staff       (20)     3876 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/sparql_util.py
--rw-r--r--   0 HHegde     (502) staff       (20)     4528 2022-02-14 20:39:14.000000 sssom-0.3.8.dev0/sssom/sssom.context.jsonld
--rw-r--r--   0 HHegde     (502) staff       (20)    92447 2022-02-14 20:39:14.000000 sssom-0.3.8.dev0/sssom/sssom.external.context.jsonld
--rw-r--r--   0 HHegde     (502) staff       (20)    18803 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/sssom.yaml
--rw-r--r--   0 HHegde     (502) staff       (20)    37280 2022-02-14 20:39:14.000000 sssom-0.3.8.dev0/sssom/sssom_datamodel.py
--rw-r--r--   0 HHegde     (502) staff       (20)     1155 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/sssom_document.py
--rw-r--r--   0 HHegde     (502) staff       (20)      414 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/typehints.py
--rw-r--r--   0 HHegde     (502) staff       (20)    34001 2022-02-24 01:26:50.000000 sssom-0.3.8.dev0/sssom/util.py
--rw-r--r--   0 HHegde     (502) staff       (20)    10273 2021-12-21 15:28:54.000000 sssom-0.3.8.dev0/sssom/writers.py
-drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-02-25 20:21:29.657239 sssom-0.3.8.dev0/sssom.egg-info/
--rw-r--r--   0 HHegde     (502) staff       (20)     4207 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/PKG-INFO
--rw-r--r--   0 HHegde     (502) staff       (20)      691 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/SOURCES.txt
--rw-r--r--   0 HHegde     (502) staff       (20)        1 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/dependency_links.txt
--rw-r--r--   0 HHegde     (502) staff       (20)       42 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/entry_points.txt
--rw-r--r--   0 HHegde     (502) staff       (20)        1 2021-05-03 14:21:44.000000 sssom-0.3.8.dev0/sssom.egg-info/not-zip-safe
--rw-r--r--   0 HHegde     (502) staff       (20)      268 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/requires.txt
--rw-r--r--   0 HHegde     (502) staff       (20)       12 2022-02-25 20:21:29.000000 sssom-0.3.8.dev0/sssom.egg-info/top_level.txt
+drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-04-29 13:03:26.248669 sssom-0.3.9/
+-rw-r--r--   0 HHegde     (502) staff       (20)     6555 2021-04-29 13:02:34.000000 sssom-0.3.9/LICENSE
+-rw-r--r--   0 HHegde     (502) staff       (20)      614 2021-12-21 15:28:54.000000 sssom-0.3.9/MANIFEST.in
+-rw-r--r--   0 HHegde     (502) staff       (20)     4202 2022-04-29 13:03:26.248803 sssom-0.3.9/PKG-INFO
+-rw-r--r--   0 HHegde     (502) staff       (20)     2807 2022-02-07 20:23:31.000000 sssom-0.3.9/README.md
+-rw-r--r--   0 HHegde     (502) staff       (20)      251 2021-09-24 13:57:01.000000 sssom-0.3.9/pyproject.toml
+-rw-r--r--   0 HHegde     (502) staff       (20)     2632 2022-04-29 13:03:26.249633 sssom-0.3.9/setup.cfg
+-rw-r--r--   0 HHegde     (502) staff       (20)      119 2021-12-08 20:45:44.000000 sssom-0.3.9/setup.py
+drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-04-29 13:03:26.246802 sssom-0.3.9/sssom/
+-rw-r--r--   0 HHegde     (502) staff       (20)      337 2022-04-07 19:38:49.000000 sssom-0.3.9/sssom/__init__.py
+-rw-r--r--   0 HHegde     (502) staff       (20)      320 2022-01-03 16:11:21.000000 sssom-0.3.9/sssom/__main__.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    16168 2022-04-29 12:57:49.000000 sssom-0.3.9/sssom/cli.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     6755 2021-12-21 15:28:54.000000 sssom-0.3.9/sssom/cliques.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    13823 2021-08-31 14:01:39.000000 sssom-0.3.9/sssom/cliquesummary.py
+-rw-r--r--   0 HHegde     (502) staff       (20)      471 2022-04-07 19:38:08.000000 sssom-0.3.9/sssom/constants.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     4709 2022-03-17 15:58:24.000000 sssom-0.3.9/sssom/context.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    92602 2022-03-07 15:54:50.000000 sssom-0.3.9/sssom/external_context.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     5020 2022-02-14 20:39:14.000000 sssom-0.3.9/sssom/internal_context.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     4893 2022-02-25 20:18:28.000000 sssom-0.3.9/sssom/io.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    27240 2022-04-29 12:57:49.000000 sssom-0.3.9/sssom/parsers.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     2912 2021-12-21 15:28:54.000000 sssom-0.3.9/sssom/rdf_util.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     3876 2021-12-21 15:28:54.000000 sssom-0.3.9/sssom/sparql_util.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     4528 2022-02-14 20:39:14.000000 sssom-0.3.9/sssom/sssom.context.jsonld
+-rw-r--r--   0 HHegde     (502) staff       (20)    92447 2022-02-14 20:39:14.000000 sssom-0.3.9/sssom/sssom.external.context.jsonld
+-rw-r--r--   0 HHegde     (502) staff       (20)    18803 2022-04-12 21:32:00.000000 sssom-0.3.9/sssom/sssom.yaml
+-rw-r--r--   0 HHegde     (502) staff       (20)    37280 2022-02-14 20:39:14.000000 sssom-0.3.9/sssom/sssom_datamodel.py
+-rw-r--r--   0 HHegde     (502) staff       (20)     1155 2021-12-21 15:28:54.000000 sssom-0.3.9/sssom/sssom_document.py
+-rw-r--r--   0 HHegde     (502) staff       (20)      414 2021-12-21 15:28:54.000000 sssom-0.3.9/sssom/typehints.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    41113 2022-04-29 12:57:49.000000 sssom-0.3.9/sssom/util.py
+-rw-r--r--   0 HHegde     (502) staff       (20)    10273 2022-03-10 00:47:53.000000 sssom-0.3.9/sssom/writers.py
+drwxr-xr-x   0 HHegde     (502) staff       (20)        0 2022-04-29 13:03:26.248467 sssom-0.3.9/sssom.egg-info/
+-rw-r--r--   0 HHegde     (502) staff       (20)     4202 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/PKG-INFO
+-rw-r--r--   0 HHegde     (502) staff       (20)      691 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/SOURCES.txt
+-rw-r--r--   0 HHegde     (502) staff       (20)        1 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/dependency_links.txt
+-rw-r--r--   0 HHegde     (502) staff       (20)       42 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/entry_points.txt
+-rw-r--r--   0 HHegde     (502) staff       (20)        1 2021-05-03 14:21:44.000000 sssom-0.3.9/sssom.egg-info/not-zip-safe
+-rw-r--r--   0 HHegde     (502) staff       (20)      268 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/requires.txt
+-rw-r--r--   0 HHegde     (502) staff       (20)       12 2022-04-29 13:03:26.000000 sssom-0.3.9/sssom.egg-info/top_level.txt
```

### Comparing `sssom-0.3.8.dev0/LICENSE` & `sssom-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/MANIFEST.in` & `sssom-0.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/PKG-INFO` & `sssom-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssom
-Version: 0.3.8.dev0
+Version: 0.3.9
 Summary: Operations on SSSOM mapping tables
 Home-page: https://github.com/mapping-commons/sssom
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Maintainer: Chris Mungall
 Maintainer-email: cjmungall@lbl.gov
 License: MIT
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: sssom Version: 0.3.8.dev0 Summary: Operations on
-SSSOM mapping tables Home-page: https://github.com/mapping-commons/sssom
-Author: Chris Mungall Author-email: cjmungall@lbl.gov Maintainer: Chris Mungall
+Metadata-Version: 2.1 Name: sssom Version: 0.3.9 Summary: Operations on SSSOM
+mapping tables Home-page: https://github.com/mapping-commons/sssom Author:
+Chris Mungall Author-email: cjmungall@lbl.gov Maintainer: Chris Mungall
 Maintainer-email: cjmungall@lbl.gov License: MIT Download-URL: https://
 github.com/mapping-commons/sssom-py/releases Project-URL: Bug Tracker, https://
 github.com/mapping-commons/sssom-py/issues Project-URL: Source Code, https://
 github.com/mapping-commons/sssom-py/ Project-URL: Documentation, https://
 mapping-commons.github.io/sssom-py Keywords: Ontologies,Indexing,Ontology
 Mapping Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
```

### Comparing `sssom-0.3.8.dev0/README.md` & `sssom-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/setup.cfg` & `sssom-0.3.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sssom
-version = 0.3.8-dev
+version = 0.3.9
 description = Operations on SSSOM mapping tables
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mapping-commons/sssom
 download_url = https://github.com/mapping-commons/sssom-py/releases
 project_urls = 
 	Bug Tracker = https://github.com/mapping-commons/sssom-py/issues
@@ -101,14 +101,15 @@
 	def __repr__
 
 [flake8]
 ignore = 
 	E501 # Line length
 	W503 # Line break before binary operator (flake8 is wrong)
 	S408 # don't worry about unsafe xml
+	S324 # Use of weak MD4, MD5, or SHA1 hash for security. Consider usedforsecurity=False
 	S318 # don't worry about unsafe xml
 	S310 # TODO remove this later and switch to using requests
 	B018 # This is 'useless' statements which are new atm.
 exclude = 
 	sssom/sssom_datamodel.py
 	sssom/cliquesummary.py
```

### Comparing `sssom-0.3.8.dev0/sssom/cli.py` & `sssom-0.3.9/sssom/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - When you import __main__ it will get executed again (as a module) because
   there's no ``sssom.__main__`` in ``sys.modules``.
 
 .. seealso:: https://click.palletsprojects.com/en/8.0.x/setuptools/
 """
 
 import logging
+import os
 import re
 import sys
 from pathlib import Path
 from typing import Dict, List, TextIO, Tuple
 
 import click
 import pandas as pd
@@ -34,15 +35,17 @@
     SSSOM_READ_FORMATS,
     MappingSetDataFrame,
     collapse,
     compare_dataframes,
     dataframe_to_ptable,
     filter_redundant_rows,
     merge_msdf,
+    reconcile_prefix_and_data,
     remove_unmatched,
+    sort_df_rows_columns,
     to_mapping_set_dataframe,
 )
 from .writers import write_table
 
 # Click input options common across commands
 input_argument = click.argument("input", required=True, type=click.Path())
 
@@ -64,25 +67,26 @@
     help=f'Desired output format, e.g. {",".join(SSSOM_EXPORT_FORMATS)}',
 )
 output_directory_option = click.option(
     "-d",
     "--output-directory",
     type=click.Path(),
     help="Output directory path.",
+    default=os.getcwd(),
 )
 metadata_option = click.option(
     "-m",
     "--metadata",
     required=False,
     type=click.Path(),
     help="The path to a file containing the sssom metadata (including prefix_map) to be used.",
 )
-transpose_option = click.option("-t", "--transpose/--no-transpose", default=False)
+transpose_option = click.option("-t", "--transpose", default=False)
 fields_option = click.option(
-    "-F",
+    "-f",
     "--fields",
     nargs=2,
     default=("subject_category", "object_category"),
     help="Fields.",
 )
 
 
@@ -188,15 +192,15 @@
     )
     msdf = read_sssom_table(input)
     # df = parse(input)
     df = collapse(msdf.df)
     # , priors=list(priors)
     rows = dataframe_to_ptable(df)
     for row in rows:
-        print(row, sep="\t", file=output)
+        print(*row, sep="\t", file=output)
 
 
 @main.command()
 @input_argument
 @output_option
 def dedupe(input: str, output: TextIO):
     """Remove lower confidence duplicate lines from an SSSOM file."""
@@ -207,15 +211,15 @@
         df=df, prefix_map=msdf.prefix_map, metadata=msdf.metadata
     )
     # df.to_csv(output, sep="\t", index=False)
     write_table(msdf_out, output)
 
 
 @main.command()
-@click.option("-q", "--query", help='SQL query. Use "df" as table name.')
+@click.option("-Q", "--query", help='SQL query. Use "df" as table name.')
 @click.argument("inputs", nargs=-1)
 @output_option
 def dosql(query: str, inputs: List[str], output: TextIO):
     """Run a SQL query over one or more SSSOM files.
 
     Each of the N inputs is assigned a table name df1, df2, ..., dfN
 
@@ -227,24 +231,30 @@
 
     Example:
         `sssom dosql -q "SELECT file1.*,file2.object_id AS ext_object_id, file2.object_label AS ext_object_label \
         FROM file1 INNER JOIN file2 WHERE file1.object_id = file2.subject_id" FROM file1.sssom.tsv file2.sssom.tsv`
     """  # noqa: DAR101
     # should start with from_tsv and MOST should return write_sssom
     n = 1
+    new_msdf = MappingSetDataFrame()
     while len(inputs) >= n:
         fn = inputs[n - 1]
-        df = read_sssom_table(fn).df
+        msdf = read_sssom_table(fn)
+        df = msdf.df
         # df = parse(fn)
         globals()[f"df{n}"] = df
         tn = re.sub("[.].*", "", Path(fn).stem).lower()
         globals()[tn] = df
         n += 1
-    df = sqldf(query)
-    df.to_csv(output, sep="\t", index=False)
+
+    new_df = sqldf(query)
+    new_msdf.df = new_df
+    new_msdf.prefix_map = msdf.prefix_map
+    new_msdf.metadata = msdf.metadata
+    write_table(new_msdf, output)
 
 
 @main.command()
 @click.option("-c", "--config", type=click.File("rb"))
 @click.option("-e", "--url")
 @click.option("-g", "--graph")
 @click.option(
@@ -414,15 +424,15 @@
     for t in tups:
         print(f"{t[0]}\t{t[1]}\t{t[2]}")
 
 
 @main.command()
 @click.argument("inputs", nargs=-1)
 @click.option(
-    "-r",
+    "-R",
     "--reconcile",
     default=True,
     help="Boolean indicating the need for reconciliation of the SSSOM tsv file.",
 )
 @output_option
 def merge(inputs: str, output: TextIO, reconcile: bool = True):
     """Merge multiple MappingSetDataFrames into one .
@@ -430,15 +440,14 @@
     if reconcile=True, then dedupe(remove redundant lower confidence mappings) and
     reconcile (if msdf contains a higher confidence _negative_ mapping,
     then remove lower confidence positive one. If confidence is the same,
     prefer HumanCurated. If both HumanCurated, prefer negative mapping).
     """  # noqa: DAR101
     msdfs = [read_sssom_table(i) for i in inputs]
     merged_msdf = merge_msdf(*msdfs, reconcile=reconcile)
-    # Export MappingSetDataFrame into a TSV
     write_table(merged_msdf, output)
 
 
 @main.command()
 @input_argument
 @click.option("-m", "--mapping-file", help="Path to SSSOM file.")
 @click.option("-I", "--input-format", default="turtle", help="Ontology input format.")
@@ -464,13 +473,65 @@
 
     # noqa: DAR101
     """
     msdf = read_sssom_table(mapping_file)
     g = Graph()
     g.parse(input, format=input_format)
     rewire_graph(g, msdf, precedence=precedence)
-    rdfstr = g.serialize(format=output_format).decode()
+    rdfstr = g.serialize(format=output_format)
     print(rdfstr, file=output)
 
 
+@main.command()
+@input_argument
+@click.option(
+    "-p",
+    "--reconcile-prefix-file",
+    help="Provide YAML file with prefix reconciliation information.",
+)
+@output_option
+def reconcile_prefixes(input: str, reconcile_prefix_file: Path, output: TextIO):
+    """
+    Reconcile prefix_map based on provided YAML file.
+
+    :param input: MappingSetDataFrame filename
+    :param reconcile_prefix_file: YAML file containing the prefix reconcilation rules.
+    :param output: Target file path.
+    """
+    msdf = read_sssom_table(input)
+    with open(reconcile_prefix_file, "rb") as rp_file:
+        rp_dict = yaml.safe_load(rp_file)
+    recon_msdf = reconcile_prefix_and_data(msdf, rp_dict)
+    write_table(recon_msdf, output)
+
+
+@main.command()
+@input_argument
+@output_option
+@click.option(
+    "-k",
+    "--by-columns",
+    default=True,
+    help="Sort columns of DataFrame canonically.",
+)
+@click.option(
+    "-r",
+    "--by-rows",
+    default=True,
+    help="Sort rows by DataFrame column #1 (ascending).",
+)
+def sort(input: str, output: TextIO, by_columns: bool, by_rows: bool):
+    """
+    Sort DataFrame columns canonically.
+
+    :param input: SSSOM TSV file.
+    :param by_columns: Boolean flag to sort columns canonically.
+    :param by_rows: Boolean flag to sort rows by column #1 (ascending order).
+    :param output: SSSOM TSV file with columns sorted.
+    """
+    msdf = read_sssom_table(input)
+    msdf.df = sort_df_rows_columns(msdf.df, by_columns, by_rows)
+    write_table(msdf, output)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `sssom-0.3.8.dev0/sssom/cliques.py` & `sssom-0.3.9/sssom/cliques.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/cliquesummary.py` & `sssom-0.3.9/sssom/cliquesummary.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/context.py` & `sssom-0.3.9/sssom/context.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/external_context.py` & `sssom-0.3.9/sssom/external_context.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/internal_context.py` & `sssom-0.3.9/sssom/internal_context.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/io.py` & `sssom-0.3.9/sssom/io.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/parsers.py` & `sssom-0.3.9/sssom/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import numpy as np
 import pandas as pd
 import validators
 import yaml
 from linkml_runtime.loaders.json_loader import JSONLoader
 from rdflib import Graph, URIRef
 
+from sssom.constants import MAPPING_SET_SLOTS, MAPPING_SLOTS
+
 from .context import (
     DEFAULT_LICENSE,
     DEFAULT_MAPPING_SET_ID,
     add_built_in_prefixes_to_prefix_map,
     get_default_metadata,
 )
 from .sssom_datamodel import Mapping, MappingSet
@@ -71,15 +73,14 @@
                     logging.info(
                         f"Externally provided metadata {k}:{v} is added to metadata set."
                     )
                     sssom_metadata[k] = v
         meta = sssom_metadata
 
     prefix_map, meta = _get_prefix_map_and_metadata(prefix_map=prefix_map, meta=meta)
-
     msdf = from_sssom_dataframe(df, prefix_map=prefix_map, meta=meta)
     return msdf
 
 
 def read_sssom_rdf(
     file_path: str,
     prefix_map: Dict[str, str] = None,
@@ -169,44 +170,46 @@
         # IF k is multivalued, then v = List[values]
         return [s.strip() for s in v.split("|")]
     else:
         return v
 
 
 def _init_mapping_set(meta: Optional[MetadataType]) -> MappingSet:
+    license = DEFAULT_LICENSE
+    mapping_set_id = DEFAULT_MAPPING_SET_ID
     if meta is not None:
-        return MappingSet(
-            mapping_set_id=meta["mapping_set_id"], license=meta["license"]
-        )
-    else:
-        return MappingSet(
-            mapping_set_id=DEFAULT_MAPPING_SET_ID, license=DEFAULT_LICENSE
-        )
+        if "mapping_set_id" in meta.keys():
+            mapping_set_id = meta["mapping_set_id"]
+        if "license" in meta.keys():
+            license = meta["license"]
+    return MappingSet(mapping_set_id=mapping_set_id, license=license)
 
 
 def _get_mdict_ms_and_bad_attrs(
     row: pd.Series, ms: MappingSet, bad_attrs: Counter
 ) -> Tuple[dict, MappingSet, Counter]:
 
     mdict = {}
+
     for k, v in row.items():
         if v and v == v:
             ok = False
             if k:
                 k = str(k)
             v = _address_multivalued_slot(k, v)
-            if hasattr(Mapping, k):
+            # if hasattr(Mapping, k):
+            if k in MAPPING_SLOTS:
                 mdict[k] = v
                 ok = True
-            if hasattr(MappingSet, k):
+            # if hasattr(MappingSet, k):
+            if k in MAPPING_SET_SLOTS:
                 ms[k] = v
                 ok = True
             if not ok:
                 bad_attrs[k] += 1
-
     return (mdict, ms, bad_attrs)
 
 
 def read_alignment_xml(
     file_path: str, prefix_map: Dict[str, str], meta: Dict[str, str]
 ) -> MappingSetDataFrame:
     """Parse a TSV -> MappingSetDocument -> MappingSetDataFrame."""
@@ -244,15 +247,14 @@
 
     mlist: List[Mapping] = []
     ms = _init_mapping_set(meta)
     bad_attrs: typing.Counter[str] = Counter()
     for _, row in df.iterrows():
         mdict, ms, bad_attrs = _get_mdict_ms_and_bad_attrs(row, ms, bad_attrs)
         mlist.append(_prepare_mapping(Mapping(**mdict)))
-
     for k, v in bad_attrs.most_common():
         logging.warning(f"No attr for {k} [{v} instances]")
     # the autogenerated code's type annotations are _really_ messy. This is in fact okay,
     # so with a heavy heart we employ type:ignore
     ms.mappings = mlist  # type:ignore
     _set_metadata_in_mapping_set(mapping_set=ms, metadata=meta)
     doc = MappingSetDocument(mapping_set=ms, prefix_map=prefix_map)
```

### Comparing `sssom-0.3.8.dev0/sssom/rdf_util.py` & `sssom-0.3.9/sssom/rdf_util.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sparql_util.py` & `sssom-0.3.9/sssom/sparql_util.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sssom.context.jsonld` & `sssom-0.3.9/sssom/sssom.context.jsonld`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sssom.external.context.jsonld` & `sssom-0.3.9/sssom/sssom.external.context.jsonld`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sssom.yaml` & `sssom-0.3.9/sssom/sssom.yaml`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sssom_datamodel.py` & `sssom-0.3.9/sssom/sssom_datamodel.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/sssom_document.py` & `sssom-0.3.9/sssom/sssom_document.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom/util.py` & `sssom-0.3.9/sssom/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 import numpy as np
 import pandas as pd
 import validators
 import yaml
 from linkml_runtime.linkml_model.types import Uriorcurie
 
-from .constants import SCHEMA_YAML
+from .constants import SCHEMA_DICT, SCHEMA_YAML
 from .context import SSSOM_URI_PREFIX, get_default_metadata, get_jsonld_context
 from .internal_context import multivalued_slots
 from .sssom_datamodel import Mapping as SSSOM_Mapping
-from .sssom_datamodel import MatchTypeEnum, PredicateModifierEnum, slots
+from .sssom_datamodel import slots
 from .sssom_document import MappingSetDocument
 from .typehints import Metadata, MetadataType, PrefixMap
 
 #: The key that's used in the YAML section of an SSSOM file
 PREFIX_MAP_KEY = "curie_map"
 
 SSSOM_READ_FORMATS = [
@@ -410,14 +410,20 @@
             predicate_type = PREDICATE_SUPERCLASS
         elif predicate == "skos:narrowMatch":
             predicate_type = PREDICATE_SUPERCLASS
         elif predicate == "owl:differentFrom":
             predicate_type = PREDICATE_SIBLING
         elif predicate == "dbpedia-owl:different":
             predicate_type = PREDICATE_SIBLING
+        # * Added by H2 ############################
+        elif predicate == "oboInOwl:hasDbXref":
+            predicate_type = PREDICATE_HAS_DBXREF
+        elif predicate == "skos:relatedMatch":
+            predicate_type = PREDICATE_RELATED_MATCH
+        # * ########################################
         else:
             raise ValueError(f"Unhandled predicate: {predicate}")
 
         if predicate_type == PREDICATE_SUBCLASS:
             ps = (
                 confidence,
                 inverse_confidence,
@@ -441,25 +447,45 @@
         elif predicate_type == PREDICATE_SIBLING:
             ps = (
                 residual_confidence,
                 residual_confidence,
                 inverse_confidence,
                 confidence,
             )
+        # * Added by H2 ############################
+        elif predicate_type == PREDICATE_HAS_DBXREF:
+            ps = (
+                residual_confidence,
+                residual_confidence,
+                confidence,
+                inverse_confidence,
+            )
+        elif predicate_type == PREDICATE_RELATED_MATCH:
+            ps = (
+                residual_confidence,
+                residual_confidence,
+                confidence,
+                inverse_confidence,
+            )
+        # * #########################################
         else:
             raise ValueError(f"predicate: {predicate_type}")
         row = [subject_id, object_id] + [str(p) for p in ps]
         rows.append(row)
     return rows
 
 
 PREDICATE_SUBCLASS = 0
 PREDICATE_SUPERCLASS = 1
 PREDICATE_EQUIVALENT = 2
 PREDICATE_SIBLING = 3
+# * Added by H2 ############################
+PREDICATE_HAS_DBXREF = 4
+PREDICATE_RELATED_MATCH = 5
+# * ########################################
 
 RDF_FORMATS = {"ttl", "turtle", "nt", "xml"}
 
 
 def sha256sum(path: str) -> str:
     """Calculate the SHA256 hash over the bytes in a file.
 
@@ -491,18 +517,23 @@
     """
     merged_msdf = MappingSetDataFrame()
 
     # Inject metadata of msdf into df
     msdf_with_meta = [inject_metadata_into_df(msdf) for msdf in msdfs]
 
     # merge df [# 'outer' join in pandas == FULL JOIN in SQL]
+    # df_merged = reduce(
+    #     lambda left, right: left.merge(right, how="outer", on=list(left.columns)),
+    #     [msdf.df for msdf in msdf_with_meta if msdf.df is not None],
+    # )
+    # Concat is an alternative to merge when columns are not the same.
     df_merged = reduce(
-        lambda left, right: left.merge(right, how="outer", on=list(left.columns)),
+        lambda left, right: pd.concat([left, right], axis=0, ignore_index=True),
         [msdf.df for msdf in msdf_with_meta if msdf.df is not None],
-    )
+    ).drop_duplicates(ignore_index=True)
 
     # merge the non DataFrame elements
     prefix_map_list = [msdf.prefix_map for msdf in msdf_with_meta]
     # prefix_map_merged = {k: v for d in prefix_map_list for k, v in d.items()}
     merged_msdf.prefix_map = dict(ChainMap(*prefix_map_list))
     merged_msdf.df = df_merged
     if reconcile:
@@ -605,15 +636,16 @@
             # In spite of this, if match_condition_1 is returning multiple rows, pick any random row from above.
             if len(match_condition_1[match_condition_1].index) > 1:
                 match_condition_1 = match_condition_1[match_condition_1].sample()
 
         reconciled_df_subset = reconciled_df_subset.append(
             combined_normalized_subset.loc[
                 match_condition_1[match_condition_1].index, :
-            ]
+            ],
+            ignore_index=True,
         )
 
     # Add negations (PREDICATE_MODIFIER) back to DataFrame
     # NOTE: negative TRUMPS positive if negative and positive with same
     # [SUBJECT_ID, OBJECT_ID, PREDICATE_ID] exist
     for _, row_2 in negation_df.iterrows():
         match_condition_2 = (
@@ -627,17 +659,22 @@
         ] = row_2[PREDICATE_MODIFIER]
 
     if PREDICATE_MODIFIER in reconciled_df_subset.columns:
         reconciled_df_subset[PREDICATE_MODIFIER] = reconciled_df_subset[
             PREDICATE_MODIFIER
         ].fillna("")
 
+    # .fillna(df) towards the end fills an empty value
+    # with a corresponding value from df.
+    # This needs to happen because the columns in df
+    # not in reconciled_df_subset will be NaN otherwise
+    # which is incorrect.
     reconciled_df = df.merge(
         reconciled_df_subset, how="right", on=list(reconciled_df_subset.columns)
-    ).fillna("")
+    ).fillna(df)
 
     if nan_df.empty:
         return_df = reconciled_df
     else:
         return_df = reconciled_df.append(nan_df).drop_duplicates()
 
     return return_df
@@ -739,15 +776,16 @@
         if extension == "tsv":
             sep = "\t"
         elif extension == "csv":
             sep = ","
         else:
             sep = "\t"
             logging.warning("Cannot automatically determine table format, trying tsv.")
-    return read_csv(file, comment="#", sep=sep).fillna("")
+        df = read_csv(file, comment="#", sep=sep).fillna("")
+    return sort_df_rows_columns(df)
 
 
 def extract_global_metadata(msdoc: MappingSetDocument) -> Dict[str, PrefixMap]:
     """Extract metadata.
 
     :param msdoc: MappingSetDocument object
     :return: Dictionary containing metadata
@@ -770,44 +808,89 @@
 def to_mapping_set_dataframe(doc: MappingSetDocument) -> MappingSetDataFrame:
     """Convert MappingSetDocument into MappingSetDataFrame.
 
     :param doc: MappingSetDocument object
     :return: MappingSetDataFrame object
     """
     data = []
+    slots_with_double_as_range = [
+        s
+        for s in SCHEMA_DICT["slots"].keys()
+        if SCHEMA_DICT["slots"][s]["range"] == "double"
+    ]
     if doc.mapping_set.mappings is not None:
         for mapping in doc.mapping_set.mappings:
             m = get_dict_from_mapping(mapping)
             data.append(m)
     df = pd.DataFrame(data=data)
     meta = extract_global_metadata(doc)
     meta.pop(PREFIX_MAP_KEY, None)
+    # The following 3 lines are to remove columns
+    # where all values are blank.
+    df.replace("", np.nan, inplace=True)
+    df = df.dropna(axis=1, how="all")  # remove columns with all row = 'None'-s.
+    df.loc[:, ~df.columns.isin(slots_with_double_as_range)].replace(
+        np.nan, "", inplace=True
+    )
     msdf = MappingSetDataFrame(df=df, prefix_map=doc.prefix_map, metadata=meta)
+    msdf.df = sort_df_rows_columns(msdf.df)
     return msdf
 
 
 def get_dict_from_mapping(map_obj: Union[Any, Dict[Any, Any], SSSOM_Mapping]) -> dict:
     """
     Get information for linkml objects (MatchTypeEnum, PredicateModifierEnum) from the Mapping object and return the dictionary form of the object.
 
     :param map_obj: Mapping object
     :return: Dictionary
     """
     map_dict = {}
+    slots_with_double_as_range = [
+        s
+        for s in SCHEMA_DICT["slots"].keys()
+        if SCHEMA_DICT["slots"][s]["range"] == "double"
+    ]
     for property in map_obj:
-        if isinstance(map_obj[property], list):
-            map_dict[property] = "|".join(
-                enum_value.code.text
-                for enum_value in map_obj[property]
-                if type(enum_value).__name__ == MatchTypeEnum._defn.name
-            )
-        elif type(map_obj[property]).__name__ == PredicateModifierEnum._defn.name:
-            map_dict[property] = map_obj[property].code.text
+        if map_obj[property] is not None:
+            if isinstance(map_obj[property], list):
+                # IF object is an enum
+                if (
+                    SCHEMA_DICT["slots"][property]["range"]
+                    in SCHEMA_DICT["enums"].keys()
+                ):
+                    # IF object is a multivalued enum
+                    if SCHEMA_DICT["slots"][property]["multivalued"]:
+                        map_dict[property] = "|".join(
+                            enum_value.code.text for enum_value in map_obj[property]
+                        )
+                    # If object is NOT multivalued BUT an enum.
+                    else:
+                        map_dict[property] = map_obj[property].code.text
+                # IF object is NOT an enum but a list
+                else:
+                    map_dict[property] = "|".join(
+                        enum_value for enum_value in map_obj[property]
+                    )
+            # IF object NOT a list
+            else:
+                # IF object is an enum
+                if (
+                    SCHEMA_DICT["slots"][property]["range"]
+                    in SCHEMA_DICT["enums"].keys()
+                ):
+                    map_dict[property] = map_obj[property].code.text
+                else:
+                    map_dict[property] = map_obj[property]
         else:
-            map_dict[property] = map_obj[property]
+            # IF map_obj[property] is None:
+            if property in slots_with_double_as_range:
+                map_dict[property] = np.nan
+            else:
+                map_dict[property] = ""
+
     return map_dict
 
 
 class NoCURIEException(ValueError):
     """An exception raised when a CURIE can not be parsed with a given prefix map."""
 
 
@@ -850,24 +933,30 @@
     # FIXME what if the curie has a subspace in it? RE will fail
     if is_curie(uri):
         return uri
     for prefix in prefix_map:
         uri_prefix = prefix_map[prefix]
         if uri.startswith(uri_prefix):
             remainder = uri.replace(uri_prefix, "")
-            return f"{prefix}:{remainder}"
+            curie = f"{prefix}:{remainder}"
+            if is_curie(curie):
+                return f"{prefix}:{remainder}"
+            else:
+                logging.warning(f"{prefix}:{remainder} is not a CURIE ... skipping")
+                continue
     raise NoCURIEException(f"{uri} does not follow any known prefixes")
 
 
 def get_prefixes_used_in_table(df: pd.DataFrame) -> List[str]:
     """Get a list of prefixes used in CURIEs in key feature columns in a dataframe."""
     prefixes = []
-    for col in KEY_FEATURES:
-        for v in df[col].values:
-            prefixes.append(get_prefix_from_curie(v))
+    if not df.empty:
+        for col in KEY_FEATURES:
+            for v in df[col].values:
+                prefixes.append(get_prefix_from_curie(v))
     return list(set(prefixes))
 
 
 def filter_out_prefixes(df: pd.DataFrame, filter_prefixes: List[str]) -> pd.DataFrame:
     """Filter any row where a CURIE in one of the key column uses one of the given prefixes.
 
     :param df: Pandas DataFrame
@@ -961,7 +1050,105 @@
     :return: Slot is multivalued or no
     """
     # Ideally:
     # view = SchemaView('schema/sssom.yaml')
     # return view.get_slot(slot).multivalued
 
     return slot in multivalued_slots
+
+
+def reconcile_prefix_and_data(
+    msdf: MappingSetDataFrame, prefix_reconciliation: dict
+) -> MappingSetDataFrame:
+    """Reconciles prefix_map and translates CURIE switch in dataframe.
+
+    :param msdf: Mapping Set DataFrame.
+    :param prefix_reconciliation: Prefix reconcilation dictionary from a YAML file
+    :return: Mapping Set DataFrame with reconciled prefix_map and data.
+    """
+    # Discussion about this found here:
+    # https://github.com/mapping-commons/sssom-py/issues/216#issue-1171701052
+
+    prefix_map = msdf.prefix_map
+    df: pd.DataFrame = msdf.df
+    data_switch_dict = dict()
+
+    prefix_synonyms = prefix_reconciliation["prefix_synonyms"]
+    prefix_expansion = prefix_reconciliation["prefix_expansion_reconciliation"]
+
+    # The prefix exists but the expansion needs to be updated.
+    expansion_replace = {
+        k: v
+        for k, v in prefix_expansion.items()
+        if k in prefix_map.keys() and v != prefix_map[k]
+    }
+
+    # Updates expansions in prefix_map
+    prefix_map.update(expansion_replace)
+
+    # Prefixes that need to be replaced
+    # IF condition:
+    #   1. Key OR Value in prefix_synonyms are keys in prefix_map
+    #       e.g.: ICD10: ICD10CM - either should be present within
+    #           the prefix_map.
+    #   AND
+    #   2. Value in prefix_synonyms is NOT a value in expansion_replace.
+    #      In other words, the existing expansion do not match the YAML.
+
+    prefix_replace = [
+        k
+        for k, v in prefix_synonyms.items()
+        if (k in prefix_map.keys() or v in prefix_map.keys())
+        and v not in expansion_replace.keys()
+    ]
+
+    if len(prefix_replace) > 0:
+        for pr in prefix_replace:
+            correct_prefix = prefix_synonyms[pr]
+            correct_expansion = prefix_expansion[correct_prefix]
+            prefix_map[correct_prefix] = correct_expansion
+            logging.info(f"Adding prefix_map {correct_prefix}: {correct_expansion}")
+            if pr in prefix_map.keys():
+                prefix_map.pop(pr, None)
+                data_switch_dict[pr] = correct_prefix
+
+                logging.warning(f"Replacing prefix {pr} with {correct_prefix}")
+
+    # Data editing
+    if len(data_switch_dict) > 0:
+        # Read schema file
+        slots = SCHEMA_DICT["slots"]
+        entity_reference_columns = [
+            k for k, v in slots.items() if v["range"] == "EntityReference"
+        ]
+        update_columns = [c for c in df.columns if c in entity_reference_columns]
+        for k, v in data_switch_dict.items():
+            df[update_columns] = df[update_columns].replace(
+                k + ":", v + ":", regex=True
+            )
+
+    msdf.df = df
+    msdf.prefix_map = prefix_map
+
+    # TODO: When expansion of 2 prefixes in the prefix_map are the same.
+    return msdf
+
+
+def sort_df_rows_columns(
+    df: pd.DataFrame, by_columns: bool = True, by_rows: bool = True
+) -> pd.DataFrame:
+    """
+    Canonical sorting of DataFrame columns.
+
+    :param df: Pandas DataFrame with random column sequence.
+    :param by_columns: Boolean flag to sort columns canonically.
+    :param by_rows: Boolean flag to sort rows by column #1 (ascending order).
+    :return: Pandas DataFrame columns sorted canonically.
+    """
+    if by_columns and len(df.columns) > 0:
+        column_sequence = [
+            col for col in SCHEMA_DICT["slots"].keys() if col in df.columns
+        ]
+        df = df.reindex(column_sequence, axis=1)
+    if by_rows and len(df) > 0:
+        df = df.sort_values(by=df.columns[0], ignore_index=True)
+    return df
```

### Comparing `sssom-0.3.8.dev0/sssom/writers.py` & `sssom-0.3.9/sssom/writers.py`

 * *Files identical despite different names*

### Comparing `sssom-0.3.8.dev0/sssom.egg-info/PKG-INFO` & `sssom-0.3.9/sssom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssom
-Version: 0.3.8.dev0
+Version: 0.3.9
 Summary: Operations on SSSOM mapping tables
 Home-page: https://github.com/mapping-commons/sssom
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Maintainer: Chris Mungall
 Maintainer-email: cjmungall@lbl.gov
 License: MIT
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: sssom Version: 0.3.8.dev0 Summary: Operations on
-SSSOM mapping tables Home-page: https://github.com/mapping-commons/sssom
-Author: Chris Mungall Author-email: cjmungall@lbl.gov Maintainer: Chris Mungall
+Metadata-Version: 2.1 Name: sssom Version: 0.3.9 Summary: Operations on SSSOM
+mapping tables Home-page: https://github.com/mapping-commons/sssom Author:
+Chris Mungall Author-email: cjmungall@lbl.gov Maintainer: Chris Mungall
 Maintainer-email: cjmungall@lbl.gov License: MIT Download-URL: https://
 github.com/mapping-commons/sssom-py/releases Project-URL: Bug Tracker, https://
 github.com/mapping-commons/sssom-py/issues Project-URL: Source Code, https://
 github.com/mapping-commons/sssom-py/ Project-URL: Documentation, https://
 mapping-commons.github.io/sssom-py Keywords: Ontologies,Indexing,Ontology
 Mapping Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
```

### Comparing `sssom-0.3.8.dev0/sssom.egg-info/SOURCES.txt` & `sssom-0.3.9/sssom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

