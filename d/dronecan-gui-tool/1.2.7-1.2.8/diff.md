# Comparing `tmp/dronecan_gui_tool-1.2.7.tar.gz` & `tmp/dronecan_gui_tool-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronecan_gui_tool-1.2.7.tar", last modified: Fri Feb 18 01:05:17 2022, max compression
+gzip compressed data, was "dronecan_gui_tool-1.2.8.tar", last modified: Sun Aug 14 23:24:09 2022, max compression
```

## Comparing `dronecan_gui_tool-1.2.7.tar` & `dronecan_gui_tool-1.2.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.111648 dronecan_gui_tool-1.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.103648 dronecan_gui_tool-1.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/.github/workflows/winbuild.yml
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-18 01:05:17.111648 dronecan_gui_tool-1.2.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     4709 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1766 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/bin/dronecan_gui_tool
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/active_data_type_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    21015 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/icons/dronecan_gui_tool.png
--rw-r--r--   0 runner    (1001) docker     (121)    55632 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/icons/logo.ico
--rw-r--r--   0 runner    (1001) docker     (121)    29741 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/actuator_panel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7695 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/esc_panel.py
--rw-r--r--   0 runner    (1001) docker     (121)    11130 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/setup_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/update_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)    23307 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/about_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/transfer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    17031 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/can_adapter_control_panel/
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/can_adapter_control_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22019 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/can_adapter_control_panel/slcan_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9491 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/dynamic_node_id_allocator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9394 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/file_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/local_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/log_message_display.py
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/node_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    34253 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/node_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/
--rw-r--r--   0 runner    (1001) docker     (121)     6486 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.111648 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/xy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6782 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/yt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/value_extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)    15255 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/value_extractor_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     5434 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/window.py
--rw-r--r--   0 runner    (1001) docker     (121)    11418 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.107648 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-18 01:05:16.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-02-18 01:05:17.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 01:05:16.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-18 01:05:16.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-02-18 01:05:17.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-18 01:05:17.000000 dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 01:05:17.111648 dronecan_gui_tool-1.2.7/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    55632 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/icons/logo.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/pip_sizes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       62 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/remove_build_outputs.sh
--rw-r--r--   0 runner    (1001) docker     (121)   299660 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-18 01:05:17.111648 dronecan_gui_tool-1.2.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     6528 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-02-18 01:04:34.000000 dronecan_gui_tool-1.2.7/winbuild.bat
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.571248 dronecan_gui_tool-1.2.8/.github/
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/.github/workflows/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      917 2022-02-09 01:04:27.000000 dronecan_gui_tool-1.2.8/.github/workflows/python-package.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1148 2022-02-09 01:04:30.000000 dronecan_gui_tool-1.2.8/.github/workflows/python-publish.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1022 2022-02-09 00:03:54.000000 dronecan_gui_tool-1.2.8/.github/workflows/winbuild.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      785 2021-11-17 06:54:22.000000 dronecan_gui_tool-1.2.8/.gitignore
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      951 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/.travis.yml
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1073 2021-11-17 06:54:22.000000 dronecan_gui_tool-1.2.8/LICENSE
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      789 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/PKG-INFO
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     4709 2022-02-15 10:38:10.000000 dronecan_gui_tool-1.2.8/README.md
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/bin/
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     1766 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/bin/dronecan_gui_tool
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        0 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2287 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/active_data_type_detector.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/icons/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    21015 2022-02-08 23:39:12.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/icons/dronecan_gui_tool.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    55632 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/icons/logo.ico
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    29741 2022-07-29 05:03:11.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/main.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      989 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7633 2022-02-15 08:41:21.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/actuator_panel.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7695 2022-02-15 08:41:21.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/esc_panel.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11130 2022-02-16 20:20:03.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/setup_window.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5137 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/update_checker.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      238 2022-08-14 22:52:32.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/version.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    23307 2022-02-17 20:36:49.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4635 2022-04-27 02:50:18.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/about_window.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.579248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     4253 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2061 2022-02-09 00:36:33.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/transfer_decoder.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    17031 2022-07-29 04:32:41.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/window.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.579248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/can_adapter_control_panel/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2010 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/can_adapter_control_panel/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    22019 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/can_adapter_control_panel/slcan_cli.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9491 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/console.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6281 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/dynamic_node_id_allocator.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     9394 2022-02-08 23:39:12.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/file_server.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6716 2022-02-17 22:41:27.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/local_node.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2219 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/log_message_display.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6552 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/node_monitor.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    34253 2022-02-15 08:41:21.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/node_properties.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6486 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/__init__.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1885 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/__init__.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     7048 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/xy.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     6782 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/yt.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     3640 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_container.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2201 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/value_extractor.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    15255 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/value_extractor_views.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     5434 2022-07-29 04:32:41.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/window.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    11418 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/subscriber.py
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.575248 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      789 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     2040 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)        1 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       63 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      199 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/requires.txt
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       18 2022-08-14 23:24:09.000000 dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/top_level.txt
+drwxrwxr-x   0 tridge    (1000) tridge    (1000)        0 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/icons/
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)    55632 2022-02-08 23:39:18.000000 dronecan_gui_tool-1.2.8/icons/logo.ico
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)     1261 2022-02-09 00:03:54.000000 dronecan_gui_tool-1.2.8/pip_sizes.py
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)       62 2021-12-09 00:17:16.000000 dronecan_gui_tool-1.2.8/remove_build_outputs.sh
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)   299660 2021-11-17 06:54:22.000000 dronecan_gui_tool-1.2.8/screenshot.png
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)       79 2022-08-14 23:24:09.583248 dronecan_gui_tool-1.2.8/setup.cfg
+-rwxrwxr-x   0 tridge    (1000) tridge    (1000)     6528 2022-08-14 22:50:46.000000 dronecan_gui_tool-1.2.8/setup.py
+-rw-rw-r--   0 tridge    (1000) tridge    (1000)      908 2022-02-09 00:03:54.000000 dronecan_gui_tool-1.2.8/winbuild.bat
```

### Comparing `dronecan_gui_tool-1.2.7/.github/workflows/python-package.yml` & `dronecan_gui_tool-1.2.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/.github/workflows/python-publish.yml` & `dronecan_gui_tool-1.2.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/.github/workflows/winbuild.yml` & `dronecan_gui_tool-1.2.8/.github/workflows/winbuild.yml`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/.gitignore` & `dronecan_gui_tool-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/.travis.yml` & `dronecan_gui_tool-1.2.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/LICENSE` & `dronecan_gui_tool-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/PKG-INFO` & `dronecan_gui_tool-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronecan_gui_tool
-Version: 1.2.7
+Version: 1.2.8
 Summary: DroneCAN Bus Management and Diagnostics App
 Home-page: http://dronecan.org
 Author: DroneCAN Development Team
 Author-email: dronecan.devel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dronecan_gui_tool-1.2.7/README.md` & `dronecan_gui_tool-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/bin/dronecan_gui_tool` & `dronecan_gui_tool-1.2.8/bin/dronecan_gui_tool`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/active_data_type_detector.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/active_data_type_detector.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/icons/dronecan_gui_tool.png` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/icons/dronecan_gui_tool.png`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/icons/logo.ico` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/main.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/main.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/actuator_panel.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/actuator_panel.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/panels/esc_panel.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/panels/esc_panel.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/setup_window.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/setup_window.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/update_checker.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/update_checker.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/about_window.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/about_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,27 @@
 
     try:
         from qtconsole import __version__ as qtconsole_version
         from IPython import __version__ as ipython_version
     except ImportError:
         qtconsole_version = 'N/A'
         ipython_version = 'N/A'
+    try:
+        from pymavlink import __version__ as pymavlink_version
+    except ImportError:
+        pymavlink_version = 'N/A'
 
     return [
-        ('PyDroneCAN',    dronecan.__version__,     'MIT',      'http://dronecan.org/Implementations/Pydronecan'),
+        ('PyDroneCAN',  dronecan.__version__,   'MIT',      'http://dronecan.org/Implementations/Pydronecan'),
         ('PyQt5',       PYQT_VERSION_STR,       'GPLv3',    'https://www.riverbankcomputing.com/software/pyqt/intro'),
         ('PyQtGraph',   pyqtgraph.__version__,  'MIT',      'http://www.pyqtgraph.org/'),
         ('QtAwesome',   qtawesome.__version__,  'MIT',      'https://github.com/spyder-ide/qtawesome'),
         ('QtConsole',   qtconsole_version,      'BSD',      'http://jupyter.org'),
         ('IPython',     ipython_version,        'BSD',      'https://ipython.org'),
+        ('pymavlink',   pymavlink_version,      'LGPLv3+',  'http://github.com/ardupilot/pymavlink'),
     ]
 
 
 class AboutWindow(QDialog):
     def __init__(self, parent):
         super(AboutWindow, self).__init__(parent)
         self.setAttribute(Qt.WA_DeleteOnClose)
```

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/transfer_decoder.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/transfer_decoder.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/bus_monitor/window.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/bus_monitor/window.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/can_adapter_control_panel/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/can_adapter_control_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/can_adapter_control_panel/slcan_cli.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/can_adapter_control_panel/slcan_cli.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/console.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/console.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/dynamic_node_id_allocator.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/dynamic_node_id_allocator.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/file_server.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/file_server.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/local_node.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/local_node.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/log_message_display.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/log_message_display.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/node_monitor.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/node_monitor.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/node_properties.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/node_properties.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/__init__.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/xy.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/xy.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_areas/yt.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_areas/yt.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/plot_container.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/plot_container.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/value_extractor.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/value_extractor.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/value_extractor_views.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/value_extractor_views.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/plotter/window.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/plotter/window.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool/widgets/subscriber.py` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool/widgets/subscriber.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/PKG-INFO` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronecan-gui-tool
-Version: 1.2.7
+Version: 1.2.8
 Summary: DroneCAN Bus Management and Diagnostics App
 Home-page: http://dronecan.org
 Author: DroneCAN Development Team
 Author-email: dronecan.devel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dronecan_gui_tool-1.2.7/dronecan_gui_tool.egg-info/SOURCES.txt` & `dronecan_gui_tool-1.2.8/dronecan_gui_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/icons/logo.ico` & `dronecan_gui_tool-1.2.8/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/pip_sizes.py` & `dronecan_gui_tool-1.2.8/pip_sizes.py`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/screenshot.png` & `dronecan_gui_tool-1.2.8/screenshot.png`

 * *Files identical despite different names*

### Comparing `dronecan_gui_tool-1.2.7/setup.py` & `dronecan_gui_tool-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     packages=find_packages(),
     setup_requires=[
         'setuptools',
         'setuptools_git>=1.0',
     ],
     install_requires=[
         'setuptools>=18.5',
-        'dronecan>=1.0.11',
+        'dronecan>=1.0.14',
         'pyserial>=3.0',
-        'pymavlink>=2.4.25',
+        'pymavlink>=2.4.26',
         'qtawesome>=0.3.1',
         'qtconsole>=4.2.0',
         'pyyaml>=5.1',
         'easywebdav>=1.2',
         'numpy',
         'pyqt5',
         'traitlets',
```

### Comparing `dronecan_gui_tool-1.2.7/winbuild.bat` & `dronecan_gui_tool-1.2.8/winbuild.bat`

 * *Files identical despite different names*

