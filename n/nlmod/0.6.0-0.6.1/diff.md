# Comparing `tmp/nlmod-0.6.0.tar.gz` & `tmp/nlmod-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlmod-0.6.0.tar", last modified: Wed Jun  7 19:39:43 2023, max compression
+gzip compressed data, was "nlmod-0.6.1.tar", last modified: Mon Jun 26 12:35:14 2023, max compression
```

## Comparing `nlmod-0.6.0.tar` & `nlmod-0.6.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.218493 nlmod-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 19:39:28.000000 nlmod-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 19:39:43.218493 nlmod-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-07 19:39:28.000000 nlmod-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/cache_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/generate_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 19:39:28.000000 nlmod-0.6.0/docs/examples/run_all_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)  1860872 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/bin/mp7_2_002_provisional
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.202493 nlmod-0.6.0/nlmod/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.202493 nlmod-0.6.0/nlmod/data/geotop/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/geo_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/geotop/litho_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/regis_2_2.gleg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.206493 nlmod-0.6.0/nlmod/data/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.cpg
--rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.prj
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.qpj
--rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.shp
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/data/shapes/opp_water.shx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/dims/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    56949 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/dims/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/gwf/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/gwf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/horizontal_flow_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/lake.py
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36621 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwf/wells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/gwt/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/gwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/gwt/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/mfoutput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/modpath/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/modpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/modpath/modpath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.210493 nlmod-0.6.0/nlmod/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/dcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/flopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/plot/plotutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.214493 nlmod-0.6.0/nlmod/read/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/ahn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/bgt.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/brp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/jarkus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/knmi_data_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/meteobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/regis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/rws.py
--rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/waterboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/read/webservices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.214493 nlmod-0.6.0/nlmod/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/sim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 19:39:28.000000 nlmod-0.6.0/nlmod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.198493 nlmod-0.6.0/nlmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:39:43.000000 nlmod-0.6.0/nlmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-07 19:39:28.000000 nlmod-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:39:43.218493 nlmod-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:39:43.218493 nlmod-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_001_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_002_regis_geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_003_mfpackages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_004_northsea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_005_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_006_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_007_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_008_waterschappen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_009_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_010_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_011_dcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_012_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_013_surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_014_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_015_gwf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_016_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_017_metbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/test_018_knmi_data_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 19:39:28.000000 nlmod-0.6.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.575728 nlmod-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 12:35:03.000000 nlmod-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-26 12:35:14.575728 nlmod-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 12:35:03.000000 nlmod-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.559728 nlmod-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-26 12:35:03.000000 nlmod-0.6.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 12:35:03.000000 nlmod-0.6.1/docs/examples/cache_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-26 12:35:03.000000 nlmod-0.6.1/docs/examples/generate_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-26 12:35:03.000000 nlmod-0.6.1/docs/examples/run_all_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/nlmod/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/nlmod/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1860872 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/bin/mp7_2_002_provisional
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/nlmod/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/nlmod/data/geotop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/geotop/geo_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/geotop/litho_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/regis_2_2.gleg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.567728 nlmod-0.6.1/nlmod/data/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.qpj
+-rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/data/shapes/opp_water.shx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.571728 nlmod-0.6.1/nlmod/dims/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21563 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57644 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35657 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/dims/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.571728 nlmod-0.6.1/nlmod/gwf/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/gwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/horizontal_flow_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36621 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwf/wells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.571728 nlmod-0.6.1/nlmod/gwt/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwt/gwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/gwt/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/mfoutput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.571728 nlmod-0.6.1/nlmod/modpath/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/modpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/modpath/modpath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.571728 nlmod-0.6.1/nlmod/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/plot/dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/plot/flopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/plot/plotutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.575728 nlmod-0.6.1/nlmod/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/ahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/bgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/brp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/jarkus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/knmi_data_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/meteobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/regis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/rws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/waterboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/read/webservices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.575728 nlmod-0.6.1/nlmod/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/sim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 12:35:03.000000 nlmod-0.6.1/nlmod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.563727 nlmod-0.6.1/nlmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-26 12:35:14.000000 nlmod-0.6.1/nlmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-26 12:35:14.000000 nlmod-0.6.1/nlmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:35:14.000000 nlmod-0.6.1/nlmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 12:35:14.000000 nlmod-0.6.1/nlmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 12:35:14.000000 nlmod-0.6.1/nlmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-26 12:35:03.000000 nlmod-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:35:14.575728 nlmod-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:35:14.575728 nlmod-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_001_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_002_regis_geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_003_mfpackages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_004_northsea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_005_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_006_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_007_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_008_waterschappen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_009_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_010_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_011_dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_012_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_013_surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_014_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_015_gwf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_016_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_017_metbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/test_018_knmi_data_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 12:35:03.000000 nlmod-0.6.1/tests/util.py
```

### Comparing `nlmod-0.6.0/LICENSE` & `nlmod-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/PKG-INFO` & `nlmod-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.6.0
+Version: 0.6.1
 Summary: nlmod is an open-source Python package for building Modflow 6 groundwater models from online data sources in The Netherlands
 Author: O. Ebbens, R. Caljé, D.A. Brakenhoff
 Maintainer-email: "O. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.N. Ebbens, D.A. Brakenhoff, R. Calje
```

### Comparing `nlmod-0.6.0/README.md` & `nlmod-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/docs/conf.py` & `nlmod-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/docs/examples/generate_logo.py` & `nlmod-0.6.1/docs/examples/generate_logo.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/docs/examples/run_all_notebooks.py` & `nlmod-0.6.1/docs/examples/run_all_notebooks.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/bin/mp7_2_002_provisional` & `nlmod-0.6.1/nlmod/bin/mp7_2_002_provisional`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/cache.py` & `nlmod-0.6.1/nlmod/cache.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/geotop/geo_eenheden.csv` & `nlmod-0.6.1/nlmod/data/geotop/geo_eenheden.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv` & `nlmod-0.6.1/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/regis_2_2.gleg` & `nlmod-0.6.1/nlmod/data/regis_2_2.gleg`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/shapes/opp_water.dbf` & `nlmod-0.6.1/nlmod/data/shapes/opp_water.dbf`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/shapes/opp_water.qpj` & `nlmod-0.6.1/nlmod/data/shapes/opp_water.qpj`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/data/shapes/opp_water.shp` & `nlmod-0.6.1/nlmod/data/shapes/opp_water.shp`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/dims/base.py` & `nlmod-0.6.1/nlmod/dims/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,19 +315,23 @@
     resample._set_angrot_attributes(extent, xorigin, yorigin, angrot, attrs)
 
     coords = {
         "x": xcenters,
         "y": ycenters,
         "layer": range(nlay),
     }
+
     if angrot != 0.0:
         affine = resample.get_affine_mod_to_world(attrs)
         xc, yc = affine * np.meshgrid(xcenters, ycenters)
         coords["xc"] = (("y", "x"), xc)
         coords["yc"] = (("y", "x"), yc)
+    else:
+        coords["x"] += xorigin
+        coords["y"] += yorigin
 
     dims = ("layer", "y", "x")
     ds = xr.Dataset(
         data_vars={
             "top": (dims[1:], top),
             "botm": (dims, botm),
         },
@@ -435,15 +439,15 @@
     )
 
     if isinstance(nlay, int):
         layers = range(nlay)
     else:
         layers = nlay
 
-    coords = {"x": x, "y": y, "layer": layers}
+    coords = {"layer": layers, "y": y, "x": x}
     dims = ("layer", "icell2d")
     ds = xr.Dataset(
         data_vars=dict(
             top=(dims[1:], top),
             botm=(dims, botm),
         ),
         coords=coords,
```

### Comparing `nlmod-0.6.0/nlmod/dims/grid.py` & `nlmod-0.6.1/nlmod/dims/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1054,21 +1054,30 @@
 
     if gdf_cellid.cellid.duplicated().any():
         # aggregate data
         if agg_method is None:
             raise ValueError(
                 "multiple geometries in one cell please define aggregation method"
             )
-        gdf_agg = aggregate_vector_per_cell(gdf_cellid, {column: agg_method})
+        if agg_method in ["nearest"]:
+            modelgrid = modelgrid_from_ds(ds)
+            gdf_agg = aggregate_vector_per_cell(
+                gdf_cellid, {column: agg_method}, modelgrid
+            )
+        else:
+            gdf_agg = aggregate_vector_per_cell(gdf_cellid, {column: agg_method})
     else:
         # aggregation not neccesary
         gdf_agg = gdf_cellid[[column]]
-        gdf_agg.set_index(
-            pd.MultiIndex.from_tuples(gdf_cellid.cellid.values), inplace=True
-        )
+        if isinstance(gdf_cellid.cellid.iloc[0], tuple):
+            gdf_agg.set_index(
+                pd.MultiIndex.from_tuples(gdf_cellid.cellid.values), inplace=True
+            )
+        else:
+            gdf_agg.set_index(gdf_cellid.cellid.values, inplace=True)
     da = util.get_da_from_da_ds(ds, dims=ds.top.dims, data=fill_value)
     for ind, row in gdf_agg.iterrows():
         da.values[ind] = row[column]
     da.attrs["_FillValue"] = fill_value
     return da
 
 
@@ -1131,40 +1140,45 @@
 
 def _agg_length_weighted(gdf, col):
     nanmask = gdf[col].isna()
     aw = (gdf.length * gdf[col]).sum(skipna=True) / gdf.loc[~nanmask].length.sum()
     return aw
 
 
-def _agg_nearest(gdf, col, gwf):
-    cid = gdf["cellid"].values[0]
-    cellcenter = Point(
-        gwf.modelgrid.xcellcenters[0][cid[1]],
-        gwf.modelgrid.ycellcenters[:, 0][cid[0]],
-    )
-    val = gdf.iloc[gdf.distance(cellcenter).argmin()].loc[col]
+def _agg_nearest(gdf, col, modelgrid):
+    if modelgrid.grid_type == "structured":
+        cid = gdf["cellid"].values[0]
+        cellcenter = Point(
+            modelgrid.xcellcenters[0, cid[1]], modelgrid.ycellcenters[cid[0], 0]
+        )
+        val = gdf.iloc[gdf.distance(cellcenter).argmin()].loc[col]
+    elif modelgrid.grid_type == "vertex":
+        cid = gdf["cellid"].values[0]
+        cellcenter = Point(modelgrid.xcellcenters[cid], modelgrid.ycellcenters[cid])
+        val = gdf.iloc[gdf.distance(cellcenter).argmin()].loc[col]
+
     return val
 
 
-def _get_aggregates_values(group, fields_methods, gwf=None):
+def _get_aggregates_values(group, fields_methods, modelgrid=None):
     agg_dic = {}
     for field, method in fields_methods.items():
         # aggregation is only necesary if group shape is greater than 1
         if (group.shape[0] == 1) or (method == "first"):
             agg_dic[field] = group[field].values[0]
         elif method == "max":
             agg_dic[field] = group[field].max()
         elif method == "min":
             agg_dic[field] = group[field].min()
         elif method == "mean":
             agg_dic[field] = group[field].mean()
         elif method == "sum":
             agg_dic[field] = group[field].sum()
         elif method == "nearest":
-            agg_dic[field] = _agg_nearest(group, field, gwf)
+            agg_dic[field] = _agg_nearest(group, field, modelgrid)
         elif method == "length_weighted":  # only for lines
             agg_dic[field] = _agg_length_weighted(group, field)
         elif method == "max_length":  # only for lines
             agg_dic[field] = _agg_max_length(group, field)
         elif method == "area_weighted":  # only for polygons
             agg_dic[field] = _agg_area_weighted(group, field)
         elif method == "max_area":  # only for polygons
@@ -1173,27 +1187,27 @@
             raise NotImplementedError
         else:
             raise ValueError(f"Method '{method}' not recognized!")
 
     return agg_dic
 
 
-def aggregate_vector_per_cell(gdf, fields_methods, gwf=None):
+def aggregate_vector_per_cell(gdf, fields_methods, modelgrid=None):
     """Aggregate vector features per cell.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         GeoDataFrame containing points, lines or polygons per grid cell.
     fields_methods: dict
         fields (keys) in the Geodataframe with their aggregation method (items)
         aggregation methods can be:
         max, min, mean, sum, length_weighted (lines), max_length (lines),
         area_weighted (polygon), max_area (polygon).
-    gwf : flopy Groundwater flow model
+    modelgrid : flopy Groundwater flow modelgrid
         only necesary if one of the field methods is 'nearest'
 
     Returns
     -------
     celldata : pd.DataFrame
         DataFrame with aggregated surface water parameters per grid cell
     """
@@ -1223,15 +1237,15 @@
     if len(missing_cols) > 0:
         raise ValueError(f"Missing columns in DataFrame: {missing_cols}")
 
     # aggregate data
     gr = gdf.groupby(by="cellid")
     celldata = pd.DataFrame(index=gr.groups.keys())
     for cid, group in tqdm(gr, desc="Aggregate vector data"):
-        agg_dic = _get_aggregates_values(group, fields_methods, gwf)
+        agg_dic = _get_aggregates_values(group, fields_methods, modelgrid)
         for key, item in agg_dic.items():
             celldata.loc[cid, key] = item
 
     return celldata
 
 
 def gdf_to_bool_da(gdf, ds):
```

### Comparing `nlmod-0.6.0/nlmod/dims/layers.py` & `nlmod-0.6.1/nlmod/dims/layers.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/dims/rdp.py` & `nlmod-0.6.1/nlmod/dims/rdp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/dims/resample.py` & `nlmod-0.6.1/nlmod/dims/resample.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/dims/time.py` & `nlmod-0.6.1/nlmod/dims/time.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gis.py` & `nlmod-0.6.1/nlmod/gis.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/gwf.py` & `nlmod-0.6.1/nlmod/gwf/gwf.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/horizontal_flow_barrier.py` & `nlmod-0.6.1/nlmod/gwf/horizontal_flow_barrier.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/lake.py` & `nlmod-0.6.1/nlmod/gwf/lake.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/output.py` & `nlmod-0.6.1/nlmod/gwf/output.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/recharge.py` & `nlmod-0.6.1/nlmod/gwf/recharge.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/surface_water.py` & `nlmod-0.6.1/nlmod/gwf/surface_water.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwf/wells.py` & `nlmod-0.6.1/nlmod/gwf/wells.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwt/gwt.py` & `nlmod-0.6.1/nlmod/gwt/gwt.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwt/output.py` & `nlmod-0.6.1/nlmod/gwt/output.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/gwt/prepare.py` & `nlmod-0.6.1/nlmod/gwt/prepare.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/mfoutput.py` & `nlmod-0.6.1/nlmod/mfoutput.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/modpath/modpath.py` & `nlmod-0.6.1/nlmod/modpath/modpath.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/plot/dcs.py` & `nlmod-0.6.1/nlmod/plot/dcs.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/plot/flopy.py` & `nlmod-0.6.1/nlmod/plot/flopy.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/plot/plot.py` & `nlmod-0.6.1/nlmod/plot/plot.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/plot/plotutil.py` & `nlmod-0.6.1/nlmod/plot/plotutil.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/ahn.py` & `nlmod-0.6.1/nlmod/read/ahn.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/bgt.py` & `nlmod-0.6.1/nlmod/read/bgt.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/brp.py` & `nlmod-0.6.1/nlmod/read/brp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/geotop.py` & `nlmod-0.6.1/nlmod/read/geotop.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/jarkus.py` & `nlmod-0.6.1/nlmod/read/jarkus.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/knmi.py` & `nlmod-0.6.1/nlmod/read/knmi.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/knmi_data_platform.py` & `nlmod-0.6.1/nlmod/read/knmi_data_platform.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/meteobase.py` & `nlmod-0.6.1/nlmod/read/meteobase.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/regis.py` & `nlmod-0.6.1/nlmod/read/regis.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/rws.py` & `nlmod-0.6.1/nlmod/read/rws.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/waterboard.py` & `nlmod-0.6.1/nlmod/read/waterboard.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/read/webservices.py` & `nlmod-0.6.1/nlmod/read/webservices.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/sim/sim.py` & `nlmod-0.6.1/nlmod/sim/sim.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/util.py` & `nlmod-0.6.1/nlmod/util.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod/version.py` & `nlmod-0.6.1/nlmod/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import metadata
 from platform import python_version
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
 def show_versions() -> None:
     """Method to print the version of dependencies."""
 
     msg = (
         f"Python version: {python_version()}\n"
```

### Comparing `nlmod-0.6.0/nlmod.egg-info/PKG-INFO` & `nlmod-0.6.1/nlmod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.6.0
+Version: 0.6.1
 Summary: nlmod is an open-source Python package for building Modflow 6 groundwater models from online data sources in The Netherlands
 Author: O. Ebbens, R. Caljé, D.A. Brakenhoff
 Maintainer-email: "O. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.N. Ebbens, D.A. Brakenhoff, R. Calje
```

### Comparing `nlmod-0.6.0/nlmod.egg-info/SOURCES.txt` & `nlmod-0.6.1/nlmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/nlmod.egg-info/requires.txt` & `nlmod-0.6.1/nlmod.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/pyproject.toml` & `nlmod-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_001_model.py` & `nlmod-0.6.1/tests/test_001_model.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_002_regis_geotop.py` & `nlmod-0.6.1/tests/test_002_regis_geotop.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_003_mfpackages.py` & `nlmod-0.6.1/tests/test_003_mfpackages.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_004_northsea.py` & `nlmod-0.6.1/tests/test_004_northsea.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_005_external_data.py` & `nlmod-0.6.1/tests/test_005_external_data.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_006_caching.py` & `nlmod-0.6.1/tests/test_006_caching.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_007_run_notebooks.py` & `nlmod-0.6.1/tests/test_007_run_notebooks.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_008_waterschappen.py` & `nlmod-0.6.1/tests/test_008_waterschappen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Created on Tue Aug 16 10:29:13 2022.
 
 @author: Ruben
 """
 
 import pytest
-
+import matplotlib
 import nlmod
 
 
 def test_download_polygons():
     nlmod.read.waterboard.get_polygons()
 
 
@@ -44,21 +44,31 @@
             if str(e) == f"{data_kind} not available for {wb}":
                 print(e)
             else:
                 raise
 
     if plot:
         # plot the winter_stage
-        ax = waterboards.plot(edgecolor="k", facecolor="none")
+        f, ax = nlmod.plot.get_map([9000, 279000, 304000, 623000], base=100000)
+        waterboards.plot(edgecolor="k", facecolor="none", ax=ax)
+        norm = matplotlib.colors.Normalize(-10.0, 20.0)
+        cmap = "viridis"
         for wb in waterboards.index:
             if wb in gdf:
                 # gdf[wb].plot(ax=ax, zorder=0)
-                gdf[wb].plot("winter_stage", ax=ax, zorder=0, vmin=-10, vmax=20)
+                gdf[wb].plot("winter_stage", ax=ax, zorder=0, norm=norm, cmap=cmap)
             c = waterboards.at[wb, "geometry"].centroid
             ax.text(c.x, c.y, wb.replace(" ", "\n"), ha="center", va="center")
+        nlmod.plot.colorbar_inside(
+            ax=ax,
+            norm=norm,
+            cmap=cmap,
+            bounds=[0.05, 0.55, 0.02, 0.4],
+            label="Summer stage (m NAP)",
+        )
 
 
 @pytest.mark.skip("too slow")
 def test_download_waterlopen(plot=True):
     def get_extent(waterboards, wb, buffer=1000.0):
         c = waterboards.at[wb, "geometry"].centroid
         extent = [c.x - buffer, c.x + buffer, c.y - buffer, c.y + buffer]
```

### Comparing `nlmod-0.6.0/tests/test_009_layers.py` & `nlmod-0.6.1/tests/test_009_layers.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_010_wells.py` & `nlmod-0.6.1/tests/test_010_wells.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_012_plot.py` & `nlmod-0.6.1/tests/test_012_plot.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_013_surface_water.py` & `nlmod-0.6.1/tests/test_013_surface_water.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_015_gwf_output.py` & `nlmod-0.6.1/tests/test_015_gwf_output.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/test_018_knmi_data_platform.py` & `nlmod-0.6.1/tests/test_018_knmi_data_platform.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.6.0/tests/util.py` & `nlmod-0.6.1/tests/util.py`

 * *Files identical despite different names*

