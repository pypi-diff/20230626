# Comparing `tmp/cwltool-3.1.20230601100705.tar.gz` & `tmp/cwltool-3.1.20230624081518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwltool-3.1.20230601100705.tar", last modified: Thu Jun  1 10:09:01 2023, max compression
+gzip compressed data, was "cwltool-3.1.20230624081518.tar", last modified: Mon Jun 26 09:04:17 2023, max compression
```

## Comparing `cwltool-3.1.20230601100705.tar` & `cwltool-3.1.20230624081518.tar`

### file list

```diff
@@ -1,938 +1,938 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4343 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     3195 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8304 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    38146 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.626845 cwltool-3.1.20230601100705/cwltool/
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30745 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/argparser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29613 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/builder.py
--rw-r--r--   0 michael   (1000) michael   (1000)    21318 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/checker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    65632 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/command_line_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9085 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2341 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cuda.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.630845 cwltool-3.1.20230601100705/cwltool/cwlprov/
--rw-r--r--   0 michael   (1000) michael   (1000)     5198 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlprov/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1887 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlprov/provenance_constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32956 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlprov/provenance_profile.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23810 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlprov/ro.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10899 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlprov/writablebagfile.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6386 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlrdf.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7317 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/cwlviewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19183 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4319 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/docker_id.py
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/env_to_stdout.py
--rw-r--r--   0 michael   (1000) michael   (1000)      346 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18175 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/executors.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/extensions-v1.1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     7950 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/extensions-v1.2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     6788 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/extensions.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/factory.py
--rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/flatten.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/hello.simg
--rw-r--r--   0 michael   (1000) michael   (1000)    39805 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.630845 cwltool-3.1.20230601100705/cwltool/jshint/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/jshint/jshint.js
--rw-r--r--   0 michael   (1000) michael   (1000)     1240 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/jshint/jshint_wrapper.js
--rw-r--r--   0 michael   (1000) michael   (1000)    24043 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/loghandler.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    53616 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2612 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3221 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/mutation.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11058 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8648 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)    51582 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/process.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4655 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.630845 cwltool-3.1.20230601100705/cwltool/rdfqueries/
--rw-r--r--   0 michael   (1000) michael   (1000)     2722 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/rdfqueries/get_inner_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/rdfqueries/get_input_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2134 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/rdfqueries/get_output_edges.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     2146 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/rdfqueries/get_root.sparql
--rw-r--r--   0 michael   (1000) michael   (1000)     3507 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/run_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.634846 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    35108 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    33209 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      856 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       83 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/UserGuide.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21941 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    18072 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      985 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      884 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     7889 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.638846 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10104 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3696 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.0/userguide-intro.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.638846 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)      904 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47777 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36571 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25923 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24688 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.646846 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.638846 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/
--rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    47285 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36569 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    25411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    24564 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.646846 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.650846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40072 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29004 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1746 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.650846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45433 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    38245 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      293 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27116 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.610845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.654846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.654846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    45578 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    39141 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    27124 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.658846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.662846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40042 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    26611 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.666846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.666846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/
--rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Operation.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    40064 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1737 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/invocation.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.670846 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2375 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19350 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1094 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/singularity_utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6340 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/software_requirements.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/stdfsaccess.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9751 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3669 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/task_queue.py
--rw-r--r--   0 michael   (1000) michael   (1000)      540 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11158 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/update.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16509 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8824 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19091 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/workflow.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41287 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool/workflow_job.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.626845 cwltool-3.1.20230601100705/cwltool.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    36734 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      477 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-01 10:09:01.000000 cwltool-3.1.20230601100705/cwltool.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 10:08:42.000000 cwltool-3.1.20230601100705/cwltool.egg-info/zip-safe
--rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/cwltool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1336 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/gittaggers.py
--rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/lint-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      165 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/arcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/arcp/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/arcp/parse.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/argcomplete/
--rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/argcomplete/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1736 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/bagit.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/black/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/black/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      194 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      843 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/coloredlogs/
--rw-r--r--   0 michael   (1000) michael   (1000)      196 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/coloredlogs/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.674846 cwltool-3.1.20230601100705/mypy-stubs/graphviz/
--rw-r--r--   0 michael   (1000) michael   (1000)      495 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/_compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/backend.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2053 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1862 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/files.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/lang.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/graphviz/tools.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.678846 cwltool-3.1.20230601100705/mypy-stubs/importlib_metadata/
--rw-r--r--   0 michael   (1000) michael   (1000)     5101 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/importlib_metadata/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      842 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/importlib_metadata/_meta.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     7565 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/mistune.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.678846 cwltool-3.1.20230601100705/mypy-stubs/prov/
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     6855 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/constants.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/dot.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1498 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/graph.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1060 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/identifier.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    15085 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/model.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.678846 cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/
--rw-r--r--   0 michael   (1000) michael   (1000)     1405 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provjson.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provn.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     3009 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provrdf.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      767 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provxml.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5310 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/pydot.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.678846 cwltool-3.1.20230601100705/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/rdflib/term.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/ruamel/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/shellescape/
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/shellescape/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/shellescape/main.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    34792 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/subprocess.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.682846 cwltool-3.1.20230601100705/mypy-stubs/urllib/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/urllib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5488 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy-stubs/urllib/parse.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)      604 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     6735 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.694847 cwltool-3.1.20230601100705/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)      671 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/2.fastq
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/arg-empty-prefix-separate-false.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3735 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/bundle-context.jsonld
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.694847 cwltool-3.1.20230601100705/tests/checker_wf/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/broken-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/broken-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/broken-wf3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/broken-wf4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/cat-a.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/cat.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/circ-dep-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/circ-dep-wf2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/functional-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/ls.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      359 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/optional_array_mismatch.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/test.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/checker_wf/wc.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.694847 cwltool-3.1.20230601100705/tests/cwl-conformance/
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/cwl-conformance/cwltool-conftest.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/debian_image_id.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/debian_image_id2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      339 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/default_values_list.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      517 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-badposition-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-job.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)       14 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-position-expr-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-position-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-stderr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo-stdout-log-dir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/echo_broken_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      285 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/env2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/env3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/env4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      157 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/env_with_software_req.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.694847 cwltool-3.1.20230601100705/tests/input_deps/
--rw-r--r--   0 michael   (1000) michael   (1000)      202 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/docker-array-secondaryfiles-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1081 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/docker-array-secondaryfiles.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/ref.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/ref.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/ref2.fasta
--rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/input_deps/ref2.fasta.fai
--rw-r--r--   0 michael   (1000) michael   (1000)      510 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/iwdr_bad_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      506 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/iwdr_dir_literal_real_file.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/listing-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/listing2-job.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.698847 cwltool-3.1.20230601100705/tests/loop/
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/all-output-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/all-output-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1038 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/default-value-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-command-line-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-expression-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      725 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      733 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-when.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-loop-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1518 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-multi-source-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      669 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-no-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      700 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-non-boolean-loopWhen.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/invalid-value-from-loop-no-requirement.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1311 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/loop-inside-loop-all.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/loop-inside-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/loop-inside-scatter-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1076 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/loop-inside-scatter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1556 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/multi-source-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/single-var-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/single-var-loop-no-iteration.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/single-var-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/two-vars-loop-2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       11 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/two-vars-loop-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      691 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/two-vars-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      711 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/loop/value-from-loop.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      371 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/non_portable.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      406 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/non_portable2.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.698847 cwltool-3.1.20230601100705/tests/override/
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/echo-job-ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      144 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/echo-job-ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/echo-job.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/echo-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      133 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool_cwl-requirement_override.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool_cwl-requirement_override_default.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool_v1.1.0-dev1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/env-tool_v1.1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      116 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/ov.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      127 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/ov2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/override/ov3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/portable.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/random_lines.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/random_lines_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/random_lines_mapping.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.698847 cwltool-3.1.20230601100705/tests/reloc/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.698847 cwltool-3.1.20230601100705/tests/reloc/dir1/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/reloc/dir1/foo
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.698847 cwltool-3.1.20230601100705/tests/reloc/dir2/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/reloc/dir2/foo
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/reloc/test.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/scatter_numbers.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/secondary-files-bad.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/secondary-files-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/secondary-files-string-v1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      609 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/secondary-files.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      430 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/seqtk_seq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/seqtk_seq_job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      504 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/seqtk_seq_with_docker.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/seqtk_seq_wrong_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/sing_pullfolder_test.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.702847 cwltool-3.1.20230601100705/tests/subgraph/
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/1432.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4722 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/count-lines17-wf.cwl.json
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-job.json
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-tool2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-tool2_no_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-tool2_req.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_hint_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      295 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_hint_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      307 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_long.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      315 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_only_hint.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      302 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_req_collision.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_subwf-packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_subwf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/env-wf2_subwf_b.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1181 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_count_output.json
--rw-r--r--   0 michael   (1000) michael   (1000)     2623 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_file1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_file2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_file3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_output3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_output4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_output5.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step2_1432.json
--rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/extract_step5.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1162 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/single_step1.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1189 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/single_step2.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1230 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/single_step3.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/single_step4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/single_step5.json
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/steplevel-resreq.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      803 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/timelimit2-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/subgraph/wc-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5329 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_anon_types.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_bad_outputs_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_check.py
--rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_conditionals.py
--rw-r--r--   0 michael   (1000) michael   (1000)      794 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_content_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)      820 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9294 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_cuda.py
--rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_cwl_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)      562 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_default_path.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5651 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_dependencies.py
--rw-r--r--   0 michael   (1000) michael   (1000)       55 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_deps_env_modules_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_deps_env_resolvers_conf.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_deps_env_resolvers_conf_rewrite.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      101 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_deps_mapping.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3881 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_docker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_docker_info.py
--rw-r--r--   0 michael   (1000) michael   (1000)      845 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_docker_paths_with_colons.py
--rw-r--r--   0 michael   (1000) michael   (1000)      513 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_empty_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8204 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_environment.py
--rw-r--r--   0 michael   (1000) michael   (1000)    62418 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7431 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_ext.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2533 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2487 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_http_input.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4335 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_input_deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10931 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_iwdr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4452 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_js_sandbox.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6890 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_load_tool.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8993 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_loop.py
--rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_make_template.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2761 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_misc_cli.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11953 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_mpi.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3979 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_override.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7708 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_pack.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1126 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_parallel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6158 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_path_checks.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2682 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_pathmapper.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1382 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_procgenerator.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28315 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_provenance.py
--rw-r--r--   0 michael   (1000) michael   (1000)      589 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_rdfprint.py
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_recursive_validation.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1829 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_relocate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_schemadef.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3034 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_secrets.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4596 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_singularity.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4443 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_singularity_versions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_stdout_stderr_log_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2725 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_streaming.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1730 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_subclass_mypyc.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11067 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_subgraph.py
--rw-r--r--   0 michael   (1000) michael   (1000)      936 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_target.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9930 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_tmpdir.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5691 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_toolargparse.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4342 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_trs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3463 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_udocker.py
--rw-r--r--   0 michael   (1000) michael   (1000)      596 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2170 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_validate_js.py
--rw-r--r--   0 michael   (1000) michael   (1000)      867 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/test_windows_warning.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/tests/tmp1/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/tests/tmp1/tmp2/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.702847 cwltool-3.1.20230601100705/tests/tmp1/tmp2/tmp3/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp1/tmp2/tmp3/.gitkeep
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.614845 cwltool-3.1.20230601100705/tests/tmp4/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.702847 cwltool-3.1.20230601100705/tests/tmp4/alpha/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp4/alpha/baker
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp4/alpha/charlie
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp4/alpha/delta
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp4/alpha/echo
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/tmp4/alpha/foxtrot
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.706847 cwltool-3.1.20230601100705/tests/trs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1505 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/trs/Dockstore.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/trs/md5sum-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/trs/md5sum-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/utf_doc_example.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5127 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/util.py
--rw-r--r--   0 michael   (1000) michael   (1000)      236 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wc-tool-bad-hints.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wc-tool-bad-reqs.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/tests/wf/
--rw-r--r--   0 michael   (1000) michael   (1000)      286 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/1496.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      468 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/1590.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      373 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/811-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/811.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       26 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/811_inputs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      212 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/816_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/816_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/910.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/arguments.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad-stderr-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad-stdin-expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad-stdout-expr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad_formattest.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad_formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad_networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/bad_timelimit.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/badout1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/badout2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/badout3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      272 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/cache_test_workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/cat-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/cat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/conditional_step_no_inputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      577 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/conflict.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/cores_float.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/count-lines1-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/default-dir5.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/default-wf5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/default_path.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/dir_deps.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/directory.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1420 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/double-nested.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/empty.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/empty2.ttl
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/expect_iwd-passthrough1_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4397 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/expect_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4564 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/expect_revsort_datetime_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     4574 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/expect_trick_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      619 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/floats_small_and_large.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      120 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/formattest-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/formattest.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/tests/wf/generator/
--rw-r--r--   0 michael   (1000) michael   (1000)      709 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/generator/pytoolgen.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/generator/zing.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/hello-workflow-badhints.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/hello-workflow-badhints2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/hello-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/hello.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/hello_single_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      580 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwd-passthrough1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      230 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr-empty.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr-entry.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr-passthrough-successive.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr_permutations.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr_permutations_inplace.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/iwdr_permutations_nocontainer.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      282 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/js_output.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/js_output_workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/listing_deep.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/listing_none.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/listing_shallow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/listing_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/literalfile-job.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/literalfile.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/malformed_outputs.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/missing-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/missing_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      249 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_env.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_expr.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_line_count.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_simple.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mpi_simple_wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mut.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mut2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/mut3.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1107 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nested.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/networkaccess-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      233 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/no-parameters-echo.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nvidia-smi-cc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      434 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nvidia-smi-container.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nvidia-smi-max.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      408 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nvidia-smi-range.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      429 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/nvidia-smi.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:09:01.722847 cwltool-3.1.20230601100705/tests/wf/operation/
--rw-r--r--   0 michael   (1000) michael   (1000)      442 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/operation/abstract-cosifer.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5209 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/operation/expect_operation-single_packed.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/operation/operation-single.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      337 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/optional-numerical-output-0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/optional_src_mandatory_sink.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/override-no-secrets.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1921 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/packed-with-loadlisting.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1056 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/packed_no_main.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      786 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/paramref_arguments_roundtrip.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      877 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/paramref_arguments_self.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/parseInt-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/record_outputeval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/resreq_expr_float_v1_0.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/resreq_expr_float_v1_2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revsort-job-shortcut.json
--rw-r--r--   0 michael   (1000) michael   (1000)      152 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revsort-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revsort_datetime.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revsort_step_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revtool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/revtool_bad_schema.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatter-job2.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatter-wf4.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2999 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatter-wf4.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1563 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatter2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1805 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatter2_subwf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/scatterfail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)    94112 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/schemadef-bug-1473.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/schemadef-tool-12.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/schemadef-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      158 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/schemadef-type.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      163 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/sec-tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      948 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/sec-wf-out.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      214 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/sec-wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/secret_job.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      380 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/secret_wf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/separate_without_prefix.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/sorttool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      391 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/storage_float.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1124 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/three_step_color.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/timelimit-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      277 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/timelimit.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/touch_tool.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/trick_defaults.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/trick_defaults2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/trick_revsort.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/updatedir.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/updatedir_inplace.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/updateval.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      102 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/updateval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/updateval_inplace.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/vf-concat.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/wc-job.json
--rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/wc-tool.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/wffail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/whale.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      329 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/workreuse-fail.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      392 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/workreuse.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/wf/wrong_cwlVersion.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      150 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/with_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tests/without_doc.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2143 2023-06-01 10:08:33.000000 cwltool-3.1.20230601100705/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.930793 cwltool-3.1.20230624081518/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4343 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3195 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8304 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-06-26 09:04:17.930793 cwltool-3.1.20230624081518/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    38146 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.838791 cwltool-3.1.20230624081518/cwltool/
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       81 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30745 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/argparser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29613 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/builder.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    21318 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/checker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    65632 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/command_line_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9085 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2341 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cuda.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.838791 cwltool-3.1.20230624081518/cwltool/cwlprov/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5198 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlprov/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1887 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlprov/provenance_constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32956 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlprov/provenance_profile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23810 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlprov/ro.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10899 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlprov/writablebagfile.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6386 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlrdf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7317 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/cwlviewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19183 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4319 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/docker_id.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/env_to_stdout.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      346 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18175 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/executors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/extensions-v1.1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     7950 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/extensions-v1.2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     6788 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/extensions.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/factory.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/flatten.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4127 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/hello.simg
+-rw-r--r--   0 michael   (1000) michael   (1000)    39847 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.842791 cwltool-3.1.20230624081518/cwltool/jshint/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  1286196 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/jshint/jshint.js
+-rw-r--r--   0 michael   (1000) michael   (1000)     1240 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/jshint/jshint_wrapper.js
+-rw-r--r--   0 michael   (1000) michael   (1000)    24043 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/loghandler.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    53529 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2612 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3221 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/mutation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11058 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8648 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    51552 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/process.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4655 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.842791 cwltool-3.1.20230624081518/cwltool/rdfqueries/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2722 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/rdfqueries/get_inner_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/rdfqueries/get_input_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2134 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/rdfqueries/get_output_edges.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     2146 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/rdfqueries/get_root.sparql
+-rw-r--r--   0 michael   (1000) michael   (1000)     3507 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/run_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.842791 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    35108 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    33209 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      856 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       83 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/UserGuide.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21941 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    18072 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      985 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      884 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     7889 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.846791 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10104 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3696 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.0/userguide-intro.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.850791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      904 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47777 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36571 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25923 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24688 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2402 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.858791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.850791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    47285 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36569 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    25411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    24564 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      891 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8140 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.854791 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1692 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      370 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    10837 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.858791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40072 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29004 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1746 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.858791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45433 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    38245 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      293 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27116 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.862792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.866792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    45578 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    39141 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    27124 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25563 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1688 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.870792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.870792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40042 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    26611 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      960 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.874792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res_src.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.874792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5435 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1004 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CommandLineTool-standalone.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    51543 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2348 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Operation.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    40064 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    29054 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    29634 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1737 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     8260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/invocation.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.826791 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.878792 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1328 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2439 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2915 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1806 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      933 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3799 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12990 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2375 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19350 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1094 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/singularity_utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6340 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/software_requirements.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/stdfsaccess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9751 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3669 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/task_queue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      540 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11158 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/update.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16509 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8519 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19091 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/workflow.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41287 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool/workflow_job.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.838791 cwltool-3.1.20230624081518/cwltool.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    47216 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    36734 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      472 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-26 09:04:17.000000 cwltool-3.1.20230624081518/cwltool.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-26 09:03:57.000000 cwltool-3.1.20230624081518/cwltool.egg-info/zip-safe
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      335 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/cwltool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1336 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/gittaggers.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       46 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/lint-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      162 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/arcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/arcp/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/arcp/parse.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/argcomplete/
+-rw-r--r--   0 michael   (1000) michael   (1000)      525 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/argcomplete/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1736 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/bagit.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/black/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/black/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      194 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      843 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/coloredlogs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      196 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/coloredlogs/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/graphviz/
+-rw-r--r--   0 michael   (1000) michael   (1000)      495 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/_compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/backend.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2053 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1862 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/files.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/lang.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/graphviz/tools.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.882792 cwltool-3.1.20230624081518/mypy-stubs/importlib_metadata/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5101 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/importlib_metadata/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      842 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/importlib_metadata/_meta.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     7565 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/mistune.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/prov/
+-rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     6855 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/constants.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/dot.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1498 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/graph.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1060 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/identifier.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    15085 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/model.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1405 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provjson.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provn.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     3009 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provrdf.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      767 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provxml.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5310 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/pydot.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/rdflib/term.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/ruamel/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.886792 cwltool-3.1.20230624081518/mypy-stubs/shellescape/
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/shellescape/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/shellescape/main.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    34792 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/subprocess.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.890792 cwltool-3.1.20230624081518/mypy-stubs/urllib/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/urllib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5488 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy-stubs/urllib/parse.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)      522 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)      582 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-06-26 09:04:17.934793 cwltool-3.1.20230624081518/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     6731 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      256 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.898792 cwltool-3.1.20230624081518/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)      671 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/2.fastq
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/arg-empty-prefix-separate-false.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3735 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/bundle-context.jsonld
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.898792 cwltool-3.1.20230624081518/tests/checker_wf/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1358 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/broken-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1350 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/broken-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      776 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/broken-wf3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      255 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/broken-wf4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      196 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/cat-a.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      188 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/cat.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      543 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/circ-dep-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      534 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/circ-dep-wf2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1283 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/functional-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      185 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/ls.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      359 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/optional_array_mismatch.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/test.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      257 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/checker_wf/wc.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.898792 cwltool-3.1.20230624081518/tests/cwl-conformance/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/cwl-conformance/cwltool-conftest.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      205 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/debian_image_id.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      215 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/debian_image_id2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      339 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/default_values_list.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      517 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-badposition-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-job.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)       14 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-position-expr-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-position-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      313 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-stderr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo-stdout-log-dir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      297 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      167 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/echo_broken_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      280 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      285 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/env2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/env3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/env4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      157 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/env_with_software_req.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.898792 cwltool-3.1.20230624081518/tests/input_deps/
+-rw-r--r--   0 michael   (1000) michael   (1000)      202 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/docker-array-secondaryfiles-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1081 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/docker-array-secondaryfiles.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/ref.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/ref.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)    12010 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/ref2.fasta
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/input_deps/ref2.fasta.fai
+-rw-r--r--   0 michael   (1000) michael   (1000)      510 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/iwdr_bad_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      506 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/iwdr_dir_literal_real_file.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/listing-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/listing2-job.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.902792 cwltool-3.1.20230624081518/tests/loop/
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/all-output-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/all-output-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1038 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/default-value-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-command-line-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-expression-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      725 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      733 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-when.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-loop-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1518 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-multi-source-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      669 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-no-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      700 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-non-boolean-loopWhen.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/invalid-value-from-loop-no-requirement.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1311 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/loop-inside-loop-all.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/loop-inside-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/loop-inside-scatter-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1076 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/loop-inside-scatter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1556 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/multi-source-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/single-var-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/single-var-loop-no-iteration.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      591 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/single-var-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/two-vars-loop-2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       11 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/two-vars-loop-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      691 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/two-vars-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      711 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/loop/value-from-loop.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      371 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/non_portable.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      406 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/non_portable2.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.906792 cwltool-3.1.20230624081518/tests/override/
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/echo-job-ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      144 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/echo-job-ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/echo-job.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      211 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/echo-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      427 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      133 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool_cwl-requirement_override.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool_cwl-requirement_override_default.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool_cwl-requirement_override_default_wrongver.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool_v1.1.0-dev1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/env-tool_v1.1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      116 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/ov.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      127 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/ov2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/override/ov3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/portable.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      530 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/random_lines.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/random_lines_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/random_lines_mapping.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.906792 cwltool-3.1.20230624081518/tests/reloc/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.906792 cwltool-3.1.20230624081518/tests/reloc/dir1/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/reloc/dir1/foo
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.906792 cwltool-3.1.20230624081518/tests/reloc/dir2/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/reloc/dir2/foo
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/reloc/test.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1063 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/scatter_numbers.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/secondary-files-bad.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/secondary-files-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/secondary-files-string-v1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      609 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/secondary-files.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      430 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/seqtk_seq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/seqtk_seq_job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      504 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/seqtk_seq_with_docker.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      539 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/seqtk_seq_wrong_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      206 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/sing_pullfolder_test.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.910792 cwltool-3.1.20230624081518/tests/subgraph/
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/1432.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      946 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4722 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/count-lines17-wf.cwl.json
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-job.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-tool2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-tool2_no_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-tool2_req.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_hint_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      295 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_hint_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      307 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_long.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      315 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_only_hint.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      302 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_req_collision.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     3679 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_subwf-packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      340 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_subwf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/env-wf2_subwf_b.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1181 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_count_output.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     2623 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_file1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_file2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_file3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_output3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_output4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_output5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step2_1432.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      854 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/extract_step5.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1162 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/single_step1.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1189 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/single_step2.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1230 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/single_step3.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1245 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/single_step4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/single_step5.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/steplevel-resreq.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      803 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/timelimit2-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/subgraph/wc-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5329 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_anon_types.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      558 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_bad_outputs_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_conditionals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      794 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_content_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      820 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9294 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_cuda.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      369 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_cwl_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      562 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_default_path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5651 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_dependencies.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       55 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_deps_env_modules_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_deps_env_resolvers_conf.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_deps_env_resolvers_conf_rewrite.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      101 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_deps_mapping.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3881 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_docker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_docker_info.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      845 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_docker_paths_with_colons.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      513 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_empty_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8204 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_environment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    62418 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7431 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_ext.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2533 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2487 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_http_input.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4335 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_input_deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10931 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_iwdr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4452 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_js_sandbox.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6890 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_load_tool.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8993 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_loop.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      831 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_make_template.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2761 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_misc_cli.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11953 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_mpi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3979 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_override.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7708 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_pack.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1126 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_parallel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6158 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_path_checks.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2682 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_pathmapper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1382 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_procgenerator.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28315 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_provenance.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      589 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_rdfprint.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_recursive_validation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1829 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_relocate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_schemadef.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3034 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_secrets.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4596 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_singularity.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4443 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_singularity_versions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_stdout_stderr_log_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2725 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_streaming.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1730 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_subclass_mypyc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11067 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_subgraph.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      936 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_target.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9930 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_tmpdir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5691 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_toolargparse.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4342 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_trs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3463 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_udocker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      596 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2170 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_validate_js.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      867 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/test_windows_warning.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.830791 cwltool-3.1.20230624081518/tests/tmp1/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.830791 cwltool-3.1.20230624081518/tests/tmp1/tmp2/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.910792 cwltool-3.1.20230624081518/tests/tmp1/tmp2/tmp3/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp1/tmp2/tmp3/.gitkeep
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.830791 cwltool-3.1.20230624081518/tests/tmp4/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.910792 cwltool-3.1.20230624081518/tests/tmp4/alpha/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp4/alpha/baker
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp4/alpha/charlie
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp4/alpha/delta
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp4/alpha/echo
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/tmp4/alpha/foxtrot
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.910792 cwltool-3.1.20230624081518/tests/trs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1505 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/trs/Dockstore.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      821 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/trs/md5sum-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/trs/md5sum-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/utf_doc_example.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5127 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/util.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      236 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wc-tool-bad-hints.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wc-tool-bad-reqs.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.930793 cwltool-3.1.20230624081518/tests/wf/
+-rw-r--r--   0 michael   (1000) michael   (1000)      286 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/1496.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      468 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/1590.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      373 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/811-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      178 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/811.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       26 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/811_inputs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      212 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/816_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/816_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/910.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/arguments.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad-stderr-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad-stdin-expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad-stdout-expr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      523 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad_formattest.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad_formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad_networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/bad_timelimit.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/badout1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      304 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/badout2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/badout3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      272 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/cache_test_workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/cat-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      130 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/cat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/conditional_step_no_inputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      577 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/conflict.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      266 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/cores_float.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      388 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/count-lines1-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      409 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/default-dir5.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/default-wf5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      212 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/default_path.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/dir_deps.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1479 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/directory.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1420 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/double-nested.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      533 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/empty.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/empty2.ttl
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/expect_iwd-passthrough1_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4397 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/expect_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4564 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/expect_revsort_datetime_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     4574 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/expect_trick_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      619 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/floats_small_and_large.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      120 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/formattest-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      412 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/formattest.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.930793 cwltool-3.1.20230624081518/tests/wf/generator/
+-rw-r--r--   0 michael   (1000) michael   (1000)      709 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/generator/pytoolgen.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      275 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/generator/zing.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      672 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/hello-workflow-badhints.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      673 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/hello-workflow-badhints2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      657 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/hello-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/hello.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/hello_single_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      580 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwd-passthrough1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      230 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr-empty.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      414 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr-entry.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1775 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr-passthrough-successive.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2268 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr_permutations.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr_permutations_inplace.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1016 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/iwdr_permutations_nocontainer.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      282 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/js_output.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      364 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/js_output_workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      291 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/listing_deep.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      276 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/listing_none.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/listing_shallow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      158 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/listing_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       35 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/literalfile-job.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/literalfile.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/malformed_outputs.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      145 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/missing-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      548 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/missing_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      249 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_env.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      644 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_expr.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_line_count.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_simple.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      640 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mpi_simple_wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mut.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mut2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      281 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/mut3.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1107 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nested.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/networkaccess-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      425 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      233 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/no-parameters-echo.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nvidia-smi-cc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      434 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nvidia-smi-container.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nvidia-smi-max.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      408 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nvidia-smi-range.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      429 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/nvidia-smi.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 09:04:17.930793 cwltool-3.1.20230624081518/tests/wf/operation/
+-rw-r--r--   0 michael   (1000) michael   (1000)      442 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/operation/abstract-cosifer.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5209 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/operation/expect_operation-single_packed.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/operation/operation-single.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      337 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/optional-numerical-output-0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/optional_src_mandatory_sink.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/override-no-secrets.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1921 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/packed-with-loadlisting.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1056 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/packed_no_main.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      786 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/paramref_arguments_roundtrip.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      877 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/paramref_arguments_self.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      279 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/parseInt-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/record_outputeval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/resreq_expr_float_v1_0.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/resreq_expr_float_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      181 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revsort-job-shortcut.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      152 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revsort-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2331 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2447 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revsort_datetime.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2317 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revsort_step_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1367 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revtool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1471 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/revtool_bad_schema.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       62 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatter-job2.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      927 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatter-wf4.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2999 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatter-wf4.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1563 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatter2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1805 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatter2_subwf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      703 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/scatterfail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)    94112 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/schemadef-bug-1473.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/schemadef-tool-12.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      412 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/schemadef-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      158 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/schemadef-type.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      163 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/sec-tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      948 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/sec-wf-out.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      214 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/sec-wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      403 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/secret_job.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      380 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/secret_wf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      363 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/separate_without_prefix.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1101 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/sorttool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      391 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/storage_float.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1124 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/three_step_color.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      222 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/timelimit-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      277 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/timelimit.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/touch_tool.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/trick_defaults.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      260 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/trick_defaults2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2400 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/trick_revsort.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      318 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/updatedir.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      431 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/updatedir_inplace.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      488 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/updateval.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      102 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/updateval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      603 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/updateval_inplace.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      382 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/vf-concat.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/wc-job.json
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      301 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/wc-tool.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      639 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/wffail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/whale.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      329 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/workreuse-fail.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      392 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/workreuse.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      565 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/wf/wrong_cwlVersion.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      150 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/with_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tests/without_doc.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2143 2023-06-26 09:03:48.000000 cwltool-3.1.20230624081518/tox.ini
```

### Comparing `cwltool-3.1.20230601100705/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230624081518/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/CONTRIBUTING.md` & `cwltool-3.1.20230624081518/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/LICENSE.txt` & `cwltool-3.1.20230624081518/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/MANIFEST.in` & `cwltool-3.1.20230624081518/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/Makefile` & `cwltool-3.1.20230624081518/Makefile`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/PKG-INFO` & `cwltool-3.1.20230624081518/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20230601100705
+Version: 3.1.20230624081518
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: UNKNOWN
 Download-URL: https://github.com/common-workflow-language/cwltool
 Description: #############################################################################################
```

### Comparing `cwltool-3.1.20230601100705/README.rst` & `cwltool-3.1.20230624081518/README.rst`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/argparser.py` & `cwltool-3.1.20230624081518/cwltool/argparser.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/builder.py` & `cwltool-3.1.20230624081518/cwltool/builder.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/checker.py` & `cwltool-3.1.20230624081518/cwltool/checker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/command_line_tool.py` & `cwltool-3.1.20230624081518/cwltool/command_line_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/context.py` & `cwltool-3.1.20230624081518/cwltool/context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cuda.py` & `cwltool-3.1.20230624081518/cwltool/cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlprov/__init__.py` & `cwltool-3.1.20230624081518/cwltool/cwlprov/__init__.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlprov/provenance_constants.py` & `cwltool-3.1.20230624081518/cwltool/cwlprov/provenance_constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlprov/provenance_profile.py` & `cwltool-3.1.20230624081518/cwltool/cwlprov/provenance_profile.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlprov/ro.py` & `cwltool-3.1.20230624081518/cwltool/cwlprov/ro.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlprov/writablebagfile.py` & `cwltool-3.1.20230624081518/cwltool/cwlprov/writablebagfile.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlrdf.py` & `cwltool-3.1.20230624081518/cwltool/cwlrdf.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/cwlviewer.py` & `cwltool-3.1.20230624081518/cwltool/cwlviewer.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/docker.py` & `cwltool-3.1.20230624081518/cwltool/docker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/docker_id.py` & `cwltool-3.1.20230624081518/cwltool/docker_id.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/env_to_stdout.py` & `cwltool-3.1.20230624081518/cwltool/env_to_stdout.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/executors.py` & `cwltool-3.1.20230624081518/cwltool/executors.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/extensions-v1.1.yml` & `cwltool-3.1.20230624081518/cwltool/extensions-v1.1.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/extensions-v1.2.yml` & `cwltool-3.1.20230624081518/cwltool/extensions-v1.2.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/extensions.yml` & `cwltool-3.1.20230624081518/cwltool/extensions.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/factory.py` & `cwltool-3.1.20230624081518/cwltool/factory.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/flatten.py` & `cwltool-3.1.20230624081518/cwltool/flatten.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/hello.simg` & `cwltool-3.1.20230624081518/cwltool/hello.simg`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/job.py` & `cwltool-3.1.20230624081518/cwltool/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,16 +578,17 @@
         self._execute([], self.environment, runtimeContext, monitor_function)
 
     def _required_env(self) -> Dict[str, str]:
         env = {}
         env["HOME"] = self.outdir
         env["TMPDIR"] = self.tmpdir
         env["PATH"] = os.environ["PATH"]
-        if "SYSTEMROOT" in os.environ:
-            env["SYSTEMROOT"] = os.environ["SYSTEMROOT"]
+        for extra in ("SYSTEMROOT", "QEMU_LD_PREFIX"):
+            if extra in os.environ:
+                env[extra] = os.environ[extra]
         return env
 
 
 CONTROL_CODE_RE = r"\x1b\[[0-9;]*[a-zA-Z]"
 
 
 class ContainerCommandLineJob(JobBase, metaclass=ABCMeta):
```

### Comparing `cwltool-3.1.20230601100705/cwltool/jshint/jshint.js` & `cwltool-3.1.20230624081518/cwltool/jshint/jshint.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/jshint/jshint_wrapper.js` & `cwltool-3.1.20230624081518/cwltool/jshint/jshint_wrapper.js`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/load_tool.py` & `cwltool-3.1.20230624081518/cwltool/load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/loghandler.py` & `cwltool-3.1.20230624081518/cwltool/loghandler.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/main.py` & `cwltool-3.1.20230624081518/cwltool/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,20 +641,17 @@
 
 def setup_schema(
     args: argparse.Namespace, custom_schema_callback: Optional[Callable[[], None]]
 ) -> None:
     if custom_schema_callback is not None:
         custom_schema_callback()
     elif args.enable_ext:
-        with files("cwltool").joinpath("extensions.yml") as res:
-            ext10 = res.read_text("utf-8")
-        with files("cwltool").joinpath("extensions-v1.1.yml") as res:
-            ext11 = res.read_text("utf-8")
-        with files("cwltool").joinpath("extensions-v1.2.yml") as res:
-            ext12 = res.read_text("utf-8")
+        ext10 = files("cwltool").joinpath("extensions.yml").read_text("utf-8")
+        ext11 = files("cwltool").joinpath("extensions-v1.1.yml").read_text("utf-8")
+        ext12 = files("cwltool").joinpath("extensions-v1.2.yml").read_text("utf-8")
         use_custom_schema("v1.0", "http://commonwl.org/cwltool", ext10)
         use_custom_schema("v1.1", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2", "http://commonwl.org/cwltool", ext12)
         use_custom_schema("v1.2.0-dev1", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2.0-dev2", "http://commonwl.org/cwltool", ext11)
         use_custom_schema("v1.2.0-dev3", "http://commonwl.org/cwltool", ext11)
     else:
```

### Comparing `cwltool-3.1.20230601100705/cwltool/mpi.py` & `cwltool-3.1.20230624081518/cwltool/mpi.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/mutation.py` & `cwltool-3.1.20230624081518/cwltool/mutation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/pack.py` & `cwltool-3.1.20230624081518/cwltool/pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/pathmapper.py` & `cwltool-3.1.20230624081518/cwltool/pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/process.py` & `cwltool-3.1.20230624081518/cwltool/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,27 +190,27 @@
 
     cache: Dict[str, Union[str, Graph, bool]] = {}
     version = version.split("#")[-1]
     if ".dev" in version:
         version = ".".join(version.split(".")[:-1])
     for f in cwl_files:
         try:
-            with files("cwltool").joinpath(f"schemas/{version}/{f}") as res:
-                cache["https://w3id.org/cwl/" + f] = res.read_text("UTF-8")
+            res = files("cwltool").joinpath(f"schemas/{version}/{f}")
+            cache["https://w3id.org/cwl/" + f] = res.read_text("UTF-8")
         except OSError:
             pass
 
     for f in salad_files:
         try:
-            with files("cwltool").joinpath(
+            res = files("cwltool").joinpath(
                 f"schemas/{version}/salad/schema_salad/metaschema/{f}",
-            ) as res:
-                cache["https://w3id.org/cwl/salad/schema_salad/metaschema/" + f] = res.read_text(
-                    "UTF-8"
-                )
+            )
+            cache["https://w3id.org/cwl/salad/schema_salad/metaschema/" + f] = res.read_text(
+                "UTF-8"
+            )
         except OSError:
             pass
 
     if version in custom_schemas:
         cache[custom_schemas[version][0]] = custom_schemas[version][1]
         SCHEMA_CACHE[version] = load_schema(custom_schemas[version][0], cache=cache)
     else:
```

### Comparing `cwltool-3.1.20230601100705/cwltool/procgenerator.py` & `cwltool-3.1.20230624081518/cwltool/procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/rdfqueries/get_inner_edges.sparql` & `cwltool-3.1.20230624081518/cwltool/rdfqueries/get_inner_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/rdfqueries/get_input_edges.sparql` & `cwltool-3.1.20230624081518/cwltool/rdfqueries/get_input_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/rdfqueries/get_output_edges.sparql` & `cwltool-3.1.20230624081518/cwltool/rdfqueries/get_output_edges.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/rdfqueries/get_root.sparql` & `cwltool-3.1.20230624081518/cwltool/rdfqueries/get_root.sparql`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/resolver.py` & `cwltool-3.1.20230624081518/cwltool/resolver.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/run_job.py` & `cwltool-3.1.20230624081518/cwltool/run_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/README.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/README.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.0/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/index.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.1.0-dev1/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Operation.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/index.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Operation.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev2/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Operation.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/index.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev3/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Operation.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/index.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev4/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CONFORMANCE_TESTS.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Operation.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Operation.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Process.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Process.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/Workflow.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/Workflow.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/concepts.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/concepts.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/contrib.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/contrib.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/index.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/index.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/intro.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/intro.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/invocation.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/invocation.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml` & `cwltool-3.1.20230624081518/cwltool/schemas/v1.2.0-dev5/salad/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/secrets.py` & `cwltool-3.1.20230624081518/cwltool/secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/singularity.py` & `cwltool-3.1.20230624081518/cwltool/singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/singularity_utils.py` & `cwltool-3.1.20230624081518/cwltool/singularity_utils.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/software_requirements.py` & `cwltool-3.1.20230624081518/cwltool/software_requirements.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/stdfsaccess.py` & `cwltool-3.1.20230624081518/cwltool/stdfsaccess.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/subgraph.py` & `cwltool-3.1.20230624081518/cwltool/subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/task_queue.py` & `cwltool-3.1.20230624081518/cwltool/task_queue.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/udocker.py` & `cwltool-3.1.20230624081518/cwltool/udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/update.py` & `cwltool-3.1.20230624081518/cwltool/update.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/utils.py` & `cwltool-3.1.20230624081518/cwltool/utils.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/validate_js.py` & `cwltool-3.1.20230624081518/cwltool/validate_js.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,28 +83,20 @@
                 valid_schema = possible_schema
 
         return get_expressions(tool, valid_schema, source_line)
     elif isinstance(schema, ArraySchema):
         if not isinstance(tool, MutableSequence):
             return []
 
-        def tmp_expr(
-            x: Tuple[int, Union[CommentedMap, str, CommentedSeq]]
-        ) -> List[Tuple[str, Optional[SourceLine]]]:
-            # using a lambda for this broke mypyc v0.910 and before
-            return get_expressions(
-                x[1],
-                cast(ArraySchema, schema).items,
-                SourceLine(tool, x[0], include_traceback=debug),
-            )
-
         return list(
             itertools.chain(
                 *map(
-                    tmp_expr,
+                    lambda x: get_expressions(
+                        x[1], getattr(schema, "items"), SourceLine(tool, x[0])  # noqa: B009
+                    ),
                     enumerate(tool),
                 )
             )
         )
 
     elif isinstance(schema, RecordSchema):
         if not isinstance(tool, MutableMapping):
@@ -146,24 +138,24 @@
                 "W104",
                 "W119",  # using ES6 features
             ],
             "strict": "implied",
             "esversion": 5,
         }
 
-    with files("cwltool").joinpath("jshint/jshint.js") as res:
-        # NOTE: we need a global variable for lodash (which jshint depends on)
-        jshint_functions_text = "var global = this;" + res.read_text("utf-8")
-
-    with files("cwltool").joinpath("jshint/jshint_wrapper.js") as res2:
-        # NOTE: we need to assign to ob, as the expression {validateJS: validateJS} as an expression
-        # is interpreted as a block with a label `validateJS`
-        jshint_functions_text += (
-            "\n" + res2.read_text("utf-8") + "\nvar ob = {validateJS: validateJS}; ob"
-        )
+    res = files("cwltool").joinpath("jshint/jshint.js")
+    # NOTE: we need a global variable for lodash (which jshint depends on)
+    jshint_functions_text = "var global = this;" + res.read_text("utf-8")
+
+    res2 = files("cwltool").joinpath("jshint/jshint_wrapper.js")
+    # NOTE: we need to assign to ob, as the expression {validateJS: validateJS} as an expression
+    # is interpreted as a block with a label `validateJS`
+    jshint_functions_text += (
+        "\n" + res2.read_text("utf-8") + "\nvar ob = {validateJS: validateJS}; ob"
+    )
 
     returncode, stdout, stderr = exec_js_process(
         "validateJS(%s)" % json_dumps({"code": js_text, "options": options, "globals": globals}),
         timeout=eval_timeout,
         context=jshint_functions_text,
         container_engine=container_engine,
     )
```

### Comparing `cwltool-3.1.20230601100705/cwltool/workflow.py` & `cwltool-3.1.20230624081518/cwltool/workflow.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool/workflow_job.py` & `cwltool-3.1.20230624081518/cwltool/workflow_job.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/cwltool.egg-info/PKG-INFO` & `cwltool-3.1.20230624081518/cwltool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwltool
-Version: 3.1.20230601100705
+Version: 3.1.20230624081518
 Summary: Common workflow language reference implementation
 Home-page: https://github.com/common-workflow-language/cwltool
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: UNKNOWN
 Download-URL: https://github.com/common-workflow-language/cwltool
 Description: #############################################################################################
```

### Comparing `cwltool-3.1.20230601100705/cwltool.egg-info/SOURCES.txt` & `cwltool-3.1.20230624081518/cwltool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/gittaggers.py` & `cwltool-3.1.20230624081518/gittaggers.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/arcp/parse.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/arcp/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/argcomplete/__init__.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/argcomplete/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/bagit.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/bagit.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/graphviz/dot.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/graphviz/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/graphviz/files.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/graphviz/files.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/graphviz/lang.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/graphviz/lang.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/importlib_metadata/__init__.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/importlib_metadata/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/importlib_metadata/_meta.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/importlib_metadata/_meta.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/mistune.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/mistune.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/constants.py` & `cwltool-3.1.20230624081518/mypy-stubs/prov/constants.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/dot.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/dot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/graph.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/identifier.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/identifier.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/model.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/model.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provjson.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provjson.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provrdf.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provrdf.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/prov/serializers/provxml.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/prov/serializers/provxml.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/pydot.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/pydot.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/__init__.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/collection.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/graph.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_ORG.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_OWL.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_PROV.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_QB.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_RDF.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SDO.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SH.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_SSN.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_TIME.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_VOID.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/_XSD.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/namespace/__init__.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/paths.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/query.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/resource.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/rdflib/term.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/subprocess.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/mypy-stubs/urllib/parse.pyi` & `cwltool-3.1.20230624081518/mypy-stubs/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/pyproject.toml` & `cwltool-3.1.20230624081518/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=45",
     'mypy==0.971; python_version == "3.6"',  # last version for Python 3.6
     'mypy==1.3.0; python_version >= "3.7"',  # also update mypy-requirements.txt
     "types-requests",
     "types-psutil",
     "importlib_resources>=1.4",  # equivalent to Python 3.9
-    "ruamel.yaml>=0.16.0,<0.17.27",
+    "ruamel.yaml>=0.16.0,<0.18",
     "schema-salad>=8.2.20211104054942,<9",
     "cwl-utils >=0.19",
     'toml',
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
```

### Comparing `cwltool-3.1.20230601100705/requirements.txt` & `cwltool-3.1.20230624081518/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 requests>=2.6.1
-ruamel.yaml>=0.16.0,<0.17.28;python_version>='3.10'
-ruamel.yaml>=0.15,<0.17.28
+ruamel.yaml>=0.15.0,<0.18
+ruamel.yaml>=0.16;python_version>='3.10'
 rdflib>=4.2.2,<6.4
-rdflib>= 4.2.2, < 6.0.0;python_version<='3.6'
+rdflib< 6.0.0;python_version<='3.6'
 shellescape>=3.4.1,<3.9
 schema-salad>=8.4,<9
 prov==1.5.1
 mypy-extensions
 psutil>=5.6.6
 typing-extensions
 importlib_resources>=1.4  # equivalent to Python 3.9
```

### Comparing `cwltool-3.1.20230601100705/setup.py` & `cwltool-3.1.20230624081518/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,18 +108,18 @@
     packages=["cwltool", "cwltool.tests", "cwltool.cwlprov"],
     package_dir={"cwltool.tests": "tests"},
     include_package_data=True,
     install_requires=[
         "setuptools",
         "requests >= 2.6.1",  # >= 2.6.1 to workaround
         # https://github.com/ionrock/cachecontrol/issues/137
-        "ruamel.yaml >= 0.15, < 0.17.28",
-        "ruamel.yaml >= 0.16.0, <0.17.28;python_version>='3.10'",
+        "ruamel.yaml >= 0.15, < 0.18",
+        "ruamel.yaml >= 0.16.0;python_version>='3.10'",
         "rdflib >= 4.2.2, < 6.4.0",
-        "rdflib >= 4.2.2, < 6.0.0;python_version<='3.6'",
+        "rdflib < 6.0.0;python_version<='3.6'",
         "shellescape >= 3.4.1, < 3.9",
         "schema-salad >= 8.4, < 9",
         "prov == 1.5.1",
         "mypy-extensions",
         "psutil >= 5.6.6",
         "typing-extensions",
         "importlib_resources>=1.4",
@@ -128,22 +128,22 @@
         "pydot >= 1.4.1",
         "argcomplete",
         "pyparsing != 3.0.2",  # breaks --print-dot (pydot) https://github.com/pyparsing/pyparsing/issues/319
         "pyparsing < 3 ;python_version<='3.6'",  # breaks --print-dot (pydot)
         "cwl-utils >= 0.22",
     ],
     extras_require={
-        "deps": ["galaxy-tool-util >= 22.1.2, <23"],
+        "deps": ["galaxy-tool-util >= 22.1.2, <23", "galaxy-util <23"],
     },
     python_requires=">=3.6, <4",
     setup_requires=PYTEST_RUNNER,
     test_suite="tests",
     tests_require=[
         "bagit >= 1.6.4, < 1.9",
-        "pytest >= 6.2, < 7.4",
+        "pytest >= 6.2, < 7.5",
         "mock >= 2.0.0",
         "pytest-mock >= 1.10.0",
         "pytest-httpserver",
         "arcp >= 0.2.0",
         "rdflib-jsonld>=0.4.0, <= 0.6.1;python_version<='3.6'",
     ],
     entry_points={"console_scripts": ["cwltool=cwltool.main:run"]},
```

### Comparing `cwltool-3.1.20230601100705/tests/2.fasta` & `cwltool-3.1.20230624081518/tests/2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/bundle-context.jsonld` & `cwltool-3.1.20230624081518/tests/bundle-context.jsonld`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/broken-wf.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/broken-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/broken-wf2.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/broken-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/broken-wf3.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/broken-wf3.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/circ-dep-wf.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/circ-dep-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/circ-dep-wf2.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/circ-dep-wf2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/checker_wf/functional-wf.cwl` & `cwltool-3.1.20230624081518/tests/checker_wf/functional-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/cwl-conformance/cwltool-conftest.py` & `cwltool-3.1.20230624081518/tests/cwl-conformance/cwltool-conftest.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/echo-badposition-expr.cwl` & `cwltool-3.1.20230624081518/tests/echo-badposition-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/echo-position-expr.cwl` & `cwltool-3.1.20230624081518/tests/echo-position-expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/input_deps/docker-array-secondaryfiles.cwl` & `cwltool-3.1.20230624081518/tests/input_deps/docker-array-secondaryfiles.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/input_deps/ref.fasta` & `cwltool-3.1.20230624081518/tests/input_deps/ref.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/input_deps/ref2.fasta` & `cwltool-3.1.20230624081518/tests/input_deps/ref2.fasta`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/all-output-loop-no-iteration.cwl` & `cwltool-3.1.20230624081518/tests/loop/all-output-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/all-output-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/all-output-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/default-value-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/default-value-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-loop-command-line-tool.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-loop-command-line-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-loop-hint.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-loop-hint.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-loop-scatter.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-loop-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-loop-when.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-loop-when.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-loop-workflow.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-loop-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-multi-source-loop-no-requirement.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-multi-source-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-no-loopWhen.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-no-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-non-boolean-loopWhen.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-non-boolean-loopWhen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/invalid-value-from-loop-no-requirement.cwl` & `cwltool-3.1.20230624081518/tests/loop/invalid-value-from-loop-no-requirement.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/loop-inside-loop-all.cwl` & `cwltool-3.1.20230624081518/tests/loop/loop-inside-loop-all.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/loop-inside-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/loop-inside-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/loop-inside-scatter.cwl` & `cwltool-3.1.20230624081518/tests/loop/loop-inside-scatter.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/multi-source-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/multi-source-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/single-var-loop-no-iteration.cwl` & `cwltool-3.1.20230624081518/tests/loop/single-var-loop-no-iteration.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/single-var-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/single-var-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/two-vars-loop-2.cwl` & `cwltool-3.1.20230624081518/tests/loop/two-vars-loop-2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/two-vars-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/two-vars-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/loop/value-from-loop.cwl` & `cwltool-3.1.20230624081518/tests/loop/value-from-loop.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/random_lines.cwl` & `cwltool-3.1.20230624081518/tests/random_lines.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/random_lines_mapping.cwl` & `cwltool-3.1.20230624081518/tests/random_lines_mapping.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/scatter_numbers.cwl` & `cwltool-3.1.20230624081518/tests/scatter_numbers.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/secondary-files-bad.cwl` & `cwltool-3.1.20230624081518/tests/secondary-files-bad.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/secondary-files.cwl` & `cwltool-3.1.20230624081518/tests/secondary-files.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/seqtk_seq_wrong_name.cwl` & `cwltool-3.1.20230624081518/tests/seqtk_seq_wrong_name.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/count-lines1-wf.cwl` & `cwltool-3.1.20230624081518/tests/subgraph/count-lines1-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/count-lines17-wf.cwl.json` & `cwltool-3.1.20230624081518/tests/subgraph/count-lines17-wf.cwl.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/env-wf2_subwf-packed.cwl` & `cwltool-3.1.20230624081518/tests/subgraph/env-wf2_subwf-packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_count_output.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_count_output.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_file1.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_file1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_file2.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_file2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_file3.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_file3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_output3.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_output3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_output4.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_output4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_output5.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_output5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step1.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step2.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step2_1432.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step2_1432.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step3.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step4.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/extract_step5.json` & `cwltool-3.1.20230624081518/tests/subgraph/extract_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/single_step1.json` & `cwltool-3.1.20230624081518/tests/subgraph/single_step1.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/single_step2.json` & `cwltool-3.1.20230624081518/tests/subgraph/single_step2.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/single_step3.json` & `cwltool-3.1.20230624081518/tests/subgraph/single_step3.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/single_step4.json` & `cwltool-3.1.20230624081518/tests/subgraph/single_step4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/single_step5.json` & `cwltool-3.1.20230624081518/tests/subgraph/single_step5.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/steplevel-resreq.cwl` & `cwltool-3.1.20230624081518/tests/subgraph/steplevel-resreq.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/subgraph/timelimit2-wf.cwl` & `cwltool-3.1.20230624081518/tests/subgraph/timelimit2-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_anon_types.py` & `cwltool-3.1.20230624081518/tests/test_anon_types.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_bad_outputs_wf.cwl` & `cwltool-3.1.20230624081518/tests/test_bad_outputs_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_conditionals.py` & `cwltool-3.1.20230624081518/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_content_type.py` & `cwltool-3.1.20230624081518/tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_context.py` & `cwltool-3.1.20230624081518/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_cuda.py` & `cwltool-3.1.20230624081518/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_default_path.py` & `cwltool-3.1.20230624081518/tests/test_default_path.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_dependencies.py` & `cwltool-3.1.20230624081518/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_docker.py` & `cwltool-3.1.20230624081518/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_docker_paths_with_colons.py` & `cwltool-3.1.20230624081518/tests/test_docker_paths_with_colons.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_empty_input.py` & `cwltool-3.1.20230624081518/tests/test_empty_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_environment.py` & `cwltool-3.1.20230624081518/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_examples.py` & `cwltool-3.1.20230624081518/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_ext.py` & `cwltool-3.1.20230624081518/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_fetch.py` & `cwltool-3.1.20230624081518/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_http_input.py` & `cwltool-3.1.20230624081518/tests/test_http_input.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_input_deps.py` & `cwltool-3.1.20230624081518/tests/test_input_deps.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_iwdr.py` & `cwltool-3.1.20230624081518/tests/test_iwdr.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_js_sandbox.py` & `cwltool-3.1.20230624081518/tests/test_js_sandbox.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_load_tool.py` & `cwltool-3.1.20230624081518/tests/test_load_tool.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_loop.py` & `cwltool-3.1.20230624081518/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_make_template.py` & `cwltool-3.1.20230624081518/tests/test_make_template.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_misc_cli.py` & `cwltool-3.1.20230624081518/tests/test_misc_cli.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_mpi.py` & `cwltool-3.1.20230624081518/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_override.py` & `cwltool-3.1.20230624081518/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_pack.py` & `cwltool-3.1.20230624081518/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_parallel.py` & `cwltool-3.1.20230624081518/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_path_checks.py` & `cwltool-3.1.20230624081518/tests/test_path_checks.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_pathmapper.py` & `cwltool-3.1.20230624081518/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_procgenerator.py` & `cwltool-3.1.20230624081518/tests/test_procgenerator.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_provenance.py` & `cwltool-3.1.20230624081518/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_rdfprint.py` & `cwltool-3.1.20230624081518/tests/test_rdfprint.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_recursive_validation.py` & `cwltool-3.1.20230624081518/tests/test_recursive_validation.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_relocate.py` & `cwltool-3.1.20230624081518/tests/test_relocate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_secrets.py` & `cwltool-3.1.20230624081518/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_singularity.py` & `cwltool-3.1.20230624081518/tests/test_singularity.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_singularity_versions.py` & `cwltool-3.1.20230624081518/tests/test_singularity_versions.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_stdout_stderr_log_dir.py` & `cwltool-3.1.20230624081518/tests/test_stdout_stderr_log_dir.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_streaming.py` & `cwltool-3.1.20230624081518/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_subclass_mypyc.py` & `cwltool-3.1.20230624081518/tests/test_subclass_mypyc.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_subgraph.py` & `cwltool-3.1.20230624081518/tests/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_target.py` & `cwltool-3.1.20230624081518/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_tmpdir.py` & `cwltool-3.1.20230624081518/tests/test_tmpdir.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_toolargparse.py` & `cwltool-3.1.20230624081518/tests/test_toolargparse.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_trs.py` & `cwltool-3.1.20230624081518/tests/test_trs.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_udocker.py` & `cwltool-3.1.20230624081518/tests/test_udocker.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_validate.py` & `cwltool-3.1.20230624081518/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_validate_js.py` & `cwltool-3.1.20230624081518/tests/test_validate_js.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/test_windows_warning.py` & `cwltool-3.1.20230624081518/tests/test_windows_warning.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/trs/Dockstore.cwl` & `cwltool-3.1.20230624081518/tests/trs/Dockstore.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/trs/md5sum-tool.cwl` & `cwltool-3.1.20230624081518/tests/trs/md5sum-tool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/utf_doc_example.cwl` & `cwltool-3.1.20230624081518/tests/utf_doc_example.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/util.py` & `cwltool-3.1.20230624081518/tests/util.py`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/910.cwl` & `cwltool-3.1.20230624081518/tests/wf/910.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/bad_formattest.cwl` & `cwltool-3.1.20230624081518/tests/wf/bad_formattest.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/bad_formattest2.cwl` & `cwltool-3.1.20230624081518/tests/wf/bad_formattest2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/conflict.cwl` & `cwltool-3.1.20230624081518/tests/wf/conflict.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/directory.cwl` & `cwltool-3.1.20230624081518/tests/wf/directory.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/double-nested.cwl` & `cwltool-3.1.20230624081518/tests/wf/double-nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/echo.cwl` & `cwltool-3.1.20230624081518/tests/wf/echo.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/expect_iwd-passthrough1_packed.cwl` & `cwltool-3.1.20230624081518/tests/wf/expect_iwd-passthrough1_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/expect_packed.cwl` & `cwltool-3.1.20230624081518/tests/wf/expect_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/expect_revsort_datetime_packed.cwl` & `cwltool-3.1.20230624081518/tests/wf/expect_revsort_datetime_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/expect_trick_packed.cwl` & `cwltool-3.1.20230624081518/tests/wf/expect_trick_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/floats_small_and_large.cwl` & `cwltool-3.1.20230624081518/tests/wf/floats_small_and_large.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/generator/pytoolgen.cwl` & `cwltool-3.1.20230624081518/tests/wf/generator/pytoolgen.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/hello-workflow-badhints.cwl` & `cwltool-3.1.20230624081518/tests/wf/hello-workflow-badhints.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/hello-workflow-badhints2.cwl` & `cwltool-3.1.20230624081518/tests/wf/hello-workflow-badhints2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/hello-workflow.cwl` & `cwltool-3.1.20230624081518/tests/wf/hello-workflow.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/iwd-passthrough1.cwl` & `cwltool-3.1.20230624081518/tests/wf/iwd-passthrough1.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/iwdr-passthrough-successive.cwl` & `cwltool-3.1.20230624081518/tests/wf/iwdr-passthrough-successive.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/iwdr_permutations.cwl` & `cwltool-3.1.20230624081518/tests/wf/iwdr_permutations.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/iwdr_permutations_nocontainer.cwl` & `cwltool-3.1.20230624081518/tests/wf/iwdr_permutations_nocontainer.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/missing_cwlVersion.cwl` & `cwltool-3.1.20230624081518/tests/wf/missing_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/mpi_expr.cwl` & `cwltool-3.1.20230624081518/tests/wf/mpi_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/mpi_simple_wf.cwl` & `cwltool-3.1.20230624081518/tests/wf/mpi_simple_wf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/nested.cwl` & `cwltool-3.1.20230624081518/tests/wf/nested.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/operation/expect_operation-single_packed.cwl` & `cwltool-3.1.20230624081518/tests/wf/operation/expect_operation-single_packed.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/operation/operation-single.cwl` & `cwltool-3.1.20230624081518/tests/wf/operation/operation-single.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/packed-with-loadlisting.cwl` & `cwltool-3.1.20230624081518/tests/wf/packed-with-loadlisting.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/packed_no_main.cwl` & `cwltool-3.1.20230624081518/tests/wf/packed_no_main.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/paramref_arguments_roundtrip.cwl` & `cwltool-3.1.20230624081518/tests/wf/paramref_arguments_roundtrip.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/paramref_arguments_self.cwl` & `cwltool-3.1.20230624081518/tests/wf/paramref_arguments_self.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/record_outputeval.cwl` & `cwltool-3.1.20230624081518/tests/wf/record_outputeval.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/revsort.cwl` & `cwltool-3.1.20230624081518/tests/wf/revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/revsort_datetime.cwl` & `cwltool-3.1.20230624081518/tests/wf/revsort_datetime.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/revsort_step_bad_schema.cwl` & `cwltool-3.1.20230624081518/tests/wf/revsort_step_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/revtool.cwl` & `cwltool-3.1.20230624081518/tests/wf/revtool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/revtool_bad_schema.cwl` & `cwltool-3.1.20230624081518/tests/wf/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/scatter-wf4.cwl` & `cwltool-3.1.20230624081518/tests/wf/scatter-wf4.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/scatter-wf4.json` & `cwltool-3.1.20230624081518/tests/wf/scatter-wf4.json`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/scatter2.cwl` & `cwltool-3.1.20230624081518/tests/wf/scatter2.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/scatter2_subwf.cwl` & `cwltool-3.1.20230624081518/tests/wf/scatter2_subwf.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/scatterfail.cwl` & `cwltool-3.1.20230624081518/tests/wf/scatterfail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/schemadef-bug-1473.cwl` & `cwltool-3.1.20230624081518/tests/wf/schemadef-bug-1473.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/sec-wf-out.cwl` & `cwltool-3.1.20230624081518/tests/wf/sec-wf-out.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/sorttool.cwl` & `cwltool-3.1.20230624081518/tests/wf/sorttool.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/three_step_color.cwl` & `cwltool-3.1.20230624081518/tests/wf/three_step_color.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/trick_revsort.cwl` & `cwltool-3.1.20230624081518/tests/wf/trick_revsort.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/updateval_inplace.cwl` & `cwltool-3.1.20230624081518/tests/wf/updateval_inplace.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/wffail.cwl` & `cwltool-3.1.20230624081518/tests/wf/wffail.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/whale.txt` & `cwltool-3.1.20230624081518/tests/wf/whale.txt`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tests/wf/wrong_cwlVersion.cwl` & `cwltool-3.1.20230624081518/tests/wf/wrong_cwlVersion.cwl`

 * *Files identical despite different names*

### Comparing `cwltool-3.1.20230601100705/tox.ini` & `cwltool-3.1.20230624081518/tox.ini`

 * *Files identical despite different names*

