# Comparing `tmp/trame-vtk-2.5.1.tar.gz` & `tmp/trame-vtk-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.5.1.tar", last modified: Fri Jun 23 21:12:15 2023, max compression
+gzip compressed data, was "trame-vtk-2.5.2.tar", last modified: Mon Jun 26 20:59:56 2023, max compression
```

## Comparing `trame-vtk-2.5.1.tar` & `trame-vtk-2.5.2.tar`

### file list

```diff
@@ -1,79 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13038 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1693943 2023-06-23 21:12:13.000000 trame-vtk-2.5.1/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5356 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    23952 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     7518 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12646 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/cache.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/export.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32816 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13038 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2338 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.666517 trame-vtk-2.5.2/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-06-26 20:59:56.666517 trame-vtk-2.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12192 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-26 20:59:56.666517 trame-vtk-2.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1693968 2023-06-26 20:59:52.000000 trame-vtk-2.5.2/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.658517 trame-vtk-2.5.2/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.658517 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    23952 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.658517 trame-vtk-2.5.2/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.658517 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.662517 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/cache.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.662517 trame-vtk-2.5.2/trame_vtk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   970199 2023-06-26 20:59:52.000000 trame-vtk-2.5.2/trame_vtk/tools/static_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.666517 trame-vtk-2.5.2/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.666517 trame-vtk-2.5.2/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33036 2023-06-26 20:59:50.000000 trame-vtk-2.5.2/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:59:56.654517 trame-vtk-2.5.2/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-06-26 20:59:56.000000 trame-vtk-2.5.2/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-06-26 20:59:56.000000 trame-vtk-2.5.2/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 20:59:56.000000 trame-vtk-2.5.2/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 20:59:56.000000 trame-vtk-2.5.2/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-26 20:59:56.000000 trame-vtk-2.5.2/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.5.1/LICENSE` & `trame-vtk-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/PKG-INFO` & `trame-vtk-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.1
+Version: 2.5.2
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -74,16 +74,15 @@
 Development: Grabbing client before push to PyPI
 -----------------------------------------------------------
 
 To update the client code, run the following command line while updating the targeted version
 
 .. code-block:: console
 
-    mkdir -p ./trame_vtk/modules/common/serve
-    curl https://unpkg.com/vue-vtk-js@3.1.5 -Lo ./trame_vtk/modules/common/serve/trame-vtk.js
+    bash .fetch_externals.sh
 
 
 Trame widgets
 -----------------------------------------------------------
 
 VtkRemoteView
 -----------------------------------------------------------
```

### Comparing `trame-vtk-2.5.1/README.rst` & `trame-vtk-2.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,15 @@
 Development: Grabbing client before push to PyPI
 -----------------------------------------------------------
 
 To update the client code, run the following command line while updating the targeted version
 
 .. code-block:: console
 
-    mkdir -p ./trame_vtk/modules/common/serve
-    curl https://unpkg.com/vue-vtk-js@3.1.5 -Lo ./trame_vtk/modules/common/serve/trame-vtk.js
+    bash .fetch_externals.sh
 
 
 Trame widgets
 -----------------------------------------------------------
 
 VtkRemoteView
 -----------------------------------------------------------
```

### Comparing `trame-vtk-2.5.1/setup.cfg` & `trame-vtk-2.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.5.1
+version = 2.5.2
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.5.1/trame_vtk/LICENSE` & `trame-vtk-2.5.2/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.5.2/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8240,16 +8240,17 @@
             }
             return e.opaqueFlag
         }, t.usingLogScale = function() {
             return !1
         }, t.getNumberOfAvailableColors = function() {
             return e.table.length / 4
         }, t.linearIndexLookup = function(n, r) {
-            var a = 0;
-            return n < r.range[0] ? a = r.maxIndex + g1 + 1.5 : n > r.range[1] ? a = r.maxIndex + d1 + 1.5 : (a = (n + r.shift) * r.scale, a = a < r.maxIndex ? a : r.maxIndex), Math.floor(a)
+            var a = 0,
+                i = Number(n);
+            return i < r.range[0] ? a = r.maxIndex + g1 + 1.5 : i > r.range[1] ? a = r.maxIndex + d1 + 1.5 : (a = (i + r.shift) * r.scale, a = a < r.maxIndex ? a : r.maxIndex), Math.floor(a)
         }, t.linearLookup = function(n, r, a) {
             var i = 0;
             qi(n) ? i = Math.floor(a.maxIndex + 1.5 + D0) : i = t.linearIndexLookup(n, a);
             var o = 4 * i;
             return r.slice(o, o + 4)
         }, t.indexedLookupFunction = function(n, r, a) {
             var i = t.getAnnotatedValueIndexInternal(n);
@@ -8637,16 +8638,16 @@
             var a = e.lookupTable.getRange(),
                 i = e.lookupTable.usingLogScale();
             i && Hn.getLogRange(a, a);
             var o = e.lookupTable.getAlpha();
             if (e.colorMapColors = null, e.colorTextureMap == null || t.getMTime() > e.colorTextureMap.getMTime() || e.lookupTable.getMTime() > e.colorTextureMap.getMTime() || e.lookupTable.getAlpha() !== r) {
                 e.lookupTable.setAlpha(r), e.colorTextureMap = null, e.lookupTable.build();
                 var s = e.lookupTable.getNumberOfAvailableColors();
-                s > 4094 && (s = 4094), s += 2;
-                for (var c = (a[1] - a[0]) / (s - 1 - 2), u = new Float64Array(s * 2), f = 0; f < s; ++f) u[f] = a[0] + f * c - c, i && (u[f] = Math.pow(10, u[f]));
+                s > 4094 && (s = 4094), s < 64 && (s = 64), s += 2;
+                for (var c = (a[1] - a[0]) / (s - 2), u = new Float64Array(s * 2), f = 0; f < s; ++f) u[f] = a[0] + f * c - c / 2, i && (u[f] = Math.pow(10, u[f]));
                 for (var l = 0; l < s; ++l) u[l + s] = NaN;
                 e.colorTextureMap = w0.newInstance(), e.colorTextureMap.setExtent(0, s - 1, 0, 1, 0, 0);
                 var p = de.newInstance({
                     numberOfComponents: 1,
                     values: u
                 });
                 e.colorTextureMap.getPointData().setScalars(e.lookupTable.mapScalars(p, e.colorMode, 0)), e.lookupTable.setAlpha(o)
```

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.5.2/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/export.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/export.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.5.2/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.5.2/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.1/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.5.2/trame_vtk/widgets/vtk/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,14 +744,17 @@
         self.server.js_call(
             self.__ref,
             "captureImage",
             format,
             opts,
         )
 
+    def release_resources(self):
+        self.__view = None
+
 
 class VtkShareDataset(HtmlElement):
     def __init__(self, children=None, **kwargs):
         super().__init__("vtk-share-dataset", children, **kwargs)
         self._attr_names += ["port", "name"]
 
 
@@ -945,14 +948,19 @@
         self.server.js_call(
             self.__ref,
             "captureImage",
             format,
             opts,
         )
 
+    def release_resources(self):
+        self._server.controller.on_server_ready.discard(self.update)
+        self.__view = None
+        self._widgets = None
+
 
 class VtkView(HtmlElement):
     def __init__(self, children=None, ref="view", **kwargs):
         super().__init__("vtk-view", children, **kwargs)
         self._ref = ref
         self._attributes["ref"] = f'ref="{ref}"'
         self._attr_names += [
```

### Comparing `trame-vtk-2.5.1/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.5.2/trame_vtk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.1
+Version: 2.5.2
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -74,16 +74,15 @@
 Development: Grabbing client before push to PyPI
 -----------------------------------------------------------
 
 To update the client code, run the following command line while updating the targeted version
 
 .. code-block:: console
 
-    mkdir -p ./trame_vtk/modules/common/serve
-    curl https://unpkg.com/vue-vtk-js@3.1.5 -Lo ./trame_vtk/modules/common/serve/trame-vtk.js
+    bash .fetch_externals.sh
 
 
 Trame widgets
 -----------------------------------------------------------
 
 VtkRemoteView
 -----------------------------------------------------------
```

### Comparing `trame-vtk-2.5.1/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.5.2/trame_vtk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 README.rst
 setup.cfg
 setup.py
 trame/__init__.py
 trame/modules/__init__.py
 trame/modules/paraview.py
 trame/modules/vtk.py
+trame/tools/__init__.py
+trame/tools/vtksz2html.py
 trame/widgets/__init__.py
 trame/widgets/paraview.py
 trame/widgets/vtk.py
 trame_vtk/LICENSE
 trame_vtk/__init__.py
 trame_vtk.egg-info/PKG-INFO
 trame_vtk.egg-info/SOURCES.txt
@@ -53,10 +55,13 @@
 trame_vtk/modules/vtk/serializers/registry.py
 trame_vtk/modules/vtk/serializers/render_windows.py
 trame_vtk/modules/vtk/serializers/serialize.py
 trame_vtk/modules/vtk/serializers/synchronization_context.py
 trame_vtk/modules/vtk/serializers/textures.py
 trame_vtk/modules/vtk/serializers/utils.py
 trame_vtk/modules/vtk/serializers/widgets.py
+trame_vtk/tools/__init__.py
+trame_vtk/tools/static_viewer.html
+trame_vtk/tools/vtksz2html.py
 trame_vtk/widgets/__init__.py
 trame_vtk/widgets/vtk/__init__.py
 trame_vtk/widgets/vtk/common.py
```

