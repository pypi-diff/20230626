# Comparing `tmp/biosteam-2.9.8.tar.gz` & `tmp/biosteam-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\biosteam-2.9.8.tar", last modified: Tue Mar 31 20:07:07 2020, max compression
+gzip compressed data, was "dist\biosteam-2.9.9.tar", last modified: Tue Mar 31 20:08:45 2020, max compression
```

## Comparing `biosteam-2.9.8.tar` & `biosteam-2.9.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/
--rw-rw-rw-   0        0        0     5234 2020-03-31 20:07:07.000000 biosteam-2.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     3631 2020-03-28 16:37:01.000000 biosteam-2.9.8/README.rst
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/
--rw-rw-rw-   0        0        0     1047 2020-03-12 03:13:21.000000 biosteam-2.9.8/biosteam/__init__.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/_digraph/
--rw-rw-rw-   0        0        0      249 2020-03-31 06:56:14.000000 biosteam-2.9.8/biosteam/_digraph/__init__.py
--rw-rw-rw-   0        0        0     7777 2020-03-31 09:46:18.000000 biosteam-2.9.8/biosteam/_digraph/digraph.py
--rw-rw-rw-   0        0        0    12845 2020-03-31 20:06:17.000000 biosteam-2.9.8/biosteam/_digraph/widget.py
--rw-rw-rw-   0        0        0      953 2020-03-16 08:22:17.000000 biosteam-2.9.8/biosteam/_exceptions.py
--rw-rw-rw-   0        0        0     1161 2020-03-19 14:36:41.000000 biosteam-2.9.8/biosteam/_facility.py
--rw-rw-rw-   0        0        0     9951 2020-03-31 17:37:36.000000 biosteam-2.9.8/biosteam/_flowsheet.py
--rw-rw-rw-   0        0        0     6243 2020-03-31 06:52:14.000000 biosteam-2.9.8/biosteam/_graphics.py
--rw-rw-rw-   0        0        0    19084 2020-03-27 19:54:02.000000 biosteam-2.9.8/biosteam/_heat_utility.py
--rw-rw-rw-   0        0        0    12709 2020-03-31 15:08:30.000000 biosteam-2.9.8/biosteam/_network.py
--rw-rw-rw-   0        0        0     2149 2020-02-15 09:14:49.000000 biosteam-2.9.8/biosteam/_power_utility.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/_report/
--rw-rw-rw-   0        0        0      255 2019-03-20 01:20:02.000000 biosteam-2.9.8/biosteam/_report/__init__.py
--rw-rw-rw-   0        0        0     3024 2019-04-01 18:00:15.000000 biosteam-2.9.8/biosteam/_report/plot.py
--rw-rw-rw-   0        0        0    10371 2020-03-16 09:09:57.000000 biosteam-2.9.8/biosteam/_report/table.py
--rw-rw-rw-   0        0        0    26554 2020-03-31 17:20:22.000000 biosteam-2.9.8/biosteam/_system.py
--rw-rw-rw-   0        0        0    34806 2020-03-28 16:43:08.000000 biosteam-2.9.8/biosteam/_tea.py
--rw-rw-rw-   0        0        0    27459 2020-03-31 17:20:54.000000 biosteam-2.9.8/biosteam/_unit.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/evaluation/
--rw-rw-rw-   0        0        0      555 2020-03-08 04:00:04.000000 biosteam-2.9.8/biosteam/evaluation/__init__.py
--rw-rw-rw-   0        0        0     2986 2020-03-28 01:02:17.000000 biosteam-2.9.8/biosteam/evaluation/_block.py
--rw-rw-rw-   0        0        0      881 2020-01-09 06:01:08.000000 biosteam-2.9.8/biosteam/evaluation/_metric.py
--rw-rw-rw-   0        0        0     9493 2020-03-31 17:37:01.000000 biosteam-2.9.8/biosteam/evaluation/_model.py
--rw-rw-rw-   0        0        0      513 2020-01-09 06:01:08.000000 biosteam-2.9.8/biosteam/evaluation/_name.py
--rw-rw-rw-   0        0        0     1878 2020-03-08 04:07:45.000000 biosteam-2.9.8/biosteam/evaluation/_parameter.py
--rw-rw-rw-   0        0        0    10822 2020-03-28 01:03:49.000000 biosteam-2.9.8/biosteam/evaluation/_state.py
--rw-rw-rw-   0        0        0     1934 2020-03-08 04:06:40.000000 biosteam-2.9.8/biosteam/evaluation/_variable.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/evaluation/evaluation_tools/
--rw-rw-rw-   0        0        0      178 2020-01-24 02:03:43.000000 biosteam-2.9.8/biosteam/evaluation/evaluation_tools/__init__.py
--rw-rw-rw-   0        0        0     1744 2020-01-25 18:06:00.000000 biosteam-2.9.8/biosteam/evaluation/evaluation_tools/in_parallel.py
--rw-rw-rw-   0        0        0     8556 2020-03-17 04:34:58.000000 biosteam-2.9.8/biosteam/evaluation/evaluation_tools/parameter.py
--rw-rw-rw-   0        0        0     8406 2020-03-17 04:36:39.000000 biosteam-2.9.8/biosteam/evaluation/evaluation_tools/plot.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/tests/
--rw-rw-rw-   0        0        0      515 2020-02-06 15:06:45.000000 biosteam-2.9.8/biosteam/tests/__init__.py
--rw-rw-rw-   0        0        0      859 2020-03-05 03:32:13.000000 biosteam-2.9.8/biosteam/tests/biorefinery_tests.py
--rw-rw-rw-   0        0        0     1886 2020-03-28 13:58:43.000000 biosteam-2.9.8/biosteam/tests/unit_operation_tests.py
--rw-rw-rw-   0        0        0      479 2020-03-08 05:25:43.000000 biosteam-2.9.8/biosteam/tests/utility_tests.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/units/
--rw-rw-rw-   0        0        0      139 2020-01-04 12:00:08.000000 biosteam-2.9.8/biosteam/units/_CAS.py
--rw-rw-rw-   0        0        0     2931 2020-03-31 06:55:53.000000 biosteam-2.9.8/biosteam/units/__init__.py
--rw-rw-rw-   0        0        0     9520 2020-03-24 23:31:44.000000 biosteam-2.9.8/biosteam/units/_balance.py
--rw-rw-rw-   0        0        0    41973 2020-03-28 02:34:53.000000 biosteam-2.9.8/biosteam/units/_binary_distillation.py
--rw-rw-rw-   0        0        0     1524 2020-02-19 14:03:20.000000 biosteam-2.9.8/biosteam/units/_clarifier.py
--rw-rw-rw-   0        0        0      894 2020-03-12 02:47:38.000000 biosteam-2.9.8/biosteam/units/_conveying_belt.py
--rw-rw-rw-   0        0        0      680 2020-02-19 14:03:20.000000 biosteam-2.9.8/biosteam/units/_crushing_mill.py
--rw-rw-rw-   0        0        0     1036 2020-03-31 07:12:29.000000 biosteam-2.9.8/biosteam/units/_diagram_only_units.py
--rw-rw-rw-   0        0        0     1774 2020-03-18 03:07:20.000000 biosteam-2.9.8/biosteam/units/_duplicator.py
--rw-rw-rw-   0        0        0     1348 2020-03-28 14:27:26.000000 biosteam-2.9.8/biosteam/units/_enzyme_treatment.py
--rw-rw-rw-   0        0        0    12962 2020-03-31 07:41:18.000000 biosteam-2.9.8/biosteam/units/_fermentation.py
--rw-rw-rw-   0        0        0    27575 2020-03-21 12:17:22.000000 biosteam-2.9.8/biosteam/units/_flash.py
--rw-rw-rw-   0        0        0    26457 2020-03-28 14:31:49.000000 biosteam-2.9.8/biosteam/units/_hx.py
--rw-rw-rw-   0        0        0     3949 2020-03-16 01:05:44.000000 biosteam-2.9.8/biosteam/units/_junction.py
--rw-rw-rw-   0        0        0     6818 2020-03-31 17:02:20.000000 biosteam-2.9.8/biosteam/units/_liquids_centrifuge.py
--rw-rw-rw-   0        0        0      300 2020-02-19 14:01:26.000000 biosteam-2.9.8/biosteam/units/_magnetic_separator.py
--rw-rw-rw-   0        0        0     1323 2020-03-16 01:02:06.000000 biosteam-2.9.8/biosteam/units/_mixer.py
--rw-rw-rw-   0        0        0     4028 2020-03-08 04:56:10.000000 biosteam-2.9.8/biosteam/units/_molecular_sieve.py
--rw-rw-rw-   0        0        0     8624 2020-03-14 06:06:05.000000 biosteam-2.9.8/biosteam/units/_multi_effect_evaporator.py
--rw-rw-rw-   0        0        0     3234 2020-03-17 06:53:17.000000 biosteam-2.9.8/biosteam/units/_process_specification.py
--rw-rw-rw-   0        0        0    10313 2020-03-14 06:31:11.000000 biosteam-2.9.8/biosteam/units/_pump.py
--rw-rw-rw-   0        0        0     3391 2020-02-15 18:15:07.000000 biosteam-2.9.8/biosteam/units/_rvf.py
--rw-rw-rw-   0        0        0      853 2020-03-16 08:10:19.000000 biosteam-2.9.8/biosteam/units/_screw_feeder.py
--rw-rw-rw-   0        0        0    16721 2020-03-28 14:33:11.000000 biosteam-2.9.8/biosteam/units/_shortcut_column.py
--rw-rw-rw-   0        0        0      300 2020-02-19 14:01:57.000000 biosteam-2.9.8/biosteam/units/_shredder.py
--rw-rw-rw-   0        0        0     2134 2020-03-16 08:08:47.000000 biosteam-2.9.8/biosteam/units/_solids_centrifuge.py
--rw-rw-rw-   0        0        0     1443 2020-03-14 06:32:28.000000 biosteam-2.9.8/biosteam/units/_solids_separator.py
--rw-rw-rw-   0        0        0     8075 2020-03-16 01:16:45.000000 biosteam-2.9.8/biosteam/units/_splitter.py
--rw-rw-rw-   0        0        0    10188 2020-03-28 12:22:09.000000 biosteam-2.9.8/biosteam/units/_tank.py
--rw-rw-rw-   0        0        0     4009 2020-03-28 11:27:03.000000 biosteam-2.9.8/biosteam/units/_transesterification.py
--rw-rw-rw-   0        0        0      880 2020-03-14 06:32:25.000000 biosteam-2.9.8/biosteam/units/_vent_scrubber.py
--rw-rw-rw-   0        0        0      596 2020-02-19 14:02:59.000000 biosteam-2.9.8/biosteam/units/_vibrating_screen.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/units/decorators/
--rw-rw-rw-   0        0        0      262 2019-06-27 02:10:45.000000 biosteam-2.9.8/biosteam/units/decorators/__init__.py
--rw-rw-rw-   0        0        0     6062 2020-02-15 09:45:30.000000 biosteam-2.9.8/biosteam/units/decorators/_cost.py
--rw-rw-rw-   0        0        0     4840 2020-03-24 22:52:23.000000 biosteam-2.9.8/biosteam/units/decorators/_design.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/units/design_tools/
--rw-rw-rw-   0        0        0      841 2020-03-28 12:19:08.000000 biosteam-2.9.8/biosteam/units/design_tools/__init__.py
--rw-rw-rw-   0        0        0     1443 2020-03-31 01:42:21.000000 biosteam-2.9.8/biosteam/units/design_tools/batch.py
--rw-rw-rw-   0        0        0    11462 2020-03-28 02:07:20.000000 biosteam-2.9.8/biosteam/units/design_tools/column_design.py
--rw-rw-rw-   0        0        0     1234 2020-03-28 02:27:34.000000 biosteam-2.9.8/biosteam/units/design_tools/cost_index.py
--rw-rw-rw-   0        0        0     9308 2020-03-28 02:26:49.000000 biosteam-2.9.8/biosteam/units/design_tools/flash_vessel_design.py
--rw-rw-rw-   0        0        0     9319 2020-03-28 02:12:22.000000 biosteam-2.9.8/biosteam/units/design_tools/heat_transfer.py
--rw-rw-rw-   0        0        0     1486 2020-03-28 02:13:06.000000 biosteam-2.9.8/biosteam/units/design_tools/mechanical.py
--rw-rw-rw-   0        0        0     5491 2020-03-28 02:23:15.000000 biosteam-2.9.8/biosteam/units/design_tools/specification_factors.py
--rw-rw-rw-   0        0        0     6367 2020-03-28 12:45:31.000000 biosteam-2.9.8/biosteam/units/design_tools/tank_design.py
--rw-rw-rw-   0        0        0     7898 2020-03-28 02:25:43.000000 biosteam-2.9.8/biosteam/units/design_tools/vacuum.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/units/facilities/
--rw-rw-rw-   0        0        0      763 2019-07-30 04:06:33.000000 biosteam-2.9.8/biosteam/units/facilities/__init__.py
--rw-rw-rw-   0        0        0     1335 2020-03-16 02:34:52.000000 biosteam-2.9.8/biosteam/units/facilities/_air_distribution_package.py
--rw-rw-rw-   0        0        0     6487 2020-03-17 04:42:27.000000 biosteam-2.9.8/biosteam/units/facilities/_boiler_turbogenerator.py
--rw-rw-rw-   0        0        0     2006 2020-03-11 12:23:30.000000 biosteam-2.9.8/biosteam/units/facilities/_chilled_water_package.py
--rw-rw-rw-   0        0        0     3154 2020-03-17 06:34:50.000000 biosteam-2.9.8/biosteam/units/facilities/_cooling_tower.py
--rw-rw-rw-   0        0        0     3521 2020-03-31 16:52:05.000000 biosteam-2.9.8/biosteam/units/facilities/_process_water_center.py
--rw-rw-rw-   0        0        0     2327 2020-01-25 10:31:38.000000 biosteam-2.9.8/biosteam/units/factories.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam/utils/
--rw-rw-rw-   0        0        0     1274 2020-03-16 08:06:25.000000 biosteam-2.9.8/biosteam/utils/__init__.py
--rw-rw-rw-   0        0        0     2555 2020-03-16 08:21:58.000000 biosteam-2.9.8/biosteam/utils/biosteam_colors.py
--rw-rw-rw-   0        0        0      626 2020-03-15 07:39:29.000000 biosteam-2.9.8/biosteam/utils/bounded_numerical_specification.py
--rw-rw-rw-   0        0        0      989 2020-03-13 17:36:14.000000 biosteam-2.9.8/biosteam/utils/functors.py
--rw-rw-rw-   0        0        0     2038 2020-03-13 17:36:33.000000 biosteam-2.9.8/biosteam/utils/misc.py
--rw-rw-rw-   0        0        0      549 2020-01-21 01:55:54.000000 biosteam-2.9.8/biosteam/utils/not_implemented_method.py
--rw-rw-rw-   0        0        0    12502 2020-03-31 09:27:25.000000 biosteam-2.9.8/biosteam/utils/piping.py
--rw-rw-rw-   0        0        0     6662 2020-02-11 08:15:51.000000 biosteam-2.9.8/biosteam/utils/plotting.py
--rw-rw-rw-   0        0        0     1142 2020-03-18 02:38:11.000000 biosteam-2.9.8/biosteam/utils/stream_link_options.py
--rw-rw-rw-   0        0        0     1607 2019-09-03 06:05:54.000000 biosteam-2.9.8/biosteam/utils/tictoc.py
--rw-rw-rw-   0        0        0     2922 2020-03-16 08:09:36.000000 biosteam-2.9.8/biosteam/utils/unit_warnings.py
-drwxrwxrwx   0        0        0        0 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/
--rw-rw-rw-   0        0        0     5234 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3398 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-03-31 20:07:07.000000 biosteam-2.9.8/biosteam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-03-31 20:07:07.000000 biosteam-2.9.8/setup.cfg
--rw-rw-rw-   0        0        0     2063 2020-03-31 20:04:20.000000 biosteam-2.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/
+-rw-rw-rw-   0        0        0     5234 2020-03-31 20:08:45.000000 biosteam-2.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3631 2020-03-28 16:37:01.000000 biosteam-2.9.9/README.rst
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/
+-rw-rw-rw-   0        0        0     1047 2020-03-12 03:13:21.000000 biosteam-2.9.9/biosteam/__init__.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/_digraph/
+-rw-rw-rw-   0        0        0      249 2020-03-31 06:56:14.000000 biosteam-2.9.9/biosteam/_digraph/__init__.py
+-rw-rw-rw-   0        0        0     7777 2020-03-31 09:46:18.000000 biosteam-2.9.9/biosteam/_digraph/digraph.py
+-rw-rw-rw-   0        0        0    12926 2020-03-31 20:08:14.000000 biosteam-2.9.9/biosteam/_digraph/widget.py
+-rw-rw-rw-   0        0        0      953 2020-03-16 08:22:17.000000 biosteam-2.9.9/biosteam/_exceptions.py
+-rw-rw-rw-   0        0        0     1161 2020-03-19 14:36:41.000000 biosteam-2.9.9/biosteam/_facility.py
+-rw-rw-rw-   0        0        0     9951 2020-03-31 17:37:36.000000 biosteam-2.9.9/biosteam/_flowsheet.py
+-rw-rw-rw-   0        0        0     6243 2020-03-31 06:52:14.000000 biosteam-2.9.9/biosteam/_graphics.py
+-rw-rw-rw-   0        0        0    19084 2020-03-27 19:54:02.000000 biosteam-2.9.9/biosteam/_heat_utility.py
+-rw-rw-rw-   0        0        0    12709 2020-03-31 15:08:30.000000 biosteam-2.9.9/biosteam/_network.py
+-rw-rw-rw-   0        0        0     2149 2020-02-15 09:14:49.000000 biosteam-2.9.9/biosteam/_power_utility.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/_report/
+-rw-rw-rw-   0        0        0      255 2019-03-20 01:20:02.000000 biosteam-2.9.9/biosteam/_report/__init__.py
+-rw-rw-rw-   0        0        0     3024 2019-04-01 18:00:15.000000 biosteam-2.9.9/biosteam/_report/plot.py
+-rw-rw-rw-   0        0        0    10371 2020-03-16 09:09:57.000000 biosteam-2.9.9/biosteam/_report/table.py
+-rw-rw-rw-   0        0        0    26554 2020-03-31 17:20:22.000000 biosteam-2.9.9/biosteam/_system.py
+-rw-rw-rw-   0        0        0    34806 2020-03-28 16:43:08.000000 biosteam-2.9.9/biosteam/_tea.py
+-rw-rw-rw-   0        0        0    27459 2020-03-31 17:20:54.000000 biosteam-2.9.9/biosteam/_unit.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/evaluation/
+-rw-rw-rw-   0        0        0      555 2020-03-08 04:00:04.000000 biosteam-2.9.9/biosteam/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     2986 2020-03-28 01:02:17.000000 biosteam-2.9.9/biosteam/evaluation/_block.py
+-rw-rw-rw-   0        0        0      881 2020-01-09 06:01:08.000000 biosteam-2.9.9/biosteam/evaluation/_metric.py
+-rw-rw-rw-   0        0        0     9493 2020-03-31 17:37:01.000000 biosteam-2.9.9/biosteam/evaluation/_model.py
+-rw-rw-rw-   0        0        0      513 2020-01-09 06:01:08.000000 biosteam-2.9.9/biosteam/evaluation/_name.py
+-rw-rw-rw-   0        0        0     1878 2020-03-08 04:07:45.000000 biosteam-2.9.9/biosteam/evaluation/_parameter.py
+-rw-rw-rw-   0        0        0    10822 2020-03-28 01:03:49.000000 biosteam-2.9.9/biosteam/evaluation/_state.py
+-rw-rw-rw-   0        0        0     1934 2020-03-08 04:06:40.000000 biosteam-2.9.9/biosteam/evaluation/_variable.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/evaluation/evaluation_tools/
+-rw-rw-rw-   0        0        0      178 2020-01-24 02:03:43.000000 biosteam-2.9.9/biosteam/evaluation/evaluation_tools/__init__.py
+-rw-rw-rw-   0        0        0     1744 2020-01-25 18:06:00.000000 biosteam-2.9.9/biosteam/evaluation/evaluation_tools/in_parallel.py
+-rw-rw-rw-   0        0        0     8556 2020-03-17 04:34:58.000000 biosteam-2.9.9/biosteam/evaluation/evaluation_tools/parameter.py
+-rw-rw-rw-   0        0        0     8406 2020-03-17 04:36:39.000000 biosteam-2.9.9/biosteam/evaluation/evaluation_tools/plot.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/tests/
+-rw-rw-rw-   0        0        0      515 2020-02-06 15:06:45.000000 biosteam-2.9.9/biosteam/tests/__init__.py
+-rw-rw-rw-   0        0        0      859 2020-03-05 03:32:13.000000 biosteam-2.9.9/biosteam/tests/biorefinery_tests.py
+-rw-rw-rw-   0        0        0     1886 2020-03-28 13:58:43.000000 biosteam-2.9.9/biosteam/tests/unit_operation_tests.py
+-rw-rw-rw-   0        0        0      479 2020-03-08 05:25:43.000000 biosteam-2.9.9/biosteam/tests/utility_tests.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/units/
+-rw-rw-rw-   0        0        0      139 2020-01-04 12:00:08.000000 biosteam-2.9.9/biosteam/units/_CAS.py
+-rw-rw-rw-   0        0        0     2931 2020-03-31 06:55:53.000000 biosteam-2.9.9/biosteam/units/__init__.py
+-rw-rw-rw-   0        0        0     9520 2020-03-24 23:31:44.000000 biosteam-2.9.9/biosteam/units/_balance.py
+-rw-rw-rw-   0        0        0    41973 2020-03-28 02:34:53.000000 biosteam-2.9.9/biosteam/units/_binary_distillation.py
+-rw-rw-rw-   0        0        0     1524 2020-02-19 14:03:20.000000 biosteam-2.9.9/biosteam/units/_clarifier.py
+-rw-rw-rw-   0        0        0      894 2020-03-12 02:47:38.000000 biosteam-2.9.9/biosteam/units/_conveying_belt.py
+-rw-rw-rw-   0        0        0      680 2020-02-19 14:03:20.000000 biosteam-2.9.9/biosteam/units/_crushing_mill.py
+-rw-rw-rw-   0        0        0     1036 2020-03-31 07:12:29.000000 biosteam-2.9.9/biosteam/units/_diagram_only_units.py
+-rw-rw-rw-   0        0        0     1774 2020-03-18 03:07:20.000000 biosteam-2.9.9/biosteam/units/_duplicator.py
+-rw-rw-rw-   0        0        0     1348 2020-03-28 14:27:26.000000 biosteam-2.9.9/biosteam/units/_enzyme_treatment.py
+-rw-rw-rw-   0        0        0    12962 2020-03-31 07:41:18.000000 biosteam-2.9.9/biosteam/units/_fermentation.py
+-rw-rw-rw-   0        0        0    27575 2020-03-21 12:17:22.000000 biosteam-2.9.9/biosteam/units/_flash.py
+-rw-rw-rw-   0        0        0    26457 2020-03-28 14:31:49.000000 biosteam-2.9.9/biosteam/units/_hx.py
+-rw-rw-rw-   0        0        0     3949 2020-03-16 01:05:44.000000 biosteam-2.9.9/biosteam/units/_junction.py
+-rw-rw-rw-   0        0        0     6818 2020-03-31 17:02:20.000000 biosteam-2.9.9/biosteam/units/_liquids_centrifuge.py
+-rw-rw-rw-   0        0        0      300 2020-02-19 14:01:26.000000 biosteam-2.9.9/biosteam/units/_magnetic_separator.py
+-rw-rw-rw-   0        0        0     1323 2020-03-16 01:02:06.000000 biosteam-2.9.9/biosteam/units/_mixer.py
+-rw-rw-rw-   0        0        0     4028 2020-03-08 04:56:10.000000 biosteam-2.9.9/biosteam/units/_molecular_sieve.py
+-rw-rw-rw-   0        0        0     8624 2020-03-14 06:06:05.000000 biosteam-2.9.9/biosteam/units/_multi_effect_evaporator.py
+-rw-rw-rw-   0        0        0     3234 2020-03-17 06:53:17.000000 biosteam-2.9.9/biosteam/units/_process_specification.py
+-rw-rw-rw-   0        0        0    10313 2020-03-14 06:31:11.000000 biosteam-2.9.9/biosteam/units/_pump.py
+-rw-rw-rw-   0        0        0     3391 2020-02-15 18:15:07.000000 biosteam-2.9.9/biosteam/units/_rvf.py
+-rw-rw-rw-   0        0        0      853 2020-03-16 08:10:19.000000 biosteam-2.9.9/biosteam/units/_screw_feeder.py
+-rw-rw-rw-   0        0        0    16721 2020-03-28 14:33:11.000000 biosteam-2.9.9/biosteam/units/_shortcut_column.py
+-rw-rw-rw-   0        0        0      300 2020-02-19 14:01:57.000000 biosteam-2.9.9/biosteam/units/_shredder.py
+-rw-rw-rw-   0        0        0     2134 2020-03-16 08:08:47.000000 biosteam-2.9.9/biosteam/units/_solids_centrifuge.py
+-rw-rw-rw-   0        0        0     1443 2020-03-14 06:32:28.000000 biosteam-2.9.9/biosteam/units/_solids_separator.py
+-rw-rw-rw-   0        0        0     8075 2020-03-16 01:16:45.000000 biosteam-2.9.9/biosteam/units/_splitter.py
+-rw-rw-rw-   0        0        0    10188 2020-03-28 12:22:09.000000 biosteam-2.9.9/biosteam/units/_tank.py
+-rw-rw-rw-   0        0        0     4009 2020-03-28 11:27:03.000000 biosteam-2.9.9/biosteam/units/_transesterification.py
+-rw-rw-rw-   0        0        0      880 2020-03-14 06:32:25.000000 biosteam-2.9.9/biosteam/units/_vent_scrubber.py
+-rw-rw-rw-   0        0        0      596 2020-02-19 14:02:59.000000 biosteam-2.9.9/biosteam/units/_vibrating_screen.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/units/decorators/
+-rw-rw-rw-   0        0        0      262 2019-06-27 02:10:45.000000 biosteam-2.9.9/biosteam/units/decorators/__init__.py
+-rw-rw-rw-   0        0        0     6062 2020-02-15 09:45:30.000000 biosteam-2.9.9/biosteam/units/decorators/_cost.py
+-rw-rw-rw-   0        0        0     4840 2020-03-24 22:52:23.000000 biosteam-2.9.9/biosteam/units/decorators/_design.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/units/design_tools/
+-rw-rw-rw-   0        0        0      841 2020-03-28 12:19:08.000000 biosteam-2.9.9/biosteam/units/design_tools/__init__.py
+-rw-rw-rw-   0        0        0     1443 2020-03-31 01:42:21.000000 biosteam-2.9.9/biosteam/units/design_tools/batch.py
+-rw-rw-rw-   0        0        0    11462 2020-03-28 02:07:20.000000 biosteam-2.9.9/biosteam/units/design_tools/column_design.py
+-rw-rw-rw-   0        0        0     1234 2020-03-28 02:27:34.000000 biosteam-2.9.9/biosteam/units/design_tools/cost_index.py
+-rw-rw-rw-   0        0        0     9308 2020-03-28 02:26:49.000000 biosteam-2.9.9/biosteam/units/design_tools/flash_vessel_design.py
+-rw-rw-rw-   0        0        0     9319 2020-03-28 02:12:22.000000 biosteam-2.9.9/biosteam/units/design_tools/heat_transfer.py
+-rw-rw-rw-   0        0        0     1486 2020-03-28 02:13:06.000000 biosteam-2.9.9/biosteam/units/design_tools/mechanical.py
+-rw-rw-rw-   0        0        0     5491 2020-03-28 02:23:15.000000 biosteam-2.9.9/biosteam/units/design_tools/specification_factors.py
+-rw-rw-rw-   0        0        0     6367 2020-03-28 12:45:31.000000 biosteam-2.9.9/biosteam/units/design_tools/tank_design.py
+-rw-rw-rw-   0        0        0     7898 2020-03-28 02:25:43.000000 biosteam-2.9.9/biosteam/units/design_tools/vacuum.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/units/facilities/
+-rw-rw-rw-   0        0        0      763 2019-07-30 04:06:33.000000 biosteam-2.9.9/biosteam/units/facilities/__init__.py
+-rw-rw-rw-   0        0        0     1335 2020-03-16 02:34:52.000000 biosteam-2.9.9/biosteam/units/facilities/_air_distribution_package.py
+-rw-rw-rw-   0        0        0     6487 2020-03-17 04:42:27.000000 biosteam-2.9.9/biosteam/units/facilities/_boiler_turbogenerator.py
+-rw-rw-rw-   0        0        0     2006 2020-03-11 12:23:30.000000 biosteam-2.9.9/biosteam/units/facilities/_chilled_water_package.py
+-rw-rw-rw-   0        0        0     3154 2020-03-17 06:34:50.000000 biosteam-2.9.9/biosteam/units/facilities/_cooling_tower.py
+-rw-rw-rw-   0        0        0     3521 2020-03-31 16:52:05.000000 biosteam-2.9.9/biosteam/units/facilities/_process_water_center.py
+-rw-rw-rw-   0        0        0     2327 2020-01-25 10:31:38.000000 biosteam-2.9.9/biosteam/units/factories.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam/utils/
+-rw-rw-rw-   0        0        0     1274 2020-03-16 08:06:25.000000 biosteam-2.9.9/biosteam/utils/__init__.py
+-rw-rw-rw-   0        0        0     2555 2020-03-16 08:21:58.000000 biosteam-2.9.9/biosteam/utils/biosteam_colors.py
+-rw-rw-rw-   0        0        0      626 2020-03-15 07:39:29.000000 biosteam-2.9.9/biosteam/utils/bounded_numerical_specification.py
+-rw-rw-rw-   0        0        0      989 2020-03-13 17:36:14.000000 biosteam-2.9.9/biosteam/utils/functors.py
+-rw-rw-rw-   0        0        0     2038 2020-03-13 17:36:33.000000 biosteam-2.9.9/biosteam/utils/misc.py
+-rw-rw-rw-   0        0        0      549 2020-01-21 01:55:54.000000 biosteam-2.9.9/biosteam/utils/not_implemented_method.py
+-rw-rw-rw-   0        0        0    12502 2020-03-31 09:27:25.000000 biosteam-2.9.9/biosteam/utils/piping.py
+-rw-rw-rw-   0        0        0     6662 2020-02-11 08:15:51.000000 biosteam-2.9.9/biosteam/utils/plotting.py
+-rw-rw-rw-   0        0        0     1142 2020-03-18 02:38:11.000000 biosteam-2.9.9/biosteam/utils/stream_link_options.py
+-rw-rw-rw-   0        0        0     1607 2019-09-03 06:05:54.000000 biosteam-2.9.9/biosteam/utils/tictoc.py
+-rw-rw-rw-   0        0        0     2922 2020-03-16 08:09:36.000000 biosteam-2.9.9/biosteam/utils/unit_warnings.py
+drwxrwxrwx   0        0        0        0 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/
+-rw-rw-rw-   0        0        0     5234 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3398 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2020-03-31 20:08:45.000000 biosteam-2.9.9/biosteam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-03-31 20:08:45.000000 biosteam-2.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     2063 2020-03-31 20:08:28.000000 biosteam-2.9.9/setup.py
```

### Comparing `biosteam-2.9.8/PKG-INFO` & `biosteam-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: biosteam
-Version: 2.9.8
+Version: 2.9.9
 Summary: The Biorefinery Simulation and Techno-Economic Analysis Modules
 Home-page: https://github.com/BioSTEAMDevelopmentGroup/biosteam
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Download-URL: https://github.com/BioSTEAMDevelopmentGroup/biosteam.git
 Description: =========================================================================
```

### Comparing `biosteam-2.9.8/README.rst` & `biosteam-2.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/__init__.py` & `biosteam-2.9.9/biosteam/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_digraph/digraph.py` & `biosteam-2.9.9/biosteam/_digraph/digraph.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_digraph/widget.py` & `biosteam-2.9.9/biosteam/_digraph/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 """
 Created on Sat Mar 28 21:59:13 2020
 
 @author: yoelr
 """
 from warnings import warn
 try:
-	from PyQt5.QtWidgets import (QAction, QApplication, QFileDialog,
-								 QLabel, QWidget, QMainWindow, QMenu,
-								 QMessageBox, QScrollArea, QSizePolicy, 
-								 QGridLayout, QSizePolicy, QFrame)
-	from PyQt5.QtCore import QSize, QTimer, Qt
-	from PyQt5.QtGui import QPixmap, QPalette, QImage, QFont
+    from PyQt5.QtWidgets import (QAction, QApplication, QFileDialog,
+                                 QLabel, QWidget, QMainWindow, QMenu,
+                                 QMessageBox, QScrollArea, QSizePolicy, 
+                                 QGridLayout, QSizePolicy, QFrame)
+    from PyQt5.QtCore import QSize, QTimer, Qt
+    from PyQt5.QtGui import QPixmap, QPalette, QImage, QFont
 except:
     QMainWindow = object
     warn(ImportWarning("install PyQt5 to enable dynamic flowsheets"))    
 
 from .digraph import (get_all_connections,
                       digraph_from_units_and_connections,
                       surface_digraph,
```

### Comparing `biosteam-2.9.8/biosteam/_exceptions.py` & `biosteam-2.9.9/biosteam/_exceptions.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_facility.py` & `biosteam-2.9.9/biosteam/_facility.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_flowsheet.py` & `biosteam-2.9.9/biosteam/_flowsheet.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_graphics.py` & `biosteam-2.9.9/biosteam/_graphics.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_heat_utility.py` & `biosteam-2.9.9/biosteam/_heat_utility.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_network.py` & `biosteam-2.9.9/biosteam/_network.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_power_utility.py` & `biosteam-2.9.9/biosteam/_power_utility.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_report/plot.py` & `biosteam-2.9.9/biosteam/_report/plot.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_report/table.py` & `biosteam-2.9.9/biosteam/_report/table.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_system.py` & `biosteam-2.9.9/biosteam/_system.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_tea.py` & `biosteam-2.9.9/biosteam/_tea.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/_unit.py` & `biosteam-2.9.9/biosteam/_unit.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/__init__.py` & `biosteam-2.9.9/biosteam/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_block.py` & `biosteam-2.9.9/biosteam/evaluation/_block.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_metric.py` & `biosteam-2.9.9/biosteam/evaluation/_metric.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_model.py` & `biosteam-2.9.9/biosteam/evaluation/_model.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_name.py` & `biosteam-2.9.9/biosteam/evaluation/_name.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_parameter.py` & `biosteam-2.9.9/biosteam/evaluation/_parameter.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_state.py` & `biosteam-2.9.9/biosteam/evaluation/_state.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/_variable.py` & `biosteam-2.9.9/biosteam/evaluation/_variable.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/evaluation_tools/in_parallel.py` & `biosteam-2.9.9/biosteam/evaluation/evaluation_tools/in_parallel.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/evaluation_tools/parameter.py` & `biosteam-2.9.9/biosteam/evaluation/evaluation_tools/parameter.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/evaluation/evaluation_tools/plot.py` & `biosteam-2.9.9/biosteam/evaluation/evaluation_tools/plot.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/tests/__init__.py` & `biosteam-2.9.9/biosteam/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/tests/biorefinery_tests.py` & `biosteam-2.9.9/biosteam/tests/biorefinery_tests.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/tests/unit_operation_tests.py` & `biosteam-2.9.9/biosteam/tests/unit_operation_tests.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/__init__.py` & `biosteam-2.9.9/biosteam/units/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_balance.py` & `biosteam-2.9.9/biosteam/units/_balance.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_binary_distillation.py` & `biosteam-2.9.9/biosteam/units/_binary_distillation.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_clarifier.py` & `biosteam-2.9.9/biosteam/units/_clarifier.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_conveying_belt.py` & `biosteam-2.9.9/biosteam/units/_conveying_belt.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_crushing_mill.py` & `biosteam-2.9.9/biosteam/units/_crushing_mill.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_diagram_only_units.py` & `biosteam-2.9.9/biosteam/units/_diagram_only_units.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_duplicator.py` & `biosteam-2.9.9/biosteam/units/_duplicator.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_enzyme_treatment.py` & `biosteam-2.9.9/biosteam/units/_enzyme_treatment.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_fermentation.py` & `biosteam-2.9.9/biosteam/units/_fermentation.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_flash.py` & `biosteam-2.9.9/biosteam/units/_flash.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_hx.py` & `biosteam-2.9.9/biosteam/units/_hx.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_junction.py` & `biosteam-2.9.9/biosteam/units/_junction.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_liquids_centrifuge.py` & `biosteam-2.9.9/biosteam/units/_liquids_centrifuge.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_mixer.py` & `biosteam-2.9.9/biosteam/units/_mixer.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_molecular_sieve.py` & `biosteam-2.9.9/biosteam/units/_molecular_sieve.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_multi_effect_evaporator.py` & `biosteam-2.9.9/biosteam/units/_multi_effect_evaporator.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_process_specification.py` & `biosteam-2.9.9/biosteam/units/_process_specification.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_pump.py` & `biosteam-2.9.9/biosteam/units/_pump.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_rvf.py` & `biosteam-2.9.9/biosteam/units/_rvf.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_screw_feeder.py` & `biosteam-2.9.9/biosteam/units/_screw_feeder.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_shortcut_column.py` & `biosteam-2.9.9/biosteam/units/_shortcut_column.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_solids_centrifuge.py` & `biosteam-2.9.9/biosteam/units/_solids_centrifuge.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_solids_separator.py` & `biosteam-2.9.9/biosteam/units/_solids_separator.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_splitter.py` & `biosteam-2.9.9/biosteam/units/_splitter.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_tank.py` & `biosteam-2.9.9/biosteam/units/_tank.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_transesterification.py` & `biosteam-2.9.9/biosteam/units/_transesterification.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_vent_scrubber.py` & `biosteam-2.9.9/biosteam/units/_vent_scrubber.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/_vibrating_screen.py` & `biosteam-2.9.9/biosteam/units/_vibrating_screen.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/decorators/_cost.py` & `biosteam-2.9.9/biosteam/units/decorators/_cost.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/decorators/_design.py` & `biosteam-2.9.9/biosteam/units/decorators/_design.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/__init__.py` & `biosteam-2.9.9/biosteam/units/design_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/batch.py` & `biosteam-2.9.9/biosteam/units/design_tools/batch.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/column_design.py` & `biosteam-2.9.9/biosteam/units/design_tools/column_design.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/cost_index.py` & `biosteam-2.9.9/biosteam/units/design_tools/cost_index.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/flash_vessel_design.py` & `biosteam-2.9.9/biosteam/units/design_tools/flash_vessel_design.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/heat_transfer.py` & `biosteam-2.9.9/biosteam/units/design_tools/heat_transfer.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/mechanical.py` & `biosteam-2.9.9/biosteam/units/design_tools/mechanical.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/specification_factors.py` & `biosteam-2.9.9/biosteam/units/design_tools/specification_factors.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/tank_design.py` & `biosteam-2.9.9/biosteam/units/design_tools/tank_design.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/design_tools/vacuum.py` & `biosteam-2.9.9/biosteam/units/design_tools/vacuum.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/__init__.py` & `biosteam-2.9.9/biosteam/units/facilities/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/_air_distribution_package.py` & `biosteam-2.9.9/biosteam/units/facilities/_air_distribution_package.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/_boiler_turbogenerator.py` & `biosteam-2.9.9/biosteam/units/facilities/_boiler_turbogenerator.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/_chilled_water_package.py` & `biosteam-2.9.9/biosteam/units/facilities/_chilled_water_package.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/_cooling_tower.py` & `biosteam-2.9.9/biosteam/units/facilities/_cooling_tower.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/facilities/_process_water_center.py` & `biosteam-2.9.9/biosteam/units/facilities/_process_water_center.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/units/factories.py` & `biosteam-2.9.9/biosteam/units/factories.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/__init__.py` & `biosteam-2.9.9/biosteam/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/biosteam_colors.py` & `biosteam-2.9.9/biosteam/utils/biosteam_colors.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/bounded_numerical_specification.py` & `biosteam-2.9.9/biosteam/utils/bounded_numerical_specification.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/functors.py` & `biosteam-2.9.9/biosteam/utils/functors.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/misc.py` & `biosteam-2.9.9/biosteam/utils/misc.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/not_implemented_method.py` & `biosteam-2.9.9/biosteam/utils/not_implemented_method.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/piping.py` & `biosteam-2.9.9/biosteam/utils/piping.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/plotting.py` & `biosteam-2.9.9/biosteam/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/stream_link_options.py` & `biosteam-2.9.9/biosteam/utils/stream_link_options.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/tictoc.py` & `biosteam-2.9.9/biosteam/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam/utils/unit_warnings.py` & `biosteam-2.9.9/biosteam/utils/unit_warnings.py`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/biosteam.egg-info/PKG-INFO` & `biosteam-2.9.9/biosteam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: biosteam
-Version: 2.9.8
+Version: 2.9.9
 Summary: The Biorefinery Simulation and Techno-Economic Analysis Modules
 Home-page: https://github.com/BioSTEAMDevelopmentGroup/biosteam
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Download-URL: https://github.com/BioSTEAMDevelopmentGroup/biosteam.git
 Description: =========================================================================
```

### Comparing `biosteam-2.9.8/biosteam.egg-info/SOURCES.txt` & `biosteam-2.9.9/biosteam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosteam-2.9.8/setup.py` & `biosteam-2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #from Cython.Build import cythonize
 #import numpy
 
 setup(
     name='biosteam',
     packages=['biosteam'],
     license='MIT',
-    version='2.9.8',
+    version='2.9.9',
     description='The Biorefinery Simulation and Techno-Economic Analysis Modules',
     long_description=open('README.rst').read(),
     author='Yoel Cortes-Pena',
     install_requires=['IPython==7.9.0', 'biorefineries>=2.8.0',
                       'thermosteam>=0.8.2', 'graphviz==0.8.3',
                       'chaospy==3.0.11'],
     python_requires=">=3.6",
```

