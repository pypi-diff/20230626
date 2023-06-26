# Comparing `tmp/scitools-iris-3.6.0rc0.tar.gz` & `tmp/scitools-iris-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitools-iris-3.6.0rc0.tar", last modified: Wed May  3 12:45:29 2023, max compression
+gzip compressed data, was "scitools-iris-3.6.1.tar", last modified: Mon Jun 26 15:15:52 2023, max compression
```

## Comparing `scitools-iris-3.6.0rc0.tar` & `scitools-iris-3.6.1.tar`

### file list

```diff
@@ -1,1785 +1,1788 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.362249 scitools-iris-3.6.0rc0/etc/
--rw-r--r--   0 runner    (1001) docker     (123)  4146252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/etc/cf-standard-name-table.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.362249 scitools-iris-3.6.0rc0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.370249 scitools-iris-3.6.0rc0/lib/iris/
--rw-r--r--   0 runner    (1001) docker     (123)    15747 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48480 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    62576 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.370249 scitools-iris-3.6.0rc0/lib/iris/_representation/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_representation/cube_printout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/_representation/cube_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 12:45:28.000000 scitools-iris-3.6.0rc0/lib/iris/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.374249 scitools-iris-3.6.0rc0/lib/iris/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)   111456 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39662 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/_area_weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/_grid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    25855 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41206 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/_regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/_scipy_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27924 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)    44792 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/cartography.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    36712 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/analysis/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)    69935 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/aux_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.374249 scitools-iris-3.6.0rc0/lib/iris/common/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/common/lenient.py
--rw-r--r--   0 runner    (1001) docker     (123)    53861 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/common/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/common/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   106896 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/common/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/coord_categorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    51390 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/coord_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)   112347 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)   177271 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.374249 scitools-iris-3.6.0rc0/lib/iris/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.330248 scitools-iris-3.6.0rc0/lib/iris/etc/palette/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.374249 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/BrBG_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PRGn_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PiYG_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PuOr_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdBu_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdGy_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdYlBu_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdYlGn_11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/Spectral_11.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.374249 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Accent_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Dark2_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Paired_12.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Pastel1_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Pastel2_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set1_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set2_08.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set3_12.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.378249 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Blues_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/BuGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/BuPu_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/GnBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Greens_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Greys_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/OrRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Oranges_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuBuGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Purples_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/RdPu_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Reds_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlGnBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlOrBr_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlOrRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/etc/site.cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.378249 scitools-iris-3.6.0rc0/lib/iris/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    27240 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/regrid_conservative.py
--rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/stratify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.378249 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/load.py
--rw-r--r--   0 runner    (1001) docker     (123)   110761 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/fileformats/
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31932 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)   196094 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_ff_cross_references.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_pp_lbproc_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/_structured_array_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/abf.py
--rw-r--r--   0 runner    (1001) docker     (123)    47602 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    44205 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/name_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/_dask_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/_thread_safe_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21742 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   112867 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/nimrod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/nimrod_load_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/pp.py
--rw-r--r--   0 runner    (1001) docker     (123)    47347 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/pp_load_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    30774 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/pp_save_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_fast_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_fast_load_structured_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_ff_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_optimal_array_structuring.py
--rw-r--r--   0 runner    (1001) docker     (123)   107325 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/fileformats/um_cf_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/io/
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/io/format_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    35983 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    71011 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.382249 scitools-iris-3.6.0rc0/lib/iris/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/quickplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.386249 scitools-iris-3.6.0rc0/lib/iris/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.394249 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.394249 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23476 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    30235 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/experimental/test_raster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.394249 scitools-iris-3.6.0rc0/lib/iris/tests/graphics/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2166 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/graphics/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     8901 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/graphics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6853 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/graphics/idiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2452 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/graphics/recreate_imagerepo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.402249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.402249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/analysis/test_area_weighted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.402249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/aux_factory/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/aux_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.402249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/concatenate/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/concatenate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/concatenate/test_concatenate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.406249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_ugrid_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_ugrid_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.410249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.410249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/fast_load/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/fast_load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27952 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/fast_load/test_fast_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.410249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/merge/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/merge/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.414249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test__dask_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_aux_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_coord_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_delayed_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_self_referencing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_thread_safety.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.418249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_netcdftime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_nzdateline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_plot_2d_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_vector_plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1556 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_Datums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_PartialDateTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_climatology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_new_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_regrid_equivalence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_regridding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.418249 scitools-iris-3.6.0rc0/lib/iris/tests/integration/um/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/um/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/integration/um/test_fieldsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/pp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.422248 scitools-iris-3.6.0rc0/lib/iris/tests/results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.422248 scitools-iris-3.6.0rc0/lib/iris/tests/results/COLPEX/
--rw-r--r--   0 runner    (1001) docker     (123)    37400 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.422248 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/air_temperature_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/air_temperature_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/ffheader.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/soil_temperature_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/surface_altitude_1.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.422248 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_char_data.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)   330620 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_x_data.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/global_test.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/nae_unpacked.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/rle_unpacked.pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.422248 scitools-iris-3.6.0rc0/lib/iris/tests/results/abf/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/abf/load.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.438248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/abs.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_coord_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_coord_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_different_std_name.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_in_place.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_in_place_coord.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_scalar.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.442248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/easy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/areaweights_original.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.442248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/cos_simple.xml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/cos_simple_radians.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.446248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.446248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/delta_one_element_explicit.xml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/midpoint_one_element_explicit.xml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1.cml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_delta.cml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_delta.cml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_delta.cml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4.cml
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_delta.cml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5.cml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_delta.cml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple6.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_array.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_singular_coord.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_scalar.cml
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exp.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exp.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exponentiate.cml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exponentiate.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log10.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log10.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/maths_original.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/multiply.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/multiply_different_std_name.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original_common.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original_hmean.cml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.450248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_weighted_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.450248 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.rlat.json
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.rlon.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.x.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.y.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.rlat.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.rlon.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.x.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.y.json
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sqrt.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_array.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_coord_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_coord_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_scalar.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_weighted_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_weighted_2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.cml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_original.cml
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_source.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.338249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cartography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cartography/get_xy_grids/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cartography/get_xy_grids/1d.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cartography/get_xy_grids/2d.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/categorisation/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/categorisation/customcheck.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/categorisation/quickcheck.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/masked_cube.cml
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/masked_save_pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.454249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/cubelist.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/cubelist.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/simple.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/unicode_attribute.__unicode__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/compatible_cubes.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.458248 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_3d_simple.cml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_anonymous.cml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.462248 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/all_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/attribute_constraint.cml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/invalid_inequality_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/pressure_950_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_load_strict.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.462248 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/complex.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.462248 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/intersection.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/intersection_missing.xml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/intersection_reversed.xml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/minimal.xml
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/nd_bounds.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.466248 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_time_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_time_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_time_repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_time_str.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.466248 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/CoordSystem_xml_element.xml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_invf.xml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_major.xml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_minor.xml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_sphere.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/Mercator.xml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/PolarStereographic.xml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/PolarStereographicScaleFactor.xml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/PolarStereographicStandardParallel.xml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init.xml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_a.xml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_b.xml
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/Stereographic.xml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_systems/TransverseMercator_osgb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.470248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/original.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.342249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.470248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/cubelist.cml
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/single_cube.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/theta.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.470248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pp/load/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pp/load/global.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.474248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_merge.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.474248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_orig.cml
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_transposed.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.474248 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/append_multi.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/append_single.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/replace_multi.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/replace_single.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.478248 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/column.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/no_orog.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/no_orog.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_derived_coord.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_orog.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_orog.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_sigma.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16859 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_sigma.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.478248 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.478248 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/known_loaders.txt
--rw-r--r--   0 runner    (1001) docker     (123)    97746 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/theta_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)    97417 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/u_wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)    97417 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/v_wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)   194764 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/imagerepo.json
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/incompatible_attr.str.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/incompatible_cubes.str.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/incompatible_meth.str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/incompatible_name.str.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/incompatible_unit.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/climatology/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/attributes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_different_saves_on_variables.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_same_saves_as_global.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/single_saves_as_global.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.346249 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.482248 scitools-iris-3.6.0rc0/lib/iris/tests/results/iterate/
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/iterate/izip_nd_ortho.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.486248 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_aux_b_aux.cml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_aux_b_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_dim_b_aux.cml
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_dim_b_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/dec.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/multi_split.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/separable_combination.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/single_split.cml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_b.cml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_with_aux.cml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_with_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_b_with_aux.cml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_b_with_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/theta.cml
--rw-r--r--   0 runner    (1001) docker     (123)    17223 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/theta_two_times.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_independent.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging3.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging4.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging5.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_non_expanding.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_series.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_single_forecast.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.490248 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/
--rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.cml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.2.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.3.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.4.json
--rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.cml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.2.json
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.3.json
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.4.json
--rw-r--r--   0 runner    (1001) docker     (123)    49155 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.cml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.2.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.cml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.data.1.json
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.data.2.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.data.3.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.data.4.json
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.cml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.data.1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.498248 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.498248 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/int64_data_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    24811 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_laea.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_lcc.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_polar.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_conf_aux.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_conf_name.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_confl_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_confl_global_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_name.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_nocoord.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samevar.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_wcoord.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_stereo.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_units_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_units_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/save_load_traj.cml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/uint32_data_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/levels_below_ground.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/load_2flds.cml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/mockography.cml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/period_of_interest.cml
--rw-r--r--   0 runner    (1001) docker     (123)   115358 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/probability_fields.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.350249 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_masked.cml
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_object.cml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_simple.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/global.cml
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/stock/
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/stock/realistic_4d.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/system/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/system/supported_filetype_.nc.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/system/supported_filetype_.pp.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/constant_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/hybrid_height.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/single_point.cml
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/zigzag.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.350249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.502248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.data.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.506248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/checksum_ignores_masked_values.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/embedded_newlines_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/long_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/multi_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/simple_string_attribute.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/stratify/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.354249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/endian.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/noise.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/noise.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/describe_diff/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/describe_diff/incompatible_array_attrs.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.510248 scitools-iris-3.6.0rc0/lib/iris/tests/results/uri_callback/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/uri_callback/pp_global.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.358249 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.514248 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.514248 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.518248 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.518248 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.518248 scitools-iris-3.6.0rc0/lib/iris/tests/stock/
--rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/_stock_2d_latlons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.518248 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/stock/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_abf.py
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_aggregate_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29521 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_analysis_calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)    32895 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_basic_maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cartography.py
--rw-r--r--   0 runner    (1001) docker     (123)    51871 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    16226 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_coding_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    40767 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_coord_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_coord_categorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_coordsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_cube_to_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_file_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_file_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_image_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_io_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_lazy_aggregate_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_nimrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_peak.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_to_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_quickplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_std_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_uri_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.518248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.522248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.522248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/area_weighted/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/area_weighted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.526248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.526248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.526248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.530248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_divide.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.530248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55068 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.534248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.534248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15028 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_AreaWeighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_COUNT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MAX.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MAX_RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MEAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MIN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PERCENTILE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PROPORTION.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PointInCell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_RMS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_STD_DEV.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_SUM.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_VARIANCE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.534248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.538248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.538248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.538248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test_Lenient.py
--rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__Lenient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__qualname.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    57770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    26669 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192764 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/resolve/test_Resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/test__CubeSignature.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/test_concatenate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/config/test_NetCDF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/test_Constraint_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/test_NameConstraint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.542248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_GeogCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Geostationary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Orthographic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8687 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Stereographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26495 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_AncillaryVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_AuxCoord.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_Cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_CellMeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_CellMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_Coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    22368 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_DimCoord.py
--rw-r--r--   0 runner    (1001) docker     (123)    38411 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   133486 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_CubeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube__operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/data_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/data_manager/test_DataManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/raster/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.546248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/stratify/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/stratify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/stratify/test_relevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    49280 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    37430 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28935 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    29533 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18569 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/abf/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/abf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.550248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/dot/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/dot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_Grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.554248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.558248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5414 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7794 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.558248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.558248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.558248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40687 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    47166 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test__data_fillvalue_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test__fillvalue_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.562248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.562248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPField.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.562248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.562248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/test_Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/test_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14432 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test__generate_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_expand_filespecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_run_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_non_lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/merge/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/merge/test_ProtoCube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.566248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/pandas/test_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.570248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/_blockplot_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__fixup_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_contourf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_outline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_pcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_pcolormesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.570248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_contourf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_outline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_pcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_pcolormesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.570248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/test_Table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/test_Future.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/test_sample_data_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/stock/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/stock/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/test_IrisTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/time/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/time/test_PartialDateTime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.574248 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__coord_regular.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__is_circular.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__mask_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__slice_data_with_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_array_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_broadcast_to_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_column_slices_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_describe_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_equalise_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_file_is_newer_than.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_find_discontiguities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_mask_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_new_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_rolling_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_unify_time_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    69751 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/lib/iris/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-03 12:45:28.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    95246 2023-05-03 12:45:29.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:45:28.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:45:27.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 12:45:28.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 12:45:28.000000 scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/requirements/pypi-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:45:29.578248 scitools-iris-3.6.0rc0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-03 12:45:18.000000 scitools-iris-3.6.0rc0/tools/generate_std_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.552352 scitools-iris-3.6.1/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)  4146252 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/etc/cf-standard-name-table.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.552352 scitools-iris-3.6.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.560352 scitools-iris-3.6.1/lib/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)    15747 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50159 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62576 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.560352 scitools-iris-3.6.1/lib/iris/_representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_representation/cube_printout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/_representation/cube_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/iris/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.560352 scitools-iris-3.6.1/lib/iris/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)   112086 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39662 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/_area_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/_grid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25855 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41206 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12833 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/_scipy_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27924 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44792 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/cartography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36712 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/analysis/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69935 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/aux_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.560352 scitools-iris-3.6.1/lib/iris/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/common/lenient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53861 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/common/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106896 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/common/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/coord_categorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51390 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/coord_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112347 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   177579 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.560352 scitools-iris-3.6.1/lib/iris/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.536352 scitools-iris-3.6.1/lib/iris/etc/palette/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.564352 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/BrBG_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PRGn_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PiYG_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PuOr_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdBu_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdGy_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdYlBu_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdYlGn_11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/diverging/Spectral_11.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.564352 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Accent_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Dark2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Paired_12.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Pastel1_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Pastel2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set1_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set3_12.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.564352 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Blues_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/BuGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/BuPu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/GnBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Greens_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Greys_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/OrRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Oranges_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuBuGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Purples_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/RdPu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Reds_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlGnBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlOrBr_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlOrRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/etc/site.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.568352 scitools-iris-3.6.1/lib/iris/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27240 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/regrid_conservative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/stratify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.568352 scitools-iris-3.6.1/lib/iris/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110761 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/experimental/ugrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.568352 scitools-iris-3.6.1/lib/iris/fileformats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31932 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)   196094 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_ff_cross_references.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.568352 scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22058 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_pp_lbproc_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/_structured_array_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/abf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47602 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44205 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/name_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.572352 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/_dask_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/_thread_safe_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21742 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112867 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/netcdf/saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/nimrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/nimrod_load_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47347 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/pp_load_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30774 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/pp_save_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.572352 scitools-iris-3.6.1/lib/iris/fileformats/um/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um/_fast_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um/_fast_load_structured_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um/_ff_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um/_optimal_array_structuring.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107325 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/fileformats/um_cf_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.572352 scitools-iris-3.6.1/lib/iris/io/
+-rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/io/format_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35983 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71011 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.572352 scitools-iris-3.6.1/lib/iris/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.576352 scitools-iris-3.6.1/lib/iris/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.576352 scitools-iris-3.6.1/lib/iris/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.576352 scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23476 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30235 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/experimental/test_raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.576352 scitools-iris-3.6.1/lib/iris/tests/graphics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2166 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/graphics/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8901 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/graphics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6853 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/graphics/idiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2452 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/graphics/recreate_imagerepo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/analysis/test_area_weighted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/aux_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/aux_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/concatenate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/concatenate/test_concatenate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_CubeRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_ugrid_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_ugrid_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/fast_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/fast_load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27952 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/fast_load/test_fast_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.580352 scitools-iris-3.6.1/lib/iris/tests/integration/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/merge/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test__dask_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_aux_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_coord_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_delayed_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_self_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/integration/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_netcdftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_nzdateline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_plot_2d_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_vector_plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1556 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_Datums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_PartialDateTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_climatology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_new_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_pp_constrained_load_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_regrid_equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_regridding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/integration/um/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/um/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/integration/um/test_fieldsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/pp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/results/COLPEX/
+-rw-r--r--   0 runner    (1001) docker     (123)    37400 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/results/FF/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/FF/air_temperature_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/FF/air_temperature_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/FF/ffheader.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/FF/soil_temperature_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/FF/surface_altitude_1.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.584352 scitools-iris-3.6.1/lib/iris/tests/results/PP/
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_char_data.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15286 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_data_time_series.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   330620 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_x_data.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/global_test.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/nae_unpacked.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30791 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/PP/rle_unpacked.pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.588352 scitools-iris-3.6.1/lib/iris/tests/results/abf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/abf/load.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.600352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/abs.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_coord_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_coord_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_different_std_name.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_in_place.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_in_place_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_scalar.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.604352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/easy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_original.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_original.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/areaweights_original.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.608352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/cos_simple.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/cos_simple_radians.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.608352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_foo_bar_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.608352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/delta_one_element_explicit.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/midpoint_one_element_explicit.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple4.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple5.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/delta_and_midpoint/simple6.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_array.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_singular_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_scalar.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/exp.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/exp.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/exponentiate.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/exponentiate.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log10.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log10.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/log2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/maths_original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/multiply.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/multiply_different_std_name.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/original_common.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/original_hmean.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_both_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_grid.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_src.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_non_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_anon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_both_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_src.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_non_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/no_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/no_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_weighted_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.0.rlat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.0.rlon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.0.x.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.0.y.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.1.rlat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.1.rlon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.1.x.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/rotated_pole.1.y.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sqrt.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_array.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_coord_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_coord_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_scalar.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_weighted_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_weighted_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_latlon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_latlon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_source.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/cartography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/cartography/get_xy_grids/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cartography/get_xy_grids/1d.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cartography/get_xy_grids/2d.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/categorisation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/categorisation/customcheck.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/categorisation/quickcheck.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/cdm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_eq_10.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_gt_10.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/masked_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/masked_save_pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.616352 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/0d_cube.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/cubelist.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/cubelist.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/simple.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/unicode_attribute.__unicode__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/compatible_cubes.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.620352 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_3d_simple.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_anonymous.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.624352 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/all_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/attribute_constraint.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/invalid_inequality_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/pressure_950_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_load_strict.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.624352 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/complex.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.624352 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/intersection.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/intersection_missing.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/intersection_reversed.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/minimal.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/nd_bounds.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.628352 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/aux_nontime_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/aux_nontime_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/aux_time_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/aux_time_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/dim_nontime_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/dim_nontime_str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/dim_time_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_api/str_repr/dim_time_str.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.628352 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/CoordSystem_xml_element.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/GeogCS_init_no_invf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/GeogCS_init_no_major.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/GeogCS_init_no_minor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/GeogCS_init_sphere.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/Mercator.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/PolarStereographic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/PolarStereographicScaleFactor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/PolarStereographicStandardParallel.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/RotatedGeogCS_init.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_a.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/Stereographic.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/coord_systems/TransverseMercator_osgb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.632352 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/original.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.632352 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/cubelist.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/single_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/theta.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.632352 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pp/load/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pp/load/global.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.636352 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_merge.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.636352 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_orig.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_transposed.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.636352 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/append_multi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/append_single.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/default_coord_system.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/replace_multi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/replace_single.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.640352 scitools-iris-3.6.1/lib/iris/tests/results/derived/
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/column.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/no_orog.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/no_orog.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_derived_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_orog.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_orog.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_sigma.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16859 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_sigma.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/derived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.640352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.640352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.640352 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/surface_mean.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/file_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/file_load/known_loaders.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    97746 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/file_load/theta_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    97417 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/file_load/u_wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    97417 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/file_load/v_wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)   194764 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/file_load/wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/imagerepo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/incompatible_attr.str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/incompatible_cubes.str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/incompatible_meth.str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/incompatible_name.str.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/incompatible_unit.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/climatology/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/climatology/TestClimatology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/attributes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_different_saves_on_variables.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_same_saves_as_global.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/single_saves_as_global.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/um/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.540352 scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.644352 scitools-iris-3.6.1/lib/iris/tests/results/iterate/
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/iterate/izip_nd_ortho.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.648352 scitools-iris-3.6.1/lib/iris/tests/results/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/a_aux_b_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/a_aux_b_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/a_dim_b_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/a_dim_b_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/dec.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/multi_split.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/separable_combination.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/single_split.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_with_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_with_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/string_b_with_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/string_b_with_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/theta.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    17223 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/theta_two_times.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_duplicate_data.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_independent.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging4.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging5.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_non_expanding.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_series.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_single_forecast.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.652352 scitools-iris-3.6.1/lib/iris/tests/results/name/
+-rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49155 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_trajectory.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_trajectory0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_timeseries.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_timeseries.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_timeseries.data.1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.656352 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.656352 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/int64_data_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    24811 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_laea.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_lcc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc_false.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_monotonic.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_polar.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_conf_aux.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_conf_name.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_confl_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_confl_global_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_no_name.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_nocoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_samevar.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_single.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_wcoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_stereo.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_units_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_units_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/save_load_traj.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/uint32_data_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.660352 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/levels_below_ground.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/load_2flds.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/mockography.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/period_of_interest.cml
+-rw-r--r--   0 runner    (1001) docker     (123)   115358 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/probability_fields.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/pandas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.660352 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_object.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_simple.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.660352 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/global.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/lbtim_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/ocean_depth.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/rotated_uk.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/stock/realistic_4d.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/system/supported_filetype_.nc.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/system/supported_filetype_.pp.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/constant_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/hybrid_height.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/single_point.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/trajectory/zigzag.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.664352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/checksum_ignores_masked_values.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/embedded_newlines_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/long_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/multi_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/simple_string_attribute.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/stratify/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/stratify/relevel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.668352 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/endian.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/ProtoCube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/noise.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/noise.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/describe_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/describe_diff/incompatible_array_attrs.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.672352 scitools-iris-3.6.1/lib/iris/tests/results/uri_callback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/uri_callback/pp_global.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.544352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.548352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.676352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.676352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.680352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.680352 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.680352 scitools-iris-3.6.1/lib/iris/tests/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)    25236 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/_stock_2d_latlons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.680352 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/stock/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_abf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_aggregate_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29521 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_analysis_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32895 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_basic_maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cartography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51871 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16226 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_coding_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35467 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_coord_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_coord_categorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_coordsystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_cube_to_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_file_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_file_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_image_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_io_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_lazy_aggregate_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39630 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_nimrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_peak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_pp_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_pp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_pp_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_pp_to_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_std_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_uri_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.680352 scitools-iris-3.6.1/lib/iris/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.684352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.684352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/area_weighted/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/area_weighted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.684352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__xy_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_area_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.684352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.684352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__get_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__output_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_divide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55068 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/scipy_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/scipy_interpolate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/stats/test_pearsonr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15028 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_AreaWeighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_COUNT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MAX.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MAX_RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MEAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MIN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PERCENTILE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PROPORTION.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PercentileAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PointInCell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_RMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_STD_DEV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_SUM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_VARIANCE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_WPERCENTILE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.688352 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test_Lenient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__Lenient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__lenient_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__lenient_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__qualname.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26669 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/common/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192764 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/common/resolve/test_Resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test__CoordMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test__CoordSignature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test__CubeSignature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test_concatenate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/config/test_NetCDF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/constraints/test_Constraint_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/constraints/test_NameConstraint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/test_add_hour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.692352 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_GeogCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Geostationary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_LambertConformal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Orthographic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8687 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_RotatedPole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Stereographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/coords/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26495 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_AncillaryVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_AuxCoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_Cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_CellMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_CellMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_Coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22368 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_DimCoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38411 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/coords/test__DimensionalMetadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134513 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_CubeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube__operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/data_manager/test_DataManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/raster/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/stratify/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/stratify/test_relevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.696352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49280 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37430 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28935 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29533 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18569 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/abf/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/abf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/abf/test_ABFField.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/test_CFReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/dot/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/dot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/dot/test__dot_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.700352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_Grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5414 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7794 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.704352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.708352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.708352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40687 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47166 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test__data_fillvalue_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test__fillvalue_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.708352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.708352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_PPField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__field_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_as_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/test_Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/test__make_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/test_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14432 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/io/test__generate_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/io/test_expand_filespecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/io/test_run_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/io/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_non_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/merge/test_ProtoCube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.712352 scitools-iris-3.6.1/lib/iris/tests/unit/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/pandas/test_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/_blockplot_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__fixup_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_defn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_contourf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_pcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_pcolormesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_contourf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_pcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_pcolormesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/test_Table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/test_Future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/test_sample_data_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/tests/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/tests/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/tests/stock/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/tests/test_IrisTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.716352 scitools-iris-3.6.1/lib/iris/tests/unit/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/time/test_PartialDateTime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/lib/iris/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test__coord_regular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test__is_circular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test__mask_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test__slice_data_with_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_array_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_broadcast_to_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_column_slices_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_describe_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_equalise_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_file_is_newer_than.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_find_discontiguities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_mask_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_new_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_rolling_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/tests/unit/util/test_unify_time_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69320 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/lib/iris/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/lib/scitools_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    95415 2023-06-26 15:15:52.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 15:15:51.000000 scitools-iris-3.6.1/lib/scitools_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/requirements/pypi-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:52.720352 scitools-iris-3.6.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-26 15:15:42.000000 scitools-iris-3.6.1/tools/generate_std_names.py
```

### Comparing `scitools-iris-3.6.0rc0/COPYING` & `scitools-iris-3.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/COPYING.LESSER` & `scitools-iris-3.6.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/MANIFEST.in` & `scitools-iris-3.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/PKG-INFO` & `scitools-iris-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitools-iris
-Version: 3.6.0rc0
+Version: 3.6.1
 Summary: A powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 Author-email: Iris Contributors <scitools.pub@gmail.com>
 License: LGPL-3.0-or-later
 Project-URL: Code, https://github.com/SciTools/iris
 Project-URL: Discussions, https://github.com/SciTools/iris/discussions
 Project-URL: Documentation, https://scitools-iris.readthedocs.io/en/stable/
 Project-URL: Issues, https://github.com/SciTools/iris/issues
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: scitools-iris Version: 3.6.0rc0 Summary: A
-powerful, format-agnostic, community-driven Python package for analysing and
-visualising Earth science data Author-email: Iris Contributors
+Metadata-Version: 2.1 Name: scitools-iris Version: 3.6.1 Summary: A powerful,
+format-agnostic, community-driven Python package for analysing and visualising
+Earth science data Author-email: Iris Contributors
 pub@gmail.com> License: LGPL-3.0-or-later Project-URL: Code, https://
 github.com/SciTools/iris Project-URL: Discussions, https://github.com/SciTools/
 iris/discussions Project-URL: Documentation, https://scitools-
 iris.readthedocs.io/en/stable/ Project-URL: Issues, https://github.com/
 SciTools/iris/issues Keywords: cf-metadata,data-analysis,earth-
 science,grib,netcdf,meteorology,oceanography,space-weather,ugrid,visualisation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `scitools-iris-3.6.0rc0/README.md` & `scitools-iris-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/etc/cf-standard-name-table.xml` & `scitools-iris-3.6.1/etc/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/__init__.py` & `scitools-iris-3.6.1/lib/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_concatenate.py` & `scitools-iris-3.6.1/lib/iris/_concatenate.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,19 +97,23 @@
             The dimension(s) associated with the coordinate.
 
         Returns:
             The new class instance.
 
         """
         defn = coord.metadata
-        points_dtype = coord.points.dtype
-        bounds_dtype = coord.bounds.dtype if coord.bounds is not None else None
+        points_dtype = coord.core_points().dtype
+        bounds_dtype = (
+            coord.core_bounds().dtype
+            if coord.core_bounds() is not None
+            else None
+        )
         kwargs = {}
         # Add scalar flag metadata.
-        kwargs["scalar"] = coord.points.size == 1
+        kwargs["scalar"] = coord.core_points().size == 1
         # Add circular flag metadata for dimensional coordinates.
         if hasattr(coord, "circular"):
             kwargs["circular"] = coord.circular
         if isinstance(coord, iris.coords.DimCoord):
             # Mix the monotonic ordering into the metadata.
             if coord.points[0] == coord.points[-1]:
                 order = _CONSTANT
@@ -696,26 +700,35 @@
 
         Returns:
             A boolean tuple pair of whether the coordinates are compatible,
             and whether they represent a candidate axis of concatenation.
 
         """
         # A candidate axis must have non-identical coordinate points.
-        candidate_axis = not array_equal(coord.points, other.points)
+        candidate_axis = not array_equal(
+            coord.core_points(), other.core_points()
+        )
 
         if candidate_axis:
             # Ensure both have equal availability of bounds.
-            result = (coord.bounds is None) == (other.bounds is None)
+            result = (coord.core_bounds() is None) == (
+                other.core_bounds() is None
+            )
         else:
-            if coord.bounds is not None and other.bounds is not None:
+            if (
+                coord.core_bounds() is not None
+                and other.core_bounds() is not None
+            ):
                 # Ensure equality of bounds.
-                result = array_equal(coord.bounds, other.bounds)
+                result = array_equal(coord.core_bounds(), other.core_bounds())
             else:
                 # Ensure both have equal availability of bounds.
-                result = coord.bounds is None and other.bounds is None
+                result = (
+                    coord.core_bounds() is None and other.core_bounds() is None
+                )
 
         return result, candidate_axis
 
     def candidate_axis(self, other):
         """
         Determine the candidate axis of concatenation with the
         given coordinate signature.
@@ -847,37 +860,44 @@
                 key=lambda skeleton: skeleton.signature.dim_extents,
                 reverse=(order == _DECREASING),
             )
 
             # Concatenate the new dimension coordinate.
             dim_coords_and_dims = self._build_dim_coordinates()
 
-            # Concatenate the new auxiliary coordinates.
+            # Concatenate the new auxiliary coordinates (does NOT include
+            # scalar coordinates!).
             aux_coords_and_dims = self._build_aux_coordinates()
 
+            # Concatenate the new scalar coordinates.
+            scalar_coords = self._build_scalar_coordinates()
+
             # Concatenate the new cell measures
             cell_measures_and_dims = self._build_cell_measures()
 
             # Concatenate the new ancillary variables
             ancillary_variables_and_dims = self._build_ancillary_variables()
 
             # Concatenate the new aux factories
             aux_factories = self._build_aux_factories(
-                dim_coords_and_dims, aux_coords_and_dims
+                dim_coords_and_dims, aux_coords_and_dims, scalar_coords
             )
 
             # Concatenate the new data payload.
             data = self._build_data()
 
             # Build the new cube.
+            all_aux_coords_and_dims = aux_coords_and_dims + [
+                (scalar_coord, ()) for scalar_coord in scalar_coords
+            ]
             kwargs = cube_signature.defn._asdict()
             cube = iris.cube.Cube(
                 data,
                 dim_coords_and_dims=dim_coords_and_dims,
-                aux_coords_and_dims=aux_coords_and_dims,
+                aux_coords_and_dims=all_aux_coords_and_dims,
                 cell_measures_and_dims=cell_measures_and_dims,
                 ancillary_variables_and_dims=ancillary_variables_and_dims,
                 aux_factories=aux_factories,
                 **kwargs,
             )
         else:
             # There are no other source-cubes to concatenate
@@ -1091,24 +1111,26 @@
         for i, (coord, dims) in enumerate(cube_signature.aux_coords_and_dims):
             # Check whether the coordinate spans the nominated
             # dimension of concatenation.
             if self.axis in dims:
                 # Concatenate the points together.
                 dim = dims.index(self.axis)
                 points = [
-                    skton.signature.aux_coords_and_dims[i].coord.points
+                    skton.signature.aux_coords_and_dims[i].coord.core_points()
                     for skton in skeletons
                 ]
                 points = np.concatenate(tuple(points), axis=dim)
 
                 # Concatenate the bounds together.
                 bnds = None
                 if coord.has_bounds():
                     bnds = [
-                        skton.signature.aux_coords_and_dims[i].coord.bounds
+                        skton.signature.aux_coords_and_dims[
+                            i
+                        ].coord.core_bounds()
                         for skton in skeletons
                     ]
                     bnds = np.concatenate(tuple(bnds), axis=dim)
 
                 # Generate the associated coordinate metadata.
                 kwargs = cube_signature.aux_metadata[i].defn._asdict()
 
@@ -1128,20 +1150,30 @@
                         _ = kwargs.pop("circular", None)
                         coord = iris.coords.AuxCoord(
                             points, bounds=bnds, **kwargs
                         )
 
             aux_coords_and_dims.append((coord.copy(), dims))
 
-        # Generate all the scalar coordinates for the new concatenated cube.
-        for coord in cube_signature.scalar_coords:
-            aux_coords_and_dims.append((coord.copy(), ()))
-
         return aux_coords_and_dims
 
+    def _build_scalar_coordinates(self):
+        """
+        Generate the scalar coordinates for the new concatenated cube.
+
+        Returns:
+            A list of scalar coordinates.
+
+        """
+        scalar_coords = []
+        for coord in self._cube_signature.scalar_coords:
+            scalar_coords.append(coord.copy())
+
+        return scalar_coords
+
     def _build_cell_measures(self):
         """
         Generate the cell measures with associated dimension(s)
         mapping for the new concatenated cube.
 
         Returns:
             A list of cell measures and dimension(s) tuple pairs.
@@ -1212,67 +1244,81 @@
                 # Build the concatenated coordinate.
                 av = iris.coords.AncillaryVariable(data, **kwargs)
 
             ancillary_variables_and_dims.append((av.copy(), dims))
 
         return ancillary_variables_and_dims
 
-    def _build_aux_factories(self, dim_coords_and_dims, aux_coords_and_dims):
+    def _build_aux_factories(
+        self, dim_coords_and_dims, aux_coords_and_dims, scalar_coords
+    ):
         """
         Generate the aux factories for the new concatenated cube.
 
         Args:
 
         * dim_coords_and_dims:
             A list of dimension coordinate and dimension tuple pairs from the
             concatenated cube.
 
         * aux_coords_and_dims:
             A list of auxiliary coordinates and dimension(s) tuple pairs from
             the concatenated cube.
 
+        * scalar_coords:
+            A list of scalar coordinates from the concatenated cube.
+
         Returns:
             A list of :class:`iris.aux_factory.AuxCoordFactory`.
 
         """
         # Setup convenience hooks.
         cube_signature = self._cube_signature
         old_dim_coords = cube_signature.dim_coords
         old_aux_coords = [a[0] for a in cube_signature.aux_coords_and_dims]
         new_dim_coords = [d[0] for d in dim_coords_and_dims]
         new_aux_coords = [a[0] for a in aux_coords_and_dims]
-        scalar_coords = cube_signature.scalar_coords
+        old_scalar_coords = cube_signature.scalar_coords
+        new_scalar_coords = scalar_coords
 
         aux_factories = []
 
         # Generate all the factories for the new concatenated cube.
-        for i, (coord, dims, factory) in enumerate(
-            cube_signature.derived_coords_and_dims
-        ):
-            # Check whether the derived coordinate of the factory spans the
-            # nominated dimension of concatenation.
-            if self.axis in dims:
-                # Update the dependencies of the factory with coordinates of
-                # the concatenated cube. We need to check all coordinate types
-                # here (dim coords, aux coords, and scalar coords).
-                new_dependencies = {}
-                for old_dependency in factory.dependencies.values():
-                    if old_dependency in old_dim_coords:
-                        dep_idx = old_dim_coords.index(old_dependency)
-                        new_dependency = new_dim_coords[dep_idx]
-                    elif old_dependency in old_aux_coords:
-                        dep_idx = old_aux_coords.index(old_dependency)
-                        new_dependency = new_aux_coords[dep_idx]
-                    else:
-                        dep_idx = scalar_coords.index(old_dependency)
-                        new_dependency = scalar_coords[dep_idx]
-                    new_dependencies[id(old_dependency)] = new_dependency
+        for _, _, factory in cube_signature.derived_coords_and_dims:
+            # Update the dependencies of the factory with coordinates of
+            # the concatenated cube. We need to check all coordinate types
+            # here (dim coords, aux coords, and scalar coords).
+
+            # Note: in contrast to other _build_... methods of this class, we
+            # do NOT need to distinguish between aux factories that span the
+            # nominated concatenation axis and aux factories that do not. The
+            # reason is that ALL aux factories need to be updated with the new
+            # coordinates of the concatenated cube (passed to this function via
+            # dim_coords_and_dims, aux_coords_and_dims, scalar_coords [these
+            # contain ALL new coordinates, not only the ones spanning the
+            # concatenation dimension]), so no special treatment for the aux
+            # factories that span the concatenation dimension is necessary. If
+            # not all aux factories are properly updated with references to the
+            # new coordinates, this may lead to KeyErrors (see
+            # https://github.com/SciTools/iris/issues/5339).
+            new_dependencies = {}
+            for old_dependency in factory.dependencies.values():
+                if old_dependency in old_dim_coords:
+                    dep_idx = old_dim_coords.index(old_dependency)
+                    new_dependency = new_dim_coords[dep_idx]
+                elif old_dependency in old_aux_coords:
+                    dep_idx = old_aux_coords.index(old_dependency)
+                    new_dependency = new_aux_coords[dep_idx]
+                else:
+                    dep_idx = old_scalar_coords.index(old_dependency)
+                    new_dependency = new_scalar_coords[dep_idx]
+                new_dependencies[id(old_dependency)] = new_dependency
 
-                # Create new factory with the updated dependencies.
-                factory = factory.updated(new_dependencies)
+            # Create new factory with the updated dependencies.
+            factory = factory.updated(new_dependencies)
 
             aux_factories.append(factory)
 
         return aux_factories
 
     def _build_data(self):
         """
@@ -1303,24 +1349,24 @@
         axis = self.axis
         dim_ind = self._cube_signature.dim_mapping.index(axis)
         metadata = self._cube_signature.dim_metadata[dim_ind]
         defn, circular = metadata.defn, metadata.kwargs["circular"]
 
         # Concatenate the points together for the nominated dimension.
         points = [
-            skeleton.signature.dim_coords[dim_ind].points
+            skeleton.signature.dim_coords[dim_ind].core_points()
             for skeleton in skeletons
         ]
         points = np.concatenate(tuple(points))
 
         # Concatenate the bounds together for the nominated dimension.
         bounds = None
         if self._cube_signature.dim_coords[dim_ind].has_bounds():
             bounds = [
-                skeleton.signature.dim_coords[dim_ind].bounds
+                skeleton.signature.dim_coords[dim_ind].core_bounds()
                 for skeleton in skeletons
             ]
             bounds = np.concatenate(tuple(bounds))
 
         # Populate the new dimension coordinate with the concatenated
         # points, bounds and associated metadata.
         kwargs = defn._asdict()
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_constraints.py` & `scitools-iris-3.6.1/lib/iris/_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_data_manager.py` & `scitools-iris-3.6.1/lib/iris/_data_manager.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_deprecation.py` & `scitools-iris-3.6.1/lib/iris/_deprecation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_lazy_data.py` & `scitools-iris-3.6.1/lib/iris/_lazy_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,23 @@
     We determine this by checking for a "compute" property.
 
     """
     result = hasattr(data, "compute")
     return result
 
 
+def is_lazy_masked_data(data):
+    """
+    Return True if the argument is both an Iris 'lazy' data array and the
+    underlying array is of masked type.  Otherwise return False.
+
+    """
+    return is_lazy_data(data) and ma.isMA(da.utils.meta_from_array(data))
+
+
 @lru_cache
 def _optimum_chunksize_internals(
     chunks,
     shape,
     limit=None,
     dtype=np.dtype("f4"),
     dask_array_chunksize=dask.config.get("array.chunk-size"),
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_merge.py` & `scitools-iris-3.6.1/lib/iris/_merge.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_representation/cube_printout.py` & `scitools-iris-3.6.1/lib/iris/_representation/cube_printout.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/_representation/cube_summary.py` & `scitools-iris-3.6.1/lib/iris/_representation/cube_summary.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/__init__.py` & `scitools-iris-3.6.1/lib/iris/analysis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,24 @@
     "MEAN",
     "MEDIAN",
     "MIN",
     "Nearest",
     "PEAK",
     "PERCENTILE",
     "PROPORTION",
+    "PercentileAggregator",
     "PointInCell",
     "RMS",
     "STD_DEV",
     "SUM",
     "UnstructuredNearest",
     "VARIANCE",
     "WPERCENTILE",
     "WeightedAggregator",
+    "WeightedPercentileAggregator",
     "clear_phenomenon_identity",
     "create_weighted_aggregator_fn",
 )
 
 
 class _CoordGroup:
     """
@@ -484,15 +486,15 @@
             call signature (units).
 
         * lazy_func (callable or None):
             An alternative to :data:`call_func` implementing a lazy
             aggregation. Note that, it need not support all features of the
             main operation, but should raise an error in unhandled cases.
 
-        Additional kwargs::
+        Additional kwargs:
             Passed through to :data:`call_func`, :data:`lazy_func`, and
             :data:`units_func`.
 
         Aggregators are used by cube aggregation methods such as
         :meth:`~iris.cube.Cube.collapsed` and
         :meth:`~iris.cube.Cube.aggregated_by`.  For example::
 
@@ -715,17 +717,20 @@
 
         * units_func (callable):
             | *Call signature*: (units, \**kwargs)
 
             If provided, called to convert a cube's units.
             Returns an :class:`cf_units.Unit`, or a
             value that can be made into one.
+            To ensure backwards-compatibility, also accepts a callable with
+            call signature (units).
 
-        Additional kwargs::
-            Passed through to :data:`call_func` and :data:`lazy_func`.
+        Additional kwargs:
+            Passed through to :data:`call_func`, :data:`lazy_func`, and
+            :data:`units_func`.
 
         This aggregator can used by cube aggregation methods such as
         :meth:`~iris.cube.Cube.collapsed` and
         :meth:`~iris.cube.Cube.aggregated_by`.  For example::
 
             cube.collapsed('longitude', iris.analysis.PERCENTILE, percent=50)
 
@@ -956,22 +961,35 @@
 
         * units_func (callable):
             | *Call signature*: (units, \**kwargs)
 
             If provided, called to convert a cube's units.
             Returns an :class:`cf_units.Unit`, or a
             value that can be made into one.
+            To ensure backwards-compatibility, also accepts a callable with
+            call signature (units).
+
+            If the aggregator is used by a cube aggregation method (e.g.,
+            :meth:`~iris.cube.Cube.collapsed`,
+            :meth:`~iris.cube.Cube.aggregated_by`,
+            :meth:`~iris.cube.Cube.rolling_window`), a keyword argument
+            `_weights_units` is provided to this function to allow updating
+            units based on the weights. `_weights_units` is determined from the
+            `weights` given to the aggregator (``None`` if no weights are
+            given). See :ref:`user guide <cube-statistics-collapsing-average>`
+            for an example of weighted aggregation that changes units.
 
         * lazy_func (callable or None):
             An alternative to :data:`call_func` implementing a lazy
             aggregation. Note that, it need not support all features of the
             main operation, but should raise an error in unhandled cases.
 
-        Additional kwargs::
-            Passed through to :data:`call_func` and :data:`lazy_func`.
+        Additional kwargs:
+            Passed through to :data:`call_func`, :data:`lazy_func`, and
+            :data:`units_func`.
 
         This aggregator can used by cube aggregation methods such as
         :meth:`~iris.cube.Cube.collapsed` and
         :meth:`~iris.cube.Cube.aggregated_by`.  For example::
 
             cube.collapsed('longitude', iris.analysis.WPERCENTILE, percent=50,
                              weights=iris.analysis.cartography.area_weights(cube))
@@ -1086,37 +1104,55 @@
     Convenience class that supports common weighted aggregation functionality.
 
     """
 
     def __init__(
         self, cell_method, call_func, units_func=None, lazy_func=None, **kwargs
     ):
-        """
+        r"""
         Create a weighted aggregator for the given :data:`call_func`.
 
         Args:
 
         * cell_method (string):
             Cell method string that supports string format substitution.
 
         * call_func (callable):
-            Data aggregation function. Call signature `(data, axis, **kwargs)`.
+            Data aggregation function. Call signature `(data, axis,
+            \**kwargs)`.
 
         Kwargs:
 
         * units_func (callable):
-            Units conversion function.
+            | *Call signature*: (units, \**kwargs)
+
+            If provided, called to convert a cube's units.
+            Returns an :class:`cf_units.Unit`, or a
+            value that can be made into one.
+            To ensure backwards-compatibility, also accepts a callable with
+            call signature (units).
+
+            If the aggregator is used by a cube aggregation method (e.g.,
+            :meth:`~iris.cube.Cube.collapsed`,
+            :meth:`~iris.cube.Cube.aggregated_by`,
+            :meth:`~iris.cube.Cube.rolling_window`), a keyword argument
+            `_weights_units` is provided to this function to allow updating
+            units based on the weights. `_weights_units` is determined from the
+            `weights` given to the aggregator (``None`` if no weights are
+            given). See :ref:`user guide <cube-statistics-collapsing-average>`
+            for an example of weighted aggregation that changes units.
 
         * lazy_func (callable or None):
             An alternative to :data:`call_func` implementing a lazy
             aggregation. Note that, it need not support all features of the
             main operation, but should raise an error in unhandled cases.
 
         Additional kwargs:
-            Passed through to :data:`call_func` and :data:`lazy_func`.
+            Passed through to :data:`call_func`, :data:`lazy_func`, and
+            :data:`units_func`.
 
         """
         Aggregator.__init__(
             self,
             cell_method,
             call_func,
             units_func=units_func,
@@ -1183,116 +1219,78 @@
             result = Aggregator.post_process(
                 self, collapsed_cube, data_result, coords, **kwargs
             )
 
         return result
 
 
-class _Weights(np.ndarray):
+class _Weights:
     """Class for handling weights for weighted aggregation.
 
-    This subclasses :class:`numpy.ndarray`; thus, all methods and properties of
-    :class:`numpy.ndarray` (e.g., `shape`, `ndim`, `view()`, etc.) are
-    available.
+    Provides the following two attributes:
 
-    Details on subclassing :class:`numpy.ndarray` are given here:
-    https://numpy.org/doc/stable/user/basics.subclassing.html
+    * ``array``: Lazy or non-lazy array of weights.
+    * ``units``: Units associated with the weights.
 
     """
 
-    def __new__(cls, weights, cube, units=None):
-        """Create class instance.
+    def __init__(self, weights, cube):
+        """Initialize class instance.
 
         Args:
 
         * weights (Cube, string, _DimensionalMetadata, array-like):
             If given as a :class:`iris.cube.Cube`, use its data and units. If
             given as a :obj:`str` or :class:`iris.coords._DimensionalMetadata`,
             assume this is (the name of) a
             :class:`iris.coords._DimensionalMetadata` object of the cube (i.e.,
             one of :meth:`iris.cube.Cube.coords`,
             :meth:`iris.cube.Cube.cell_measures`, or
             :meth:`iris.cube.Cube.ancillary_variables`). If given as an
-            array-like object, use this directly and assume units of `1`.  If
-            `units` is given, ignore all units derived above and use the ones
-            given by `units`.
+            array-like object, use this directly and assume units of `1`. Note:
+            this does **not** create a copy of the input array.
         * cube (Cube):
             Input cube for aggregation. If weights is given as :obj:`str` or
             :class:`iris.coords._DimensionalMetadata`, try to extract the
             :class:`iris.coords._DimensionalMetadata` object and corresponding
             dimensional mappings from this cube. Otherwise, this argument is
             ignored.
-        * units (string, Unit):
-            If ``None``, use units derived from `weights`. Otherwise, overwrite
-            the units derived from `weights` and use `units`.
 
         """
         # `weights` is a cube
         # Note: to avoid circular imports of Cube we use duck typing using the
         # "hasattr" syntax here
         # --> Extract data and units from cube
         if hasattr(weights, "add_aux_coord"):
-            obj = np.asarray(weights.data).view(cls)
-            obj.units = weights.units
+            derived_array = weights.core_data()
+            derived_units = weights.units
 
         # `weights`` is a string or _DimensionalMetadata object
         # --> Extract _DimensionalMetadata object from cube, broadcast it to
         # correct shape using the corresponding dimensional mapping, and use
         # its data and units
         elif isinstance(weights, (str, _DimensionalMetadata)):
             dim_metadata = cube._dimensional_metadata(weights)
-            arr = dim_metadata._values
+            derived_array = dim_metadata._core_values()
             if dim_metadata.shape != cube.shape:
-                arr = iris.util.broadcast_to_shape(
-                    arr,
+                derived_array = iris.util.broadcast_to_shape(
+                    derived_array,
                     cube.shape,
                     dim_metadata.cube_dims(cube),
                 )
-            obj = np.asarray(arr).view(cls)
-            obj.units = dim_metadata.units
+            derived_units = dim_metadata.units
 
-        # Remaining types (e.g., np.ndarray): try to convert to ndarray.
+        # Remaining types (e.g., np.ndarray, dask.array.core.Array, etc.)
+        # --> Use array directly and assign units of "1"
         else:
-            obj = np.asarray(weights).view(cls)
-            obj.units = Unit("1")
-
-        # Overwrite units from units argument if necessary
-        if units is not None:
-            obj.units = units
+            derived_array = weights
+            derived_units = Unit("1")
 
-        return obj
-
-    def __array_finalize__(self, obj):
-        """See https://numpy.org/doc/stable/user/basics.subclassing.html.
-
-        Note
-        ----
-        `obj` cannot be `None` here since ``_Weights.__new__`` does not call
-        ``super().__new__`` explicitly.
-
-        """
-        self.units = getattr(obj, "units", Unit("1"))
-
-    @classmethod
-    def update_kwargs(cls, kwargs, cube):
-        """Update ``weights`` keyword argument in-place.
-
-        Args:
-
-        * kwargs (dict):
-            Keyword arguments that will be updated in-place if a `weights`
-            keyword is present which is not ``None``.
-        * cube (Cube):
-            Input cube for aggregation. If weights is given as :obj:`str`, try
-            to extract a cell measure with the corresponding name from this
-            cube. Otherwise, this argument is ignored.
-
-        """
-        if kwargs.get("weights") is not None:
-            kwargs["weights"] = cls(kwargs["weights"], cube)
+        self.array = derived_array
+        self.units = derived_units
 
 
 def create_weighted_aggregator_fn(aggregator_fn, axis, **kwargs):
     """Return an aggregator function that can explicitly handle weights.
 
     Args:
 
@@ -1748,19 +1746,25 @@
         rvalue = wsum
     return rvalue
 
 
 def _sum_units_func(units, **kwargs):
     """Multiply original units with weight units if possible."""
     weights = kwargs.get("weights")
-    if weights is None:  # no weights given or weights are None
-        result = units
-    elif hasattr(weights, "units"):  # weights are _Weights
-        result = units * weights.units
-    else:  # weights are regular np.ndarrays
+    weights_units = kwargs.get("_weights_units")
+    multiply_by_weights_units = all(
+        [
+            weights is not None,
+            weights_units is not None,
+            weights_units != "1",
+        ]
+    )
+    if multiply_by_weights_units:
+        result = units * weights_units
+    else:
         result = units
     return result
 
 
 def _peak(array, **kwargs):
     def column_segments(column):
         nan_indices = np.where(np.isnan(column))[0]
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/_area_weighted.py` & `scitools-iris-3.6.1/lib/iris/analysis/_area_weighted.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/_grid_angles.py` & `scitools-iris-3.6.1/lib/iris/analysis/_grid_angles.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/_interpolation.py` & `scitools-iris-3.6.1/lib/iris/analysis/_interpolation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/_regrid.py` & `scitools-iris-3.6.1/lib/iris/analysis/_regrid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/_scipy_interpolate.py` & `scitools-iris-3.6.1/lib/iris/analysis/_scipy_interpolate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/calculus.py` & `scitools-iris-3.6.1/lib/iris/analysis/calculus.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/cartography.py` & `scitools-iris-3.6.1/lib/iris/analysis/cartography.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/geometry.py` & `scitools-iris-3.6.1/lib/iris/analysis/geometry.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/maths.py` & `scitools-iris-3.6.1/lib/iris/analysis/maths.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/stats.py` & `scitools-iris-3.6.1/lib/iris/analysis/stats.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/analysis/trajectory.py` & `scitools-iris-3.6.1/lib/iris/analysis/trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/aux_factory.py` & `scitools-iris-3.6.1/lib/iris/aux_factory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/common/lenient.py` & `scitools-iris-3.6.1/lib/iris/common/lenient.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/common/metadata.py` & `scitools-iris-3.6.1/lib/iris/common/metadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/common/mixin.py` & `scitools-iris-3.6.1/lib/iris/common/mixin.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/common/resolve.py` & `scitools-iris-3.6.1/lib/iris/common/resolve.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/config.py` & `scitools-iris-3.6.1/lib/iris/config.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/coord_categorisation.py` & `scitools-iris-3.6.1/lib/iris/coord_categorisation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/coord_systems.py` & `scitools-iris-3.6.1/lib/iris/coord_systems.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/coords.py` & `scitools-iris-3.6.1/lib/iris/coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/cube.py` & `scitools-iris-3.6.1/lib/iris/cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from copy import deepcopy
 from functools import partial, reduce
 import operator
 import warnings
 from xml.dom.minidom import Document
 import zlib
 
+from cf_units import Unit
 import dask.array as da
 import numpy as np
 import numpy.ma as ma
 
 import iris._constraints
 from iris._data_manager import DataManager
 import iris._lazy_data as _lazy
@@ -1140,15 +1141,15 @@
         if self.units.is_unknown():
             raise iris.exceptions.UnitConversionError(
                 "Cannot convert from unknown units. "
                 'The "cube.units" attribute may be set directly.'
             )
         if self.has_lazy_data():
             # Make fixed copies of old + new units for a delayed conversion.
-            old_unit = self.units
+            old_unit = Unit(self.units)
             new_unit = unit
 
             pointwise_convert = partial(old_unit.convert, other=new_unit)
 
             new_data = _lazy.lazy_elementwise(
                 self.lazy_data(), pointwise_convert
             )
@@ -3831,15 +3832,18 @@
             may be created etc.) as::
 
                 cube.collapsed(['latitude', 'longitude'],
                                iris.analysis.VARIANCE)
         """
         # Update weights kwargs (if necessary) to handle different types of
         # weights
-        _Weights.update_kwargs(kwargs, self)
+        weights_info = None
+        if kwargs.get("weights") is not None:
+            weights_info = _Weights(kwargs["weights"], self)
+            kwargs["weights"] = weights_info.array
 
         # Convert any coordinate names to coordinates
         coords = self._as_list_of_coords(coords)
 
         if isinstance(
             aggregator, iris.analysis.WeightedAggregator
         ) and not aggregator.uses_weighting(**kwargs):
@@ -3976,15 +3980,19 @@
                 )
 
             data_result = aggregator.aggregate(
                 unrolled_data, axis=-1, **kwargs
             )
 
         aggregator.update_metadata(
-            collapsed_cube, coords, axis=collapse_axis, **kwargs
+            collapsed_cube,
+            coords,
+            axis=collapse_axis,
+            _weights_units=getattr(weights_info, "units", None),
+            **kwargs,
         )
         result = aggregator.post_process(
             collapsed_cube, data_result, coords, **kwargs
         )
         return result
 
     def aggregated_by(
@@ -4069,15 +4077,18 @@
                 Attributes:
                     Conventions                 'CF-1.5'
                     STASH                       m01s00i024
 
         """
         # Update weights kwargs (if necessary) to handle different types of
         # weights
-        _Weights.update_kwargs(kwargs, self)
+        weights_info = None
+        if kwargs.get("weights") is not None:
+            weights_info = _Weights(kwargs["weights"], self)
+            kwargs["weights"] = weights_info.array
 
         groupby_coords = []
         dimension_to_groupby = None
 
         coords = self._as_list_of_coords(coords)
         for coord in sorted(coords, key=lambda coord: coord.metadata):
             if coord.ndim > 1:
@@ -4109,24 +4120,18 @@
             if weights.ndim == 1:
                 if len(weights) != self.shape[dimension_to_groupby]:
                     raise ValueError(
                         f"1D weights must have the same length as the dimension "
                         f"that is aggregated, got {len(weights):d}, expected "
                         f"{self.shape[dimension_to_groupby]:d}"
                     )
-
-                # iris.util.broadcast_to_shape does not preserve _Weights type
-                weights = _Weights(
-                    iris.util.broadcast_to_shape(
-                        weights,
-                        self.shape,
-                        (dimension_to_groupby,),
-                    ),
-                    self,
-                    units=weights.units,
+                weights = iris.util.broadcast_to_shape(
+                    weights,
+                    self.shape,
+                    (dimension_to_groupby,),
                 )
             if weights.shape != self.shape:
                 raise ValueError(
                     f"Weights must either be 1D or have the same shape as the "
                     f"cube, got shape {weights.shape} for weights, "
                     f"{self.shape} for cube"
                 )
@@ -4269,15 +4274,19 @@
 
             # Restore original weights.
             if weights is not None:
                 kwargs["weights"] = weights
 
         # Add the aggregation meta data to the aggregate-by cube.
         aggregator.update_metadata(
-            aggregateby_cube, groupby_coords, aggregate=True, **kwargs
+            aggregateby_cube,
+            groupby_coords,
+            aggregate=True,
+            _weights_units=getattr(weights_info, "units", None),
+            **kwargs,
         )
         # Replace the appropriate coordinates within the aggregate-by cube.
         (dim_coord,) = self.coords(
             dimensions=dimension_to_groupby, dim_coords=True
         ) or [None]
         for coord in groupby.coords:
             new_coord = coord.copy()
@@ -4408,15 +4417,18 @@
 
             Notice that the forecast_period dimension now represents the 4
             possible windows of size 3 from the original cube.
 
         """
         # Update weights kwargs (if necessary) to handle different types of
         # weights
-        _Weights.update_kwargs(kwargs, self)
+        weights_info = None
+        if kwargs.get("weights") is not None:
+            weights_info = _Weights(kwargs["weights"], self)
+            kwargs["weights"] = weights_info.array
 
         coord = self._as_list_of_coords(coord)[0]
 
         if getattr(coord, "circular", False):
             raise iris.exceptions.NotYetImplementedError(
                 "Rolling window over a circular coordinate."
             )
@@ -4495,14 +4507,15 @@
             new_coord.bounds = new_bounds
 
         # update the metadata of the cube itself
         aggregator.update_metadata(
             new_cube,
             [coord],
             action="with a rolling window of length %s over" % window,
+            _weights_units=getattr(weights_info, "units", None),
             **kwargs,
         )
         # and perform the data transformation, generating weights first if
         # needed
         if isinstance(
             aggregator, iris.analysis.WeightedAggregator
         ) and aggregator.uses_weighting(**kwargs):
@@ -4511,22 +4524,16 @@
                 if weights.ndim > 1 or weights.shape[0] != window:
                     raise ValueError(
                         "Weights for rolling window aggregation "
                         "must be a 1d array with the same length "
                         "as the window."
                     )
                 kwargs = dict(kwargs)
-
-                # iris.util.broadcast_to_shape does not preserve _Weights type
-                kwargs["weights"] = _Weights(
-                    iris.util.broadcast_to_shape(
-                        weights, rolling_window_data.shape, (dimension + 1,)
-                    ),
-                    self,
-                    units=weights.units,
+                kwargs["weights"] = iris.util.broadcast_to_shape(
+                    weights, rolling_window_data.shape, (dimension + 1,)
                 )
         data_result = aggregator.aggregate(
             rolling_window_data, axis=dimension + 1, **kwargs
         )
         result = aggregator.post_process(
             new_cube, data_result, [coord], **kwargs
         )
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/BrBG_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/BrBG_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PRGn_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PRGn_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PiYG_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PiYG_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/PuOr_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/PuOr_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdBu_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdBu_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdGy_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdGy_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdYlBu_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdYlBu_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/RdYlGn_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/RdYlGn_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/diverging/Spectral_11.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/diverging/Spectral_11.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Accent_08.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Accent_08.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Dark2_08.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Dark2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Paired_12.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Paired_12.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Pastel1_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Pastel1_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Pastel2_08.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Pastel2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set1_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set1_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set2_08.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/qualitative/Set3_12.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/qualitative/Set3_12.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Blues_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Blues_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/BuGn_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/BuGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/BuPu_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/BuPu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/GnBu_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/GnBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Greens_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Greens_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Greys_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Greys_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/OrRd_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/OrRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Oranges_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Oranges_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuBuGn_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuBuGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuBu_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/PuRd_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/PuRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Purples_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Purples_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/RdPu_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/RdPu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/Reds_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/Reds_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlGnBu_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlGnBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlGn_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlOrBr_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlOrBr_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/etc/palette/sequential/YlOrRd_09.txt` & `scitools-iris-3.6.1/lib/iris/etc/palette/sequential/YlOrRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/exceptions.py` & `scitools-iris-3.6.1/lib/iris/exceptions.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/animate.py` & `scitools-iris-3.6.1/lib/iris/experimental/animate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/raster.py` & `scitools-iris-3.6.1/lib/iris/experimental/raster.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/regrid.py` & `scitools-iris-3.6.1/lib/iris/experimental/regrid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/regrid_conservative.py` & `scitools-iris-3.6.1/lib/iris/experimental/regrid_conservative.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/representation.py` & `scitools-iris-3.6.1/lib/iris/experimental/representation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/stratify.py` & `scitools-iris-3.6.1/lib/iris/experimental/stratify.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/__init__.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/cf.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/cf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/load.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/mesh.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/mesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/metadata.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/metadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/save.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/experimental/ugrid/utils.py` & `scitools-iris-3.6.1/lib/iris/experimental/ugrid/utils.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/__init__.py` & `scitools-iris-3.6.1/lib/iris/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_ff.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_ff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_ff_cross_references.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_ff_cross_references.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/actions.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/actions.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/engine.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/engine.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_nc_load_rules/helpers.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_nc_load_rules/helpers.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_pp_lbproc_pairs.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_pp_lbproc_pairs.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/_structured_array_identification.py` & `scitools-iris-3.6.1/lib/iris/fileformats/_structured_array_identification.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/abf.py` & `scitools-iris-3.6.1/lib/iris/fileformats/abf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/cf.py` & `scitools-iris-3.6.1/lib/iris/fileformats/cf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/dot.py` & `scitools-iris-3.6.1/lib/iris/fileformats/dot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/name.py` & `scitools-iris-3.6.1/lib/iris/fileformats/name.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/name_loaders.py` & `scitools-iris-3.6.1/lib/iris/fileformats/name_loaders.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/__init__.py` & `scitools-iris-3.6.1/lib/iris/fileformats/netcdf/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/_dask_locks.py` & `scitools-iris-3.6.1/lib/iris/fileformats/netcdf/_dask_locks.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/_thread_safe_nc.py` & `scitools-iris-3.6.1/lib/iris/fileformats/netcdf/_thread_safe_nc.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/loader.py` & `scitools-iris-3.6.1/lib/iris/fileformats/netcdf/loader.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/netcdf/saver.py` & `scitools-iris-3.6.1/lib/iris/fileformats/netcdf/saver.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/nimrod.py` & `scitools-iris-3.6.1/lib/iris/fileformats/nimrod.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/nimrod_load_rules.py` & `scitools-iris-3.6.1/lib/iris/fileformats/nimrod_load_rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/pp.py` & `scitools-iris-3.6.1/lib/iris/fileformats/pp.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/pp_load_rules.py` & `scitools-iris-3.6.1/lib/iris/fileformats/pp_load_rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/pp_save_rules.py` & `scitools-iris-3.6.1/lib/iris/fileformats/pp_save_rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/rules.py` & `scitools-iris-3.6.1/lib/iris/fileformats/rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um/__init__.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_fast_load.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um/_fast_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_fast_load_structured_fields.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um/_fast_load_structured_fields.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_ff_replacement.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um/_ff_replacement.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um/_optimal_array_structuring.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um/_optimal_array_structuring.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/fileformats/um_cf_map.py` & `scitools-iris-3.6.1/lib/iris/fileformats/um_cf_map.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/io/__init__.py` & `scitools-iris-3.6.1/lib/iris/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/io/format_picker.py` & `scitools-iris-3.6.1/lib/iris/io/format_picker.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/iterate.py` & `scitools-iris-3.6.1/lib/iris/iterate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/palette.py` & `scitools-iris-3.6.1/lib/iris/palette.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/pandas.py` & `scitools-iris-3.6.1/lib/iris/pandas.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/plot.py` & `scitools-iris-3.6.1/lib/iris/plot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/quickplot.py` & `scitools-iris-3.6.1/lib/iris/quickplot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/symbols.py` & `scitools-iris-3.6.1/lib/iris/symbols.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py` & `scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py` & `scitools-iris-3.6.1/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/experimental/test_raster.py` & `scitools-iris-3.6.1/lib/iris/tests/experimental/test_raster.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/graphics/README.md` & `scitools-iris-3.6.1/lib/iris/tests/graphics/README.md`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/graphics/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/graphics/idiff.py` & `scitools-iris-3.6.1/lib/iris/tests/graphics/idiff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/graphics/recreate_imagerepo.py` & `scitools-iris-3.6.1/lib/iris/tests/graphics/recreate_imagerepo.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/analysis/test_area_weighted.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/analysis/test_area_weighted.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/concatenate/test_concatenate.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/concatenate/test_concatenate.py`

 * *Files 3% similar despite different names*

```diff
@@ -274,14 +274,25 @@
             result[0].coord("air_pressure").points, [100.0, -880.0]
         )
         np.testing.assert_allclose(
             result[0].coord("altitude").points,
             [[10.0, 20.0], [10.0, 40.0], [10.0, 20.0], [10.0, 40.0]],
         )
 
+        # Make sure indexing the resulting cube works correctly
+        # (see https://github.com/SciTools/iris/issues/5339)
+        self.assertEqual(result[0][0].shape, (2,))
+
+        # Make sure ALL aux factory dependencies of the resulting cube were
+        # properly updated (i.e., they are different from the original cubes).
+        for aux_factory in result[0].aux_factories:
+            for coord in aux_factory.dependencies.values():
+                self.assertNotEqual(id(coord), id(cube_a.coord(coord.name())))
+                self.assertNotEqual(id(coord), id(cube_b.coord(coord.name())))
+
     def test_equal_derived_coords_with_bounds(self):
         cube_a = self.create_cube()
         cube_a.coord("sigma").bounds = [[0.0, 5.0], [5.0, 20.0]]
         cube_b = cube_a.copy()
         cube_b.coord("time").points = [12, 18]
 
         result = concatenate([cube_a, cube_b])
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_CubeRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_ugrid_load.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_ugrid_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/test_ugrid_save.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/test_ugrid_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl` & `scitools-iris-3.6.1/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/fast_load/test_fast_load.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/fast_load/test_fast_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/merge/test_merge.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/merge/test_merge.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test__dask_locks.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test__dask_locks.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_attributes.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_attributes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_aux_factories.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_aux_factories.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_coord_systems.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_coord_systems.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_delayed_save.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_delayed_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_general.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_general.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_self_referencing.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_self_referencing.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/netcdf/test_thread_safety.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/netcdf/test_thread_safety.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_animate.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_animate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_colorbar.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_colorbar.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_netcdftime.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_netcdftime.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_nzdateline.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_nzdateline.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_plot_2d_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_plot_2d_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/plot/test_vector_plots.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/plot/test_vector_plots.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_Datums.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_Datums.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_PartialDateTime.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_PartialDateTime.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_climatology.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_climatology.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_ff.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_ff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_new_axis.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_new_axis.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pickle.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_pickle.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pp.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_pp.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_pp_constrained_load_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_regrid_equivalence.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_regrid_equivalence.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_regridding.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_regridding.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_subset.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_subset.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/test_trajectory.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/integration/um/test_fieldsfile.py` & `scitools-iris-3.6.1/lib/iris/tests/integration/um/test_fieldsfile.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/pp.py` & `scitools-iris-3.6.1/lib/iris/tests/pp.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/air_temperature_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/FF/air_temperature_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/air_temperature_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/FF/air_temperature_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/ffheader.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/FF/ffheader.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/soil_temperature_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/FF/soil_temperature_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/FF/surface_altitude_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/FF/surface_altitude_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_char_data.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_char_data.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_data_time_series.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/extra_x_data.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/extra_x_data.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/global_test.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/global_test.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/nae_unpacked.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/nae_unpacked.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/PP/rle_unpacked.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/PP/rle_unpacked.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/abf/load.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/abf/load.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/abs.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/abs.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_coord_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_coord_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_coord_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_coord_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_different_std_name.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_different_std_name.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_in_place.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_in_place.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_in_place_coord.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_in_place_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/addition_scalar.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/addition_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/easy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/easy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ifunc_original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/apply_ufunc_original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/areaweights_original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/areaweights_original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_foo_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/count_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_array.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_array.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_by_singular_coord.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_by_singular_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/division_scalar.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/division_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exp.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/exp.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/exponentiate.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/exponentiate.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/log.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log10.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/log10.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/log2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/log2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/maths_original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/maths_original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/max_run_foo_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/max_run_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/multiply.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/multiply.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/multiply_different_std_name.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/multiply_different_std_name.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original_common.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/original_common.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/original_hmean.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/original_hmean.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/regrid/no_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rms_weighted_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rms_weighted_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sqrt.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/sqrt.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_array.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_array.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_coord_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_coord_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_coord_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_coord_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/subtract_scalar.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/subtract_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/sum_weighted_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/sum_weighted_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_latlon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/analysis/weighted_mean_source.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/analysis/weighted_mean_source.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/categorisation/customcheck.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/categorisation/customcheck.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/categorisation/quickcheck.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/categorisation/quickcheck.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_eq_10.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_gt_10.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/masked_cube.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/masked_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/masked_save_pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/masked_save_pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_3d_simple.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_3d_simple.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_anonymous.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_anonymous.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/all_10_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/all_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/attribute_constraint.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/attribute_constraint.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_load_match.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/constrained_load/theta_load_strict.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/constrained_load/theta_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/coord_api/nd_bounds.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/coord_api/nd_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/original.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/original.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/cubelist.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/cubelist.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/single_cube.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/single_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pickling/theta.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pickling/theta.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_io/pp/load/global.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_io/pp/load/global.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_merge/test_simple_merge.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_merge/test_simple_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_orig.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_orig.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/2d_transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/2d_transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/append_multi.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/append_multi.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/append_single.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/append_single.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/default_coord_system.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/replace_multi.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/replace_multi.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/replace_single.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/replace_single.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/cube_to_pp/simple.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/cube_to_pp/simple.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/column.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/column.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/no_orog.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/no_orog.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/no_orog.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/no_orog.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_derived_coord.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_derived_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_orog.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_orog.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_orog.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_orog.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_sigma.__str__.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_sigma.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/removed_sigma.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/removed_sigma.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/derived/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/derived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/experimental/ugrid/surface_mean.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/known_loaders.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/file_load/known_loaders.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/theta_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/file_load/theta_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/u_wind_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/file_load/u_wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/v_wind_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/file_load/v_wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/file_load/wind_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/file_load/wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/imagerepo.json` & `scitools-iris-3.6.1/lib/iris/tests/results/imagerepo.json`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/iterate/izip_nd_ortho.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/iterate/izip_nd_ortho.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_aux_b_aux.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/a_aux_b_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_aux_b_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/a_aux_b_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_dim_b_aux.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/a_dim_b_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/a_dim_b_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/a_dim_b_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/dec.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/dec.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/multi_split.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/multi_split.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/separable_combination.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/separable_combination.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/single_split.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/single_split.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_with_aux.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_with_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_a_with_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/string_a_with_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_b_with_aux.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/string_b_with_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/string_b_with_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/string_b_with_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/theta.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/theta.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/theta_two_times.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/theta_two_times.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_duplicate_data.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_independent.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_independent.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging4.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging4.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_merging5.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_merging5.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_non_expanding.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_non_expanding.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_series.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_series.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_single_forecast.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_single_forecast.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_field.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_field.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_timeseries.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_trajectory.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_trajectory0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEIII_version2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEIII_version2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/name/NAMEII_timeseries.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_laea.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_laea.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_lcc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_lcc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc_false.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_monotonic.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_polar.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_polar.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_save_single.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_stereo.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_stereo.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_units_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_units_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/netcdf_units_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/netcdf_units_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/save_load_traj.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/save_load_traj.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/load_2flds.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/load_2flds.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/probability_fields.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/probability_fields.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/global.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/global.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/lbtim_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/ocean_depth.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/pp_load_rules/rotated_uk.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/stock/realistic_4d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/stock/realistic_4d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/system/supported_filetype_.nc.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/system/supported_filetype_.nc.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/system/supported_filetype_.pp.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/system/supported_filetype_.pp.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/constant_latitude.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/trajectory/constant_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/hybrid_height.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/trajectory/hybrid_height.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/single_point.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/trajectory/single_point.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/trajectory/zigzag.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/trajectory/zigzag.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/uri_callback/pp_global.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/uri_callback/pp_global.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt` & `scitools-iris-3.6.1/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/_stock_2d_latlons.py` & `scitools-iris-3.6.1/lib/iris/tests/stock/_stock_2d_latlons.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl` & `scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl` & `scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl` & `scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl` & `scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl` & `scitools-iris-3.6.1/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/mesh.py` & `scitools-iris-3.6.1/lib/iris/tests/stock/mesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/stock/netcdf.py` & `scitools-iris-3.6.1/lib/iris/tests/stock/netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/system_test.py` & `scitools-iris-3.6.1/lib/iris/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_abf.py` & `scitools-iris-3.6.1/lib/iris/tests/test_abf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_aggregate_by.py` & `scitools-iris-3.6.1/lib/iris/tests/test_aggregate_by.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_analysis.py` & `scitools-iris-3.6.1/lib/iris/tests/test_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import cf_units
 import dask.array as da
 import numpy as np
 import numpy.ma as ma
 import pytest
 
 import iris
+from iris.analysis import _Weights
 import iris.analysis.cartography
 import iris.analysis.maths
 import iris.coord_systems
 import iris.coords
 import iris.cube
 import iris.tests.stock
 import iris.util
@@ -1702,249 +1703,178 @@
         self.assertEqual(output[2], {"test_kwarg": "test", "weights": "w"})
         self.assertEqual(kwargs, {"test_kwarg": "test", "weights": "ignored"})
 
 
 class TestWeights:
     @pytest.fixture(autouse=True)
     def setup_test_data(self):
+        self.array_lib = np
+        self.target_type = np.ndarray
+        self.create_test_data()
+
+    def create_test_data(self):
+        self.data = self.array_lib.arange(6).reshape(2, 3)
         self.lat = iris.coords.DimCoord(
-            [0, 1], standard_name="latitude", units="degrees"
+            self.array_lib.array([0, 1]),
+            standard_name="latitude",
+            units="degrees",
         )
         self.lon = iris.coords.DimCoord(
-            [0, 1, 2], standard_name="longitude", units="degrees"
+            self.array_lib.array([0, 1, 2]),
+            standard_name="longitude",
+            units="degrees",
         )
         self.cell_measure = iris.coords.CellMeasure(
-            np.arange(6).reshape(2, 3), standard_name="cell_area", units="m2"
+            self.data, standard_name="cell_area", units="m2"
         )
         self.aux_coord = iris.coords.AuxCoord(
-            [3, 4], long_name="auxcoord", units="s"
+            self.array_lib.array([3, 4]), long_name="auxcoord", units="s"
         )
         self.ancillary_variable = iris.coords.AncillaryVariable(
-            [5, 6, 7], var_name="ancvar", units="kg"
+            self.array_lib.array([5, 6, 7]), var_name="ancvar", units="kg"
         )
         self.cube = iris.cube.Cube(
-            np.arange(6).reshape(2, 3),
+            self.data,
             standard_name="air_temperature",
             units="K",
             dim_coords_and_dims=[(self.lat, 0), (self.lon, 1)],
             aux_coords_and_dims=[(self.aux_coord, 0)],
             cell_measures_and_dims=[(self.cell_measure, (0, 1))],
             ancillary_variables_and_dims=[(self.ancillary_variable, 1)],
         )
 
-    def test_init_with_weights(self):
-        weights = iris.analysis._Weights([], self.cube)
-        new_weights = iris.analysis._Weights(weights, self.cube)
-        assert isinstance(new_weights, iris.analysis._Weights)
-        assert new_weights is not weights
-        np.testing.assert_array_equal(new_weights, [])
-        assert new_weights.units == "1"
-        assert weights.units == "1"
-
-    def test_init_with_weights_and_units(self):
-        weights = iris.analysis._Weights([], self.cube)
-        new_weights = iris.analysis._Weights(weights, self.cube, units="J")
-        assert isinstance(new_weights, iris.analysis._Weights)
-        assert new_weights is not weights
-        np.testing.assert_array_equal(new_weights, [])
-        assert new_weights.units == "J"
+    def test_init_with_array(self):
+        weights = _Weights(self.data, self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        assert weights.array is self.data
         assert weights.units == "1"
 
     def test_init_with_cube(self):
-        weights = iris.analysis._Weights(self.cube, self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
+        weights = _Weights(self.cube, self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        assert weights.array is self.data
         assert weights.units == "K"
 
-    def test_init_with_cube_and_units(self):
-        weights = iris.analysis._Weights(self.cube, self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
-        assert weights.units == "J"
-
     def test_init_with_str_dim_coord(self):
-        weights = iris.analysis._Weights("latitude", self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[0, 0, 0], [1, 1, 1]])
+        weights = _Weights("latitude", self.cube)
+        # DimCoord always realizes points
+        assert isinstance(weights.array, np.ndarray)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[0, 0, 0], [1, 1, 1]])
         assert weights.units == "degrees"
 
-    def test_init_with_str_dim_coord_and_units(self):
-        weights = iris.analysis._Weights("latitude", self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[0, 0, 0], [1, 1, 1]])
-        assert weights.units == "J"
-
     def test_init_with_str_aux_coord(self):
-        weights = iris.analysis._Weights("auxcoord", self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[3, 3, 3], [4, 4, 4]])
+        weights = _Weights("auxcoord", self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[3, 3, 3], [4, 4, 4]])
         assert weights.units == "s"
 
-    def test_init_with_str_aux_coord_and_units(self):
-        weights = iris.analysis._Weights("auxcoord", self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[3, 3, 3], [4, 4, 4]])
-        assert weights.units == "J"
-
     def test_init_with_str_ancillary_variable(self):
-        weights = iris.analysis._Weights("ancvar", self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[5, 6, 7], [5, 6, 7]])
+        weights = _Weights("ancvar", self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[5, 6, 7], [5, 6, 7]])
         assert weights.units == "kg"
 
-    def test_init_with_str_ancillary_variable_and_units(self):
-        weights = iris.analysis._Weights("ancvar", self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[5, 6, 7], [5, 6, 7]])
-        assert weights.units == "J"
-
     def test_init_with_str_cell_measure(self):
-        weights = iris.analysis._Weights("cell_area", self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
+        weights = _Weights("cell_area", self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, self.data)
         assert weights.units == "m2"
 
-    def test_init_with_str_cell_measure_and_units(self):
-        weights = iris.analysis._Weights("cell_area", self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
-        assert weights.units == "J"
-
     def test_init_with_dim_coord(self):
-        weights = iris.analysis._Weights(self.lat, self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[0, 0, 0], [1, 1, 1]])
+        weights = _Weights(self.lat, self.cube)
+        # DimCoord always realizes points
+        assert isinstance(weights.array, np.ndarray)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[0, 0, 0], [1, 1, 1]])
         assert weights.units == "degrees"
 
-    def test_init_with_dim_coord_and_units(self):
-        weights = iris.analysis._Weights(self.lat, self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[0, 0, 0], [1, 1, 1]])
-        assert weights.units == "J"
-
     def test_init_with_aux_coord(self):
-        weights = iris.analysis._Weights(self.aux_coord, self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[3, 3, 3], [4, 4, 4]])
+        weights = _Weights(self.aux_coord, self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[3, 3, 3], [4, 4, 4]])
         assert weights.units == "s"
 
-    def test_init_with_aux_coord_and_units(self):
-        weights = iris.analysis._Weights(self.aux_coord, self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[3, 3, 3], [4, 4, 4]])
-        assert weights.units == "J"
-
     def test_init_with_ancillary_variable(self):
-        weights = iris.analysis._Weights(self.ancillary_variable, self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[5, 6, 7], [5, 6, 7]])
+        weights = _Weights(self.ancillary_variable, self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, [[5, 6, 7], [5, 6, 7]])
         assert weights.units == "kg"
 
-    def test_init_with_ancillary_variable_and_units(self):
-        weights = iris.analysis._Weights(
-            self.ancillary_variable, self.cube, units="J"
-        )
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [[5, 6, 7], [5, 6, 7]])
-        assert weights.units == "J"
-
     def test_init_with_cell_measure(self):
-        weights = iris.analysis._Weights(self.cell_measure, self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
+        weights = _Weights(self.cell_measure, self.cube)
+        assert isinstance(weights.array, self.target_type)
+        assert isinstance(weights.units, cf_units.Unit)
+        np.testing.assert_array_equal(weights.array, self.data)
         assert weights.units == "m2"
 
-    def test_init_with_cell_measure_and_units(self):
-        weights = iris.analysis._Weights(
-            self.cell_measure, self.cube, units="J"
-        )
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.arange(6).reshape(2, 3))
-        assert weights.units == "J"
-
     def test_init_with_list(self):
-        weights = iris.analysis._Weights([1, 2, 3], self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [1, 2, 3])
+        list_in = [0, 1, 2]
+        weights = _Weights(list_in, self.cube)
+        assert isinstance(weights.array, list)
+        assert isinstance(weights.units, cf_units.Unit)
+        assert weights.array is list_in
         assert weights.units == "1"
 
-    def test_init_with_list_and_units(self):
-        weights = iris.analysis._Weights([1, 2, 3], self.cube, units="J")
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, [1, 2, 3])
-        assert weights.units == "J"
-
-    def test_init_with_ndarray(self):
-        weights = iris.analysis._Weights(np.zeros((5, 5)), self.cube)
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.zeros((5, 5)))
-        assert weights.units == "1"
 
-    def test_init_with_ndarray_and_units(self):
-        weights = iris.analysis._Weights(
-            np.zeros((5, 5)), self.cube, units="J"
-        )
-        assert isinstance(weights, iris.analysis._Weights)
-        np.testing.assert_array_equal(weights, np.zeros((5, 5)))
-        assert weights.units == "J"
-
-    def test_init_with_invalid_obj(self):
-        with pytest.raises(KeyError):
-            iris.analysis._Weights("invalid_obj", self.cube)
-
-    def test_init_with_invalid_obj_and_units(self):
-        with pytest.raises(KeyError):
-            iris.analysis._Weights("invalid_obj", self.cube, units="J")
-
-    def test_update_kwargs_no_weights(self):
-        kwargs = {"test": [1, 2, 3]}
-        iris.analysis._Weights.update_kwargs(kwargs, self.cube)
-        assert kwargs == {"test": [1, 2, 3]}
-
-    def test_update_kwargs_weights_none(self):
-        kwargs = {"test": [1, 2, 3], "weights": None}
-        iris.analysis._Weights.update_kwargs(kwargs, self.cube)
-        assert kwargs == {"test": [1, 2, 3], "weights": None}
-
-    def test_update_kwargs_weights(self):
-        kwargs = {"test": [1, 2, 3], "weights": [1, 2]}
-        iris.analysis._Weights.update_kwargs(kwargs, self.cube)
-        assert len(kwargs) == 2
-        assert kwargs["test"] == [1, 2, 3]
-        assert isinstance(kwargs["weights"], iris.analysis._Weights)
-        np.testing.assert_array_equal(kwargs["weights"], [1, 2])
-        assert kwargs["weights"].units == "1"
+class TestWeightsLazy(TestWeights):
+    """Repeat tests from ``TestWeights`` with lazy arrays."""
+
+    @pytest.fixture(autouse=True)
+    def setup_test_data(self):
+        self.array_lib = da
+        self.target_type = da.core.Array
+        self.create_test_data()
 
 
 def test__Groupby_repr():
     groupby_coord = iris.coords.AuxCoord([2000, 2000], var_name="year")
     shared_coord = iris.coords.DimCoord(
         [0, 1],
         var_name="time",
         units=cf_units.Unit("days since 2000-01-01"),
     )
     grouper = iris.analysis._Groupby([groupby_coord], [(shared_coord, 0)])
     assert repr(grouper) == "_Groupby(['year'], shared_coords=['time'])"
 
 
-CUBE = iris.cube.Cube(0)
-
-
 @pytest.mark.parametrize(
     "kwargs,expected",
     [
-        ({}, "s"),
-        ({"test": "m"}, "s"),
-        ({"weights": None}, "s"),
-        ({"weights": [1, 2, 3]}, "s"),
-        ({"weights": iris.analysis._Weights([1], CUBE)}, "s"),
-        ({"weights": iris.analysis._Weights([1], CUBE, units="kg")}, "s kg"),
+        ({}, "kg m-2"),
+        ({"test": "m"}, "kg m-2"),
+        ({"weights": None}, "kg m-2"),
+        ({"weights": [1, 2, 3]}, "kg m-2"),
+        ({"_weights_units": None}, "kg m-2"),
+        ({"test": "m", "_weights_units": None}, "kg m-2"),
+        ({"weights": None, "_weights_units": None}, "kg m-2"),
+        ({"weights": [1, 2, 3], "_weights_units": None}, "kg m-2"),
+        ({"_weights_units": "1"}, "kg m-2"),
+        ({"test": "m", "_weights_units": "1"}, "kg m-2"),
+        ({"weights": None, "_weights_units": "1"}, "kg m-2"),
+        ({"weights": [1, 2, 3], "_weights_units": "1"}, "kg m-2"),
+        ({"_weights_units": "s"}, "kg m-2"),
+        ({"test": "m", "_weights_units": "s"}, "kg m-2"),
+        ({"weights": None, "_weights_units": "s"}, "kg m-2"),
+        ({"weights": [1, 2, 3], "_weights_units": "s"}, "kg m-2 s"),
     ],
 )
 def test_sum_units_func(kwargs, expected):
-    units = cf_units.Unit("s")
+    units = cf_units.Unit("kg m-2")
     result = iris.analysis._sum_units_func(units, **kwargs)
     assert result == expected
 
+    # Make sure that the units' string representation (= origin) has not
+    # changed if the units have not changed (even when weights units are "1")
+    if result == units:
+        assert result.origin == expected
+
 
 if __name__ == "__main__":
     tests.main()
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_analysis_calculus.py` & `scitools-iris-3.6.1/lib/iris/tests/test_analysis_calculus.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_basic_maths.py` & `scitools-iris-3.6.1/lib/iris/tests/test_basic_maths.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cartography.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cartography.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cdm.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cdm.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cell.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cf.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_coding_standards.py` & `scitools-iris-3.6.1/lib/iris/tests/test_coding_standards.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_concatenate.py` & `scitools-iris-3.6.1/lib/iris/tests/test_concatenate.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 """
 
 # import iris tests first so that some things can be initialised
 # before importing anything else.
 import iris.tests as tests  # isort:skip
 
+import dask.array as da
 import numpy as np
 import numpy.ma as ma
 
 from iris.aux_factory import HybridHeightFactory
 from iris.coords import AncillaryVariable, AuxCoord, CellMeasure, DimCoord
 import iris.cube
 import iris.tests.stock as stock
@@ -796,14 +797,38 @@
         cubes.append(_make_cube(x, (4, 6), 1, derived="x,y,xy"))
         result = concatenate(cubes)
         com = _make_cube(x, (0, 6), 1, derived="x,y,xy")
         self.assertEqual(len(result), 1)
         self.assertEqual(result[0].shape, (6, 2))
         self.assertEqual(result[0], com)
 
+    def test_concat_lazy_aux_coords(self):
+        cubes = []
+        y = (0, 2)
+        cube = _make_cube((2, 4), y, 2, aux="xy")
+        cubes.append(cube)
+        cubes.append(_make_cube((0, 2), y, 1, aux="xy"))
+        for cube in cubes:
+            cube.data = cube.lazy_data()
+            cube.coord("xy-aux").points = cube.coord("xy-aux").lazy_points()
+            bounds = da.arange(
+                4 * cube.coord("xy-aux").core_points().size
+            ).reshape(cube.shape + (4,))
+            cube.coord("xy-aux").bounds = bounds
+        result = concatenate(cubes)
+
+        self.assertTrue(cubes[0].coord("xy-aux").has_lazy_points())
+        self.assertTrue(cubes[0].coord("xy-aux").has_lazy_bounds())
+
+        self.assertTrue(cubes[1].coord("xy-aux").has_lazy_points())
+        self.assertTrue(cubes[1].coord("xy-aux").has_lazy_bounds())
+
+        self.assertTrue(result[0].coord("xy-aux").has_lazy_points())
+        self.assertTrue(result[0].coord("xy-aux").has_lazy_bounds())
+
 
 class TestMulti2D(tests.IrisTest):
     def test_concat_4x2d_aux_xy(self):
         cubes = []
         y = (0, 2)
         cubes.append(_make_cube((0, 2), y, 1, aux="xy", offset=1))
         cubes.append(_make_cube((2, 4), y, 2, aux="xy", offset=2))
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_constraints.py` & `scitools-iris-3.6.1/lib/iris/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_coord_api.py` & `scitools-iris-3.6.1/lib/iris/tests/test_coord_api.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_coord_categorisation.py` & `scitools-iris-3.6.1/lib/iris/tests/test_coord_categorisation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_coordsystem.py` & `scitools-iris-3.6.1/lib/iris/tests/test_coordsystem.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_cube_to_pp.py` & `scitools-iris-3.6.1/lib/iris/tests/test_cube_to_pp.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_ff.py` & `scitools-iris-3.6.1/lib/iris/tests/test_ff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_file_load.py` & `scitools-iris-3.6.1/lib/iris/tests/test_file_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_file_save.py` & `scitools-iris-3.6.1/lib/iris/tests/test_file_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_hybrid.py` & `scitools-iris-3.6.1/lib/iris/tests/test_hybrid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_image_json.py` & `scitools-iris-3.6.1/lib/iris/tests/test_image_json.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_imports.py` & `scitools-iris-3.6.1/lib/iris/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_intersect.py` & `scitools-iris-3.6.1/lib/iris/tests/test_intersect.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_io_init.py` & `scitools-iris-3.6.1/lib/iris/tests/test_io_init.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_iterate.py` & `scitools-iris-3.6.1/lib/iris/tests/test_iterate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_lazy_aggregate_by.py` & `scitools-iris-3.6.1/lib/iris/tests/test_lazy_aggregate_by.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_load.py` & `scitools-iris-3.6.1/lib/iris/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_mapping.py` & `scitools-iris-3.6.1/lib/iris/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_merge.py` & `scitools-iris-3.6.1/lib/iris/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_name.py` & `scitools-iris-3.6.1/lib/iris/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_netcdf.py` & `scitools-iris-3.6.1/lib/iris/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_nimrod.py` & `scitools-iris-3.6.1/lib/iris/tests/test_nimrod.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_peak.py` & `scitools-iris-3.6.1/lib/iris/tests/test_peak.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_pickling.py` & `scitools-iris-3.6.1/lib/iris/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_plot.py` & `scitools-iris-3.6.1/lib/iris/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_cf.py` & `scitools-iris-3.6.1/lib/iris/tests/test_pp_cf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_module.py` & `scitools-iris-3.6.1/lib/iris/tests/test_pp_module.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_stash.py` & `scitools-iris-3.6.1/lib/iris/tests/test_pp_stash.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_pp_to_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/test_pp_to_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_quickplot.py` & `scitools-iris-3.6.1/lib/iris/tests/test_quickplot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_std_names.py` & `scitools-iris-3.6.1/lib/iris/tests/test_std_names.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_uri_callback.py` & `scitools-iris-3.6.1/lib/iris/tests/test_uri_callback.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/test_util.py` & `scitools-iris-3.6.1/lib/iris/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test__xy_range.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_area_weights.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_project.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_project.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__get_dtype.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test__output_dtype.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_add.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_add.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_divide.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_divide.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_multiply.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_multiply.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/maths/test_subtract.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/maths/test_subtract.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/stats/test_pearsonr.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Aggregator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Aggregator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_AreaWeighted.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_AreaWeighted.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_COUNT.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_COUNT.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Linear.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Linear.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MAX.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MAX.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MAX_RUN.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MAX_RUN.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MEAN.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MEAN.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_MIN.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_MIN.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_Nearest.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_Nearest.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PERCENTILE.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PERCENTILE.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PROPORTION.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PROPORTION.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PercentileAggregator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_PointInCell.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_PointInCell.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_RMS.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_RMS.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_STD_DEV.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_STD_DEV.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_SUM.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_SUM.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_VARIANCE.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_VARIANCE.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_WPERCENTILE.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test_Lenient.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test_Lenient.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__Lenient.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__Lenient.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_client.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__lenient_client.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_service.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__lenient_service.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/lenient/test__qualname.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/lenient/test__qualname.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_hexdigest.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_hexdigest.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/common/resolve/test_Resolve.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/common/resolve/test_Resolve.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/test__CubeSignature.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test__CubeSignature.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/concatenate/test_concatenate.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/concatenate/test_concatenate.py`

 * *Files 3% similar despite different names*

```diff
@@ -351,31 +351,54 @@
         result2 = concatenate([bottom, top])
         self.assertEqual(len(result1), 1)
         self.assertEqual(len(result2), 1)
         self.assertEqual(result1, result2)
 
 
 class TestConcatenate__dask(tests.IrisTest):
-    def build_lazy_cube(self, points, bounds=None, nx=4):
+    def build_lazy_cube(self, points, bounds=None, nx=4, aux_coords=False):
         data = np.arange(len(points) * nx).reshape(len(points), nx)
         data = as_lazy_data(data)
         cube = iris.cube.Cube(data, standard_name="air_temperature", units="K")
         lat = iris.coords.DimCoord(points, "latitude", bounds=bounds)
         lon = iris.coords.DimCoord(np.arange(nx), "longitude")
         cube.add_dim_coord(lat, 0)
         cube.add_dim_coord(lon, 1)
+        if aux_coords:
+            bounds = np.arange(len(points) * nx * 4).reshape(
+                len(points), nx, 4
+            )
+            bounds = as_lazy_data(bounds)
+            aux_coord = iris.coords.AuxCoord(
+                data, var_name="aux_coord", bounds=bounds
+            )
+            cube.add_aux_coord(aux_coord, (0, 1))
         return cube
 
     def test_lazy_concatenate(self):
         c1 = self.build_lazy_cube([1, 2])
         c2 = self.build_lazy_cube([3, 4, 5])
         (cube,) = concatenate([c1, c2])
         self.assertTrue(cube.has_lazy_data())
         self.assertFalse(ma.isMaskedArray(cube.data))
 
+    def test_lazy_concatenate_aux_coords(self):
+        c1 = self.build_lazy_cube([1, 2], aux_coords=True)
+        c2 = self.build_lazy_cube([3, 4, 5], aux_coords=True)
+        (result,) = concatenate([c1, c2])
+
+        self.assertTrue(c1.coord("aux_coord").has_lazy_points())
+        self.assertTrue(c1.coord("aux_coord").has_lazy_bounds())
+
+        self.assertTrue(c2.coord("aux_coord").has_lazy_points())
+        self.assertTrue(c2.coord("aux_coord").has_lazy_bounds())
+
+        self.assertTrue(result.coord("aux_coord").has_lazy_points())
+        self.assertTrue(result.coord("aux_coord").has_lazy_bounds())
+
     def test_lazy_concatenate_masked_array_mixed_deferred(self):
         c1 = self.build_lazy_cube([1, 2])
         c2 = self.build_lazy_cube([3, 4, 5])
         c2.data = np.ma.masked_greater(c2.data, 3)
         (cube,) = concatenate([c1, c2])
         self.assertTrue(cube.has_lazy_data())
         self.assertTrue(ma.isMaskedArray(cube.data))
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/config/test_NetCDF.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/config/test_NetCDF.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/test_Constraint_equality.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/constraints/test_Constraint_equality.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/constraints/test_NameConstraint.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/constraints/test_NameConstraint.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_categorisation/test_add_hour.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_GeogCS.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_GeogCS.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Geostationary.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Geostationary.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_LambertConformal.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Mercator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Mercator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Orthographic.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Orthographic.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_RotatedPole.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_Stereographic.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_Stereographic.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_AncillaryVariable.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_AncillaryVariable.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_AuxCoord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_AuxCoord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_Cell.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_Cell.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_CellMeasure.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_CellMeasure.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_CellMethod.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_CellMethod.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_Coord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_Coord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test_DimCoord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test_DimCoord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/coords/test__DimensionalMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import iris.tests as tests  # isort:skip
 
 from collections import namedtuple
 from itertools import permutations
 from unittest import mock
 
 from cf_units import Unit
+import dask.array as da
+from distributed import Client
 import numpy as np
 import numpy.ma as ma
 import pytest
 
 from iris._lazy_data import as_lazy_data
 import iris.analysis
 from iris.analysis import MEAN, SUM, Aggregator, WeightedAggregator
@@ -361,22 +363,21 @@
 
 
 class Test_collapsed__multidim_weighted_with_arr(tests.IrisTest):
     def setUp(self):
         self.data = np.arange(6.0).reshape((2, 3))
         self.lazydata = as_lazy_data(self.data)
         # Test cubes with (same-valued) real and lazy data
-        cube_real = Cube(self.data, units="m")
+        cube_real = Cube(self.data, units="kg m-2 s-1")
         for i_dim, name in enumerate(("y", "x")):
             npts = cube_real.shape[i_dim]
             coord = DimCoord(np.arange(npts), long_name=name)
             cube_real.add_dim_coord(coord, i_dim)
         self.cube_real = cube_real
         self.cube_lazy = cube_real.copy(data=self.lazydata)
-        self.cube_lazy.units = "kg"
         # Test weights and expected result for a y-collapse
         self.y_weights = np.array([0.3, 0.5])
         self.full_weights_y = np.broadcast_to(
             self.y_weights.reshape((2, 1)), cube_real.shape
         )
         self.expected_result_y = np.array([1.875, 2.875, 3.875])
         # Test weights and expected result for an x-collapse
@@ -390,112 +391,121 @@
         # Supplying full-shape weights for collapsing over a single dimension.
         cube_collapsed = self.cube_real.collapsed(
             "y", MEAN, weights=self.full_weights_y
         )
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_y
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_fullweights_lazy_y(self):
         # Full-shape weights, lazy data :  Check lazy result, same values as real calc.
         cube_collapsed = self.cube_lazy.collapsed(
             "y", MEAN, weights=self.full_weights_y
         )
         self.assertTrue(cube_collapsed.has_lazy_data())
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_y
         )
-        self.assertEqual(cube_collapsed.units, "kg")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
 
     def test_weighted_1dweights_real_y(self):
         # 1-D weights, real data :  Check same results as full-shape.
         cube_collapsed = self.cube_real.collapsed(
             "y", MEAN, weights=self.y_weights
         )
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_y
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_1dweights_lazy_y(self):
         # 1-D weights, lazy data :  Check lazy result, same values as real calc.
         cube_collapsed = self.cube_lazy.collapsed(
             "y", MEAN, weights=self.y_weights
         )
         self.assertTrue(cube_collapsed.has_lazy_data())
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_y
         )
-        self.assertEqual(cube_collapsed.units, "kg")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
 
     def test_weighted_fullweights_real_x(self):
         # Full weights, real data, ** collapse X ** :  as for 'y' case above
         cube_collapsed = self.cube_real.collapsed(
             "x", MEAN, weights=self.full_weights_x
         )
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_x
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_fullweights_lazy_x(self):
         # Full weights, lazy data, ** collapse X ** :  as for 'y' case above
         cube_collapsed = self.cube_lazy.collapsed(
             "x", MEAN, weights=self.full_weights_x
         )
         self.assertTrue(cube_collapsed.has_lazy_data())
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_x
         )
-        self.assertEqual(cube_collapsed.units, "kg")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_1dweights_real_x(self):
         # 1-D weights, real data, ** collapse X ** :  as for 'y' case above
         cube_collapsed = self.cube_real.collapsed(
             "x", MEAN, weights=self.x_weights
         )
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_x
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_1dweights_lazy_x(self):
         # 1-D weights, lazy data, ** collapse X ** :  as for 'y' case above
         cube_collapsed = self.cube_lazy.collapsed(
             "x", MEAN, weights=self.x_weights
         )
         self.assertTrue(cube_collapsed.has_lazy_data())
         self.assertArrayAlmostEqual(
             cube_collapsed.data, self.expected_result_x
         )
-        self.assertEqual(cube_collapsed.units, "kg")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_sum_fullweights_adapt_units_real_y(self):
-        # Check that units are adapted correctly ('m' * '1' = 'm')
+        # Check that units are adapted correctly (kg m-2 s-1 * 1 = kg m-2 s-1)
         cube_collapsed = self.cube_real.collapsed(
             "y", SUM, weights=self.full_weights_y
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_sum_fullweights_adapt_units_lazy_y(self):
-        # Check that units are adapted correctly ('kg' * '1' = 'kg')
+        # Check that units are adapted correctly (kg m-2 s-1 * 1 = kg m-2 s-1)
         cube_collapsed = self.cube_lazy.collapsed(
             "y", SUM, weights=self.full_weights_y
         )
-        self.assertEqual(cube_collapsed.units, "kg")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_sum_1dweights_adapt_units_real_y(self):
-        # Check that units are adapted correctly ('m' * '1' = 'm')
+        # Check that units are adapted correctly (kg m-2 s-1 * 1 = kg m-2 s-1)
         # Note: the same test with lazy data fails:
         # https://github.com/SciTools/iris/issues/5083
         cube_collapsed = self.cube_real.collapsed(
             "y", SUM, weights=self.y_weights
         )
-        self.assertEqual(cube_collapsed.units, "m")
+        self.assertEqual(cube_collapsed.units, "kg m-2 s-1")
+        self.assertEqual(cube_collapsed.units.origin, "kg m-2 s-1")
 
     def test_weighted_sum_with_unknown_units_real_y(self):
         # Check that units are adapted correctly ('unknown' * '1' = 'unknown')
         # Note: does not need to be adapted in subclasses since 'unknown'
         # multiplied by any unit is 'unknown'
         self.cube_real.units = "unknown"
         cube_collapsed = self.cube_real.collapsed(
@@ -537,35 +547,35 @@
         self.y_weights.units = "m2"
         self.full_weights_y = self.cube_real.copy(self.full_weights_y_original)
         self.full_weights_y.units = "m2"
         self.x_weights = self.cube_real[0, :].copy(self.x_weights_original)
         self.full_weights_x = self.cube_real.copy(self.full_weights_x_original)
 
     def test_weighted_sum_fullweights_adapt_units_real_y(self):
-        # Check that units are adapted correctly ('m' * 'm2' = 'm3')
+        # Check that units are adapted correctly (kg m-2 s-1 * m2 = kg s-1)
         cube_collapsed = self.cube_real.collapsed(
             "y", SUM, weights=self.full_weights_y
         )
-        self.assertEqual(cube_collapsed.units, "m3")
+        self.assertEqual(cube_collapsed.units, "kg s-1")
 
     def test_weighted_sum_fullweights_adapt_units_lazy_y(self):
-        # Check that units are adapted correctly ('kg' * 'm2' = 'kg m2')
+        # Check that units are adapted correctly (kg m-2 s-1 * m2 = kg s-1)
         cube_collapsed = self.cube_lazy.collapsed(
             "y", SUM, weights=self.full_weights_y
         )
-        self.assertEqual(cube_collapsed.units, "kg m2")
+        self.assertEqual(cube_collapsed.units, "kg s-1")
 
     def test_weighted_sum_1dweights_adapt_units_real_y(self):
-        # Check that units are adapted correctly ('m' * 'm2' = 'm3')
+        # Check that units are adapted correctly (kg m-2 s-1 * m2 = kg s-1)
         # Note: the same test with lazy data fails:
         # https://github.com/SciTools/iris/issues/5083
         cube_collapsed = self.cube_real.collapsed(
             "y", SUM, weights=self.y_weights
         )
-        self.assertEqual(cube_collapsed.units, "m3")
+        self.assertEqual(cube_collapsed.units, "kg s-1")
 
 
 class Test_collapsed__multidim_weighted_with_str(
     Test_collapsed__multidim_weighted_with_cube
 ):
     def setUp(self):
         super().setUp()
@@ -982,15 +992,15 @@
         res_cube = self.multi_dim_cube.rolling_window(
             "extra", self.mock_agg, 3
         )
         self.assertEqual(res_cube.ancillary_variables(), [])
         self.assertEqual(res_cube.cell_measures(), [])
 
     def test_weights_arr(self):
-        weights = [0, 0, 1, 0, 2]
+        weights = np.array([0, 0, 1, 0, 2])
         res_cube = self.cube.rolling_window("val", SUM, 5, weights=weights)
         np.testing.assert_array_equal(res_cube.data, [10, 13])
         self.assertEqual(res_cube.units, "kg")
 
     def test_weights_cube(self):
         weights = Cube([0, 0, 1, 0, 2], units="m2")
         res_cube = self.cube.rolling_window("val", SUM, 5, weights=weights)
@@ -3008,14 +3018,22 @@
         lazy_data = as_lazy_data(real_data)
         cube = iris.cube.Cube(lazy_data, units="m")
         real_data_ft = Unit("m").convert(real_data, "ft")
         cube.convert_units("ft")
         self.assertTrue(cube.has_lazy_data())
         self.assertArrayAllClose(cube.data, real_data_ft)
 
+    def test_unit_multiply(self):
+        _client = Client()
+        cube = iris.cube.Cube(da.arange(1), units="m")
+        cube.units *= "s-1"
+        cube.convert_units("m s-1")
+        cube.data
+        _client.close()
+
 
 class Test__eq__data(tests.IrisTest):
     """Partial cube equality testing, for data type only."""
 
     def test_data_float_eq(self):
         cube1 = Cube([1.0])
         cube2 = Cube([1.0])
```

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_CubeList.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_CubeList.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/cube/test_Cube__operators.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/cube/test_Cube__operators.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/data_manager/test_DataManager.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/data_manager/test_DataManager.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/stratify/test_relevel.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/stratify/test_relevel.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/abf/test_ABFField.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/cf/test_CFReader.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/dot/test__dot_path.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_Grid.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_Grid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test__data_fillvalue_check.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test__data_fillvalue_check.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test__fillvalue_report.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test__fillvalue_report.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPField.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_PPField.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__field_gen.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_as_fields.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_load.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_load.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save_fields.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/test_Loader.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/test_Loader.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/rules/test__make_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/test_rules.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/test_rules.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test__generate_cubes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/io/test__generate_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_expand_filespecs.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/io/test_expand_filespecs.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_run_callback.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/io/test_run_callback.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/io/test_save.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/io/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/lazy_data/test_non_lazy.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/lazy_data/test_non_lazy.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/merge/test_ProtoCube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/merge/test_ProtoCube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/pandas/test_pandas.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/pandas/test_pandas.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/__init__.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/_blockplot_common.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/_blockplot_common.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__fixup_dates.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__fixup_dates.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_defn.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__get_plot_objects.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__get_plot_objects.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_contour.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_contour.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_contourf.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_contourf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_hist.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_hist.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_outline.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_outline.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_pcolor.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_pcolormesh.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_pcolormesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_plot.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_points.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_points.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/plot/test_scatter.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/plot/test_scatter.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_contour.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_contour.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_contourf.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_contourf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_outline.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_outline.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_pcolor.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_pcolormesh.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_pcolormesh.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_plot.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_points.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_points.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/quickplot/test_scatter.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/quickplot/test_scatter.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_printout/test_Table.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_printout/test_Table.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/test_Future.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/test_Future.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/test_sample_data_path.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/test_sample_data_path.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/stock/test_netcdf.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/tests/stock/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/tests/test_IrisTest.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/tests/test_IrisTest.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/time/test_PartialDateTime.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/time/test_PartialDateTime.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__coord_regular.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test__coord_regular.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__is_circular.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test__is_circular.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__mask_array.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test__mask_array.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test__slice_data_with_keys.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test__slice_data_with_keys.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_array_equal.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_array_equal.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_column_slices_generator.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_column_slices_generator.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_describe_diff.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_describe_diff.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_equalise_attributes.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_equalise_attributes.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_file_is_newer_than.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_file_is_newer_than.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_find_discontiguities.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_find_discontiguities.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_mask_cube.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_mask_cube.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_new_axis.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_new_axis.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_reverse.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_reverse.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_rolling_window.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_rolling_window.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_squeeze.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/tests/unit/util/test_unify_time_units.py` & `scitools-iris-3.6.1/lib/iris/tests/unit/util/test_unify_time_units.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/time.py` & `scitools-iris-3.6.1/lib/iris/time.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/lib/iris/util.py` & `scitools-iris-3.6.1/lib/iris/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,26 @@
 
 import cf_units
 from dask import array as da
 import numpy as np
 import numpy.ma as ma
 
 from iris._deprecation import warn_deprecated
-from iris._lazy_data import as_concrete_data, is_lazy_data
+from iris._lazy_data import as_concrete_data, is_lazy_data, is_lazy_masked_data
 from iris.common import SERVICES
 from iris.common.lenient import _lenient_client
 import iris.exceptions
 
 
 def broadcast_to_shape(array, shape, dim_map):
     """
     Broadcast an array to a given shape.
 
     Each dimension of the array must correspond to a dimension in the
-    given shape. Striding is used to repeat the array until it matches
-    the desired shape, returning repeated views on the original array.
+    given shape. The result is a read-only view (see :func:`numpy.broadcast_to`).
     If you need to write to the resulting array, make a copy first.
 
     Args:
 
     * array (:class:`numpy.ndarray`-like)
         An array to broadcast.
 
@@ -72,43 +71,38 @@
 
     Notes
     ------
     This function maintains laziness when called; it does not realise data.
     See more at :doc:`/userguide/real_and_lazy_data`.
 
     """
-    if len(dim_map) != array.ndim:
-        # We must check for this condition here because we cannot rely on
-        # getting an error from numpy if the dim_map argument is not the
-        # correct length, we might just get a segfault.
-        raise ValueError(
-            "dim_map must have an entry for every "
-            "dimension of the input array"
-        )
-
-    def _broadcast_helper(a):
-        strides = [0] * len(shape)
-        for idim, dim in enumerate(dim_map):
-            if shape[dim] != a.shape[idim]:
-                # We'll get garbage values if the dimensions of array are not
-                # those indicated by shape.
-                raise ValueError("shape and array are not compatible")
-            strides[dim] = a.strides[idim]
-        return np.lib.stride_tricks.as_strided(a, shape=shape, strides=strides)
-
-    array_view = _broadcast_helper(array)
-    if ma.isMaskedArray(array):
-        if array.mask is ma.nomask:
-            # Degenerate masks can be applied as-is.
-            mask_view = array.mask
+    n_orig_dims = len(array.shape)
+    n_new_dims = len(shape) - n_orig_dims
+    array = array.reshape(array.shape + (1,) * n_new_dims)
+
+    # Get dims in required order.
+    array = np.moveaxis(array, range(n_orig_dims), dim_map)
+    new_array = np.broadcast_to(array, shape)
+
+    if ma.isMA(array):
+        # broadcast_to strips masks so we need to handle them explicitly.
+        mask = ma.getmask(array)
+        if mask is ma.nomask:
+            new_mask = ma.nomask
         else:
-            # Mask arrays need to be handled in the same way as the data array.
-            mask_view = _broadcast_helper(array.mask)
-        array_view = ma.array(array_view, mask=mask_view)
-    return array_view
+            new_mask = np.broadcast_to(mask, shape)
+        new_array = ma.array(new_array, mask=new_mask)
+
+    elif is_lazy_masked_data(array):
+        # broadcast_to strips masks so we need to handle them explicitly.
+        mask = da.ma.getmaskarray(array)
+        new_mask = da.broadcast_to(mask, shape)
+        new_array = da.ma.masked_array(new_array, new_mask)
+
+    return new_array
 
 
 def delta(ndarray, dimension, circular=False):
     """
     Calculates the difference between values along a given dimension.
 
     Args:
```

### Comparing `scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/PKG-INFO` & `scitools-iris-3.6.1/lib/scitools_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitools-iris
-Version: 3.6.0rc0
+Version: 3.6.1
 Summary: A powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 Author-email: Iris Contributors <scitools.pub@gmail.com>
 License: LGPL-3.0-or-later
 Project-URL: Code, https://github.com/SciTools/iris
 Project-URL: Discussions, https://github.com/SciTools/iris/discussions
 Project-URL: Documentation, https://scitools-iris.readthedocs.io/en/stable/
 Project-URL: Issues, https://github.com/SciTools/iris/issues
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: scitools-iris Version: 3.6.0rc0 Summary: A
-powerful, format-agnostic, community-driven Python package for analysing and
-visualising Earth science data Author-email: Iris Contributors
+Metadata-Version: 2.1 Name: scitools-iris Version: 3.6.1 Summary: A powerful,
+format-agnostic, community-driven Python package for analysing and visualising
+Earth science data Author-email: Iris Contributors
 pub@gmail.com> License: LGPL-3.0-or-later Project-URL: Code, https://
 github.com/SciTools/iris Project-URL: Discussions, https://github.com/SciTools/
 iris/discussions Project-URL: Documentation, https://scitools-
 iris.readthedocs.io/en/stable/ Project-URL: Issues, https://github.com/
 SciTools/iris/issues Keywords: cf-metadata,data-analysis,earth-
 science,grib,netcdf,meteorology,oceanography,space-weather,ugrid,visualisation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `scitools-iris-3.6.0rc0/lib/scitools_iris.egg-info/SOURCES.txt` & `scitools-iris-3.6.1/lib/scitools_iris.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1269,14 +1269,16 @@
 lib/iris/tests/unit/common/mixin/__init__.py
 lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py
 lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py
 lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py
 lib/iris/tests/unit/common/resolve/__init__.py
 lib/iris/tests/unit/common/resolve/test_Resolve.py
 lib/iris/tests/unit/concatenate/__init__.py
+lib/iris/tests/unit/concatenate/test__CoordMetaData.py
+lib/iris/tests/unit/concatenate/test__CoordSignature.py
 lib/iris/tests/unit/concatenate/test__CubeSignature.py
 lib/iris/tests/unit/concatenate/test_concatenate.py
 lib/iris/tests/unit/config/__init__.py
 lib/iris/tests/unit/config/test_NetCDF.py
 lib/iris/tests/unit/constraints/__init__.py
 lib/iris/tests/unit/constraints/test_Constraint_equality.py
 lib/iris/tests/unit/constraints/test_NameConstraint.py
@@ -1464,14 +1466,15 @@
 lib/iris/tests/unit/io/test_run_callback.py
 lib/iris/tests/unit/io/test_save.py
 lib/iris/tests/unit/lazy_data/__init__.py
 lib/iris/tests/unit/lazy_data/test_as_concrete_data.py
 lib/iris/tests/unit/lazy_data/test_as_lazy_data.py
 lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py
 lib/iris/tests/unit/lazy_data/test_is_lazy_data.py
+lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py
 lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py
 lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py
 lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py
 lib/iris/tests/unit/lazy_data/test_non_lazy.py
 lib/iris/tests/unit/merge/__init__.py
 lib/iris/tests/unit/merge/test_ProtoCube.py
 lib/iris/tests/unit/pandas/__init__.py
```

### Comparing `scitools-iris-3.6.0rc0/pyproject.toml` & `scitools-iris-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/setup.py` & `scitools-iris-3.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `scitools-iris-3.6.0rc0/tools/generate_std_names.py` & `scitools-iris-3.6.1/tools/generate_std_names.py`

 * *Files identical despite different names*

