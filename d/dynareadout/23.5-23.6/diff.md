# Comparing `tmp/dynareadout-23.5.tar.gz` & `tmp/dynareadout-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-23.5.tar", last modified: Thu May 25 12:55:51 2023, max compression
+gzip compressed data, was "dynareadout-23.6.tar", last modified: Mon Jun 26 09:18:13 2023, max compression
```

## Comparing `dynareadout-23.5.tar` & `dynareadout-23.6.tar`

### file list

```diff
@@ -1,105 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.794273 dynareadout-23.5/
--rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.5/LICENSE
--rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5295 2023-05-25 12:55:51.794273 dynareadout-23.5/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2023-05-08 11:43:26.000000 dynareadout-23.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.390680 dynareadout-23.5/lib/
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.389682 dynareadout-23.5/lib/dynareadout/
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.546511 dynareadout-23.5/lib/dynareadout/src/
--rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binary_search.c
--rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binary_search.h
--rw-rw-rw-   0        0        0    30340 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout.c
--rw-rw-rw-   0        0        0     5758 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout.h
--rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_defines.h
--rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_directory.c
--rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_directory.h
--rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_glob.c
--rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_glob.h
--rw-rw-rw-   0        0        0    12007 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_read.c
--rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/binout_read.h
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.586717 dynareadout-23.5/lib/dynareadout/src/cpp/
--rw-rw-rw-   0        0        0    11031 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/array.hpp
--rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/binout.cpp
--rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/binout.hpp
--rw-rw-rw-   0        0        0    18739 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.cpp
--rw-rw-rw-   0        0        0     7831 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.hpp
--rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.cpp
--rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.hpp
--rw-rw-rw-   0        0        0     4418 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.cpp
--rw-rw-rw-   0        0        0     2636 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.hpp
--rw-rw-rw-   0        0        0     6911 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/cpp/key.cpp
--rw-rw-rw-   0        0        0    16564 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/key.hpp
--rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/cpp/vec.hpp
--rw-rw-rw-   0        0        0    18933 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_buffer.c
--rw-rw-rw-   0        0        0     3786 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_buffer.h
--rw-rw-rw-   0        0        0     6785 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3_defines.h
--rw-rw-rw-   0        0        0    90823 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot.c
--rw-rw-rw-   0        0        0    17901 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot.h
--rw-rw-rw-   0        0        0    12090 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_data.c
--rw-rw-rw-   0        0        0     4169 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_error_macros.h
--rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.c
--rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.h
--rw-rw-rw-   0        0        0    11850 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/d3plot_state.c
--rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/extra_string.c
--rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/extra_string.h
--rw-rw-rw-   0        0        0    48374 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/key.c
--rw-rw-rw-   0        0        0    10040 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/key.h
--rw-rw-rw-   0        0        0     5980 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/path.c
--rw-rw-rw-   0        0        0     2671 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/path.h
--rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/path_view.c
--rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/path_view.h
--rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/pgni.h
--rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/profiling.c
--rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/profiling.h
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.605811 dynareadout-23.5/lib/dynareadout/src/python/
--rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/conversions.hpp
--rw-rw-rw-   0        0        0     5735 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_binout.cpp
--rw-rw-rw-   0        0        0    19773 2023-05-25 12:53:57.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_d3plot.cpp
--rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_key.cpp
--rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.5/lib/dynareadout/src/python/pybind11_module.cpp
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.611795 dynareadout-23.5/lib/pybind11/
--rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.391678 dynareadout-23.5/lib/pybind11/include/
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.726198 dynareadout-23.5/lib/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.768676 dynareadout-23.5/lib/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.774324 dynareadout-23.5/lib/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.5/lib/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0      858 2023-05-25 12:54:31.000000 dynareadout-23.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 12:55:51.794273 dynareadout-23.5/setup.cfg
--rw-rw-rw-   0        0        0     2489 2023-05-25 12:55:08.000000 dynareadout-23.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.392675 dynareadout-23.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.775335 dynareadout-23.5/src/dynareadout/
--rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.5/src/dynareadout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:55:51.793275 dynareadout-23.5/src/dynareadout.egg-info/
--rw-rw-rw-   0        0        0     5295 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3177 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.5/src/dynareadout.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-25 12:55:51.000000 dynareadout-23.5/src/dynareadout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.675493 dynareadout-23.6/
+-rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.6/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5295 2023-06-26 09:18:13.675493 dynareadout-23.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4520 2023-05-08 11:43:26.000000 dynareadout-23.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.592892 dynareadout-23.6/lib/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.591894 dynareadout-23.6/lib/dynareadout/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.631789 dynareadout-23.6/lib/dynareadout/src/
+-rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binary_search.c
+-rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binary_search.h
+-rw-rw-rw-   0        0        0    30254 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout.c
+-rw-rw-rw-   0        0        0     5776 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout.h
+-rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_defines.h
+-rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_directory.c
+-rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_directory.h
+-rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_glob.c
+-rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_glob.h
+-rw-rw-rw-   0        0        0    13180 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/binout_read.c
+-rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/binout_read.h
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.640765 dynareadout-23.6/lib/dynareadout/src/cpp/
+-rw-rw-rw-   0        0        0    11763 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/array.hpp
+-rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/binout.cpp
+-rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/binout.hpp
+-rw-rw-rw-   0        0        0    18739 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.cpp
+-rw-rw-rw-   0        0        0     7831 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.hpp
+-rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.cpp
+-rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.hpp
+-rw-rw-rw-   0        0        0     4418 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.cpp
+-rw-rw-rw-   0        0        0     2848 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.hpp
+-rw-rw-rw-   0        0        0     7096 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/key.cpp
+-rw-rw-rw-   0        0        0    16902 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/cpp/key.hpp
+-rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/cpp/vec.hpp
+-rw-rw-rw-   0        0        0    22780 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3_buffer.c
+-rw-rw-rw-   0        0        0     4304 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3_buffer.h
+-rw-rw-rw-   0        0        0     6785 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/d3_defines.h
+-rw-rw-rw-   0        0        0    93920 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot.c
+-rw-rw-rw-   0        0        0    18155 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot.h
+-rw-rw-rw-   0        0        0    12437 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_data.c
+-rw-rw-rw-   0        0        0     4251 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_error_macros.h
+-rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.c
+-rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.h
+-rw-rw-rw-   0        0        0    12188 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/d3plot_state.c
+-rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/extra_string.c
+-rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/extra_string.h
+-rw-rw-rw-   0        0        0    51337 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/key.c
+-rw-rw-rw-   0        0        0    10852 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/key.h
+-rw-rw-rw-   0        0        0     6492 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/multi_file.c
+-rw-rw-rw-   0        0        0     3161 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/multi_file.h
+-rw-rw-rw-   0        0        0     5980 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/path.c
+-rw-rw-rw-   0        0        0     2671 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/path.h
+-rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/path_view.c
+-rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/path_view.h
+-rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/pgni.h
+-rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/profiling.c
+-rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/profiling.h
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.645753 dynareadout-23.6/lib/dynareadout/src/python/
+-rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/conversions.hpp
+-rw-rw-rw-   0        0        0     5735 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_binout.cpp
+-rw-rw-rw-   0        0        0    19773 2023-05-25 12:53:57.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_d3plot.cpp
+-rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_key.cpp
+-rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.6/lib/dynareadout/src/python/pybind11_module.cpp
+-rw-rw-rw-   0        0        0     3348 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/sync.c
+-rw-rw-rw-   0        0        0     2158 2023-06-26 09:08:06.000000 dynareadout-23.6/lib/dynareadout/src/sync.h
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.646750 dynareadout-23.6/lib/pybind11/
+-rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.593890 dynareadout-23.6/lib/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.662709 dynareadout-23.6/lib/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.668291 dynareadout-23.6/lib/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.669291 dynareadout-23.6/lib/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.6/lib/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0      858 2023-06-26 09:13:20.000000 dynareadout-23.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:18:13.675493 dynareadout-23.6/setup.cfg
+-rw-rw-rw-   0        0        0     2776 2023-06-26 09:13:08.000000 dynareadout-23.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.594888 dynareadout-23.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.670288 dynareadout-23.6/src/dynareadout/
+-rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.6/src/dynareadout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:18:13.674495 dynareadout-23.6/src/dynareadout.egg-info/
+-rw-rw-rw-   0        0        0     5295 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3297 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.6/src/dynareadout.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 09:18:13.000000 dynareadout-23.6/src/dynareadout.egg-info/top_level.txt
```

### Comparing `dynareadout-23.5/LICENSE` & `dynareadout-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/PKG-INFO` & `dynareadout-23.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.5
+Version: 23.6
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-23.5/README.md` & `dynareadout-23.6/README.md`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binary_search.c` & `dynareadout-23.6/lib/dynareadout/src/binary_search.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binary_search.h` & `dynareadout-23.6/lib/dynareadout/src/binary_search.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout.c` & `dynareadout-23.6/lib/dynareadout/src/binout.c`

 * *Files 9% similar despite different names*

```diff
@@ -30,83 +30,93 @@
 #include "path.h"
 #include "profiling.h"
 #include <assert.h>
 #include <errno.h>
 #include <string.h>
 
 #define FILE_FAILED(message)                                                   \
-  fclose(file_handle);                                                         \
-  bin_file.file_handles[cur_file_index] = NULL;                                \
+  multi_file_close(file);                                                      \
   _binout_add_file_error(&bin_file, file_names[cur_file_index], message);      \
   cur_file_index++;                                                            \
   continue
 
 #define BIN_FILE_READ(dst, size, count, message)                               \
-  read_count = fread(&dst, size, count, file_handle);                          \
+  read_count = multi_file_read(file, &file_index, &dst, size, count);          \
   if (read_count != count) {                                                   \
     cur_file_failed = 1;                                                       \
     _binout_add_file_error(&bin_file, file_names[cur_file_index], message);    \
     break;                                                                     \
   }
 
 #define BIN_FILE_READ_FREE(dst, size, count, obj, message)                     \
-  read_count = fread(dst, size, count, file_handle);                           \
+  read_count = multi_file_read(file, &file_index, dst, size, count);           \
   if (read_count != count) {                                                   \
     free(obj);                                                                 \
     _binout_add_file_error(&bin_file, file_names[cur_file_index], message);    \
     cur_file_failed = 1;                                                       \
     break;                                                                     \
   }
 
 binout_file binout_open(const char *file_name) {
   BEGIN_PROFILE_FUNC();
 
   binout_file bin_file;
   bin_file.directory.children = NULL;
   bin_file.directory.num_children = 0;
-  bin_file.file_handles = NULL;
+  bin_file.files = NULL;
   bin_file.file_errors = NULL;
   bin_file.error_string = NULL;
-  bin_file.num_file_handles = 0;
+  bin_file.num_files = 0;
   bin_file.num_file_errors = 0;
 
-  char **file_names = binout_glob(file_name, &bin_file.num_file_handles);
-  if (bin_file.num_file_handles == 0) {
+  char **file_names = binout_glob(file_name, &bin_file.num_files);
+  if (bin_file.num_files == 0) {
     _binout_add_file_error(&bin_file, file_name, "No files have been found");
     END_PROFILE_FUNC();
     return bin_file;
   }
 
-  bin_file.file_handles = malloc(bin_file.num_file_handles * sizeof(FILE *));
+  bin_file.files = malloc(bin_file.num_files * sizeof(multi_file_t));
 
   size_t cur_file_index = 0;
-  while (cur_file_index < bin_file.num_file_handles) {
-    bin_file.file_handles[cur_file_index] =
-        fopen(file_names[cur_file_index], "rb");
-    if (!bin_file.file_handles[cur_file_index]) {
+  while (cur_file_index < bin_file.num_files) {
+    bin_file.files[cur_file_index] =
+        multi_file_open(file_names[cur_file_index]);
+#ifndef THREAD_SAFE
+    if (!bin_file.files[cur_file_index]) {
       _binout_add_file_error(&bin_file, file_names[cur_file_index],
                              strerror(errno));
     }
+#endif
 
     cur_file_index++;
   }
 
   cur_file_index = 0;
-  while (cur_file_index < bin_file.num_file_handles) {
-    FILE *file_handle = bin_file.file_handles[cur_file_index];
+  while (cur_file_index < bin_file.num_files) {
+    multi_file_t *file = &bin_file.files[cur_file_index];
+    multi_file_index_t file_index = multi_file_access(file);
+
     /* Just ignore the file if it failed to open*/
-    if (!file_handle) {
+#ifdef THREAD_SAFE
+    if (file_index.index == ULONG_MAX) {
+      FILE_FAILED(strerror(errno));
+    }
+#else
+    if (!(*file)) {
       cur_file_index++;
       continue;
     }
+#endif
 
     binout_header header;
 
     /* Read header */
-    size_t read_count = fread(&header, sizeof(binout_header), 1, file_handle);
+    size_t read_count =
+        multi_file_read(file, &file_index, &header, sizeof(binout_header), 1);
     if (read_count == 0) {
       FILE_FAILED("Failed to read header");
     }
 
     /* Check if the binout file is actually supported (Might also be an
      * indicator that the given file is not a binout) */
     if (header.endianess != BINOUT_HEADER_LITTLE_ENDIAN) {
@@ -122,23 +132,15 @@
       FILE_FAILED("The typeid field size is unsupported");
     }
     if (header.float_format != BINOUT_HEADER_FLOAT_IEEE) {
       FILE_FAILED("The float format is unsupported");
     }
 
     /* Get the file size*/
-    const long cur_pos = ftell(file_handle);
-    if (fseek(file_handle, 0, SEEK_END) != 0) {
-      FILE_FAILED("Failed to get the file size");
-    }
-
-    const long file_size = ftell(file_handle);
-    if (fseek(file_handle, cur_pos, SEEK_SET) != 0) {
-      FILE_FAILED("Failed to get the file size");
-    }
+    const long file_size = (long)path_get_file_size(file_names[cur_file_index]);
 
     /* Parse all records */
 
     /* Store the current path which is changed by the CD commands*/
     /* Store 1KB on the stack, this should totally suffice*/
     char current_path_string[1024];
     current_path_string[0] = PATH_SEP;
@@ -150,15 +152,15 @@
 
     /* A buffer for the path of the CD command*/
     char path_buffer[1024];
 
     /* We cannot use EOF, so we use this*/
     while (1) {
       /* Check if we are already at the end or if an error occurred in ftell*/
-      const long current_file_pos = ftell(file_handle);
+      const long current_file_pos = multi_file_tell(file, &file_index);
       if (current_file_pos == -1 || current_file_pos == file_size) {
         break;
       }
 
       uint64_t record_length = 0, record_command = 0;
 
       BIN_FILE_READ(record_length, header.record_length_field_size, 1,
@@ -178,16 +180,16 @@
         path_buffer[record_data_length] = '\0';
         BIN_FILE_READ(path_buffer, 1, record_data_length,
                       "Failed to read PATH of CD record");
 
         if (PATH_IS_ABS(path_buffer)) {
           memcpy(current_path_string, path_buffer, record_data_length + 1);
           current_path = path_view_new(current_path_string);
-          /* Only insert the current folder if the current path is not the root
-           * folder*/
+          /* Only insert the current folder if the current path is not the
+           * root folder*/
           if (path_view_advance(&current_path)) {
             current_folder = binout_directory_insert_folder(&bin_file.directory,
                                                             &current_path);
           }
         } else {
           path_view_t path = path_view_new(path_buffer);
 
@@ -245,61 +247,66 @@
         BIN_FILE_READ_FREE(variable_name, 1, variable_name_length,
                            variable_name, "Failed to read Name of DATA record");
 
         /* How large the data segment of the data record is*/
         const uint64_t data_length =
             record_data_length - header.record_typeid_field_size -
             BINOUT_DATA_NAME_LENGTH - variable_name_length;
-        const long file_pos = ftell(file_handle);
+        const long file_pos = multi_file_tell(file, &file_index);
         /* Skip the data since we will read it at a later point, if it is
          * requested by the programmer*/
-        if (fseek(file_handle, data_length, SEEK_CUR) != 0) {
+        if (multi_file_seek(file, &file_index, data_length, SEEK_CUR) != 0) {
           free(variable_name);
           cur_file_failed = 1;
           _binout_add_file_error(&bin_file, file_names[cur_file_index],
                                  "Failed to skip Data of DATA record");
           break;
         }
 
         binout_folder_insert_file(current_folder, variable_name,
                                   (uint8_t)type_id, data_length,
                                   (uint8_t)cur_file_index, file_pos);
       } else {
         /* Just skip the record and ignore its data*/
-        if (fseek(file_handle, record_data_length, SEEK_CUR) != 0) {
+        if (multi_file_seek(file, &file_index, record_data_length, SEEK_CUR) !=
+            0) {
           cur_file_failed = 1;
           _binout_add_file_error(&bin_file, file_names[cur_file_index],
                                  "Failed to skip data of a record");
           break;
         }
       }
     }
 
+    multi_file_return(file, &file_index);
+
     if (cur_file_failed) {
-      fclose(file_handle);
-      bin_file.file_handles[cur_file_index] = NULL;
+      multi_file_close(file);
     }
 
     cur_file_index++;
   }
 
-  binout_free_glob(file_names, bin_file.num_file_handles);
+  binout_free_glob(file_names, bin_file.num_files);
 
   /* Clean up failed files*/
   cur_file_index = 0;
-  while (cur_file_index < bin_file.num_file_handles) {
-    if (!bin_file.file_handles[cur_file_index]) {
+  while (cur_file_index < bin_file.num_files) {
+#ifdef THREAD_SAFE
+    if (bin_file.files[cur_file_index].file_handles == NULL) {
+#else
+    if (!bin_file.files[cur_file_index]) {
+#endif
       /* Swap with the last element*/
-      bin_file.file_handles[cur_file_index] =
-          bin_file.file_handles[bin_file.num_file_handles - 1];
+      bin_file.files[cur_file_index] = bin_file.files[bin_file.num_files - 1];
 
       /* Reallocate memory*/
-      bin_file.num_file_handles--;
-      bin_file.file_handles = realloc(
-          bin_file.file_handles, bin_file.num_file_handles * sizeof(FILE *));
+      bin_file.num_files--;
+      bin_file.files =
+          realloc(bin_file.files, bin_file.num_files * sizeof(multi_file_t));
 
       cur_file_index--;
     }
 
     cur_file_index++;
   }
 
@@ -309,17 +316,16 @@
 }
 
 void binout_close(binout_file *bin_file) {
   BEGIN_PROFILE_FUNC();
 
   /* Free all files*/
   size_t cur_file_index = 0;
-  while (cur_file_index < bin_file->num_file_handles) {
-    if (fclose(bin_file->file_handles[cur_file_index]) != 0) {
-    }
+  while (cur_file_index < bin_file->num_files) {
+    multi_file_close(&bin_file->files[cur_file_index]);
 
     cur_file_index++;
   }
 
   /* Free all file errors*/
   size_t i = 0;
   while (i < bin_file->num_file_errors) {
@@ -330,18 +336,18 @@
 
   binout_directory_free(&bin_file->directory);
 
   /* Set everything to 0 so that no error happens if function get called after
    * binout_close*/
   bin_file->directory.children = NULL;
   bin_file->directory.num_children = 0;
-  bin_file->file_handles = NULL;
+  bin_file->files = NULL;
   bin_file->file_errors = NULL;
   bin_file->error_string = NULL;
-  bin_file->num_file_handles = 0;
+  bin_file->num_files = 0;
   bin_file->num_file_errors = 0;
 
   END_PROFILE_FUNC();
 }
 
 uint8_t binout_get_type_id(binout_file *bin_file,
                            const char *path_to_variable) {
@@ -454,16 +460,16 @@
   if (num_children == (size_t)~0 || folder_or_file->type == BINOUT_FILE) {
     END_PROFILE_FUNC();
     return ~0;
   }
 
   const binout_folder_t *folders = (const binout_folder_t *)folder_or_file;
 
-  /* Loop until the first dxxxxxx string has been found. It's probably the first
-   * one.*/
+  /* Loop until the first dxxxxxx string has been found. It's probably the
+   * first one.*/
   size_t start_index = 0;
   while (start_index < num_children &&
          !_binout_is_d_string(folders[start_index].name)) {
     start_index++;
   }
 
   /* If no dxxxxxx folders are found*/
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout.h` & `dynareadout-23.6/lib/dynareadout/src/binout.h`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #ifndef BINOUT_H
 #define BINOUT_H
 #include "binout_directory.h"
+#include "multi_file.h"
 #include "path.h"
 #include <stdint.h>
 #include <stdio.h>
 
 /* The header of a binout file (The first 8 byte of a binout file)*/
 typedef struct {
   uint8_t header_size;
@@ -43,16 +44,16 @@
 } binout_header;
 
 /* A binout file used to read data from a binout file*/
 typedef struct {
   /* A data structure which holds the structure of the files*/
   binout_directory_t directory;
 
-  FILE **file_handles;
-  size_t num_file_handles;
+  multi_file_t *files;
+  size_t num_files;
 
   char **file_errors;
   size_t num_file_errors;
 
   /* Holds errors from read and other functions that are not open. If NULL no
    * error occurred*/
   char *error_string;
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_defines.h` & `dynareadout-23.6/lib/dynareadout/src/binout_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_directory.c` & `dynareadout-23.6/lib/dynareadout/src/binout_directory.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_directory.h` & `dynareadout-23.6/lib/dynareadout/src/binout_directory.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_glob.c` & `dynareadout-23.6/lib/dynareadout/src/binout_glob.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_glob.h` & `dynareadout-23.6/lib/dynareadout/src/binout_glob.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_read.c` & `dynareadout-23.6/lib/dynareadout/src/binout_read.c`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #include "binary_search.h"
 #include "binout.h"
 #include "binout_defines.h"
 #include "profiling.h"
+#include <errno.h>
 #include <stdlib.h>
 #include <string.h>
 
 void *_binout_read(binout_file *bin_file, const char *path_to_variable,
                    size_t *data_size, const uint8_t binout_type) {
   CLEAR_ERROR_STRING();
 
@@ -46,28 +47,42 @@
     NEW_ERROR_STRING_F("\"%s\" is of type %s instead of %s", path_to_variable,
                        _binout_get_type_name(file->var_type),
                        _binout_get_type_name((uint64_t)binout_type));
     return NULL;
   }
 
   const size_t type_size = (size_t)_binout_get_type_size((uint64_t)binout_type);
-  FILE *file_handle = bin_file->file_handles[file->file_index];
+  multi_file_t *multi_file = &bin_file->files[file->file_index];
 
-  if (fseek(file_handle, file->file_pos, SEEK_SET) != 0) {
+  multi_file_index_t multi_file_index = multi_file_access(multi_file);
+#ifdef THREAD_SAFE
+  if (multi_file_index.index == ULONG_MAX) {
+    NEW_ERROR_STRING_F("Failed to access file of \"%s\": %s", path_to_variable,
+                       strerror(errno));
+    return NULL;
+  }
+#endif
+
+  if (multi_file_seek(multi_file, &multi_file_index, file->file_pos,
+                      SEEK_SET) != 0) {
+    multi_file_return(multi_file, &multi_file_index);
     NEW_ERROR_STRING_F("Failed to seek to the position of \"%s\"",
                        path_to_variable);
     return NULL;
   }
 
   void *data = malloc(file->size);
-  if (fread(data, file->size, 1, file_handle) != 1) {
+  if (multi_file_read(multi_file, &multi_file_index, data, file->size, 1) !=
+      1) {
     free(data);
+    multi_file_return(multi_file, &multi_file_index);
     NEW_ERROR_STRING_F("Failed to read \"%s\"", path_to_variable);
     return NULL;
   }
+  multi_file_return(multi_file, &multi_file_index);
 
   *data_size = file->size / type_size;
   return data;
 }
 
 void *_binout_read_timed(binout_file *bin_file, const char *variable,
                          size_t *num_values, size_t *num_timesteps,
@@ -203,28 +218,44 @@
         NEW_ERROR_STRING_F("\"%s\" has not been found", variable);
         return NULL;
       }
 
       file = &((const binout_file_t *)current_d_folder->children)[file_index];
     }
 
-    FILE *file_handle = bin_file->file_handles[file->file_index];
-    if (fseek(file_handle, file->file_pos, SEEK_SET) != 0) {
+    multi_file_t *multi_file = &bin_file->files[file->file_index];
+    multi_file_index_t multi_file_index = multi_file_access(multi_file);
+#ifdef THREAD_SAFE
+    if (multi_file_index.index == ULONG_MAX) {
+      free(data);
+      NEW_ERROR_STRING_F("Failed to access the file of \"%s\": %s", variable,
+                         strerror(errno));
+      return NULL;
+    }
+#endif
+
+    if (multi_file_seek(multi_file, &multi_file_index, file->file_pos,
+                        SEEK_SET) != 0) {
       free(data);
+      multi_file_return(multi_file, &multi_file_index);
       NEW_ERROR_STRING_F("Failed to seek to the data of \"%s\"", variable);
       return NULL;
     }
 
-    if (fread(&((uint8_t *)data)[(i - start_index) * file->size], file->size, 1,
-              file_handle) != 1) {
+    if (multi_file_read(multi_file, &multi_file_index,
+                        &((uint8_t *)data)[(i - start_index) * file->size],
+                        file->size, 1) != 1) {
       free(data);
+      multi_file_return(multi_file, &multi_file_index);
       NEW_ERROR_STRING_F("Failed to read the data of \"%s\"", variable);
       return NULL;
     }
 
+    multi_file_return(multi_file, &multi_file_index);
+
     i++;
   }
 
   return data;
 }
 
 int8_t *binout_read_i8(binout_file *bin_file, const char *path_to_variable,
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/binout_read.h` & `dynareadout-23.6/lib/dynareadout/src/binout_read.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/array.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/array.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -67,35 +67,59 @@
     }
     bool operator!=(const ConstIterator &rhs) const noexcept {
       return m_index != rhs.m_index;
     }
     difference_type operator-(const ConstIterator &rhs) const {
       return m_index - rhs.m_index;
     }
-    const reference operator*() { return m_data[m_index]; }
+    const reference operator*() const { return m_data[m_index]; }
     const pointer operator->() const { return &m_data[m_index]; }
 
   public:
     pointer m_data;
     difference_type m_index;
   };
 
   // An Iterator which can write the array
-  class Iterator : public ConstIterator {
+  class Iterator {
   public:
-    Iterator(typename ConstIterator::pointer data,
-             typename ConstIterator::difference_type index) noexcept
-        : ConstIterator(data, index) {}
+    using iterator_category = std::input_iterator_tag;
+    using difference_type = std::ptrdiff_t;
+    using value_type = T;
+    using pointer = T *;   // or also value_type*
+    using reference = T &; // or also value_type&
 
-    typename ConstIterator::reference operator*() {
-      return ConstIterator::m_data[ConstIterator::m_index];
+    explicit Iterator(pointer data, difference_type index) noexcept
+        : m_data(data), m_index(index) {}
+    Iterator operator++() noexcept {
+      m_index++;
+      return *this;
     }
-    typename ConstIterator::pointer operator->() {
-      return &ConstIterator::m_data[ConstIterator::m_index];
+    Iterator operator++(int) noexcept {
+      auto rv = *this;
+      ++(*this);
+      return rv;
     }
+    bool operator==(const Iterator &rhs) const noexcept {
+      return m_index == rhs.m_index;
+    }
+    bool operator!=(const Iterator &rhs) const noexcept {
+      return m_index != rhs.m_index;
+    }
+    difference_type operator-(const Iterator &rhs) const {
+      return m_index - rhs.m_index;
+    }
+    const reference operator*() const { return m_data[m_index]; }
+    const pointer operator->() const { return &m_data[m_index]; }
+    reference operator*() { return m_data[m_index]; }
+    pointer operator->() { return &m_data[m_index]; }
+
+  public:
+    pointer m_data;
+    difference_type m_index;
   };
 
   // Allocates memory and creates a new array with it
   // size ........... Number of elements of the new array
   static Array<T> New(size_t size);
 
   // data ........... An C array allocated by malloc
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/binout.cpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/binout.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/binout.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.cpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.cpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_part.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_part.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.cpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/d3plot_state.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/d3plot_state.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 public:
   D3plotShellsState(d3plot_shell *data, size_t size,
                     size_t num_history_variables,
                     bool delete_data = true) noexcept;
   D3plotShellsState(D3plotShellsState &&rhs) noexcept;
   ~D3plotShellsState() noexcept override;
 
+  inline size_t get_num_history_variables() const noexcept {
+    return m_num_history_variables;
+  }
+
   const Array<double> get_mid_history_variables(size_t index) const;
   const Array<double> get_inner_history_variables(size_t index) const;
   const Array<double> get_outer_history_variables(size_t index) const;
 
 private:
   size_t m_num_history_variables;
 };
@@ -50,14 +54,18 @@
 public:
   D3plotThickShellsState(d3plot_thick_shell *data, size_t size,
                          size_t num_history_variables,
                          bool delete_data = true) noexcept;
   D3plotThickShellsState(D3plotThickShellsState &&rhs) noexcept;
   ~D3plotThickShellsState() noexcept override;
 
+  inline size_t get_num_history_variables() const noexcept {
+    return m_num_history_variables;
+  }
+
   const Array<double> get_mid_history_variables(size_t index) const;
   const Array<double> get_inner_history_variables(size_t index) const;
   const Array<double> get_outer_history_variables(size_t index) const;
 
 private:
   size_t m_num_history_variables;
 };
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/key.cpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/key.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -191,21 +191,24 @@
 void KeyFile::parse_with_callback(const std::filesystem::path &file_name,
                                   KeyFile::Callback callback,
                                   bool parse_includes) {
   char *error_string;
 
   key_file_parse_with_callback(
       file_name.string().c_str(),
-      [](const char *keyword_name, const card_t *card, size_t card_index,
-         void *user_data) {
+      [](const char *file_name, size_t line_number, const char *keyword_name,
+         card_t *card, size_t card_index, void *user_data) {
         KeyFile::Callback *callback =
             reinterpret_cast<KeyFile::Callback *>(user_data);
 
-        (*callback)(String(const_cast<char *>(keyword_name), false),
-                    Card(const_cast<card_t *>(card)), card_index);
+        auto card_opt = card ? std::make_optional<Card>(card) : std::nullopt;
+
+        (*callback)(String(const_cast<char *>(file_name), false), line_number,
+                    String(const_cast<char *>(keyword_name), false),
+                    std::move(card_opt), card_index);
       },
       static_cast<int>(parse_includes), &error_string, &callback, NULL, NULL,
       NULL);
 
   if (error_string) {
     throw Exception(String(error_string));
   }
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/key.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/key.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #include <cstdio>
 #include <cstdlib>
 #include <exception>
 #include <filesystem>
 #include <functional>
 #include <key.h>
 #include <limits>
+#include <optional>
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <typeinfo>
 
 #define THROW_KEY_FILE_EXCEPTION(msg, ...)                                     \
   const int error_buffer_size = snprintf(NULL, 0, msg, __VA_ARGS__);           \
@@ -116,17 +117,14 @@
   // Uses the values of the value_widths array as the value width for every
   // value. Example NODE: auto [nid, x, y, z, tc, rc] =
   // card.parse_whole<int, float, float, float, int, int>({8, 16, 16, 16, 8,
   // 8});
   template <typename... T>
   std::tuple<T...> parse_whole(std::array<uint8_t, sizeof...(T)> value_widths);
 
-  // Returns wether the card can be parsed
-  inline bool is_valid() const noexcept { return m_handle != nullptr; }
-
 private:
   card_t *m_handle;
 };
 
 // A Keyword of a LS Dyna key file (input deck) with all its cards
 class Keyword {
 public:
@@ -260,17 +258,17 @@
 
     const char *what() const noexcept override;
 
   private:
     const String m_error_str;
   };
 
-  // TODO: Card is sometimes NULL
-  using Callback =
-      std::function<void(String keyword_name, Card card, size_t card_index)>;
+  using Callback = std::function<void(
+      String file_name, size_t line_number, String keyword_name,
+      std::optional<Card> card, size_t card_index)>;
 
   // Parses a LS Dyna key file for keywords and their respective cards. Returns
   // an array keywords
   // parse_includes: tells the function wether to parse include files via the
   // *INCLUDE and similar keywords or if they should be added as regular
   // keywords to the array.
   // Throws a dro::KeyFile::Exception if an error occurs.
@@ -294,22 +292,34 @@
 template <> constexpr bool is_string_v<std::string> = true;
 
 template <typename T> T Card::parse() const {
   return parse<T>(m_handle->value_width);
 }
 
 template <typename T> T Card::parse(uint8_t value_width) const {
-  /* TODO: Bounds check*/
   if constexpr (std::is_integral_v<T>) {
     const auto value = card_parse_int_width(m_handle, value_width);
     if (value < 0 && std::is_unsigned_v<T>) {
-      THROW_KEY_FILE_EXCEPTION("Can not convert %ld into %s because of sign",
+      THROW_KEY_FILE_EXCEPTION("Can not convert %lld into %s because of sign",
                                value, typeid(T).name());
     }
-    return value;
+
+    if (value < 0 && value < std::numeric_limits<T>::min()) {
+      THROW_KEY_FILE_EXCEPTION(
+          "Can not convert %lld into %s because it is too small", value,
+          typeid(T).name());
+    }
+
+    if (value > 0 && value > std::numeric_limits<T>::max()) {
+      THROW_KEY_FILE_EXCEPTION(
+          "Can not convert %lld into %s because it is too large", value,
+          typeid(T).name());
+    }
+
+    return static_cast<T>(value);
   } else if constexpr (std::is_floating_point_v<T>) {
     if constexpr (sizeof(T) == sizeof(float)) {
       const auto value = card_parse_float32_width(m_handle, value_width);
       if (value < 0.0f && std::is_unsigned_v<T>) {
         THROW_KEY_FILE_EXCEPTION("Can not convert %f into %s because of sign",
                                  value, typeid(T).name());
       }
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/cpp/vec.hpp` & `dynareadout-23.6/lib/dynareadout/src/cpp/vec.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3_buffer.h` & `dynareadout-23.6/lib/dynareadout/src/d3_buffer.h`

 * *Files 13% similar despite different names*

```diff
@@ -21,31 +21,36 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #ifndef D3_BUFFER_H
 #define D3_BUFFER_H
+#include "multi_file.h"
 #include <stdint.h>
 #include <stdio.h>
 
 typedef struct {
+  multi_file_index_t multi_file_index;
+  size_t cur_file;
+  size_t cur_word;
+} d3_pointer;
+
+typedef struct {
   char index_string[4];
   uint64_t file_size;
-  FILE *file_handle;
+  multi_file_t file;
 } d3_file;
 
 /* Represents a whole family of d3 files*/
 typedef struct {
   char *root_file_name;
   size_t root_file_name_length;
   d3_file *files;
   size_t num_files;
-  size_t cur_file;
-  size_t cur_word;
   size_t first_open_file;
   size_t last_open_file;
 
   uint8_t word_size; /* 4 byte for single precision and 8 byte for double
                         precision*/
   char *error_string;
 } d3_buffer;
@@ -58,35 +63,45 @@
  * the word_size. Sets error_string on error*/
 d3_buffer d3_buffer_open(const char *root_file_name);
 /* Cleans everything up. Should be called sometime after d3_buffer_open*/
 void d3_buffer_close(d3_buffer *buffer);
 /* Read a given number of words from the current position. words already needs
  * to be allocated with at least num_words*word_size bytes. Sets error_string on
  * error*/
-void d3_buffer_read_words(d3_buffer *buffer, void *words, size_t num_words);
+void d3_buffer_read_words(d3_buffer *buffer, d3_pointer *ptr, void *words,
+                          size_t num_words);
 /* Read a given number of words from the given position. words already needs
  * to be allocated with at least num_words*word_size bytes. Sets error_string on
  * error*/
-void d3_buffer_read_words_at(d3_buffer *buffer, void *words, size_t num_words,
-                             size_t word_pos);
+d3_pointer d3_buffer_read_words_at(d3_buffer *buffer, void *words,
+                                   size_t num_words, size_t word_pos);
 /* Sets error_string on error*/
-void d3_buffer_read_double_word(d3_buffer *buffer, double *word);
+void d3_buffer_read_double_word(d3_buffer *buffer, d3_pointer *ptr,
+                                double *word);
 /* Sets error_string on error*/
-void d3_buffer_read_vec3(d3_buffer *buffer, double *words);
+void d3_buffer_read_vec3(d3_buffer *buffer, d3_pointer *ptr, double *words);
 /* Skip an arbitrary amount of words. Also handles skips across multiple files.
  * Sets error_string on error*/
-void d3_buffer_skip_words(d3_buffer *buffer, size_t num_words);
+void d3_buffer_skip_words(d3_buffer *buffer, d3_pointer *ptr, size_t num_words);
 /* Similar to d3_buffer_skip_words, but it skips bytes instead of words. Try to
  * use the words one. This function ist just for some cases where the number of
  * bytes is always the same no matter what the words size is*/
-void d3_buffer_skip_bytes(d3_buffer *buffer, size_t num_bytes);
+void d3_buffer_skip_bytes(d3_buffer *buffer, d3_pointer *ptr, size_t num_bytes);
 /* Skip to the next file. Especially needed a the end of the first file when
  * done with all the headers. Sets error_string on error*/
-int d3_buffer_next_file(d3_buffer *buffer);
+int d3_buffer_next_file(d3_buffer *buffer, d3_pointer *ptr);
 /* Jumps to the word position indicated by word pos*/
-void d3_buffer_seek(d3_buffer *buffer, size_t word_pos);
+d3_pointer d3_buffer_seek(d3_buffer *buffer, size_t word_pos);
+
+void d3_pointer_close(d3_buffer *buffer, d3_pointer *ptr);
+
+#ifdef THREAD_SAFE
+/* Panic and close all open file handles of all multi files that are currently
+ * unused*/
+void _d3_buffer_kill_idle_files(d3_buffer *buffer);
+#endif
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3_defines.h` & `dynareadout-23.6/lib/dynareadout/src/d3_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot.c` & `dynareadout-23.6/lib/dynareadout/src/d3plot.c`

 * *Files 12% similar despite different names*

```diff
@@ -31,26 +31,27 @@
 #ifndef inline
 #define inline
 #endif
 #include <time.h>
 
 #define READ_CONTROL_DATA_PLOT_FILE_WORD(value)                                \
   plot_file.control_data.value = 0;                                            \
-  d3_buffer_read_words(&plot_file.buffer, &plot_file.control_data.value, 1)
+  d3_buffer_read_words(&plot_file.buffer, &d3_ptr,                             \
+                       &plot_file.control_data.value, 1)
 #define READ_CONTROL_DATA_PLOT_FILE_SIGNED_WORD(value)                         \
   if (plot_file.buffer.word_size == 4) {                                       \
     int32_t value32;                                                           \
-    d3_buffer_read_words(&plot_file.buffer, &value32, 1);                      \
+    d3_buffer_read_words(&plot_file.buffer, &d3_ptr, &value32, 1);             \
     CDA.value = value32;                                                       \
   } else {                                                                     \
-    d3_buffer_read_words(&plot_file.buffer, &CDA.value, 1);                    \
+    d3_buffer_read_words(&plot_file.buffer, &d3_ptr, &CDA.value, 1);           \
   }
 #define READ_CONTROL_DATA_WORD(value)                                          \
   d3_word value = 0;                                                           \
-  d3_buffer_read_words(&plot_file.buffer, &value, 1)
+  d3_buffer_read_words(&plot_file.buffer, &d3_ptr, &value, 1)
 #define CDA plot_file.control_data
 
 #include "d3plot_error_macros.h"
 
 d3plot_file d3plot_open(const char *root_file_name) {
   BEGIN_PROFILE_FUNC();
 
@@ -74,82 +75,86 @@
   size_t i = 0;
   while (i < D3PLT_PTR_COUNT) {
     plot_file.data_pointers[i] = 0;
 
     i++;
   }
 
-  d3_buffer_skip_words(&plot_file.buffer, 10); /* Title*/
-  plot_file.data_pointers[D3PLT_PTR_RUN_TIME] = plot_file.buffer.cur_word;
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* Run time*/
+  d3_pointer d3_ptr = d3_buffer_seek(&plot_file.buffer, 0);
+
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 10); /* Title*/
+  plot_file.data_pointers[D3PLT_PTR_RUN_TIME] = d3_ptr.cur_word;
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* Run time*/
 
   READ_CONTROL_DATA_WORD(file_type);
   if (file_type > 1000) {
     file_type -= 1000;
     /* TODO: all external(users) numbers (Node, Element, Material and Rigid
   Surface Nodes) will be written in I8 format.*/
   }
   /* Quit immediately if this is not a d3plot file*/
   if (file_type != D3_FILE_TYPE_D3PLOT) {
+    d3_pointer_close(&plot_file.buffer, &d3_ptr);
     plot_file.error_string = malloc(50);
     sprintf(plot_file.error_string, "Wrong file type: %s",
             _d3plot_get_file_type_name(file_type));
 
     END_PROFILE_FUNC();
     return plot_file;
   }
 
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: Source version*/
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: Release version*/
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: Version*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: Source version*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr,
+                       1); /* TODO: Release version*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: Version*/
   READ_CONTROL_DATA_PLOT_FILE_WORD(ndim);
   READ_CONTROL_DATA_PLOT_FILE_WORD(numnp);
   READ_CONTROL_DATA_WORD(icode);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nglbv);
   READ_CONTROL_DATA_PLOT_FILE_WORD(it);
   READ_CONTROL_DATA_PLOT_FILE_WORD(iu);
   READ_CONTROL_DATA_PLOT_FILE_WORD(iv);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ia);
   READ_CONTROL_DATA_PLOT_FILE_SIGNED_WORD(nel8);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nummat8);
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: NUMDS*/
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: NUMST*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: NUMDS*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: NUMST*/
   READ_CONTROL_DATA_PLOT_FILE_WORD(nv3d);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nel2);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nummat2);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nv1d);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nel4);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nummat4);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nv2d);
   READ_CONTROL_DATA_PLOT_FILE_WORD(neiph);
   READ_CONTROL_DATA_PLOT_FILE_WORD(neips);
   READ_CONTROL_DATA_PLOT_FILE_SIGNED_WORD(maxint);
   /*READ_CONTROL_DATA_PLOT_FILE_WORD(edlopt); Not used in LS-Dyna?*/
   READ_CONTROL_DATA_PLOT_FILE_WORD(nmsph);
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: NGPSPH*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: NGPSPH*/
   READ_CONTROL_DATA_PLOT_FILE_WORD(narbs);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nelt);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nummatt);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nv3dt);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ioshl[0]);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ioshl[1]);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ioshl[2]);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ioshl[3]);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ialemat);
   READ_CONTROL_DATA_PLOT_FILE_WORD(ncfdv1);
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: NCFDV2*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: NCFDV2*/
   READ_CONTROL_DATA_PLOT_FILE_WORD(nadapt);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nmmat);
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: NUMFLUID*/
-  d3_buffer_skip_words(&plot_file.buffer, 1); /* TODO: INN*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: NUMFLUID*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 1); /* TODO: INN*/
   READ_CONTROL_DATA_WORD(npefg);
   READ_CONTROL_DATA_PLOT_FILE_WORD(nel48);
   READ_CONTROL_DATA_WORD(idtdt);
   READ_CONTROL_DATA_WORD(extra);
-  d3_buffer_skip_words(&plot_file.buffer, 6); /* TODO: WORDS*/
+  d3_buffer_skip_words(&plot_file.buffer, &d3_ptr, 6); /* TODO: WORDS*/
 
   uint8_t mattyp;
 
   if (extra > 0) {
     READ_CONTROL_DATA_PLOT_FILE_WORD(nel20);
     READ_CONTROL_DATA_PLOT_FILE_WORD(nt3d);
   } else {
@@ -296,30 +301,30 @@
     ERROR_AND_RETURN(
         "SMOOTH PARTICLE HYDRODYNAMICS ELEMENT DATA FLAGS is not implemented");
   }
   if (npefg) {
     ERROR_AND_RETURN("PARTICLE DATA is not implemented");
   }
 
-  if (!_d3plot_read_geometry_data(&plot_file)) {
+  if (!_d3plot_read_geometry_data(&plot_file, &d3_ptr)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
 
-  if (!_d3plot_read_user_identification_numbers(&plot_file)) {
+  if (!_d3plot_read_user_identification_numbers(&plot_file, &d3_ptr)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
 
-  if (!_d3plot_read_extra_node_connectivity(&plot_file)) {
+  if (!_d3plot_read_extra_node_connectivity(&plot_file, &d3_ptr)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
 
-  if (!_d3plot_read_adapted_element_parent_list(&plot_file)) {
+  if (!_d3plot_read_adapted_element_parent_list(&plot_file, &d3_ptr)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
 
   if (CDA.nmsph > 0) {
     ERROR_AND_RETURN("SMOOTH PARTICLE HYDRODYNAMICS NODE AND "
                      "MATERIAL LIST is not implemented");
@@ -331,46 +336,46 @@
 
   if (CDA.ndim > 5) {
     ERROR_AND_RETURN("RIGID ROAD SURFACE DATA is not implemented");
   }
 
   /* Read EOF marker*/
   double eof_marker;
-  d3_buffer_read_double_word(&plot_file.buffer, &eof_marker);
+  d3_buffer_read_double_word(&plot_file.buffer, &d3_ptr, &eof_marker);
 
   if (eof_marker != D3_EOF) {
     ERROR_AND_RETURN_F(
         "Here (before header) 'd3plot':(%zu) should be the EOF marker",
-        plot_file.buffer.cur_word - 1);
+        d3_ptr.cur_word - 1);
   }
 
-  if (!_d3plot_read_header(&plot_file)) {
+  if (!_d3plot_read_header(&plot_file, &d3_ptr)) {
     END_PROFILE_FUNC();
     return plot_file;
   }
 
   if (CDA.ncfdv1 == 67108864) {
     ERROR_AND_RETURN("EXTRA DATA TYPES is not implemented");
   }
 
-  if (!d3_buffer_next_file(&plot_file.buffer)) {
+  if (!d3_buffer_next_file(&plot_file.buffer, &d3_ptr)) {
     ERROR_AND_RETURN("Too few files");
   }
   if (plot_file.buffer.error_string) {
     ERROR_AND_RETURN_F("Failed to switch to the next file: %s",
                        plot_file.buffer.error_string);
   }
 
   /* Here comes the STATE DATA*/
 
   int result = 1;
   while (result) {
-    result = _d3plot_read_state_data(&plot_file);
+    result = _d3plot_read_state_data(&plot_file, &d3_ptr);
     if (result == 2) {
-      if (!d3_buffer_next_file(&plot_file.buffer)) {
+      if (!d3_buffer_next_file(&plot_file.buffer, &d3_ptr)) {
         break;
       }
       if (plot_file.buffer.error_string) {
         ERROR_AND_RETURN_F("Failed to switch to the next file: %s",
                            plot_file.buffer.error_string);
       }
     }
@@ -502,30 +507,33 @@
       return NULL;
     }
 
     /* Read the part ids from the header if NSORT >= 0*/
     *num_parts = plot_file->control_data.nmmat;
     d3_word *part_ids = malloc(*num_parts * sizeof(d3_word));
 
+    d3_pointer d3_ptr;
+
     size_t i = 0;
     while (i < *num_parts) {
       part_ids[i] = 0;
 
       if (i == 0) {
-        d3_buffer_read_words_at(
+        d3_ptr = d3_buffer_read_words_at(
             &plot_file->buffer, &part_ids[i], 1,
             plot_file->data_pointers[D3PLT_PTR_PART_TITLES]);
       } else {
-        d3_buffer_read_words(&plot_file->buffer, &part_ids[i], 1);
+        d3_buffer_read_words(&plot_file->buffer, &d3_ptr, &part_ids[i], 1);
       }
-      d3_buffer_skip_bytes(&plot_file->buffer, 72);
+      d3_buffer_skip_bytes(&plot_file->buffer, &d3_ptr, 72);
 
       i++;
     }
 
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     END_PROFILE_FUNC();
     return part_ids;
   }
 
   d3_word *ids = _d3plot_read_ids(plot_file, num_parts, D3PLT_PTR_PART_IDS,
                                   plot_file->control_data.nmmat);
 
@@ -536,31 +544,34 @@
 char **d3plot_read_part_titles(d3plot_file *plot_file, size_t *num_parts) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   *num_parts = plot_file->control_data.nmmat;
   char **part_titles = malloc(*num_parts * sizeof(char *));
 
+  d3_pointer d3_ptr;
+
   size_t i = 0;
   while (i < *num_parts) {
     part_titles[i] = malloc(72 + 1);
     if (i == 0)
       /* PTITLE is always 72 bytes. So we need to divide by to get the correct
        * number of words*/
-      d3_buffer_read_words_at(&plot_file->buffer, part_titles[i],
-                              18 / (plot_file->buffer.word_size == 8 ? 2 : 1),
-                              plot_file->data_pointers[D3PLT_PTR_PART_TITLES] +
-                                  1);
+      d3_ptr = d3_buffer_read_words_at(
+          &plot_file->buffer, part_titles[i],
+          18 / (plot_file->buffer.word_size == 8 ? 2 : 1),
+          plot_file->data_pointers[D3PLT_PTR_PART_TITLES] + 1);
     else {
-      d3_buffer_skip_words(&plot_file->buffer, 1);
-      d3_buffer_read_words(&plot_file->buffer, part_titles[i],
+      d3_buffer_skip_words(&plot_file->buffer, &d3_ptr, 1);
+      d3_buffer_read_words(&plot_file->buffer, &d3_ptr, part_titles[i],
                            18 / (plot_file->buffer.word_size == 8 ? 2 : 1));
     }
 
     if (plot_file->buffer.error_string) {
+      d3_pointer_close(&plot_file->buffer, &d3_ptr);
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       size_t j = 0;
       while (j <= i) {
         free(part_titles[j]);
         j++;
       }
@@ -572,14 +583,15 @@
     }
 
     part_titles[i][72] = '\0';
 
     i++;
   }
 
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   END_PROFILE_FUNC();
   return part_titles;
 }
 
 double *d3plot_read_node_coordinates(d3plot_file *plot_file, size_t state,
                                      size_t *num_nodes) {
   BEGIN_PROFILE_FUNC();
@@ -628,18 +640,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   double *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(double));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_COORDS]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -701,18 +714,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   double *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(double));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_VEL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -775,18 +789,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   double *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(double));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_ACC]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -849,18 +864,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   float *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(float));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_COORDS]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -923,18 +939,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   float *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(float));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_VEL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -997,18 +1014,19 @@
   *num_nodes = (size_t)plot_file->control_data.numnp;
 
   float *big_data = malloc(*num_nodes * *num_time_steps * 3 * sizeof(float));
 
   size_t current_pointer = 0;
   size_t t = 0;
   while (t < *num_time_steps) {
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, &big_data[current_pointer], *num_nodes * 3,
         plot_file->data_pointers[D3PLT_PTR_STATES + t] +
             plot_file->data_pointers[D3PLT_PTR_STATE_NODE_ACC]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_nodes = 0;
       *num_time_steps = 0;
       free(big_data);
       END_PROFILE_FUNC();
@@ -1033,22 +1051,26 @@
     END_PROFILE_FUNC();
     return -1.0;
   }
 
   double time;
   if (plot_file->buffer.word_size == 4) {
     float time32;
-    d3_buffer_read_words_at(&plot_file->buffer, &time32, 1,
-                            plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                                plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, &time32, 1,
+        plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+            plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     time = (double)time32;
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, &time, 1,
-                            plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                                plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, &time, 1,
+        plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+            plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
   }
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
@@ -1067,18 +1089,19 @@
   double *times = malloc(plot_file->num_states * sizeof(double));
 
   if (plot_file->buffer.word_size == 4) {
     float time32;
 
     size_t i = 0;
     while (i < plot_file->num_states) {
-      d3_buffer_read_words_at(
+      d3_pointer d3_ptr = d3_buffer_read_words_at(
           &plot_file->buffer, &time32, 1,
           plot_file->data_pointers[D3PLT_PTR_STATES + i] +
               plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+      d3_pointer_close(&plot_file->buffer, &d3_ptr);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                   plot_file->buffer.error_string);
         *num_states = 0;
         free(times);
         times = NULL;
         break;
@@ -1087,18 +1110,19 @@
       times[i] = (double)time32;
 
       i++;
     }
   } else {
     size_t i = 0;
     while (i < plot_file->num_states) {
-      d3_buffer_read_words_at(
+      d3_pointer d3_ptr = d3_buffer_read_words_at(
           &plot_file->buffer, &times[i], 1,
           plot_file->data_pointers[D3PLT_PTR_STATES + i] +
               plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+      d3_pointer_close(&plot_file->buffer, &d3_ptr);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                   plot_file->buffer.error_string);
         *num_states = 0;
         free(times);
         times = NULL;
         break;
@@ -1122,22 +1146,26 @@
     END_PROFILE_FUNC();
     return -1.0f;
   }
 
   float time;
   if (plot_file->buffer.word_size == 8) {
     double time64;
-    d3_buffer_read_words_at(&plot_file->buffer, &time64, 1,
-                            plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                                plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, &time64, 1,
+        plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+            plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     time = (float)time64;
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, &time, 1,
-                            plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                                plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, &time, 1,
+        plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+            plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
   }
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
@@ -1156,18 +1184,19 @@
   float *times = malloc(plot_file->num_states * sizeof(float));
 
   if (plot_file->buffer.word_size == 8) {
     double time64;
 
     size_t i = 0;
     while (i < plot_file->num_states) {
-      d3_buffer_read_words_at(
+      d3_pointer d3_ptr = d3_buffer_read_words_at(
           &plot_file->buffer, &time64, 1,
           plot_file->data_pointers[D3PLT_PTR_STATES + i] +
               plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+      d3_pointer_close(&plot_file->buffer, &d3_ptr);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                   plot_file->buffer.error_string);
         *num_states = 0;
         free(times);
         times = NULL;
         break;
@@ -1176,18 +1205,19 @@
       times[i] = (float)time64;
 
       i++;
     }
   } else {
     size_t i = 0;
     while (i < plot_file->num_states) {
-      d3_buffer_read_words_at(
+      d3_pointer d3_ptr = d3_buffer_read_words_at(
           &plot_file->buffer, &times[i], 1,
           plot_file->data_pointers[D3PLT_PTR_STATES + i] +
               plot_file->data_pointers[D3PLT_PTR_STATE_TIME]);
+      d3_pointer_close(&plot_file->buffer, &d3_ptr);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                   plot_file->buffer.error_string);
         *num_states = 0;
         free(times);
         times = NULL;
         break;
@@ -1222,19 +1252,20 @@
 
   d3plot_solid *solids = malloc(*num_solids * sizeof(d3plot_solid));
   if (plot_file->buffer.word_size == 4) {
     float *data =
         malloc((plot_file->control_data.nel8 * plot_file->control_data.nv3d) *
                sizeof(float));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel8 * plot_file->control_data.nv3d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_SOLID]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_solids = 0;
       free(data);
       free(solids);
 
@@ -1289,19 +1320,20 @@
 
     free(data);
   } else {
     double *data =
         malloc((plot_file->control_data.nel8 * plot_file->control_data.nv3d) *
                sizeof(double));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel8 * plot_file->control_data.nv3d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_SOLID]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_solids = 0;
       free(data);
       free(solids);
 
@@ -1377,19 +1409,20 @@
 
   d3plot_thick_shell *thick_shells =
       malloc(*num_thick_shells * sizeof(d3plot_thick_shell));
   if (plot_file->buffer.word_size == 4) {
     float *data = malloc(plot_file->control_data.nelt *
                          plot_file->control_data.nv3dt * sizeof(float));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nelt * plot_file->control_data.nv3dt,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_THICK_SHELL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_thick_shells = 0;
       free(data);
       free(thick_shells);
 
@@ -1494,19 +1527,20 @@
     }
 
     free(data);
   } else {
     double *data = malloc(plot_file->control_data.nelt *
                           plot_file->control_data.nv3dt * sizeof(double));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nelt * plot_file->control_data.nv3dt,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_THICK_SHELL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_thick_shells = 0;
       free(data);
       free(thick_shells);
 
@@ -1613,19 +1647,20 @@
   }
 
   d3plot_beam *beams = malloc(*num_beams * sizeof(d3plot_beam));
   if (plot_file->buffer.word_size == 4) {
     float *data = malloc(plot_file->control_data.nel2 *
                          plot_file->control_data.nv1d * sizeof(float));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel2 * plot_file->control_data.nv1d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_BEAM]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_beams = 0;
       free(data);
       free(beams);
 
@@ -1652,19 +1687,20 @@
     }
 
     free(data);
   } else {
     double *data = malloc(plot_file->control_data.nel2 *
                           plot_file->control_data.nv1d * sizeof(double));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel2 * plot_file->control_data.nv1d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_BEAM]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_beams = 0;
       free(data);
       free(beams);
 
@@ -1720,19 +1756,20 @@
       malloc(*num_history_variables * *num_shells * sizeof(double));
 
   d3plot_shell *shells = malloc(*num_shells * sizeof(d3plot_shell));
   if (plot_file->buffer.word_size == 4) {
     float *data = malloc(plot_file->control_data.nel4 *
                          plot_file->control_data.nv2d * sizeof(float));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel4 * plot_file->control_data.nv2d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_SHELL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_shells = 0;
       free(data);
       free(shells);
 
@@ -1858,19 +1895,20 @@
     }
 
     free(data);
   } else {
     double *data = malloc(plot_file->control_data.nel4 *
                           plot_file->control_data.nv2d * sizeof(double));
 
-    d3_buffer_read_words_at(
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
         &plot_file->buffer, data,
         plot_file->control_data.nel4 * plot_file->control_data.nv2d,
         plot_file->data_pointers[D3PLT_PTR_STATES + state] +
             plot_file->data_pointers[D3PLT_PTR_STATE_ELEMENT_SHELL]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_shells = 0;
       free(data);
       free(shells);
 
@@ -1987,70 +2025,72 @@
     return NULL;
   }
 
   *num_solids = plot_file->control_data.nel8;
   d3plot_solid_con *solids = malloc(*num_solids * sizeof(d3plot_solid_con));
   if (plot_file->buffer.word_size == 4) {
     uint32_t *solids32 = malloc(*num_solids * 9 * sizeof(uint32_t));
-    d3_buffer_read_words_at(&plot_file->buffer, solids32, 9 * *num_solids,
-                            plot_file->data_pointers[D3PLT_PTR_EL8_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, solids32, 9 * *num_solids,
+        plot_file->data_pointers[D3PLT_PTR_EL8_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_solids = 0;
       free(solids32);
       free(solids);
 
       END_PROFILE_FUNC();
       return NULL;
     }
 
     size_t i = 0;
     while (i < *num_solids) {
-      size_t j = 0;
-      while (j < 8) {
-        /* Subtract 1 because Fortran starts by 1 and C starts by 0*/
-        solids[i].node_indices[j + 0] = solids32[i * 9 + j + 0] - 1;
-        solids[i].node_indices[j + 1] = solids32[i * 9 + j + 1] - 1;
-        solids[i].node_indices[j + 2] = solids32[i * 9 + j + 2] - 1;
-        solids[i].node_indices[j + 3] = solids32[i * 9 + j + 3] - 1;
-
-        j += 4;
-      }
+      /* Subtract 1 because Fortran starts by 1 and C starts by 0*/
+      solids[i].node_indices[0] = solids32[i * 9 + 0] - 1;
+      solids[i].node_indices[1] = solids32[i * 9 + 1] - 1;
+      solids[i].node_indices[2] = solids32[i * 9 + 2] - 1;
+      solids[i].node_indices[3] = solids32[i * 9 + 3] - 1;
+      solids[i].node_indices[4] = solids32[i * 9 + 4] - 1;
+      solids[i].node_indices[5] = solids32[i * 9 + 5] - 1;
+      solids[i].node_indices[6] = solids32[i * 9 + 6] - 1;
+      solids[i].node_indices[7] = solids32[i * 9 + 7] - 1;
       solids[i].material_index = solids32[i * 9 + 8] - 1;
 
       i++;
     }
 
     free(solids32);
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, solids, 9 * *num_solids,
-                            plot_file->data_pointers[D3PLT_PTR_EL8_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, solids, 9 * *num_solids,
+        plot_file->data_pointers[D3PLT_PTR_EL8_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_solids = 0;
       free(solids);
 
       END_PROFILE_FUNC();
       return NULL;
     }
 
     size_t i = 0;
     while (i < *num_solids) {
-      size_t j = 0;
-      while (j < 8) {
-        /* Subtract 1 because Fortran starts by 1 and C starts by 0*/
-        solids[i].node_indices[j + 0] -= 1;
-        solids[i].node_indices[j + 1] -= 1;
-        solids[i].node_indices[j + 2] -= 1;
-        solids[i].node_indices[j + 3] -= 1;
-
-        j += 4;
-      }
+      /* Subtract 1 because Fortran starts by 1 and C starts by 0*/
+      solids[i].node_indices[0] -= 1;
+      solids[i].node_indices[1] -= 1;
+      solids[i].node_indices[2] -= 1;
+      solids[i].node_indices[3] -= 1;
+      solids[i].node_indices[4] -= 1;
+      solids[i].node_indices[5] -= 1;
+      solids[i].node_indices[6] -= 1;
+      solids[i].node_indices[7] -= 1;
       solids[i].material_index -= 1;
 
       i++;
     }
   }
 
   END_PROFILE_FUNC();
@@ -2070,17 +2110,18 @@
   }
 
   *num_thick_shells = plot_file->control_data.nelt;
   d3plot_thick_shell_con *thick_shells =
       malloc(*num_thick_shells * sizeof(d3plot_thick_shell_con));
   if (plot_file->buffer.word_size == 4) {
     uint32_t *thick_shells32 = malloc(*num_thick_shells * 9 * sizeof(uint32_t));
-    d3_buffer_read_words_at(&plot_file->buffer, thick_shells32,
-                            9 * *num_thick_shells,
-                            plot_file->data_pointers[D3PLT_PTR_ELT_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, thick_shells32, 9 * *num_thick_shells,
+        plot_file->data_pointers[D3PLT_PTR_ELT_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_thick_shells = 0;
       free(thick_shells32);
       free(thick_shells);
 
@@ -2103,17 +2144,18 @@
       thick_shells[i].material_index = thick_shells32[i * 9 + 8] - 1;
 
       i++;
     }
 
     free(thick_shells32);
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, thick_shells,
-                            9 * *num_thick_shells,
-                            plot_file->data_pointers[D3PLT_PTR_ELT_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, thick_shells, 9 * *num_thick_shells,
+        plot_file->data_pointers[D3PLT_PTR_ELT_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_thick_shells = 0;
       free(thick_shells);
 
       END_PROFILE_FUNC();
@@ -2153,16 +2195,18 @@
     return NULL;
   }
 
   *num_beams = plot_file->control_data.nel2;
   d3plot_beam_con *beams = malloc(*num_beams * sizeof(d3plot_beam_con));
   if (plot_file->buffer.word_size == 4) {
     uint32_t *beams32 = malloc(*num_beams * 6 * sizeof(uint32_t));
-    d3_buffer_read_words_at(&plot_file->buffer, beams32, 6 * *num_beams,
-                            plot_file->data_pointers[D3PLT_PTR_EL2_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, beams32, 6 * *num_beams,
+        plot_file->data_pointers[D3PLT_PTR_EL2_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_beams = 0;
       free(beams32);
       free(beams);
 
@@ -2181,16 +2225,18 @@
       beams[i].material_index = beams32[i * 6 + 5] - 1;
 
       i++;
     }
 
     free(beams32);
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, beams, 6 * *num_beams,
-                            plot_file->data_pointers[D3PLT_PTR_EL2_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, beams, 6 * *num_beams,
+        plot_file->data_pointers[D3PLT_PTR_EL2_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_beams = 0;
       free(beams);
 
       END_PROFILE_FUNC();
@@ -2224,16 +2270,18 @@
     return NULL;
   }
 
   *num_shells = plot_file->control_data.nel4;
   d3plot_shell_con *shells = malloc(*num_shells * sizeof(d3plot_shell_con));
   if (plot_file->buffer.word_size == 4) {
     uint32_t *shells32 = malloc(*num_shells * 5 * sizeof(uint32_t));
-    d3_buffer_read_words_at(&plot_file->buffer, shells32, 5 * *num_shells,
-                            plot_file->data_pointers[D3PLT_PTR_EL4_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, shells32, 5 * *num_shells,
+        plot_file->data_pointers[D3PLT_PTR_EL4_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_shells = 0;
       free(shells32);
       free(shells);
 
@@ -2251,16 +2299,18 @@
       shells[i].material_index = shells32[i * 5 + 4] - 1;
 
       i++;
     }
 
     free(shells32);
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, shells, 5 * *num_shells,
-                            plot_file->data_pointers[D3PLT_PTR_EL4_CONNECT]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, shells, 5 * *num_shells,
+        plot_file->data_pointers[D3PLT_PTR_EL4_CONNECT]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_shells = 0;
       free(shells);
 
       END_PROFILE_FUNC();
@@ -2287,16 +2337,17 @@
 char *d3plot_read_title(d3plot_file *plot_file) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   char *title = malloc(10 * plot_file->buffer.word_size + 1);
   /* We never set D3PLT_PTR_TITLE, but because the Title is at position 0 we
    * don't need to*/
-  d3_buffer_read_words_at(&plot_file->buffer, title, 10,
-                          plot_file->data_pointers[D3PLT_PTR_TITLE]);
+  d3_pointer d3_ptr = d3_buffer_read_words_at(
+      &plot_file->buffer, title, 10, plot_file->data_pointers[D3PLT_PTR_TITLE]);
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
     free(title);
 
     END_PROFILE_FUNC();
     return NULL;
@@ -2308,16 +2359,18 @@
 }
 
 struct tm *d3plot_read_run_time(d3plot_file *plot_file) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   d3_word run_time = 0;
-  d3_buffer_read_words_at(&plot_file->buffer, &run_time, 1,
-                          plot_file->data_pointers[D3PLT_PTR_RUN_TIME]);
+  d3_pointer d3_ptr =
+      d3_buffer_read_words_at(&plot_file->buffer, &run_time, 1,
+                              plot_file->data_pointers[D3PLT_PTR_RUN_TIME]);
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
     return NULL;
   }
   const time_t epoch_time = run_time;
   struct tm *time_value = localtime(&epoch_time);
@@ -2327,16 +2380,18 @@
 }
 
 time_t d3plot_read_epoch_run_time(d3plot_file *plot_file) {
   BEGIN_PROFILE_FUNC();
   CLEAR_ERROR_STRING();
 
   d3_word run_time = 0;
-  d3_buffer_read_words_at(&plot_file->buffer, &run_time, 1,
-                          plot_file->data_pointers[D3PLT_PTR_RUN_TIME]);
+  d3_pointer d3_ptr =
+      d3_buffer_read_words_at(&plot_file->buffer, &run_time, 1,
+                              plot_file->data_pointers[D3PLT_PTR_RUN_TIME]);
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
     return (time_t)0;
   }
   const time_t epoch_time = run_time;
 
@@ -2561,17 +2616,19 @@
     ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     return NULL;
   }
 
   *num_nodes = plot_file->control_data.numnp;
   double *coords = malloc(*num_nodes * 3 * sizeof(double));
 
-  d3_buffer_read_words_at(&plot_file->buffer, coords, *num_nodes * 3,
-                          plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                              plot_file->data_pointers[data_type]);
+  d3_pointer d3_ptr = d3_buffer_read_words_at(
+      &plot_file->buffer, coords, *num_nodes * 3,
+      plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+          plot_file->data_pointers[data_type]);
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
     *num_nodes = 0;
     free(coords);
     return NULL;
   }
@@ -2609,17 +2666,19 @@
     ERROR_AND_NO_RETURN_F_PTR("%zu is out of bounds for the states", state);
     return NULL;
   }
 
   *num_nodes = plot_file->control_data.numnp;
   float *coords = malloc(*num_nodes * 3 * sizeof(float));
 
-  d3_buffer_read_words_at(&plot_file->buffer, coords, *num_nodes * 3,
-                          plot_file->data_pointers[D3PLT_PTR_STATES + state] +
-                              plot_file->data_pointers[data_type]);
+  d3_pointer d3_ptr = d3_buffer_read_words_at(
+      &plot_file->buffer, coords, *num_nodes * 3,
+      plot_file->data_pointers[D3PLT_PTR_STATES + state] +
+          plot_file->data_pointers[data_type]);
+  d3_pointer_close(&plot_file->buffer, &d3_ptr);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
     *num_nodes = 0;
     free(coords);
     return NULL;
   }
@@ -2635,16 +2694,18 @@
   if (num_ids_value == 0) {
     return NULL;
   }
 
   d3_word *ids = malloc(*num_ids * sizeof(d3_word));
   if (plot_file->buffer.word_size == 4) {
     uint32_t *ids32 = malloc(*num_ids * plot_file->buffer.word_size);
-    d3_buffer_read_words_at(&plot_file->buffer, ids32, *num_ids,
-                            plot_file->data_pointers[data_type]);
+    d3_pointer d3_ptr =
+        d3_buffer_read_words_at(&plot_file->buffer, ids32, *num_ids,
+                                plot_file->data_pointers[data_type]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_ids = 0;
       free(ids32);
       free(ids);
       return NULL;
@@ -2655,16 +2716,17 @@
       ids[i] = ids32[i];
 
       i++;
     }
 
     free(ids32);
   } else {
-    d3_buffer_read_words_at(&plot_file->buffer, ids, *num_ids,
-                            plot_file->data_pointers[data_type]);
+    d3_pointer d3_ptr = d3_buffer_read_words_at(
+        &plot_file->buffer, ids, *num_ids, plot_file->data_pointers[data_type]);
+    d3_pointer_close(&plot_file->buffer, &d3_ptr);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                                 plot_file->buffer.error_string);
       *num_ids = 0;
       free(ids);
       return NULL;
     }
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot.h` & `dynareadout-23.6/lib/dynareadout/src/d3plot.h`

 * *Files 2% similar despite different names*

```diff
@@ -258,26 +258,29 @@
  * multiple times, it is best to preload the part ids. The return value needs to
  * be deallocated by d3plot_free_part.*/
 d3plot_part d3plot_read_part_by_id(d3plot_file *plot_file, d3_word part_id,
                                    const d3_word *part_ids, size_t num_parts);
 
 /***** Data sections *******/
 /* GEOMETRY DATA pg. 17*/
-int _d3plot_read_geometry_data(d3plot_file *plot_file);
+int _d3plot_read_geometry_data(d3plot_file *plot_file, d3_pointer *d3_ptr);
 /* USER MATERIAL, NODE, AND ELEMENT IDENTIFICATION NUMBERS pg. 18*/
-int _d3plot_read_user_identification_numbers(d3plot_file *plot_file);
+int _d3plot_read_user_identification_numbers(d3plot_file *plot_file,
+                                             d3_pointer *d3_ptr);
 /* EXTRA 2, 4, 12 NODE CONNECTIVITY FOR 10, 8, 20 NODE TETRAHEDRON, SHELL, SOLID
  * ELEMENTS pg. 19*/
-int _d3plot_read_extra_node_connectivity(d3plot_file *plot_file);
+int _d3plot_read_extra_node_connectivity(d3plot_file *plot_file,
+                                         d3_pointer *d3_ptr);
 /* ADAPTED ELEMENT PARENT LIST (not implemented) pg. 19*/
-int _d3plot_read_adapted_element_parent_list(d3plot_file *plot_file);
+int _d3plot_read_adapted_element_parent_list(d3plot_file *plot_file,
+                                             d3_pointer *d3_ptr);
 /* HEADER, PART & CONTACT INTERFACE TITLES pg. 22*/
-int _d3plot_read_header(d3plot_file *plot_file);
+int _d3plot_read_header(d3plot_file *plot_file, d3_pointer *d3_ptr);
 /* STATE DATA pg. 31*/
-int _d3plot_read_state_data(d3plot_file *plot_file);
+int _d3plot_read_state_data(d3plot_file *plot_file, d3_pointer *d3_ptr);
 /***************************/
 
 /***** Private Functions ********/
 /* Return a string representing the given file type*/
 const char *_d3plot_get_file_type_name(d3_word file_type);
 /* Return the nth digit of an integer as an integer.
  * Example: value=32, n=0 -> rv=2; value=32, n=1 -> rv=3;
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot_data.c` & `dynareadout-23.6/lib/dynareadout/src/d3plot_data.c`

 * *Files 19% similar despite different names*

```diff
@@ -30,47 +30,48 @@
 
 #ifndef CDP
 #define CDP plot_file->control_data
 #endif
 #ifdef DT_PTR_SET
 #undef DT_PTR_SET
 #endif
-#define DT_PTR_SET(index)                                                      \
-  plot_file->data_pointers[index] = plot_file->buffer.cur_word
+#define DT_PTR_SET(index) plot_file->data_pointers[index] = d3_ptr->cur_word
 #define DT_PTR_SET_DPTR(index) plot_file->data_pointers[index] = data_pointer
 
 #include "d3plot_error_macros.h"
 
-int _d3plot_read_geometry_data(d3plot_file *plot_file) {
+int _d3plot_read_geometry_data(d3plot_file *plot_file, d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
   /* We can skip the entire GEOMETRY DATA section since we already know
    * how big it is and where to find the data*/
-  const size_t geometry_start_word = plot_file->buffer.cur_word;
+  const size_t geometry_start_word = d3_ptr->cur_word;
   size_t data_pointer = geometry_start_word;
 
   if (CDP.element_connectivity_packed) {
     ERROR_AND_NO_RETURN_PTR("Packed Element Connectivity is not supported");
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* Here are the node coordinates*/
   DT_PTR_SET_DPTR(D3PLT_PTR_NODE_COORDS);
 
   data_pointer += CDP.numnp * CDP.ndim;
 
+  DT_PTR_SET_DPTR(D3PLT_PTR_EL8_CONNECT);
+  int64_t nel8;
   if (CDP.nel8 > 0) {
-    DT_PTR_SET_DPTR(D3PLT_PTR_EL8_CONNECT);
-    data_pointer += 9 * CDP.nel8;
-  } else if (CDP.nel8 < 0) {
-    const int64_t nel8 = CDP.nel8 * -1;
+    nel8 = CDP.nel8;
+  } else {
+    nel8 = -CDP.nel8;
     data_pointer += 2 * nel8;
     /* TODO: read function for -nel8 data*/
   }
+  data_pointer += 9 * nel8;
 
   if (CDP.nelt > 0) {
     DT_PTR_SET_DPTR(D3PLT_PTR_ELT_CONNECT);
     data_pointer += 9 * CDP.nelt;
   }
 
   if (CDP.nel2 > 0) {
@@ -80,93 +81,95 @@
 
   if (CDP.nel4 > 0) {
     DT_PTR_SET_DPTR(D3PLT_PTR_EL4_CONNECT);
     data_pointer += 5 * CDP.nel4;
   }
 
   /* Skip the entire geometry section*/
-  d3_buffer_skip_words(&plot_file->buffer, data_pointer - geometry_start_word);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr,
+                       data_pointer - geometry_start_word);
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
   return 1;
 }
 
-int _d3plot_read_user_identification_numbers(d3plot_file *plot_file) {
+int _d3plot_read_user_identification_numbers(d3plot_file *plot_file,
+                                             d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
   if (CDP.narbs == 0) {
     CDP.numrbs = 0;
 
     END_PROFILE_FUNC();
     return 1;
   }
 
-  const size_t user_ids_start = plot_file->buffer.cur_word;
+  const size_t user_ids_start = d3_ptr->cur_word;
 
   int64_t nsort;
   d3_word nsortd = 0, nsrhd = 0, nsrbd = 0, nsrsd = 0, nsrtd = 0,
           nmmat = plot_file->control_data.nmmat;
   if (plot_file->buffer.word_size == 4) {
     int32_t nsort32;
-    d3_buffer_read_words(&plot_file->buffer, &nsort32, 1);
+    d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsort32, 1);
     nsort = nsort32;
   } else {
-    d3_buffer_read_words(&plot_file->buffer, &nsort, 1);
+    d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsort, 1);
   }
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read NSORT: %s",
                               plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
-  d3_buffer_skip_words(&plot_file->buffer, 4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 4);
   /* TODO: Find out what NSRH, NSRB, NSRS and NSRT is for*/
-  d3_buffer_read_words(&plot_file->buffer, &nsortd, 1);
-  d3_buffer_read_words(&plot_file->buffer, &nsrhd, 1);
-  d3_buffer_read_words(&plot_file->buffer, &nsrbd, 1);
-  d3_buffer_read_words(&plot_file->buffer, &nsrsd, 1);
-  d3_buffer_read_words(&plot_file->buffer, &nsrtd, 1);
+  d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsortd, 1);
+  d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsrhd, 1);
+  d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsrbd, 1);
+  d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsrsd, 1);
+  d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nsrtd, 1);
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR(
         "Failed to read NSORTD, NSRHD, NSRBD, NSRSD and NSRTD: %s",
         plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
   CDP.numrbs = 0;
 
   if (nsort < 0) {
-    d3_buffer_skip_words(&plot_file->buffer, 4);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 4);
     /* TODO: Find out what NSRMA, NSRMU, NSRMP and NSRTM is for*/
-    d3_buffer_read_words(&plot_file->buffer, &CDP.numrbs, 1);
-    d3_buffer_read_words(&plot_file->buffer, &nmmat, 1);
+    d3_buffer_read_words(&plot_file->buffer, d3_ptr, &CDP.numrbs, 1);
+    d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nmmat, 1);
 
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read NUMRBS and NMMAT: %s",
                                 plot_file->buffer.error_string);
 
       END_PROFILE_FUNC();
       return 0;
     }
   }
 
-  const size_t data_pointer_start = plot_file->buffer.cur_word;
-  size_t data_pointer = plot_file->buffer.cur_word;
+  const size_t data_pointer_start = d3_ptr->cur_word;
+  size_t data_pointer = d3_ptr->cur_word;
   DT_PTR_SET_DPTR(D3PLT_PTR_NODE_IDS);
   data_pointer += nsortd; /* nusern*/
   DT_PTR_SET_DPTR(D3PLT_PTR_EL8_IDS);
   data_pointer += nsrhd; /* nuserh*/
   DT_PTR_SET_DPTR(D3PLT_PTR_EL2_IDS);
   data_pointer += nsrbd; /* nuserb*/
   DT_PTR_SET_DPTR(D3PLT_PTR_EL4_IDS);
@@ -179,43 +182,45 @@
     /* TODO: Find out what NSRMU and NSRMP is for*/
   } else {
     /* These values are not used when nsort >= 0*/
     data_pointer += 3 * nmmat;
   }
 
   /* Skip multiple values at once*/
-  d3_buffer_skip_words(&plot_file->buffer, data_pointer - data_pointer_start);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr,
+                       data_pointer - data_pointer_start);
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
-  const size_t user_ids_end = plot_file->buffer.cur_word;
+  const size_t user_ids_end = d3_ptr->cur_word;
   const size_t user_ids_size = user_ids_end - user_ids_start;
   if (user_ids_size != CDP.narbs) {
     ERROR_AND_NO_RETURN_F_PTR(
         "The USER IDENTIFICATION NUMBERS section is false (%zu != %llu)",
         user_ids_size, CDP.narbs);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
   return 1;
 }
 
-int _d3plot_read_extra_node_connectivity(d3plot_file *plot_file) {
+int _d3plot_read_extra_node_connectivity(d3plot_file *plot_file,
+                                         d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
-  const size_t data_pointer_start = plot_file->buffer.cur_word;
+  const size_t data_pointer_start = d3_ptr->cur_word;
   size_t data_pointer = data_pointer_start;
   if (CDP.nel8 < 0) {
     const int64_t nel8 = CDP.nel8 * -1;
     data_pointer += 2 * nel8;
     /* TODO: read function for -nel8 data*/
   }
 
@@ -226,124 +231,126 @@
 
   if (CDP.nel20 > 0) {
     data_pointer += 13 * CDP.nel20;
     /* TODO: read function for nel20 data*/
   }
 
   /* Skip everything at once*/
-  d3_buffer_skip_words(&plot_file->buffer, data_pointer - data_pointer_start);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr,
+                       data_pointer - data_pointer_start);
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
 
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
   return 1;
 }
 
-int _d3plot_read_adapted_element_parent_list(d3plot_file *plot_file) {
+int _d3plot_read_adapted_element_parent_list(d3plot_file *plot_file,
+                                             d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
   if (CDP.nadapt == 0) {
     END_PROFILE_FUNC();
     return 1;
   }
 
-  d3_buffer_skip_words(&plot_file->buffer, 2 * CDP.nadapt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 2 * CDP.nadapt);
   /* TODO: read function for aepl*/
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
   END_PROFILE_FUNC();
   return 1;
 }
 
-int _d3plot_read_header(d3plot_file *plot_file) {
+int _d3plot_read_header(d3plot_file *plot_file, d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
   while (1) {
     d3_word ntype = 0;
-    d3_buffer_read_words(&plot_file->buffer, &ntype, 1);
+    d3_buffer_read_words(&plot_file->buffer, d3_ptr, &ntype, 1);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to read NTYPE: %s",
                                 plot_file->buffer.error_string);
       END_PROFILE_FUNC();
       return 0;
     }
 
     if (ntype == 90000) {
       /* HEAD is always 72 bytes*/
-      d3_buffer_skip_bytes(&plot_file->buffer, 72);
+      d3_buffer_skip_bytes(&plot_file->buffer, d3_ptr, 72);
       /* TODO: read function for head*/
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
 
     } else if (ntype == 90001) {
       d3_word numprop = 0;
-      d3_buffer_read_words(&plot_file->buffer, &numprop, 1);
+      d3_buffer_read_words(&plot_file->buffer, d3_ptr, &numprop, 1);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read NUMPROP: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
       DT_PTR_SET(D3PLT_PTR_PART_TITLES);
       /* PTITLE is always 72 bytes*/
-      d3_buffer_skip_bytes(&plot_file->buffer,
+      d3_buffer_skip_bytes(&plot_file->buffer, d3_ptr,
                            (1 * plot_file->buffer.word_size + 72) * numprop);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
     } else if (ntype == 90002) {
       d3_word numcon = 0;
-      d3_buffer_read_words(&plot_file->buffer, &numcon, 1);
+      d3_buffer_read_words(&plot_file->buffer, d3_ptr, &numcon, 1);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read NUMCON: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
       /* CTITLE is always 72 bytes*/
-      d3_buffer_skip_bytes(&plot_file->buffer,
+      d3_buffer_skip_bytes(&plot_file->buffer, d3_ptr,
                            (1 * plot_file->buffer.word_size + 72) * numcon);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
       /* TODO: read function for contact titles*/
 
     } else if (ntype == 900100) {
       d3_word nline = 0;
-      d3_buffer_read_words(&plot_file->buffer, &nline, 1);
+      d3_buffer_read_words(&plot_file->buffer, d3_ptr, &nline, 1);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to read NLINE: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
       /* KEYWORD is always 80 bytes*/
-      d3_buffer_skip_bytes(&plot_file->buffer, 80 * nline);
+      d3_buffer_skip_bytes(&plot_file->buffer, d3_ptr, 80 * nline);
       if (plot_file->buffer.error_string) {
         ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                                   plot_file->buffer.error_string);
         END_PROFILE_FUNC();
         return 0;
       }
       /* TODO: read function for extra keyword lines?*/
@@ -358,15 +365,15 @@
         memcpy(&eof_marker, &ntype, plot_file->buffer.word_size);
       }
 
       if (eof_marker != D3_EOF) {
         ERROR_AND_NO_RETURN_F_PTR(
             "Here (after header) 'd3plot':(%zu) should be "
             "the EOF marker (%f != %f)",
-            plot_file->buffer.cur_word - 1, eof_marker, D3_EOF);
+            d3_ptr->cur_word - 1, eof_marker, D3_EOF);
         END_PROFILE_FUNC();
         return 0;
       }
 
       break;
     }
   }
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot_error_macros.h` & `dynareadout-23.6/lib/dynareadout/src/d3plot_error_macros.h`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 #define ERROR_AND_NO_RETURN_F_PTR(format_str, ...)                             \
   {                                                                            \
     char format_buffer[1024];                                                  \
     sprintf(format_buffer, format_str, __VA_ARGS__);                           \
     ERROR_AND_NO_RETURN_PTR(format_buffer);                                    \
   }
 #define ERROR_AND_RETURN(msg)                                                  \
+  d3_pointer_close(&plot_file.buffer, &d3_ptr);                                \
   if (plot_file.error_string)                                                  \
     free(plot_file.error_string);                                              \
   plot_file.error_string = malloc(strlen(msg) + 1);                            \
   sprintf(plot_file.error_string, "%s", msg);                                  \
   END_PROFILE_FUNC();                                                          \
   return plot_file;
 #define ERROR_AND_RETURN_F(format_str, ...)                                    \
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.c` & `dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot_part_nodes.h` & `dynareadout-23.6/lib/dynareadout/src/d3plot_part_nodes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/d3plot_state.c` & `dynareadout-23.6/lib/dynareadout/src/d3plot_state.c`

 * *Files 23% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 #define CDP plot_file->control_data
 #endif
 #ifdef DT_PTR_SET
 #undef DT_PTR_SET
 #endif
 #define DT_PTR_SET(value)                                                      \
   if (plot_file->num_states == 1)                                              \
-  plot_file->data_pointers[value] = plot_file->buffer.cur_word - state_start
+  plot_file->data_pointers[value] = d3_ptr->cur_word - state_start
 
 #include "d3plot_error_macros.h"
 
-int _d3plot_read_state_data(d3plot_file *plot_file) {
+int _d3plot_read_state_data(d3plot_file *plot_file, d3_pointer *d3_ptr) {
   BEGIN_PROFILE_FUNC();
 
-  const size_t state_start = plot_file->buffer.cur_word;
+  const size_t state_start = d3_ptr->cur_word;
 
   double time;
-  d3_buffer_read_double_word(&plot_file->buffer, &time);
+  d3_buffer_read_double_word(&plot_file->buffer, d3_ptr, &time);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read time: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
@@ -62,94 +62,94 @@
   plot_file->data_pointers =
       realloc(plot_file->data_pointers,
               (D3PLT_PTR_COUNT + plot_file->num_states) * sizeof(size_t));
   plot_file->data_pointers[D3PLT_PTR_STATES + plot_file->num_states - 1] =
       state_start;
 
   /* GLOBAL*/
-  const size_t global_start = plot_file->buffer.cur_word;
+  const size_t global_start = d3_ptr->cur_word;
 
-  d3_buffer_skip_words(&plot_file->buffer, 6);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 6);
   /* TODO: read functions for KE, IE, TE, X, Y and Z*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 IE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 IE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 IE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT IE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS IE*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 KE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 KE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 KE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT KE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS KE*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 X*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 X*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 X*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT X*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS X*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 Y*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 Y*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 Y*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT Y*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS Y*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 Z*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 Z*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 Z*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT Z*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS Z*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 MASS*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 MASS*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 MASS*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT MASS*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS MASS*/
 
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat8);
   /* TODO: read function for MAT8 FORCE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat2);
   /* TODO: read function for MAT2 FORCE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummat4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummat4);
   /* TODO: read function for MAT4 FORCE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nummatt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nummatt);
   /* TODO: read function for MATT FORCE*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.numrbs);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numrbs);
   /* TODO: read function for RBS FORCE*/
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
@@ -161,105 +161,105 @@
   {
     numrw = (CDP.nglbv - 6 -
              7 * (CDP.nummat8 + CDP.nummat2 + CDP.nummat4 + CDP.nummatt +
                   CDP.numrbs)) /
             RWN;
   }
 
-  d3_buffer_skip_words(&plot_file->buffer, numrw);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, numrw);
   /* TODO: read function for RW_FORCE*/
 
   if (RWN == 4) {
-    d3_buffer_skip_words(&plot_file->buffer, numrw * 3);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, numrw * 3);
     /* TODO: read function for RW_POS*/
   }
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip RW: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
-  const size_t global_end = plot_file->buffer.cur_word;
+  const size_t global_end = d3_ptr->cur_word;
   const size_t global_size = global_end - global_start;
 
   if (global_size != CDP.nglbv) {
     ERROR_AND_NO_RETURN_F_PTR("Size of GLOBAL is %zu instead of %llu",
                               global_size, CDP.nglbv);
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* NODEDATA*/
   /**** Order of Node Data ******
    * IT, U, Mass Scaling, V, A
    ******************************/
 
-  const size_t node_data_start = plot_file->buffer.cur_word;
+  const size_t node_data_start = d3_ptr->cur_word;
 
   uint8_t it = _get_nth_digit(CDP.it, 0);
   uint8_t N = it * (it > 1);
   if (N == 2) {
     it = 1;
     N = 3;
   }
   const uint8_t mass_N = _get_nth_digit(CDP.it, 1) == 1;
 
   const size_t NND =
       ((it + N + mass_N) + CDP.ndim * (CDP.iu + CDP.iv + CDP.ia)) * CDP.numnp;
 
   if (it > 0) {
-    d3_buffer_skip_words(&plot_file->buffer, it * CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, it * CDP.numnp);
     /* TODO: read function for IT data*/
   }
 
   if (N > 0) {
-    d3_buffer_skip_words(&plot_file->buffer, N * CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, N * CDP.numnp);
     /* TODO: read function for NODE FLUX data*/
   }
 
   if (mass_N) {
-    d3_buffer_skip_words(&plot_file->buffer, CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.numnp);
     /* TODO: read function for MASS SCALING*/
   }
 
   if (CDP.iu) {
     DT_PTR_SET(D3PLT_PTR_STATE_NODE_COORDS);
-    d3_buffer_skip_words(&plot_file->buffer, 3 * CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 3 * CDP.numnp);
   }
 
   if (CDP.iv) {
     DT_PTR_SET(D3PLT_PTR_STATE_NODE_VEL);
-    d3_buffer_skip_words(&plot_file->buffer, 3 * CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 3 * CDP.numnp);
   }
 
   if (CDP.ia) {
     DT_PTR_SET(D3PLT_PTR_STATE_NODE_ACC);
-    d3_buffer_skip_words(&plot_file->buffer, 3 * CDP.numnp);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, 3 * CDP.numnp);
   }
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip words: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
-  const size_t node_data_end = plot_file->buffer.cur_word;
+  const size_t node_data_end = d3_ptr->cur_word;
   const size_t node_data_size = node_data_end - node_data_start;
   if (node_data_size != NND) {
     ERROR_AND_NO_RETURN_F_PTR("NODEDATA should be %zu instead of %zu", NND,
                               node_data_size);
     END_PROFILE_FUNC();
     return 0;
   }
 
   /* THERMDATA*/
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nt3d * CDP.nel8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nt3d * CDP.nel8);
   /* TODO: read function for nt3d data*/
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip THERMDATA: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
@@ -268,38 +268,38 @@
   /* CFDDATA is no longer output*/
 
   /* ELEMDATA*/
   const size_t ENN =
       CDP.nel8 * CDP.nv3d + CDP.nelt * CDP.nv3dt + CDP.nel2 * CDP.nv1d +
       CDP.nel4 * CDP.nv2d +
       CDP.nmsph * 0; /* We don't support SMOOTH PARTICLE HYDRODYNAMICS*/
-  const size_t elem_data_start = plot_file->buffer.cur_word;
+  const size_t elem_data_start = d3_ptr->cur_word;
 
   DT_PTR_SET(D3PLT_PTR_STATE_ELEMENT_SOLID);
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nv3d * CDP.nel8);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nv3d * CDP.nel8);
 
   DT_PTR_SET(D3PLT_PTR_STATE_ELEMENT_BEAM);
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nv1d * CDP.nel2);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nv1d * CDP.nel2);
 
   DT_PTR_SET(D3PLT_PTR_STATE_ELEMENT_SHELL);
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nv2d * CDP.nel4);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nv2d * CDP.nel4);
 
   /* Then follows who knows what -_(′_′)_-*/
   /* But because we don't support NMSPH, we can assume that NELT follows*/
   DT_PTR_SET(D3PLT_PTR_STATE_ELEMENT_THICK_SHELL);
-  d3_buffer_skip_words(&plot_file->buffer, CDP.nv3dt * CDP.nelt);
+  d3_buffer_skip_words(&plot_file->buffer, d3_ptr, CDP.nv3dt * CDP.nelt);
 
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to skip ELEMDATA: %s",
                               plot_file->buffer.error_string);
     END_PROFILE_FUNC();
     return 0;
   }
 
-  const size_t elem_data_end = plot_file->buffer.cur_word;
+  const size_t elem_data_end = d3_ptr->cur_word;
   const size_t elem_data_size = elem_data_end - elem_data_start;
   if (elem_data_size < ENN) {
     ERROR_AND_NO_RETURN_F_PTR("ELEMDATA should be %zu instead of %zu", ENN,
                               elem_data_size);
     END_PROFILE_FUNC();
     return 0;
   }
@@ -315,23 +315,23 @@
   } else {
     ERROR_AND_NO_RETURN_F_PTR("The value of MDLOPT is invalid: %d", CDP.mdlopt);
     END_PROFILE_FUNC();
     return 0;
   }
 
   if (skip_words > 0) {
-    d3_buffer_skip_words(&plot_file->buffer, skip_words);
+    d3_buffer_skip_words(&plot_file->buffer, d3_ptr, skip_words);
     if (plot_file->buffer.error_string) {
       ERROR_AND_NO_RETURN_F_PTR("Failed to skip Element Deletion Option: %s",
                                 plot_file->buffer.error_string);
       END_PROFILE_FUNC();
       return 0;
     }
   }
 
-  const size_t state_end = plot_file->buffer.cur_word;
+  const size_t state_end = d3_ptr->cur_word;
   const size_t state_size =
       (state_end - state_start) * plot_file->buffer.word_size;
 
   END_PROFILE_FUNC();
   return 1;
 }
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/extra_string.c` & `dynareadout-23.6/lib/dynareadout/src/extra_string.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/extra_string.h` & `dynareadout-23.6/lib/dynareadout/src/extra_string.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/key.c` & `dynareadout-23.6/lib/dynareadout/src/key.c`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 
 typedef struct {
   keyword_t *current_keyword;
   keyword_t *keywords;
   size_t *num_keywords;
 } key_file_parse_data;
 
-void key_file_parse_callback(const char *keyword_name, const card_t *card,
+void key_file_parse_callback(const char *file_name, size_t line_number,
+                             const char *keyword_name, card_t *card,
                              size_t card_index, void *user_data) {
   key_file_parse_data *data = (key_file_parse_data *)user_data;
 
   if (!data->current_keyword || card_index == 0 || card_index == (size_t)~0) {
     size_t index = 0;
 
     if (data->keywords) {
@@ -113,16 +114,17 @@
   /* Add the card to the keyword*/
   data->current_keyword->num_cards++;
   data->current_keyword->cards =
       realloc(data->current_keyword->cards,
               data->current_keyword->num_cards * sizeof(card_t));
   card_t *keyword_card =
       &data->current_keyword->cards[data->current_keyword->num_cards - 1];
-  keyword_card->string = malloc(LINE_WIDTH + 1);
-  memcpy(keyword_card->string, card->string, LINE_WIDTH + 1);
+  const size_t card_len = strlen(card->string);
+  keyword_card->string = malloc(card_len + 1);
+  memcpy(keyword_card->string, card->string, card_len + 1);
 }
 
 keyword_t *key_file_parse(const char *file_name, size_t *num_keywords,
                           int parse_includes, char **error_string) {
   BEGIN_PROFILE_FUNC();
 
   key_file_parse_data data;
@@ -371,15 +373,16 @@
         } else {
           keyword_name = malloc(current_keyword_length + 1);
           extra_string_copy_to_string(keyword_name, &current_keyword_name,
                                       current_keyword_length);
           keyword_name[current_keyword_length] = '\0';
         }
 
-        callback(keyword_name, NULL, (size_t)~0, user_data);
+        callback(file_name, line_count, keyword_name, NULL, (size_t)~0,
+                 user_data);
 
         if (keyword_name != current_keyword_name.buffer) {
           free(keyword_name);
         }
       }
 
       extra_string_copy(&current_keyword_name, &line, line_length, i + 1);
@@ -413,177 +416,226 @@
       } else {
         card.string = malloc(line_length + 1);
         extra_string_copy_to_string(card.string, &line, line_length);
         card.string[line_length] = '\0';
       }
 
       /* -------- ⛅ Include Parsing ⛅ -------*/
-      if (parse_includes &&
-          extra_string_starts_with(&current_keyword_name, "INCLUDE")) {
-        /* Parse all the different INCLUDE keywords*/
-        if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0) {
-          _parse_include_file_name_card(
-              &card, &card_index, &line, line_length,
-              &current_multi_line_string, &current_multi_line_index,
-              num_include_paths_ptr, include_paths_ptr, callback, user_data,
-              &error_stack, &error_stack_size, &error_ptr, file_name,
-              line_count, root_folder_ptr);
-          continue;
-        } else if (extra_string_compare(&current_keyword_name,
-                                        "INCLUDE_PATH") == 0) {
-          /* Support multi line file names (LS Dyna Manual Volume I
-           * *INCLUDE Remark 2, p. 2690)*/
-          if (!_parse_multi_line_string(&current_multi_line_string,
-                                        &current_multi_line_index, &card,
-                                        line_length)) {
+      if (extra_string_starts_with(&current_keyword_name, "INCLUDE")) {
+        /* Also parse the INCLUDE keywords even when parse_includes is set to 0
+         * to support multi line include file names*/
+        if (parse_includes) {
+          /* Parse all the different INCLUDE keywords*/
+          if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0) {
+            _parse_include_file_name_card(
+                &card, &card_index, &line, line_length,
+                &current_multi_line_string, &current_multi_line_index,
+                num_include_paths_ptr, include_paths_ptr, callback, user_data,
+                &error_stack, &error_stack_size, &error_ptr, file_name,
+                line_count, root_folder_ptr);
+            continue;
+          } else if (extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_PATH") == 0) {
+            /* Support multi line file names (LS Dyna Manual Volume I
+             * *INCLUDE Remark 2, p. 2690)*/
+            if (!_parse_multi_line_string(&current_multi_line_string,
+                                          &current_multi_line_index, &card,
+                                          line_length)) {
+              /* continue without calling the callback for the card*/
+              if (card.string != line.buffer) {
+                free(card.string);
+              }
+              continue;
+            }
+
+            (*num_include_paths_ptr)++;
+            *include_paths_ptr = realloc(
+                *include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
+            (*include_paths_ptr)[*num_include_paths_ptr - 1] =
+                current_multi_line_string;
+
+            current_multi_line_string = NULL;
+            current_multi_line_index = 0;
+
             /* continue without calling the callback for the card*/
             if (card.string != line.buffer) {
               free(card.string);
             }
+
+            card_index++;
             continue;
-          }
+          } else if (extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_PATH_RELATIVE") == 0) {
+            /* Support multi line file names (LS Dyna Manual Volume I
+             * *INCLUDE Remark 2, p. 2690)*/
+            if (!_parse_multi_line_string(&current_multi_line_string,
+                                          &current_multi_line_index, &card,
+                                          line_length)) {
+              /* continue without calling the callback for the card*/
+              if (card.string != line.buffer) {
+                free(card.string);
+              }
+              continue;
+            }
 
-          (*num_include_paths_ptr)++;
-          *include_paths_ptr = realloc(*include_paths_ptr,
-                                       *num_include_paths_ptr * sizeof(char *));
-          (*include_paths_ptr)[*num_include_paths_ptr - 1] =
-              current_multi_line_string;
-
-          current_multi_line_string = NULL;
-          current_multi_line_index = 0;
-
-          /* continue without calling the callback for the card*/
-          if (card.string != line.buffer) {
-            free(card.string);
-          }
+            char *full_include_path_name =
+                path_join(root_folder_ptr, current_multi_line_string);
+            free(current_multi_line_string);
+            current_multi_line_string = NULL;
+            current_multi_line_index = 0;
+
+            (*num_include_paths_ptr)++;
+            *include_paths_ptr = realloc(
+                *include_paths_ptr, *num_include_paths_ptr * sizeof(char *));
+            (*include_paths_ptr)[*num_include_paths_ptr - 1] =
+                full_include_path_name;
 
-          card_index++;
-          continue;
-        } else if (extra_string_compare(&current_keyword_name,
-                                        "INCLUDE_PATH_RELATIVE") == 0) {
-          /* Support multi line file names (LS Dyna Manual Volume I
-           * *INCLUDE Remark 2, p. 2690)*/
-          if (!_parse_multi_line_string(&current_multi_line_string,
-                                        &current_multi_line_index, &card,
-                                        line_length)) {
             /* continue without calling the callback for the card*/
             if (card.string != line.buffer) {
               free(card.string);
             }
+
+            card_index++;
             continue;
-          }
+          } else if (extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_BINARY") == 0) {
+            /* Parse the first card like a normal INCLUDE*/
+            if (card_index == 0) {
+              _parse_include_file_name_card(
+                  &card, &card_index, &line, line_length,
+                  &current_multi_line_string, &current_multi_line_index,
+                  num_include_paths_ptr, include_paths_ptr, callback, user_data,
+                  &error_stack, &error_stack_size, &error_ptr, file_name,
+                  line_count, root_folder_ptr);
+              continue;
+            } else {
+              ERROR_F(
+                  "%s:%zu: Invalid number of cards for INCLUDE_BINARY keyword",
+                  file_name, line_count);
+            }
 
-          char *full_include_path_name =
-              path_join(root_folder_ptr, current_multi_line_string);
-          free(current_multi_line_string);
-          current_multi_line_string = NULL;
-          current_multi_line_index = 0;
-
-          (*num_include_paths_ptr)++;
-          *include_paths_ptr = realloc(*include_paths_ptr,
-                                       *num_include_paths_ptr * sizeof(char *));
-          (*include_paths_ptr)[*num_include_paths_ptr - 1] =
-              full_include_path_name;
-
-          /* continue without calling the callback for the card*/
-          if (card.string != line.buffer) {
-            free(card.string);
-          }
+            /* continue without calling the callback for the card*/
+            if (card.string != line.buffer) {
+              free(card.string);
+            }
 
-          card_index++;
-          continue;
-        } else if (extra_string_compare(&current_keyword_name,
-                                        "INCLUDE_BINARY") == 0) {
-          /* Parse the first card like a normal INCLUDE*/
-          if (card_index == 0) {
-            _parse_include_file_name_card(
-                &card, &card_index, &line, line_length,
-                &current_multi_line_string, &current_multi_line_index,
-                num_include_paths_ptr, include_paths_ptr, callback, user_data,
-                &error_stack, &error_stack_size, &error_ptr, file_name,
-                line_count, root_folder_ptr);
+            card_index++;
             continue;
-          } else {
-            ERROR_F(
-                "%s:%zu: Invalid number of cards for INCLUDE_BINARY keyword",
-                file_name, line_count);
-          }
+          } else if (extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_NASTRAN") == 0) {
+            /* Parse the first card like a normal INCLUDE*/
+            if (card_index == 0) {
+              _parse_include_file_name_card(
+                  &card, &card_index, &line, line_length,
+                  &current_multi_line_string, &current_multi_line_index,
+                  num_include_paths_ptr, include_paths_ptr, callback, user_data,
+                  &error_stack, &error_stack_size, &error_ptr, file_name,
+                  line_count, root_folder_ptr);
+              continue;
+            } else if (card_index == 1) {
+              /* Ignore the card it is irrelevant for the parsing*/
+            } else {
+              ERROR_F(
+                  "%s:%zu: Invalid number of cards for INCLUDE_NASTRAN keyword",
+                  file_name, line_count);
+            }
 
-          /* continue without calling the callback for the card*/
-          if (card.string != line.buffer) {
-            free(card.string);
-          }
+            /* continue without calling the callback for the card*/
+            if (card.string != line.buffer) {
+              free(card.string);
+            }
 
-          card_index++;
-          continue;
-        } else if (extra_string_compare(&current_keyword_name,
-                                        "INCLUDE_NASTRAN") == 0) {
-          /* Parse the first card like a normal INCLUDE*/
-          if (card_index == 0) {
-            _parse_include_file_name_card(
-                &card, &card_index, &line, line_length,
-                &current_multi_line_string, &current_multi_line_index,
-                num_include_paths_ptr, include_paths_ptr, callback, user_data,
-                &error_stack, &error_stack_size, &error_ptr, file_name,
-                line_count, root_folder_ptr);
+            card_index++;
             continue;
-          } else if (card_index == 1) {
-            /* Ignore the card it is irrelevant for the parsing*/
           } else {
-            ERROR_F(
-                "%s:%zu: Invalid number of cards for INCLUDE_NASTRAN keyword",
-                file_name, line_count);
-          }
+            char *keyword_name;
+            if (current_keyword_length < EXTRA_STRING_BUFFER_SIZE) {
+              keyword_name = current_keyword_name.buffer;
+            } else {
+              keyword_name = malloc(current_keyword_length + 1);
+              extra_string_copy_to_string(keyword_name, &current_keyword_name,
+                                          current_keyword_length);
+              keyword_name[current_keyword_length] = '\0';
+            }
 
-          /* continue without calling the callback for the card*/
-          if (card.string != line.buffer) {
-            free(card.string);
-          }
+            ERROR_F("%s:%zu: Unsupported INCLUDE keyword: \"%s\"", file_name,
+                    current_keyword_line, keyword_name);
 
-          card_index++;
-          continue;
-        } else {
-          char *keyword_name;
-          if (current_keyword_length < EXTRA_STRING_BUFFER_SIZE) {
-            keyword_name = current_keyword_name.buffer;
-          } else {
-            keyword_name = malloc(current_keyword_length + 1);
-            extra_string_copy_to_string(keyword_name, &current_keyword_name,
-                                        current_keyword_length);
-            keyword_name[current_keyword_length] = '\0';
+            if (keyword_name != current_keyword_name.buffer) {
+              free(keyword_name);
+            }
           }
-
-          ERROR_F("%s:%zu: Unsupported INCLUDE keyword: \"%s\"", file_name,
-                  current_keyword_line, keyword_name);
-
-          if (keyword_name != current_keyword_name.buffer) {
-            free(keyword_name);
+        } else {
+          if (extra_string_compare(&current_keyword_name, "INCLUDE") == 0 ||
+              extra_string_compare(&current_keyword_name, "INCLUDE_PATH") ==
+                  0 ||
+              extra_string_compare(&current_keyword_name,
+                                   "INCLUDE_PATH_RELATIVE") == 0) {
+            if (!_parse_multi_line_string(&current_multi_line_string,
+                                          &current_multi_line_index, &card,
+                                          line_length)) {
+              /* continue without calling the callback for the card*/
+              if (card.string != line.buffer) {
+                free(card.string);
+              }
+              continue;
+            }
+          } else if (extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_BINARY") == 0 ||
+                     extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_NASTRAN") == 0 ||
+                     extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_TRANSFORM") == 0 ||
+                     extra_string_compare(&current_keyword_name,
+                                          "INCLUDE_TRANSFORM_BINARY") == 0) {
+            /* Parse the first card like a normal INCLUDE*/
+            if (card_index == 0) {
+              if (!_parse_multi_line_string(&current_multi_line_string,
+                                            &current_multi_line_index, &card,
+                                            line_length)) {
+                /* continue without calling the callback for the card*/
+                if (card.string != line.buffer) {
+                  free(card.string);
+                }
+                continue;
+              }
+            }
           }
         }
       }
       /* ------- ⛅ End of Include Parsing ⛅ -------*/
 
+      if (current_multi_line_string) {
+        if (card.string != line.buffer) {
+          free(card.string);
+        }
+        card.string = current_multi_line_string;
+      }
+
       char *keyword_name;
       if (current_keyword_length < EXTRA_STRING_BUFFER_SIZE) {
         keyword_name = current_keyword_name.buffer;
       } else {
         keyword_name = malloc(current_keyword_length + 1);
         extra_string_copy_to_string(keyword_name, &current_keyword_name,
                                     current_keyword_length);
         keyword_name[current_keyword_length] = '\0';
       }
 
-      callback(keyword_name, &card, card_index, user_data);
+      callback(file_name, line_count, keyword_name, &card, card_index,
+               user_data);
 
       if (card.string != line.buffer) {
         free(card.string);
+        current_multi_line_string = NULL;
       }
       if (keyword_name != current_keyword_name.buffer) {
         free(keyword_name);
       }
+      current_multi_line_index = 0;
 
       card_index++;
     }
 
     /* ---------------------------------------- */
   }
 
@@ -601,19 +653,30 @@
       } else {
         keyword_name = malloc(current_keyword_length + 1);
         extra_string_copy_to_string(keyword_name, &current_keyword_name,
                                     current_keyword_length);
         keyword_name[current_keyword_length] = '\0';
       }
 
-      callback(keyword_name, NULL, (size_t)~0, user_data);
+      card_t card;
+      if (current_multi_line_string) {
+        card.string = current_multi_line_string;
+      } else {
+        card.string = NULL;
+      }
+
+      callback(file_name, line_count, keyword_name, card.string ? &card : NULL,
+               (size_t)~0, user_data);
 
       if (keyword_name != current_keyword_name.buffer) {
         free(keyword_name);
       }
+      if (card.string) {
+        free(card.string);
+      }
     }
   }
 
   /* Free all include paths*/
   if (!include_paths) {
     size_t i = 0;
     while (i < *num_include_paths_ptr) {
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/key.h` & `dynareadout-23.6/lib/dynareadout/src/key.h`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 typedef struct {
   char *name;       /* The name of the keyword*/
   card_t *cards;    /* An array stroing the cards*/
   size_t num_cards; /* The number of cards in the array*/
 } keyword_t;
 
 /* The type of the callback that is called in key_file_parse_with_callback*/
-typedef void (*key_file_callback)(const char *keyword_name, const card_t *card,
+typedef void (*key_file_callback)(const char *file_name, size_t line_number,
+                                  const char *keyword_name, card_t *card,
                                   size_t card_index, void *user_data);
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /* Parses a LS Dyna key file for keywords and their respective cards. Returns an
@@ -74,16 +75,16 @@
  * tells about an error if one occurred. If it gets set to a non NULL value it
  * needs to be deallocated by free.*/
 keyword_t *key_file_parse(const char *file_name, size_t *num_keywords,
                           int parse_includes, char **error_string);
 /* Same as key_file_parse, but instead of returning an array it calls an
  * callback every time a card (or empty keyword) is encountered.
  * user_data: will be given to the callback untouched.
- * include_paths and num_include_paths: this is only used for recursion and both
- * should be set to NULL*/
+ * include_paths, num_include_paths, root_folder: these are only used for
+ * recursion and should be set to NULL*/
 void key_file_parse_with_callback(const char *file_name,
                                   key_file_callback callback,
                                   int parse_includes, char **error_string,
                                   void *user_data, char ***include_paths,
                                   size_t *num_include_paths,
                                   const char *root_folder);
 /* Deallocates the data returned by key_file_parse*/
@@ -124,27 +125,36 @@
 void card_parse_next(card_t *card);
 /* Advance to the next value. Uses the value width provided here.*/
 void card_parse_next_width(card_t *card, uint8_t value_width);
 /* Returns wether the card has been completely parsed. Breaks if incorrect value
  * widths have been supplied*/
 int card_parse_done(const card_t *card);
 /* Parses the current value as an int. Uses the value width from
- * card_parse_begin.*/
+ * card_parse_begin. Note: This does not handle overflow, since the width of key
+ * file values is too small to reach the maximum of int64_t*/
 int64_t card_parse_int(const card_t *card);
-/* Parses the current value as an int. Uses the value width provided here.*/
+/* Parses the current value as an int. Uses the value width provided here. Note:
+ * This does not handle overflow, since the width of key file values is too
+ * small to reach the maximum of int64_t*/
 int64_t card_parse_int_width(const card_t *card, uint8_t value_width);
 /* Parses the current value as an float. Uses the value width from
- * card_parse_begin.*/
+ * card_parse_begin. Note: This does not handle overflow, since the width of key
+ * file values is too small to reach the maximum of float*/
 float card_parse_float32(const card_t *card);
-/* Parses the current value as an float. Uses the value width provided here.*/
+/* Parses the current value as an float. Uses the value width provided here.
+ * Note: This does not handle overflow, since the width of key file values is
+ * too small to reach the maximum of float*/
 float card_parse_float32_width(const card_t *card, uint8_t value_width);
 /* Parses the current value as an double. Uses the value width from
- * card_parse_begin.*/
+ * card_parse_begin. Note: This does not handle overflow, since the width of key
+ * file values is too small to reach the maximum of double*/
 double card_parse_float64(const card_t *card);
-/* Parses the current value as an double. Uses the value width provided here.*/
+/* Parses the current value as an double. Uses the value width provided here.
+ * Note: This does not handle overflow, since the width of key file values is
+ * too small to reach the maximum of double*/
 double card_parse_float64_width(const card_t *card, uint8_t value_width);
 /* Parses the current value as an string (which means no parsing at all).
  * Trims trailing and leading spaces. Uses the value width from
  * card_parse_begin. Return value should be deallocated by
  * free*/
 char *card_parse_string(const card_t *card);
 /* Parses the current value as an string (which means no parsing at all).
@@ -180,15 +190,15 @@
 card_parse_type card_parse_get_type_width(const card_t *card,
                                           uint8_t value_width);
 
 /* ----- Private Functions -----*/
 /* Copy the contents of the card as a string directly into dst.*/
 void _card_cpy(const card_t *card, char *dst, size_t len);
 /* Handles the parsing of multi line string for include file names. Returns
- * wether to multi line string has been completely parsed.*/
+ * wether the multi line string has been completely parsed.*/
 int _parse_multi_line_string(char **multi_line_string, size_t *multi_line_index,
                              const card_t *card, size_t line_length);
 void _parse_include_file_name_card(
     const card_t *card, size_t *card_index, const extra_string *line,
     size_t line_length, char **current_multi_line_string,
     size_t *current_multi_line_index, size_t *num_include_paths,
     char ***include_paths, key_file_callback callback, void *user_data,
```

### Comparing `dynareadout-23.5/lib/dynareadout/src/path.c` & `dynareadout-23.6/lib/dynareadout/src/path.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/path.h` & `dynareadout-23.6/lib/dynareadout/src/path.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/path_view.c` & `dynareadout-23.6/lib/dynareadout/src/path_view.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/path_view.h` & `dynareadout-23.6/lib/dynareadout/src/path_view.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/pgni.h` & `dynareadout-23.6/lib/dynareadout/src/pgni.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/profiling.c` & `dynareadout-23.6/lib/dynareadout/src/profiling.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/profiling.h` & `dynareadout-23.6/lib/dynareadout/src/profiling.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/python/conversions.hpp` & `dynareadout-23.6/lib/dynareadout/src/python/conversions.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/python/pybind11_binout.cpp` & `dynareadout-23.6/lib/dynareadout/src/python/pybind11_binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/python/pybind11_d3plot.cpp` & `dynareadout-23.6/lib/dynareadout/src/python/pybind11_d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/python/pybind11_key.cpp` & `dynareadout-23.6/lib/dynareadout/src/python/pybind11_key.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/dynareadout/src/python/pybind11_module.cpp` & `dynareadout-23.6/lib/dynareadout/src/python/pybind11_module.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/LICENSE` & `dynareadout-23.6/lib/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/attr.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/buffer_info.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/cast.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/chrono.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/complex.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/class.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/common.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/descr.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/init.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/internals.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/detail/typeid.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/eigen.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/embed.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/eval.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/functional.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/gil.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/iostream.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/numpy.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/operators.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/options.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/pybind11.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/pytypes.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/stl/filesystem.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/stl.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/lib/pybind11/include/pybind11/stl_bind.h` & `dynareadout-23.6/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/pyproject.toml` & `dynareadout-23.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynareadout"
-version = "23.05"
+version = "23.06"
 authors = [
   { name = "PucklaJ", email = "jonaas.pucher000000@gmail.com"},
 ]
 description = "Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dynareadout-23.5/setup.py` & `dynareadout-23.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 from setuptools import setup
 from setuptools.extension import Extension
 
 this_dir = os.path.dirname(os.path.abspath(__file__))
 dynareadout_dir = os.path.join('lib', 'dynareadout')
 
 compile_args = []
+link_args = []
 if os.name == "nt":
     compile_args.append("/std:c++17")
     compile_args.append("/w")
+    compile_args.append("/DTHREAD_SAFE")
 else:
     compile_args.append("-std=c++17")
     compile_args.append("-w")
+    compile_args.append("-DTHREAD_SAFE")
+    link_args.append("-lpthread")
 
 dynareadout_c = Extension(
     name='dynareadout_c',
     extra_compile_args=compile_args,
+    extra_link_args=link_args,
     include_dirs=[
         os.path.join(this_dir, 'lib', 'pybind11', 'include'),
         os.path.join(dynareadout_dir, 'src'),
         os.path.join(dynareadout_dir, 'src', 'cpp')
     ],
     sources=[
         # C Source Files
@@ -31,27 +36,29 @@
         os.path.join(dynareadout_dir, 'src', 'd3_buffer.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_data.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_part_nodes.c'),
         os.path.join(dynareadout_dir, 'src', 'd3plot_state.c'),
         os.path.join(dynareadout_dir, 'src', 'extra_string.c'),
         os.path.join(dynareadout_dir, 'src', 'key.c'),
+        os.path.join(dynareadout_dir, 'src', 'multi_file.c'),
         os.path.join(dynareadout_dir, 'src', 'path.c'),
         os.path.join(dynareadout_dir, 'src', 'path_view.c'),
+        os.path.join(dynareadout_dir, 'src', 'sync.c'),
         # C++ Source Files
         os.path.join(dynareadout_dir, 'src', 'cpp', 'binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_part.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'd3plot_state.cpp'),
         os.path.join(dynareadout_dir, 'src', 'cpp', 'key.cpp'),
         # C++ Source Files for pybind11 module
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_d3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_key.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_module.cpp'),
     ])
 
 setup(name='dynareadout',
-      version='23.05',
+      version='23.06',
       ext_modules=[dynareadout_c],
       zip_safe=False,
       include_package_data=True)
```

### Comparing `dynareadout-23.5/src/dynareadout/__init__.py` & `dynareadout-23.6/src/dynareadout/__init__.py`

 * *Files identical despite different names*

### Comparing `dynareadout-23.5/src/dynareadout.egg-info/PKG-INFO` & `dynareadout-23.6/src/dynareadout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.5
+Version: 23.6
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-23.5/src/dynareadout.egg-info/SOURCES.txt` & `dynareadout-23.6/src/dynareadout.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,25 @@
 lib/dynareadout/src/d3plot_part_nodes.c
 lib/dynareadout/src/d3plot_part_nodes.h
 lib/dynareadout/src/d3plot_state.c
 lib/dynareadout/src/extra_string.c
 lib/dynareadout/src/extra_string.h
 lib/dynareadout/src/key.c
 lib/dynareadout/src/key.h
+lib/dynareadout/src/multi_file.c
+lib/dynareadout/src/multi_file.h
 lib/dynareadout/src/path.c
 lib/dynareadout/src/path.h
 lib/dynareadout/src/path_view.c
 lib/dynareadout/src/path_view.h
 lib/dynareadout/src/pgni.h
 lib/dynareadout/src/profiling.c
 lib/dynareadout/src/profiling.h
+lib/dynareadout/src/sync.c
+lib/dynareadout/src/sync.h
 lib/dynareadout/src/cpp/array.hpp
 lib/dynareadout/src/cpp/binout.cpp
 lib/dynareadout/src/cpp/binout.hpp
 lib/dynareadout/src/cpp/d3plot.cpp
 lib/dynareadout/src/cpp/d3plot.hpp
 lib/dynareadout/src/cpp/d3plot_part.cpp
 lib/dynareadout/src/cpp/d3plot_part.hpp
```

