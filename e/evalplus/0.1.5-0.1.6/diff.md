# Comparing `tmp/evalplus-0.1.5.tar.gz` & `tmp/evalplus-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalplus-0.1.5.tar", last modified: Fri Jun  2 08:01:15 2023, max compression
+gzip compressed data, was "evalplus-0.1.6.tar", last modified: Mon Jun 26 06:40:02 2023, max compression
```

## Comparing `evalplus-0.1.5.tar` & `evalplus-0.1.6.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.5/.dockerignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-09 16:43:25.000000 evalplus-0.1.5/.gitignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.5/.pre-commit-config.yaml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1142 2023-05-07 05:34:58.000000 evalplus-0.1.5/CITATION.cff
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.5/Dockerfile
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.5/LICENSE
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.5/MANIFEST.in
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8763 2023-06-02 08:01:15.209326 evalplus-0.1.5/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8316 2023-06-02 08:00:30.000000 evalplus-0.1.5/README.md
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.205326 evalplus-0.1.5/codegen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5418 2023-05-11 05:46:41.000000 evalplus-0.1.5/codegen/generate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    24360 2023-05-12 01:31:35.000000 evalplus-0.1.5/codegen/model.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.205326 evalplus-0.1.5/evalplus/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.5/evalplus/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus/_version.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/data/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8038 2023-06-02 07:51:04.000000 evalplus-0.1.5/evalplus/data/__init__.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/eval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6860 2023-05-12 20:25:03.000000 evalplus-0.1.5/evalplus/eval/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.5/evalplus/eval/utils.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8749 2023-06-02 07:51:04.000000 evalplus-0.1.5/evalplus/evaluate.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/gen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/chatgpt_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/mut_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.5/evalplus/gen/type_mut.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/gen/util/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.5/evalplus/gen/util/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.5/evalplus/gen/util/api_request.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.5/evalplus/inputgen.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/tsr/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3684 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/coverage_init.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8091 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/minimization.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3562 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/mutation_init.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1887 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/run.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2165 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/sample_init.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      614 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/utils.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus.egg-info/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8763 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1317 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/SOURCES.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/dependency_links.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/entry_points.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/requires.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/top_level.txt
--rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1989 2023-06-02 07:38:42.000000 evalplus-0.1.5/evo.sh
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/gallary/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   100686 2023-06-02 07:18:33.000000 evalplus-0.1.5/gallary/overview.png
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.5/gallary/render.gif
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.5/pyproject.toml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.5/requirements-llm.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.5/requirements-tools.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.5/requirements.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-06-02 08:01:15.209326 evalplus-0.1.5/setup.cfg
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/_experimental/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.5/tools/_experimental/README.md
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/_experimental/set_cover.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/_experimental/topset_distill.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3428 2023-05-09 21:12:09.000000 evalplus-0.1.5/tools/checker.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/filter_inputs.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/humaneval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/humaneval/check_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/humaneval/init_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.5/tools/init_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.5/tools/merge_dataset.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/render.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3737 2023-05-09 21:15:14.000000 evalplus-0.1.5/tools/sanitize.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/stat_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.5/tools/viz_passrate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1007 2023-06-02 07:51:04.000000 evalplus-0.1.5/zipper.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.029366 evalplus-0.1.6/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-06-26 06:38:07.000000 evalplus-0.1.6/.dockerignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-09 16:43:25.000000 evalplus-0.1.6/.gitignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.6/.pre-commit-config.yaml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      827 2023-06-15 07:29:53.000000 evalplus-0.1.6/CITATION.cff
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.6/Dockerfile
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.6/LICENSE
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.6/MANIFEST.in
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     9634 2023-06-26 06:40:02.029366 evalplus-0.1.6/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     9187 2023-06-26 05:48:40.000000 evalplus-0.1.6/README.md
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/codegen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5418 2023-05-11 05:46:41.000000 evalplus-0.1.6/codegen/generate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    24360 2023-05-12 01:31:35.000000 evalplus-0.1.6/codegen/model.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.6/evalplus/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus/_version.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/data/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8038 2023-06-26 05:27:43.000000 evalplus-0.1.6/evalplus/data/__init__.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/eval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7110 2023-06-26 03:26:58.000000 evalplus-0.1.6/evalplus/eval/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.6/evalplus/eval/utils.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     9283 2023-06-26 05:29:02.000000 evalplus-0.1.6/evalplus/evaluate.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/gen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.6/evalplus/gen/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.6/evalplus/gen/chatgpt_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.6/evalplus/gen/mut_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.6/evalplus/gen/type_mut.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/gen/util/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.6/evalplus/gen/util/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.6/evalplus/gen/util/api_request.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.6/evalplus/inputgen.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus/tsr/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3684 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/coverage_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8091 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/minimization.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3562 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/mutation_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1887 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/run.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2165 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/sample_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      614 2023-06-02 07:46:01.000000 evalplus-0.1.6/evalplus/tsr/utils.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/evalplus.egg-info/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     9634 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus.egg-info/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1373 2023-06-26 06:40:02.000000 evalplus-0.1.6/evalplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus.egg-info/entry_points.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus.egg-info/requires.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-06-26 06:40:01.000000 evalplus-0.1.6/evalplus.egg-info/top_level.txt
+-rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1989 2023-06-02 07:38:42.000000 evalplus-0.1.6/evo.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.025366 evalplus-0.1.6/gallary/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   100686 2023-06-02 07:18:33.000000 evalplus-0.1.6/gallary/overview.png
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.6/gallary/render.gif
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.6/pyproject.toml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.6/requirements-llm.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.6/requirements-tools.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.6/requirements.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-06-26 06:40:02.029366 evalplus-0.1.6/setup.cfg
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.029366 evalplus-0.1.6/tools/
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.029366 evalplus-0.1.6/tools/_experimental/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.6/tools/_experimental/README.md
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/_experimental/set_cover.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/_experimental/topset_distill.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3428 2023-05-09 21:12:09.000000 evalplus-0.1.6/tools/checker.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/filter_inputs.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-26 06:40:02.029366 evalplus-0.1.6/tools/humaneval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/humaneval/check_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2236 2023-06-26 03:31:58.000000 evalplus-0.1.6/tools/humaneval/fix_v011.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2930 2023-06-26 05:11:30.000000 evalplus-0.1.6/tools/humaneval/fix_v012.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/humaneval/init_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.6/tools/init_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.6/tools/merge_dataset.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/render.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3737 2023-05-09 21:15:14.000000 evalplus-0.1.6/tools/sanitize.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.6/tools/stat_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.6/tools/viz_passrate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1007 2023-06-26 05:05:19.000000 evalplus-0.1.6/zipper.sh
```

### Comparing `evalplus-0.1.5/.dockerignore` & `evalplus-0.1.6/.dockerignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/.gitignore` & `evalplus-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/LICENSE` & `evalplus-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/PKG-INFO` & `evalplus-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.5
+Version: 0.1.6
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -71,14 +71,16 @@
 ```
 
 </div>
 </details>
 
 ### HumanEval+
 
+#### Generate Code Samples
+
 The usage is just like the original HumanEval where you just need to implement the `generate_one_completion` function!
 
 ```python
 from evalplus.data import get_human_eval_plus, write_jsonl
 
 problems = get_human_eval_plus()
 
@@ -100,40 +102,47 @@
 + `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
 + `base_input` is the test inputs in original HumanEval
 + `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
-To evaluate the samples:
+#### Evaluate Code Samples with HumanEval+
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
-🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
-
-```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
-# ...Or locally ⚠️
-# evalplus.evaluate --dataset humaneval --samples samples.jsonl
-```
+> **Warning** ⚠️ Do you use a very slow machine?
+>
+> LLM solutions are regarded as **failed** on timeout (and OOM etc.).
+> Specifically, we set the timeout $T=\max(T_{base}, T_{gt}\times k)$, where:
+>
+> - $T_{base}$ is the minimal timeout (configurable by `--min-time-limit`; default to 0.2s);
+> - $T_{gt}$ is the runtime of the ground-truth solutions (achieved via profiling);
+> - $k$ is a configurable factor `--gt-time-limit-factor` (default to 4);
+>
+> If your machine is too slow and you are getting high-variance results, try to use larger $k$ and $T_{base}$.
+>
+> Additionally, you are **NOT** encouraged to make your test-bed over stressed while running evaluation.
+> For example, using `--parallel 64` on a 4-core machine or doing something else during evaluation are bad ideas...
 
-<details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
+<details><summary>🤔 Evaluate with local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
+export PYTHONPATH=$PYTHONPATH:$(pwd)
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
 </div>
 </details>
 
 <details><summary>⌨️ More command-line flags <i>:: click to expand ::</i></summary>
@@ -142,28 +151,14 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
-<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
-<div>
-
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
-Here are some tips to speed up the evaluation:
-
-* Use `--parallel $(nproc)`
-* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
-* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
-* We will release an distilled version of HumanEval+ soon. Stay tuned!
-
-</div>
-</details>
-
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
@@ -176,14 +171,36 @@
 ```
 
 - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do **NOT** use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (700+ on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* Use HumanEval+ Mini
+
+</div>
+</details>
+
+> 🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests without fail-stop with `--test-details`).
+>
+> ```bash
+> docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl --mini
+> # ...Or locally ⚠️
+> # evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini
+> ```
+
 ### MBPP+ (TBD)
 
 
 ## 💻 LLM-generated code
 
 Please kindly find the LLM-pre-generated code samples [in the attachment of our v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0).
 Each sample file is packaged in a zip file named like `${model_name}_temp_${temperature}.zip`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.5 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.6 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
 [https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
@@ -22,89 +22,101 @@
 (./gallary/overview.png) ## ð¥ Quick Start To get started, please first setup
 the environment: ```bash pip install evalplus --upgrade ``` ...Or you can try
 out the latest developing version: ```bash pip install "git+https://github.com/
 evalplus/evalplus.git" --upgrade ``` ð¤ Want to use local GitHub repo? ::
 click to expand ::
 ```bash git clone https://github.com/evalplus/evalplus.git cd evalplus export
 PYTHONPATH=$PYTHONPATH:$(pwd) pip install -r requirements.txt ```
- ### HumanEval+ The usage is just like the original HumanEval where you just
-need to implement the `generate_one_completion` function! ```python from
-evalplus.data import get_human_eval_plus, write_jsonl problems =
-get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
+ ### HumanEval+ #### Generate Code Samples The usage is just like the original
+HumanEval where you just need to implement the `generate_one_completion`
+function! ```python from evalplus.data import get_human_eval_plus, write_jsonl
+problems = get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is name of
 the function * `prompt` is the function signature with docstring +
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
- To evaluate the samples: You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
-out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
-with the highest quality, achieving almost the same effectiveness of the full
-version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
-you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
-...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
-samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
-```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
-```
+ #### Evaluate Code Samples with HumanEval+ You are strongly recommended to use
+a sandbox such as [docker](https://docs.docker.com/get-docker/): ```bash docker
+run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples
+samples.jsonl ``` ...Or if you want to try it locally regardless of the risks
+â ï¸: ```bash evalplus.evaluate --dataset humaneval --samples samples.jsonl
+``` > **Warning** â ï¸ Do you use a very slow machine? > > LLM solutions are
+regarded as **failed** on timeout (and OOM etc.). > Specifically, we set the
+timeout $T=\max(T_{base}, T_{gt}\times k)$, where: > > - $T_{base}$ is the
+minimal timeout (configurable by `--min-time-limit`; default to 0.2s); > - $T_
+{gt}$ is the runtime of the ground-truth solutions (achieved via profiling); >
+- $k$ is a configurable factor `--gt-time-limit-factor` (default to 4); > > If
+your machine is too slow and you are getting high-variance results, try to use
+larger $k$ and $T_{base}$. > > Additionally, you are **NOT** encouraged to make
+your test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... ð¤ Evaluate with local GitHub repo? :: click to expand ::
+```bash export PYTHONPATH=$PYTHONPATH:$(pwd) python evalplus/evaluate.py --
+dataset humaneval --samples samples.jsonl ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ð¤ How long it would take? :: click to expand ::
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
-8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
-speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
-details` if you just want to quickly get pass@k as `--test-details` will run
-all tests (~775 on average for each task), while without `--test-details` the
-testing for a sample stops immediately when it fails the first test. * Use our
-pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
-will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
 used - A cache file named like `samples_eval_results.jsonl` will be cached.
-Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð» LLM-generated code
-Please kindly find the LLM-pre-generated code samples [in the attachment of our
-v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0). Each
-sample file is packaged in a zip file named like `${model_name}_temp_$
-{temperature}.zip`. You can unzip them to a folder named like `$
-{model_name}_temp_${temperature}` and run the evaluation from scratch with:
-```bash evalplus.evaluate --dataset humaneval --samples ${model_name}_temp_$
-{temperature} ``` ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+Remove it to re-run the evaluation ð¤ How long it would take? :: click to
+expand ::
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10
+minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do **NOT** use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (700+ on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * Use
+HumanEval+ Mini
+ > ð **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of
+additional tests with the highest quality, achieving almost the same
+effectiveness of the full version. Just add a **`--mini`** flag, it can run
+23+% faster! (even faster if you evaluate all tests without fail-stop with `--
+test-details`). > > ```bash > docker run -v $(pwd):/app ganler/evalplus:latest
+--dataset humaneval --samples samples.jsonl --mini > # ...Or locally â ï¸ > #
+evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini > ``` ###
+MBPP+ (TBD) ## ð» LLM-generated code Please kindly find the LLM-pre-generated
+code samples [in the attachment of our v0.1.0 release](https://github.com/
+evalplus/evalplus/releases/tag/v0.1.0). Each sample file is packaged in a zip
+file named like `${model_name}_temp_${temperature}.zip`. You can unzip them to
+a folder named like `${model_name}_temp_${temperature}` and run the evaluation
+from scratch with: ```bash evalplus.evaluate --dataset humaneval --samples $
+{model_name}_temp_${temperature} ``` ## ð Papers Read our [**paper**](https:
+//arxiv.org/abs/2305.01210) for more detailed findings! ```bibtex @article
+{evalplus, title={Is Your Code Generated by ChatGPT Really Correct? Rigorous
+Evaluation of Large Language Models for Code Generation}, author={Jiawei Liu
+and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang}, journal={arXiv
+preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful tools To use
+these tools, please first install the repository from GitHub: ```bash git clone
+https://github.com/evalplus/evalplus.git cd evalplus pip install -
+r requirements-tools.txt ``` ### Syntax checker for LLM-generated code Check
+LLM-produced code and answer the following questions: 1. Is the generation
+entirely done for all samples / all problems in the dataset? 2. Are LLM-
+generated code compilable? (if no, something could be wrong and you'd better
+check) ```shell python tools/checker.py --folder /path/to/[model]-[??]b_temp_
+[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated code may
+contain some syntax errors. But some of them can be easily fixable by doing
+simple post-processing. This tool will make the LLM-generated code more clean/
+compilable by doing certain post-processing such as trimming with more magical
+EOFs and some garbage non-code tokens. ```shell python tools/sanitize.py --eof
+--folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to
+`/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to
+`rich` and LaTeX tables ```shell python tools/render.py --type /path/to/
+[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/render.gif) ### Perform
+test input generation from scratch (TBD) ## ð· Development Before you start:
+```bash pip install pre-commit pre-commit install export
+PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is the
+package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.5/README.md` & `evalplus-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 ```
 
 </div>
 </details>
 
 ### HumanEval+
 
+#### Generate Code Samples
+
 The usage is just like the original HumanEval where you just need to implement the `generate_one_completion` function!
 
 ```python
 from evalplus.data import get_human_eval_plus, write_jsonl
 
 problems = get_human_eval_plus()
 
@@ -86,40 +88,47 @@
 + `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
 + `base_input` is the test inputs in original HumanEval
 + `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
-To evaluate the samples:
+#### Evaluate Code Samples with HumanEval+
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
-🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
-
-```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
-# ...Or locally ⚠️
-# evalplus.evaluate --dataset humaneval --samples samples.jsonl
-```
+> **Warning** ⚠️ Do you use a very slow machine?
+>
+> LLM solutions are regarded as **failed** on timeout (and OOM etc.).
+> Specifically, we set the timeout $T=\max(T_{base}, T_{gt}\times k)$, where:
+>
+> - $T_{base}$ is the minimal timeout (configurable by `--min-time-limit`; default to 0.2s);
+> - $T_{gt}$ is the runtime of the ground-truth solutions (achieved via profiling);
+> - $k$ is a configurable factor `--gt-time-limit-factor` (default to 4);
+>
+> If your machine is too slow and you are getting high-variance results, try to use larger $k$ and $T_{base}$.
+>
+> Additionally, you are **NOT** encouraged to make your test-bed over stressed while running evaluation.
+> For example, using `--parallel 64` on a 4-core machine or doing something else during evaluation are bad ideas...
 
-<details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
+<details><summary>🤔 Evaluate with local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
+export PYTHONPATH=$PYTHONPATH:$(pwd)
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
 </div>
 </details>
 
 <details><summary>⌨️ More command-line flags <i>:: click to expand ::</i></summary>
@@ -128,28 +137,14 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
-<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
-<div>
-
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
-Here are some tips to speed up the evaluation:
-
-* Use `--parallel $(nproc)`
-* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
-* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
-* We will release an distilled version of HumanEval+ soon. Stay tuned!
-
-</div>
-</details>
-
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
@@ -162,14 +157,36 @@
 ```
 
 - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do **NOT** use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (700+ on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* Use HumanEval+ Mini
+
+</div>
+</details>
+
+> 🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests without fail-stop with `--test-details`).
+>
+> ```bash
+> docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl --mini
+> # ...Or locally ⚠️
+> # evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini
+> ```
+
 ### MBPP+ (TBD)
 
 
 ## 💻 LLM-generated code
 
 Please kindly find the LLM-pre-generated code samples [in the attachment of our v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0).
 Each sample file is packaged in a zip file named like `${model_name}_temp_${temperature}.zip`.
```

#### html2text {}

```diff
@@ -16,89 +16,101 @@
 (./gallary/overview.png) ## ð¥ Quick Start To get started, please first setup
 the environment: ```bash pip install evalplus --upgrade ``` ...Or you can try
 out the latest developing version: ```bash pip install "git+https://github.com/
 evalplus/evalplus.git" --upgrade ``` ð¤ Want to use local GitHub repo? ::
 click to expand ::
 ```bash git clone https://github.com/evalplus/evalplus.git cd evalplus export
 PYTHONPATH=$PYTHONPATH:$(pwd) pip install -r requirements.txt ```
- ### HumanEval+ The usage is just like the original HumanEval where you just
-need to implement the `generate_one_completion` function! ```python from
-evalplus.data import get_human_eval_plus, write_jsonl problems =
-get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
+ ### HumanEval+ #### Generate Code Samples The usage is just like the original
+HumanEval where you just need to implement the `generate_one_completion`
+function! ```python from evalplus.data import get_human_eval_plus, write_jsonl
+problems = get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is name of
 the function * `prompt` is the function signature with docstring +
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
- To evaluate the samples: You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
-out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
-with the highest quality, achieving almost the same effectiveness of the full
-version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
-you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
-...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
-samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
-```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
-```
+ #### Evaluate Code Samples with HumanEval+ You are strongly recommended to use
+a sandbox such as [docker](https://docs.docker.com/get-docker/): ```bash docker
+run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples
+samples.jsonl ``` ...Or if you want to try it locally regardless of the risks
+â ï¸: ```bash evalplus.evaluate --dataset humaneval --samples samples.jsonl
+``` > **Warning** â ï¸ Do you use a very slow machine? > > LLM solutions are
+regarded as **failed** on timeout (and OOM etc.). > Specifically, we set the
+timeout $T=\max(T_{base}, T_{gt}\times k)$, where: > > - $T_{base}$ is the
+minimal timeout (configurable by `--min-time-limit`; default to 0.2s); > - $T_
+{gt}$ is the runtime of the ground-truth solutions (achieved via profiling); >
+- $k$ is a configurable factor `--gt-time-limit-factor` (default to 4); > > If
+your machine is too slow and you are getting high-variance results, try to use
+larger $k$ and $T_{base}$. > > Additionally, you are **NOT** encouraged to make
+your test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... ð¤ Evaluate with local GitHub repo? :: click to expand ::
+```bash export PYTHONPATH=$PYTHONPATH:$(pwd) python evalplus/evaluate.py --
+dataset humaneval --samples samples.jsonl ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ð¤ How long it would take? :: click to expand ::
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
-8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
-speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
-details` if you just want to quickly get pass@k as `--test-details` will run
-all tests (~775 on average for each task), while without `--test-details` the
-testing for a sample stops immediately when it fails the first test. * Use our
-pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
-will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
 used - A cache file named like `samples_eval_results.jsonl` will be cached.
-Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð» LLM-generated code
-Please kindly find the LLM-pre-generated code samples [in the attachment of our
-v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0). Each
-sample file is packaged in a zip file named like `${model_name}_temp_$
-{temperature}.zip`. You can unzip them to a folder named like `$
-{model_name}_temp_${temperature}` and run the evaluation from scratch with:
-```bash evalplus.evaluate --dataset humaneval --samples ${model_name}_temp_$
-{temperature} ``` ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+Remove it to re-run the evaluation ð¤ How long it would take? :: click to
+expand ::
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10
+minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do **NOT** use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (700+ on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * Use
+HumanEval+ Mini
+ > ð **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of
+additional tests with the highest quality, achieving almost the same
+effectiveness of the full version. Just add a **`--mini`** flag, it can run
+23+% faster! (even faster if you evaluate all tests without fail-stop with `--
+test-details`). > > ```bash > docker run -v $(pwd):/app ganler/evalplus:latest
+--dataset humaneval --samples samples.jsonl --mini > # ...Or locally â ï¸ > #
+evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini > ``` ###
+MBPP+ (TBD) ## ð» LLM-generated code Please kindly find the LLM-pre-generated
+code samples [in the attachment of our v0.1.0 release](https://github.com/
+evalplus/evalplus/releases/tag/v0.1.0). Each sample file is packaged in a zip
+file named like `${model_name}_temp_${temperature}.zip`. You can unzip them to
+a folder named like `${model_name}_temp_${temperature}` and run the evaluation
+from scratch with: ```bash evalplus.evaluate --dataset humaneval --samples $
+{model_name}_temp_${temperature} ``` ## ð Papers Read our [**paper**](https:
+//arxiv.org/abs/2305.01210) for more detailed findings! ```bibtex @article
+{evalplus, title={Is Your Code Generated by ChatGPT Really Correct? Rigorous
+Evaluation of Large Language Models for Code Generation}, author={Jiawei Liu
+and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang}, journal={arXiv
+preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful tools To use
+these tools, please first install the repository from GitHub: ```bash git clone
+https://github.com/evalplus/evalplus.git cd evalplus pip install -
+r requirements-tools.txt ``` ### Syntax checker for LLM-generated code Check
+LLM-produced code and answer the following questions: 1. Is the generation
+entirely done for all samples / all problems in the dataset? 2. Are LLM-
+generated code compilable? (if no, something could be wrong and you'd better
+check) ```shell python tools/checker.py --folder /path/to/[model]-[??]b_temp_
+[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated code may
+contain some syntax errors. But some of them can be easily fixable by doing
+simple post-processing. This tool will make the LLM-generated code more clean/
+compilable by doing certain post-processing such as trimming with more magical
+EOFs and some garbage non-code tokens. ```shell python tools/sanitize.py --eof
+--folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to
+`/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to
+`rich` and LaTeX tables ```shell python tools/render.py --type /path/to/
+[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/render.gif) ### Perform
+test input generation from scratch (TBD) ## ð· Development Before you start:
+```bash pip install pre-commit pre-commit install export
+PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is the
+package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.5/codegen/generate.py` & `evalplus-0.1.6/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/codegen/model.py` & `evalplus-0.1.6/codegen/model.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/data/__init__.py` & `evalplus-0.1.6/evalplus/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 CACHE_DIR = user_cache_dir("evalplus")
 
 
 HUMANEVAL_URL = (
     "https://github.com/openai/human-eval/raw/master/data/HumanEval.jsonl.gz"
 )
-HUMANEVAL_PLUS_VERSION = "v0.1.1"
+HUMANEVAL_PLUS_VERSION = "v0.1.3"
 
 
 def get_dataset_metadata(name, version, mini):
     assert name in ["HumanEvalPlus"], f"Unknown/unsupported dataset: {name}"
     extra = "-Mini" if mini else ""
     url = f"https://github.com/ganler/release/releases/download/humanevalplus/{name}{extra}-{version}.jsonl.gz"
     cache_path = os.path.join(CACHE_DIR, f"{name}{extra}-{version}.jsonl")
```

### Comparing `evalplus-0.1.5/evalplus/eval/__init__.py` & `evalplus-0.1.6/evalplus/eval/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -165,17 +165,18 @@
     code: str,
     inputs: List[Any],
     entry_point: str,
     expected,
     atol,
     ref_time: List[float],
     fast_check: bool = False,
+    min_time_limit: float = 0.1,
+    gt_time_limit_factor: float = 2.0,
 ) -> Tuple[str, np.ndarray]:
-    min_limit = 0.05
-    time_limits = [max(min_limit, 2 * t) for t in ref_time]
+    time_limits = [max(min_time_limit, gt_time_limit_factor * t) for t in ref_time]
     timeout = sum(time_limits) + 1
     if not fast_check:
         timeout += 1  # extra time for data collection
 
     # shared memory objects
     progress = Value("i", 0)
     stat = Value("i", _UNKNOWN)
@@ -223,24 +224,28 @@
     files: List[str],
     inputs: List,
     expected: List,
     entry_point: str,
     atol: float,
     ref_time: List[float],
     fast_check: bool = False,
+    min_time_limit: float = 0.1,
+    gt_time_limit_factor: float = 2.0,
 ) -> List[Tuple[str, List[bool]]]:
     ret = []
     # sort files by the id in name (i.e., "../n.py")
     files = sorted(files, key=lambda x: int(x.split("/")[-1].split(".")[0]))
     for file in files:
         code = open(file, "r").read()
         stat, det = untrusted_check(
             code,
             inputs,
             entry_point,
             expected=expected,
             atol=atol,
             ref_time=ref_time,
             fast_check=fast_check,
+            min_time_limit=min_time_limit,
+            gt_time_limit_factor=gt_time_limit_factor,
         )
         ret.append((stat, det.tolist()))
     return ret
```

### Comparing `evalplus-0.1.5/evalplus/eval/utils.py` & `evalplus-0.1.6/evalplus/eval/utils.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/evaluate.py` & `evalplus-0.1.6/evalplus/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # 2nd item (optional): the detailed pass/fail boolean for each input
 Result = Tuple[str, List[bool]]
 
 
 def get_groundtruth(problems, hashcode):
     cache_file = os.path.join(CACHE_DIR, f"{hashcode}.pkl")
     if os.path.exists(cache_file):
-        print(f"Load from {cache_file}")
+        print(f"Load from ground-truth from {cache_file}")
         with open(cache_file, "rb") as f:
             return pickle.load(f)
 
     print("Computing expected output...")
     tbegin = time.time()
     expected_output = {}
     for task_id, problem in problems.items():
@@ -70,39 +70,45 @@
     completion_id: int,
     problem: Dict[str, Any],
     solution: str,
     expected_output: Dict[str, List],
     base_only=False,
     fast_check=False,
     identifier=None,
+    min_time_limit: float = 0.1,
+    gt_time_limit_factor: float = 2.0,
 ) -> Dict[str, Union[int, Optional[Result]]]:
     ret = {
         "completion_id": completion_id,
         "task_id": problem["task_id"],
         "_identifier": identifier,
     }
     ret["base"] = untrusted_check(
         solution,
         problem["base_input"],
         problem["entry_point"],
         expected=expected_output["base"],
         atol=problem["atol"],
         ref_time=expected_output["base_time"],
         fast_check=fast_check,
+        min_time_limit=min_time_limit,
+        gt_time_limit_factor=gt_time_limit_factor,
     )
 
     if not base_only:
         ret["plus"] = untrusted_check(
             solution,
             problem["plus_input"],
             problem["entry_point"],
             expected=expected_output["plus"],
             atol=problem["atol"],
             ref_time=expected_output["plus_time"],
             fast_check=fast_check,
+            min_time_limit=min_time_limit,
+            gt_time_limit_factor=gt_time_limit_factor,
         )
 
     return ret
 
 
 def evaluate_humaneval(flags):
     if flags.parallel is None:
@@ -113,15 +119,15 @@
     if os.path.isdir(flags.samples):
         result_path = os.path.join(flags.samples, "eval_results.json")
     else:
         assert flags.samples.endswith(".jsonl")
         result_path = flags.samples.replace(".jsonl", "_eval_results.json")
 
     if os.path.isfile(result_path) and not flags.i_just_wanna_run:
-        print(f"Load from {result_path}")
+        print(f"Load from previous results from {result_path}")
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
     else:
         problems = get_human_eval_plus(mini=flags.mini)
 
@@ -154,14 +160,16 @@
                     completion_id[task_id],
                     problems[task_id],
                     solution,
                     expected_output[task_id],
                     flags.base_only,
                     not flags.test_details,  # fast_check
                     sample["_identifier"],
+                    flags.min_time_limit,
+                    flags.gt_time_limit_factor,
                 )
                 futures.append(executor.submit(check_correctness, *args))
                 completion_id[task_id] += 1
                 n_samples += 1
 
             assert n_samples == len(remainings), "Missing problems in unfinished"
             assert len(completion_id) == len(problems), "Missing problems in samples"
@@ -252,14 +260,16 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--dataset", required=True, type=str)
     parser.add_argument("--samples", required=True, type=str)
     parser.add_argument("--base-only", action="store_true")
     parser.add_argument("--parallel", default=None, type=int)
     parser.add_argument("--i-just-wanna-run", action="store_true")
     parser.add_argument("--test-details", action="store_true")
+    parser.add_argument("--min-time-limit", default=0.2, type=float)
+    parser.add_argument("--gt-time-limit-factor", default=4.0, type=float)
     parser.add_argument("--mini", action="store_true")
     args = parser.parse_args()
 
     if args.dataset == "humaneval":
         evaluate_humaneval(args)
     else:
         raise NotImplementedError("Unsupported dataset: {}".format(args.dataset))
```

### Comparing `evalplus-0.1.5/evalplus/gen/__init__.py` & `evalplus-0.1.6/evalplus/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/gen/chatgpt_gen.py` & `evalplus-0.1.6/evalplus/gen/chatgpt_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/gen/mut_gen.py` & `evalplus-0.1.6/evalplus/gen/mut_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/gen/type_mut.py` & `evalplus-0.1.6/evalplus/gen/type_mut.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/gen/util/__init__.py` & `evalplus-0.1.6/evalplus/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/gen/util/api_request.py` & `evalplus-0.1.6/evalplus/gen/util/api_request.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/inputgen.py` & `evalplus-0.1.6/evalplus/inputgen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/coverage_init.py` & `evalplus-0.1.6/evalplus/tsr/coverage_init.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/minimization.py` & `evalplus-0.1.6/evalplus/tsr/minimization.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/mutation_init.py` & `evalplus-0.1.6/evalplus/tsr/mutation_init.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/run.py` & `evalplus-0.1.6/evalplus/tsr/run.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/sample_init.py` & `evalplus-0.1.6/evalplus/tsr/sample_init.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus/tsr/utils.py` & `evalplus-0.1.6/evalplus/tsr/utils.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/evalplus.egg-info/PKG-INFO` & `evalplus-0.1.6/evalplus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.5
+Version: 0.1.6
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -71,14 +71,16 @@
 ```
 
 </div>
 </details>
 
 ### HumanEval+
 
+#### Generate Code Samples
+
 The usage is just like the original HumanEval where you just need to implement the `generate_one_completion` function!
 
 ```python
 from evalplus.data import get_human_eval_plus, write_jsonl
 
 problems = get_human_eval_plus()
 
@@ -100,40 +102,47 @@
 + `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
 + `base_input` is the test inputs in original HumanEval
 + `plus_input` is the test inputs brought by EvalPlus
 
 </div>
 </details>
 
-To evaluate the samples:
+#### Evaluate Code Samples with HumanEval+
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl
+docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
-🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
-
-```bash
-docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
-# ...Or locally ⚠️
-# evalplus.evaluate --dataset humaneval --samples samples.jsonl
-```
+> **Warning** ⚠️ Do you use a very slow machine?
+>
+> LLM solutions are regarded as **failed** on timeout (and OOM etc.).
+> Specifically, we set the timeout $T=\max(T_{base}, T_{gt}\times k)$, where:
+>
+> - $T_{base}$ is the minimal timeout (configurable by `--min-time-limit`; default to 0.2s);
+> - $T_{gt}$ is the runtime of the ground-truth solutions (achieved via profiling);
+> - $k$ is a configurable factor `--gt-time-limit-factor` (default to 4);
+>
+> If your machine is too slow and you are getting high-variance results, try to use larger $k$ and $T_{base}$.
+>
+> Additionally, you are **NOT** encouraged to make your test-bed over stressed while running evaluation.
+> For example, using `--parallel 64` on a 4-core machine or doing something else during evaluation are bad ideas...
 
-<details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
+<details><summary>🤔 Evaluate with local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
+export PYTHONPATH=$PYTHONPATH:$(pwd)
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
 </div>
 </details>
 
 <details><summary>⌨️ More command-line flags <i>:: click to expand ::</i></summary>
@@ -142,28 +151,14 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
-<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
-<div>
-
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
-Here are some tips to speed up the evaluation:
-
-* Use `--parallel $(nproc)`
-* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
-* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
-* We will release an distilled version of HumanEval+ soon. Stay tuned!
-
-</div>
-</details>
-
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
@@ -176,14 +171,36 @@
 ```
 
 - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do **NOT** use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (700+ on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* Use HumanEval+ Mini
+
+</div>
+</details>
+
+> 🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests without fail-stop with `--test-details`).
+>
+> ```bash
+> docker run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples samples.jsonl --mini
+> # ...Or locally ⚠️
+> # evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini
+> ```
+
 ### MBPP+ (TBD)
 
 
 ## 💻 LLM-generated code
 
 Please kindly find the LLM-pre-generated code samples [in the attachment of our v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0).
 Each sample file is packaged in a zip file named like `${model_name}_temp_${temperature}.zip`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.5 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.6 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
 [https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
@@ -22,89 +22,101 @@
 (./gallary/overview.png) ## ð¥ Quick Start To get started, please first setup
 the environment: ```bash pip install evalplus --upgrade ``` ...Or you can try
 out the latest developing version: ```bash pip install "git+https://github.com/
 evalplus/evalplus.git" --upgrade ``` ð¤ Want to use local GitHub repo? ::
 click to expand ::
 ```bash git clone https://github.com/evalplus/evalplus.git cd evalplus export
 PYTHONPATH=$PYTHONPATH:$(pwd) pip install -r requirements.txt ```
- ### HumanEval+ The usage is just like the original HumanEval where you just
-need to implement the `generate_one_completion` function! ```python from
-evalplus.data import get_human_eval_plus, write_jsonl problems =
-get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
+ ### HumanEval+ #### Generate Code Samples The usage is just like the original
+HumanEval where you just need to implement the `generate_one_completion`
+function! ```python from evalplus.data import get_human_eval_plus, write_jsonl
+problems = get_human_eval_plus() num_samples_per_task = 200 samples = [ dict
 (task_id=task_id, completion=generate_one_completion(problems[task_id]
 ["prompt"])) for task_id in problems for _ in range(num_samples_per_task) ]
 write_jsonl("samples.jsonl", samples) ``` ð¤ What is in a `problem`? :: click
 to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is name of
 the function * `prompt` is the function signature with docstring +
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
- To evaluate the samples: You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
-out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
-with the highest quality, achieving almost the same effectiveness of the full
-version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
-you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
-app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
-...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
-samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
-```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
-```
+ #### Evaluate Code Samples with HumanEval+ You are strongly recommended to use
+a sandbox such as [docker](https://docs.docker.com/get-docker/): ```bash docker
+run -v $(pwd):/app ganler/evalplus:latest --dataset humaneval --samples
+samples.jsonl ``` ...Or if you want to try it locally regardless of the risks
+â ï¸: ```bash evalplus.evaluate --dataset humaneval --samples samples.jsonl
+``` > **Warning** â ï¸ Do you use a very slow machine? > > LLM solutions are
+regarded as **failed** on timeout (and OOM etc.). > Specifically, we set the
+timeout $T=\max(T_{base}, T_{gt}\times k)$, where: > > - $T_{base}$ is the
+minimal timeout (configurable by `--min-time-limit`; default to 0.2s); > - $T_
+{gt}$ is the runtime of the ground-truth solutions (achieved via profiling); >
+- $k$ is a configurable factor `--gt-time-limit-factor` (default to 4); > > If
+your machine is too slow and you are getting high-variance results, try to use
+larger $k$ and $T_{base}$. > > Additionally, you are **NOT** encouraged to make
+your test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... ð¤ Evaluate with local GitHub repo? :: click to expand ::
+```bash export PYTHONPATH=$PYTHONPATH:$(pwd) python evalplus/evaluate.py --
+dataset humaneval --samples samples.jsonl ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
- ð¤ How long it would take? :: click to expand ::
-When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
-8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
-speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
-details` if you just want to quickly get pass@k as `--test-details` will run
-all tests (~775 on average for each task), while without `--test-details` the
-testing for a sample stops immediately when it fails the first test. * Use our
-pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
-will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
 - The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be
 used - A cache file named like `samples_eval_results.jsonl` will be cached.
-Remove it to re-run the evaluation ### MBPP+ (TBD) ## ð» LLM-generated code
-Please kindly find the LLM-pre-generated code samples [in the attachment of our
-v0.1.0 release](https://github.com/evalplus/evalplus/releases/tag/v0.1.0). Each
-sample file is packaged in a zip file named like `${model_name}_temp_$
-{temperature}.zip`. You can unzip them to a folder named like `$
-{model_name}_temp_${temperature}` and run the evaluation from scratch with:
-```bash evalplus.evaluate --dataset humaneval --samples ${model_name}_temp_$
-{temperature} ``` ## ð Papers Read our [**paper**](https://arxiv.org/abs/
-2305.01210) for more detailed findings! ```bibtex @article{evalplus, title={Is
-Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large
-Language Models for Code Generation}, author={Jiawei Liu and Chunqiu Steven Xia
-and Yuyao Wang and Lingming Zhang}, journal={arXiv preprint arXiv:2305.01210},
-year={2023}, } ``` ## ð¨ Useful tools To use these tools, please first
-install the repository from GitHub: ```bash git clone https://github.com/
-evalplus/evalplus.git cd evalplus pip install -r requirements-tools.txt ``` ###
-Syntax checker for LLM-generated code Check LLM-produced code and answer the
-following questions: 1. Is the generation entirely done for all samples / all
-problems in the dataset? 2. Are LLM-generated code compilable? (if no,
-something could be wrong and you'd better check) ```shell python tools/
-checker.py --folder /path/to/[model]-[??]b_temp_[??] --dataset humaneval ```
-### Post code sanitizer LLM-generated code may contain some syntax errors. But
-some of them can be easily fixable by doing simple post-processing. This tool
-will make the LLM-generated code more clean/compilable by doing certain post-
-processing such as trimming with more magical EOFs and some garbage non-code
-tokens. ```shell python tools/sanitize.py --eof --folder /path/to/vicuna-
-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/vicuna-
-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to `rich` and LaTeX
-tables ```shell python tools/render.py --type /path/to/[model]-[??]b # NOTE: no
-`_temp_[??]` ``` ![](./gallary/render.gif) ### Perform test input generation
-from scratch (TBD) ## ð· Development Before you start: ```bash pip install
-pre-commit pre-commit install export PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name
-convention - `evalplus` is the package name. - `${DATASET}_plus` is the name of
-dataset applied with `evalplus`. ## ð Acknowledgement - [HumanEval](https://
-github.com/openai/human-eval)
+Remove it to re-run the evaluation ð¤ How long it would take? :: click to
+expand ::
+When running 200 samples x 164 tasks x ~700+ tests, it can take around 2-10
+minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do **NOT** use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (700+ on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * Use
+HumanEval+ Mini
+ > ð **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of
+additional tests with the highest quality, achieving almost the same
+effectiveness of the full version. Just add a **`--mini`** flag, it can run
+23+% faster! (even faster if you evaluate all tests without fail-stop with `--
+test-details`). > > ```bash > docker run -v $(pwd):/app ganler/evalplus:latest
+--dataset humaneval --samples samples.jsonl --mini > # ...Or locally â ï¸ > #
+evalplus.evaluate --dataset humaneval --samples samples.jsonl --mini > ``` ###
+MBPP+ (TBD) ## ð» LLM-generated code Please kindly find the LLM-pre-generated
+code samples [in the attachment of our v0.1.0 release](https://github.com/
+evalplus/evalplus/releases/tag/v0.1.0). Each sample file is packaged in a zip
+file named like `${model_name}_temp_${temperature}.zip`. You can unzip them to
+a folder named like `${model_name}_temp_${temperature}` and run the evaluation
+from scratch with: ```bash evalplus.evaluate --dataset humaneval --samples $
+{model_name}_temp_${temperature} ``` ## ð Papers Read our [**paper**](https:
+//arxiv.org/abs/2305.01210) for more detailed findings! ```bibtex @article
+{evalplus, title={Is Your Code Generated by ChatGPT Really Correct? Rigorous
+Evaluation of Large Language Models for Code Generation}, author={Jiawei Liu
+and Chunqiu Steven Xia and Yuyao Wang and Lingming Zhang}, journal={arXiv
+preprint arXiv:2305.01210}, year={2023}, } ``` ## ð¨ Useful tools To use
+these tools, please first install the repository from GitHub: ```bash git clone
+https://github.com/evalplus/evalplus.git cd evalplus pip install -
+r requirements-tools.txt ``` ### Syntax checker for LLM-generated code Check
+LLM-produced code and answer the following questions: 1. Is the generation
+entirely done for all samples / all problems in the dataset? 2. Are LLM-
+generated code compilable? (if no, something could be wrong and you'd better
+check) ```shell python tools/checker.py --folder /path/to/[model]-[??]b_temp_
+[??] --dataset humaneval ``` ### Post code sanitizer LLM-generated code may
+contain some syntax errors. But some of them can be easily fixable by doing
+simple post-processing. This tool will make the LLM-generated code more clean/
+compilable by doing certain post-processing such as trimming with more magical
+EOFs and some garbage non-code tokens. ```shell python tools/sanitize.py --eof
+--folder /path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to
+`/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ### Render `pass@k` results to
+`rich` and LaTeX tables ```shell python tools/render.py --type /path/to/
+[model]-[??]b # NOTE: no `_temp_[??]` ``` ![](./gallary/render.gif) ### Perform
+test input generation from scratch (TBD) ## ð· Development Before you start:
+```bash pip install pre-commit pre-commit install export
+PYTHONPATH=$PYTHONPATH:$(pwd) ``` ### Name convention - `evalplus` is the
+package name. - `${DATASET}_plus` is the name of dataset applied with
+`evalplus`. ## ð Acknowledgement - [HumanEval](https://github.com/openai/
+human-eval)
```

### Comparing `evalplus-0.1.5/evalplus.egg-info/SOURCES.txt` & `evalplus-0.1.6/evalplus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,8 +51,10 @@
 tools/sanitize.py
 tools/stat_plus.py
 tools/viz_passrate.py
 tools/_experimental/README.md
 tools/_experimental/set_cover.py
 tools/_experimental/topset_distill.py
 tools/humaneval/check_ground_truth.py
+tools/humaneval/fix_v011.py
+tools/humaneval/fix_v012.py
 tools/humaneval/init_plus.py
```

### Comparing `evalplus-0.1.5/evo.sh` & `evalplus-0.1.6/evo.sh`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/gallary/overview.png` & `evalplus-0.1.6/gallary/overview.png`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/gallary/render.gif` & `evalplus-0.1.6/gallary/render.gif`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/setup.cfg` & `evalplus-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/_experimental/set_cover.py` & `evalplus-0.1.6/tools/_experimental/set_cover.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/_experimental/topset_distill.py` & `evalplus-0.1.6/tools/_experimental/topset_distill.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/checker.py` & `evalplus-0.1.6/tools/checker.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/filter_inputs.py` & `evalplus-0.1.6/tools/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/humaneval/check_ground_truth.py` & `evalplus-0.1.6/tools/humaneval/check_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/humaneval/init_plus.py` & `evalplus-0.1.6/tools/humaneval/init_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/init_ground_truth.py` & `evalplus-0.1.6/tools/init_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/merge_dataset.py` & `evalplus-0.1.6/tools/merge_dataset.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/render.py` & `evalplus-0.1.6/tools/render.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/sanitize.py` & `evalplus-0.1.6/tools/sanitize.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/stat_plus.py` & `evalplus-0.1.6/tools/stat_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/tools/viz_passrate.py` & `evalplus-0.1.6/tools/viz_passrate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.5/zipper.sh` & `evalplus-0.1.6/zipper.sh`

 * *Files identical despite different names*

