# Comparing `tmp/chaco-5.1.1.tar.gz` & `tmp/chaco-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaco-5.1.1.tar", last modified: Tue Jan 24 13:56:18 2023, max compression
+gzip compressed data, was "chaco-6.0.0.tar", last modified: Mon Jun 26 14:00:38 2023, max compression
```

## Comparing `chaco-5.1.1.tar` & `chaco-6.0.0.tar`

### file list

```diff
@@ -1,520 +1,489 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.536709 chaco-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-01-24 13:55:55.000000 chaco-5.1.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-01-24 13:55:55.000000 chaco-5.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-24 13:55:55.000000 chaco-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-01-24 13:56:18.536709 chaco-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-01-24 13:55:55.000000 chaco-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.500709 chaco-5.1.1/chaco/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   394078 2023-01-24 13:56:16.000000 chaco-5.1.1/chaco/_cython_speedups.c
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/_cython_speedups.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/_isnan.h
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/_speedups_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_data_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/abstract_plot_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/array_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/array_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31402 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/axis_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_1d_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_1d_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_2d_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_candle_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_contour_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_data_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_plot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/base_xy_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/candle_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/chaco_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/cmap_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/color_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/color_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/color_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/colormap_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/colormapped_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/colormapped_selection_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/contour_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/contour_poly_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/data_frame_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/data_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/data_range_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/data_range_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/data_view.py
--rw-r--r--   0 runner    (1001) docker     (123)   490330 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/default_colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/default_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/discrete_color_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.500709 chaco-5.1.1/chaco/downsample/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/downsample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   806527 2023-01-24 13:56:17.000000 chaco-5.1.1/chaco/downsample/_lttb.c
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/downsample/_lttb.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/downsample/lttb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.500709 chaco-5.1.1/chaco/downsample/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/downsample/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/downsample/tests/test_lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/errorbar_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/example_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.500709 chaco-5.1.1/chaco/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/_etsdemo_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.504709 chaco-5.1.1/chaco/examples/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.504709 chaco-5.1.1/chaco/examples/demo/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/asynchronous_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/cmap_variable_sized_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/data_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/advanced/scalar_image_function_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/examples/demo/basic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/bar_plot_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/bar_plot_stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/bounded_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/capitol.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    70993 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cmap_image_aspect_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cmap_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cmap_image_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cmap_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/cmap_segment_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/contour_cmap_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/contour_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/discrete_cmap_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/discrete_cmap_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/draw_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/grid_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/grid_container_aspect_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/hittest_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/horizon_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/image_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/image_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/image_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/inset_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/line_drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/line_plot1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/line_plot_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/log_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/minard_napoleon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/minor_ticks_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/nans_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/pandas_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/polygon_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/polygon_plot_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_custom_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_inspector2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_rect_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scatter_variable_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/scrollbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/segment_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/tabbed_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/basic/zoomable_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/bigdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/chaco_trait_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/coordinate_line_overlay_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/cursor_tool_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/data_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/data_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/edit_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/examples/demo/financial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/financial/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/financial/stock_prices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/functionplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/hyetograph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/image_plot_origin_and_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/multi_line_plot_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/nonlinear_color_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/qt_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/range_selection_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/scales_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/simple_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/simple_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/stacked_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/status_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/toolbar_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/two_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/vanderwaals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/vertical_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/demo/xray_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/examples/tests/test_etsdemo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/filled_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/function_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/function_image_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/grid_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/grid_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/horizon_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/image_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/jitterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/label_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/lasso_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/layers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/layers/status_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/layers/svg_range_selection_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/line_scatterplot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/linear_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/multi_array_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/multi_line_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/overlays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/aligned_container_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/colormapped_selection_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/container_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/coordinate_line_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)    20834 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/data_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/lasso_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/overlays/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/overlays/layers/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/data/Dialog-error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/data/Dialog-warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/data/range_selection.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/status_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/layers/svg_range_selection_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/plot_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/scatter_inspector_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/simple_inspector_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.512709 chaco-5.1.1/chaco/overlays/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/tests/test_data_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/text_box_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/text_grid_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/overlays/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/pdf_graphics_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    59225 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_canvas_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_graphics_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plot_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.516709 chaco-5.1.1/chaco/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/candle_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/cmap_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/color_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/colormapped_scatterplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.516709 chaco-5.1.1/chaco/plots/contour/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57592 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/cntr.c
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/contour_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/contour_poly_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.516709 chaco-5.1.1/chaco/plots/contour/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/contour/tests/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/errorbar_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/filled_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/horizon_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/jitterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/line_scatterplot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/multi_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/polar_line_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/polygon_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/quiverplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    21400 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/scatterplot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/segment_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.516709 chaco-5.1.1/chaco/plots/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_cmap_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_colormapped_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_errorbarplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_image_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_jitterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_line_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_scatterplot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_scatterplot_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_segment_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_text_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/tests/test_text_plot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/text_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plots/text_plot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/plotscrollbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/point_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/polar_line_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/polar_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/polygon_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/quiverplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.516709 chaco-5.1.1/chaco/scales/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/safetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/scales.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.520709 chaco-5.1.1/chaco/scales/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/tests/test_scales.py
--rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/tests/test_time_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/tests/test_time_scale_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales/time_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scales_tick_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scaly_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scatter_inspector_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/scatterplot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/segment_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/selectable_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/speedups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/svg_graphics_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.520709 chaco-5.1.1/chaco/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.472709 chaco-5.1.1/chaco/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.520709 chaco-5.1.1/chaco/tests/data/PngSuite/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/data/PngSuite/basi6a08.png
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/data/PngSuite/basn2c08.png
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_2d_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_array_or_none.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_array_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_arraydatasource.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_chaco_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_colormapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_data_frame_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_data_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_datarange_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_datarange_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_default_colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_discrete_colormapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_function_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_grid_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_grid_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_highlight_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_hittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_image_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_instantiation_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_linearmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_logmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_multi_array_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_plot_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_plotcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_speedups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tests/test_ticks.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/text_box_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/text_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/text_plot_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/ticks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/toolbar_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.524709 chaco-5.1.1/chaco/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/better_selecting_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/better_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/cursor_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/data_label_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/dataprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/drag_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/draw_points_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/highlight_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/image_inspector_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/lasso_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/legend_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/legend_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/line_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/line_segment_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/move_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/pan_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/pan_tool2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/point_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/range_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/range_selection_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/range_selection_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/rect_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/rectangular_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/regression_lasso.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/save_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/scatter_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/select_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/simple_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.524709 chaco-5.1.1/chaco/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_better_zoom_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_cursor_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_data_label_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_image_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_pan_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_range_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_range_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_rectangular_selection_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tests/test_scatter_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tool_history_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tool_states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/chaco/tools/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/chaco/tools/toolbars/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/application-vnd-ms-excel.png
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/document-save.png
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/edit-copy.png
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/zoom-fit-height.png
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/zoom-fit-width.png
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/images/zoom-original.png
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/plot_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/toolbars/toolbar_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tracking_pan_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/tracking_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4841 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/traits_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tools/zoom_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/transform_color_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/chaco/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/ui/axis_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-24 13:55:55.000000 chaco-5.1.1/chaco/ui/plot_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.500709 chaco-5.1.1/chaco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 13:56:17.000000 chaco-5.1.1/chaco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 13:56:18.000000 chaco-5.1.1/chaco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.476709 chaco-5.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/examples/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/examples/demo/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21194 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/advanced/javascript_hover_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/advanced/spec_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/advanced/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/aspect_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/examples/demo/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/axis_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/cliptest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/data_source_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/mp_move_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/mp_viewport_pan_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/mptools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/plot_clone_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/canvas/transient_plot_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/examples/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    75794 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/data/sample.wav
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/domain_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/financial_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/financial_plot_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/multi_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/multiaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/multiaxis_using_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/noninteractive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.528709 chaco-5.1.1/examples/demo/updating_plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/updating_plot1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/updating_plot2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/updating_plot3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/updating_plot4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/updating_plot/updating_plot5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/world_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.532709 chaco-5.1.1/examples/demo/zoomed_plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/zoomed_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/zoomed_plot/grid_plot_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/zoomed_plot/wav_to_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/zoomed_plot/zoom_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/demo/zoomed_plot/zoom_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.532709 chaco-5.1.1/examples/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.536709 chaco-5.1.1/examples/tutorials/scipy2008/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/connected_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/connected_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/connected_single_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/connected_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/container_nospace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/container_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay_dataspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay_movetool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_tool_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/custom_tool_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/data_chooser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/first_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/overlapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/ploteditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/tool_chooser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/traits_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/scipy2008/traits_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial1.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial10.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial10b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial11.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial2_ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial3.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial4.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial5.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial6.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial8.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial9.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorial9b.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/tutorials/tutorials.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.536709 chaco-5.1.1/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/grid_plot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/h_plot_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/h_plot_container_add_multiple_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/h_plot_container_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/overlay_container_inset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 13:56:18.536709 chaco-5.1.1/examples/user_guide/plot_types/
--rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/plot_types/create_plot_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/plot_types/plot_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-01-24 13:55:55.000000 chaco-5.1.1/examples/user_guide/power_function_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-24 13:55:55.000000 chaco-5.1.1/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-24 13:55:55.000000 chaco-5.1.1/image_LICENSE_PngSuite.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-24 13:55:55.000000 chaco-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 13:56:18.536709 chaco-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-01-24 13:55:55.000000 chaco-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.363243 chaco-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    27706 2023-06-26 14:00:18.000000 chaco-6.0.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-26 14:00:18.000000 chaco-6.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 14:00:18.000000 chaco-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 14:00:38.363243 chaco-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-26 14:00:18.000000 chaco-6.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.315242 chaco-6.0.0/chaco/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396362 2023-06-26 14:00:37.000000 chaco-6.0.0/chaco/_cython_speedups.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/_cython_speedups.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/_isnan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/_speedups_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_data_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/abstract_plot_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/array_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/array_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/axis_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_1d_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_1d_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_2d_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_candle_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_contour_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_data_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_plot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/base_xy_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/chaco_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/color_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/color_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/colormap_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/data_frame_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/data_range_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/data_range_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/data_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)   490330 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/default_colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/default_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/discrete_color_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.319242 chaco-6.0.0/chaco/downsample/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/downsample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   806948 2023-06-26 14:00:37.000000 chaco-6.0.0/chaco/downsample/_lttb.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/downsample/_lttb.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/downsample/lttb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.319242 chaco-6.0.0/chaco/downsample/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/downsample/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/downsample/tests/test_lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/example_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.319242 chaco-6.0.0/chaco/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/_etsdemo_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.323243 chaco-6.0.0/chaco/examples/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.323243 chaco-6.0.0/chaco/examples/demo/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/asynchronous_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/cmap_variable_sized_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/data_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/advanced/scalar_image_function_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/examples/demo/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/bar_plot_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/bar_plot_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/bounded_grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/capitol.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    70993 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cmap_image_aspect_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cmap_image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cmap_image_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cmap_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/cmap_segment_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/contour_cmap_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/contour_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/discrete_cmap_image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/discrete_cmap_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/draw_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/grid_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/grid_container_aspect_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/hittest_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/horizon_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/image_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/image_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/image_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/inset_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/line_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/line_plot1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/line_plot_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/log_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/minard_napoleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/minor_ticks_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/nans_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/pandas_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/polygon_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/polygon_plot_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_custom_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_inspector2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_rect_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scatter_variable_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/scrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/segment_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/tabbed_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/basic/zoomable_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/bigdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/chaco_trait_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/coordinate_line_overlay_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/cursor_tool_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/data_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/data_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/edit_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/examples/demo/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/financial/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/financial/stock_prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/functionplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/hyetograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/image_plot_origin_and_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/multi_line_plot_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/nonlinear_color_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/qt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/range_selection_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/scales_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/simple_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/simple_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/stacked_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/status_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/toolbar_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/two_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/vanderwaals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/vertical_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/demo/xray_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/examples/tests/test_etsdemo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/function_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/function_image_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/grid_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/grid_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/label_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/layers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/linear_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/multi_array_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/overlays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/aligned_container_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/colormapped_selection_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/container_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/coordinate_line_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20834 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/data_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/lasso_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.331243 chaco-6.0.0/chaco/overlays/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.335243 chaco-6.0.0/chaco/overlays/layers/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/data/Dialog-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/data/Dialog-warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/data/range_selection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/status_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/layers/svg_range_selection_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/plot_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/scatter_inspector_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/simple_inspector_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.335243 chaco-6.0.0/chaco/overlays/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/tests/test_data_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/text_box_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/text_grid_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/overlays/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/pdf_graphics_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59225 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_canvas_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plot_graphics_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.335243 chaco-6.0.0/chaco/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/candle_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/cmap_image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/color_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/colormapped_scatterplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.335243 chaco-6.0.0/chaco/plots/contour/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57592 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/cntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/contour_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/contour_poly_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.339243 chaco-6.0.0/chaco/plots/contour/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/contour/tests/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/errorbar_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/filled_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/horizon_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/jitterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/line_scatterplot_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/multi_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/polar_line_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/polygon_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/quiverplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21400 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/scatterplot_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/segment_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.339243 chaco-6.0.0/chaco/plots/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_cmap_image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_colormapped_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_errorbarplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_image_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_jitterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_line_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_scatterplot_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_scatterplot_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_segment_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_text_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/tests/test_text_plot_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/text_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plots/text_plot_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/plotscrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/point_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/polar_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.339243 chaco-6.0.0/chaco/scales/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/safetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/scales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.339243 chaco-6.0.0/chaco/scales/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/tests/test_scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/tests/test_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/tests/test_time_scale_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales/time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scales_tick_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/scaly_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/selectable_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/speedups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/svg_graphics_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.343243 chaco-6.0.0/chaco/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.303242 chaco-6.0.0/chaco/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.343243 chaco-6.0.0/chaco/tests/data/PngSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/data/PngSuite/basi6a08.png
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/data/PngSuite/basn2c08.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_2d_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_array_or_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_array_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_arraydatasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_chaco_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_data_frame_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_data_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_datarange_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_datarange_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_default_colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_discrete_colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_function_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_grid_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_grid_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_highlight_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_hittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_image_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_instantiation_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_linearmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_logmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_multi_array_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_plot_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_plotcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_speedups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tests/test_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/ticks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/toolbar_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.351243 chaco-6.0.0/chaco/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/better_selecting_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/better_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/cursor_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/data_label_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/dataprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/drag_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/draw_points_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/highlight_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/image_inspector_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/lasso_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/legend_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/legend_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/line_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/line_segment_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/move_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/pan_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/pan_tool2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/point_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/range_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/range_selection_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/range_selection_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/rect_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/rectangular_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/regression_lasso.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/save_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/scatter_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/select_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/simple_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.351243 chaco-6.0.0/chaco/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_better_zoom_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_cursor_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_data_label_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_image_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_pan_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_range_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_range_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_rectangular_selection_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tests/test_scatter_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tool_history_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tool_states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.351243 chaco-6.0.0/chaco/tools/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.351243 chaco-6.0.0/chaco/tools/toolbars/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/application-vnd-ms-excel.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/document-save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/edit-copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/zoom-fit-height.png
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/zoom-fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/images/zoom-original.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/plot_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/toolbars/toolbar_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tracking_pan_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/tracking_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4841 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/traits_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/tools/zoom_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/transform_color_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.351243 chaco-6.0.0/chaco/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/ui/axis_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 14:00:18.000000 chaco-6.0.0/chaco/ui/plot_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.315242 chaco-6.0.0/chaco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:00:37.000000 chaco-6.0.0/chaco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 14:00:38.000000 chaco-6.0.0/chaco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.307242 chaco-6.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21191 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/advanced/javascript_hover_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/advanced/spec_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/advanced/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/aspect_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/axis_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/cliptest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/data_source_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/mp_move_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/mp_viewport_pan_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/mptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/plot_clone_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/canvas/transient_plot_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    75794 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/data/sample.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/domain_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/financial_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/financial_plot_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/multi_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/multiaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/multiaxis_using_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/noninteractive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/updating_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/updating_plot1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/updating_plot2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/updating_plot3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/updating_plot4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/updating_plot/updating_plot5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/world_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.355243 chaco-6.0.0/examples/demo/zoomed_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/zoomed_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/zoomed_plot/grid_plot_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/zoomed_plot/wav_to_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/zoomed_plot/zoom_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/demo/zoomed_plot/zoom_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.359243 chaco-6.0.0/examples/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.363243 chaco-6.0.0/examples/tutorials/scipy2008/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/connected_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/connected_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/connected_single_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/connected_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/container_nospace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/container_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay_dataspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay_movetool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_tool_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/custom_tool_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/data_chooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/first_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/ploteditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/tool_chooser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/traits_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/scipy2008/traits_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial10b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial2_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial9.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorial9b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/tutorials/tutorials.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.363243 chaco-6.0.0/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/grid_plot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/h_plot_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/h_plot_container_add_multiple_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/h_plot_container_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/overlay_container_inset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:00:38.363243 chaco-6.0.0/examples/user_guide/plot_types/
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/plot_types/create_plot_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/plot_types/plot_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-26 14:00:18.000000 chaco-6.0.0/examples/user_guide/power_function_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-26 14:00:18.000000 chaco-6.0.0/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-26 14:00:18.000000 chaco-6.0.0/image_LICENSE_PngSuite.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-26 14:00:18.000000 chaco-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:00:38.363243 chaco-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-06-26 14:00:18.000000 chaco-6.0.0/setup.py
```

### Comparing `chaco-5.1.1/CHANGES.txt` & `chaco-6.0.0/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,52 @@
+
 Chaco CHANGELOG
 ===============
 
+Release 6.0.0
+-------------
+
+This is a major release which includes support for Python 3.11, and more recent
+versions of PySide6, TraitsUI and Enable.  There are no substantial new
+features, but some backwards compatibility support has been removed as
+advertised in deprecation warnings.  Substantial work has been done to ensure
+that demos and examples are working and up-to-date where possible.
+
+As usual, this release includes a number of bugfixes and minor improvements.
+
+Thanks to all who contributed to the release:
+
+* Chengyu Liu
+* Didrik Pinte
+* Corran Webster
+
+Enhancements
+
+* Remove deprecated stub files (#903)
+* Replace "modern" font with "san-serif" (#901)
+
+Fixes
+
+* Update textPlot when aesthetics change (#905)
+* Fix Wx Bitmap usage (#904)
+* Fix imports of `marker_trait` (#902)
+* Fire `updated` trait and Ranges when data sources are emptied (#900)
+* Fix LegendHighlighter hit detection (#897)
+* Properly handle NaN in BarPlots (#895)
+* Fix polar line renderer (#883)
+
+Documentation/Examples
+
+* Fix imports of ufuncs in Scalar Image Function Inspector example (#894)
+* Various small fixes for examples (#859, #864, #870, #871, #873, #874, #880, #882, #884, #885, #892, #893)
+
+Build/CI
+
+* Update testing infrastructure, including Python 3.11 (#891, #898)
+
 Release 5.1.1
 -------------
 
 This is a small bugfix release centered around Python 3.8+ support.
 
 Thanks to all who contributed to the release:
 
@@ -19,14 +61,15 @@
 * Prevent exceptions when plot size too small (#848)
 
 Build/CI
 
 * Get CI running on Python 3.8 (#851)
 * Fix CI for changes to GitHub infrastructure (#849)
 
+
 Release 5.1.0
 -------------
 
 This is an incremental release which modernises the usage of Traits in a
 number of places, and fixes a number of bugs.
 
 Thanks to all who contributed to the release:
```

### Comparing `chaco-5.1.1/LICENSE.txt` & `chaco-6.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/PKG-INFO` & `chaco-6.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaco
-Version: 5.1.1
+Version: 6.0.0
 Summary: interactive 2-dimensional plotting
 Home-page: http://docs.enthought.com/chaco
 Download-URL: https://github.com/enthought/chaco
 Author: Peter Wang, et. al.
 Author-email: info@enthought.com
 Maintainer: ETS Developers
 Maintainer-email: enthought-dev@enthought.com
@@ -27,14 +27,21 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: tests
+Provides-Extra: pyside2
+Provides-Extra: pyside6
+Provides-Extra: pyqt5
+Provides-Extra: pyqt6
+Provides-Extra: wx
+Provides-Extra: null
 License-File: LICENSE.txt
 
 =========================================
 chaco: interactive 2-dimensional plotting
 =========================================
 
 http://www.github.com/enthought/chaco
```

### Comparing `chaco-5.1.1/README.rst` & `chaco-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/_cython_speedups.c` & `chaco-6.0.0/chaco/_cython_speedups.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "chaco/_isnan.h"
         ],
         "include_dirs": [
             "chaco",
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "chaco._cython_speedups",
         "sources": [
             "chaco/_cython_speedups.pyx"
         ]
     },
     "module_name": "chaco._cython_speedups"
@@ -29,16 +29,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -98,16 +98,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -223,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -262,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1044,195 +1048,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1259,42 +1263,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1626,22 +1630,30 @@
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -4766,15 +4778,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_blue_lut);
   __Pyx_XDECREF((PyObject *)__pyx_v_i8mask);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4783,29 +4795,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4816,15 +4828,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4833,29 +4845,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4866,15 +4878,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4883,29 +4895,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4916,15 +4928,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4933,29 +4945,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4966,15 +4978,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4983,29 +4995,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5016,212 +5028,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5237,15 +5249,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5253,84 +5265,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5345,15 +5357,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5369,15 +5381,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5385,84 +5397,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5477,15 +5489,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5501,15 +5513,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5517,84 +5529,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5609,176 +5621,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5890,15 +5902,15 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_uint8, __pyx_k_uint8, sizeof(__pyx_k_uint8), 0, 0, 1, 1},
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 91, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -5925,33 +5937,33 @@
   __pyx_slice__2 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__2)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__2);
   __Pyx_GIVEREF(__pyx_slice__2);
   __pyx_tuple__3 = PyTuple_Pack(2, __pyx_slice__2, __pyx_int_0); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "chaco/_cython_speedups.pyx":35
  * @cython.boundscheck(False)
  * @cython.cdivision(True)
  * def map_colors(             # <<<<<<<<<<<<<<
@@ -6050,55 +6062,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6386,15 +6382,15 @@
  * #
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8021,84 +8017,102 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-    #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8808,15 +8822,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9080,15 +9094,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `chaco-5.1.1/chaco/_cython_speedups.pyx` & `chaco-6.0.0/chaco/_cython_speedups.pyx`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/_speedups_fallback.py` & `chaco-6.0.0/chaco/_speedups_fallback.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/_version.py` & `chaco-6.0.0/chaco/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Thanks for using Enthought open source!
 
 # THIS FILE IS GENERATED FROM SETUP.PY
 
 #: The full version of the package, including a development suffix
 #: for unreleased versions of the package.
-version = '5.1.1'
+version = '6.0.0'
 
 #: The full version of the package, same as 'version'
 #: Kept for backward compatibility
 full_version = version
 
 #: The Git revision from which this release was made.
 git_revision = 'Unknown'
```

### Comparing `chaco-5.1.1/chaco/abstract_colormap.py` & `chaco-6.0.0/chaco/abstract_colormap.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_controller.py` & `chaco-6.0.0/chaco/abstract_controller.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_data_range.py` & `chaco-6.0.0/chaco/abstract_data_range.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_data_source.py` & `chaco-6.0.0/chaco/abstract_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_mapper.py` & `chaco-6.0.0/chaco/abstract_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_overlay.py` & `chaco-6.0.0/chaco/abstract_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_plot_data.py` & `chaco-6.0.0/chaco/abstract_plot_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/abstract_plot_renderer.py` & `chaco-6.0.0/chaco/abstract_plot_renderer.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/api.py` & `chaco-6.0.0/chaco/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -494,15 +494,15 @@
     RdYlBu,
     RdYlGn,
     Reds,
     Spectral,
     YlGn,
     YlGnBu,
     YlOrBr,
-    YlOrRd,  
+    YlOrRd,
     gist_earth,
     gist_gray,
     gist_heat,
     gist_ncar,
     gist_rainbow,
     gist_stern,
     gist_yarg,
@@ -523,7 +523,24 @@
     Pastel1,
     Pastel2,
     Set1,
     Set2,
     Set3,
 )
 from .default_colors import cbrewer, palette11, palette14, PALETTES
+
+
+def __getattr__(name):
+    """Backward compatibility lazy imports.
+
+    These imports warn about backwards incompatible changes.
+    """
+    if name in {'marker_trait'}:
+        from warnings import warn
+        import enable.api
+        warn(
+            f"Please import {name} from enable.api instead of chaco.api.",
+            DeprecationWarning,
+        )
+        return getattr(enable.api, name)
+
+    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
```

### Comparing `chaco-5.1.1/chaco/array_data_source.py` & `chaco-6.0.0/chaco/array_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/array_plot_data.py` & `chaco-6.0.0/chaco/array_plot_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/axis.py` & `chaco-6.0.0/chaco/axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     #: Keep an origin for plots that aren't attached to a component
     origin = Enum("bottom left", "top left", "bottom right", "top right")
 
     #: The text of the axis title.
     title = Str()  # May want to add PlotLabel option
 
     #: The font of the title.
-    title_font = KivaFont("modern 12")
+    title_font = KivaFont("sans-serif 12")
 
     #: The spacing between the axis line and the title
     title_spacing = Union(Constant("auto"), Float)
 
     #: The color of the title.
     title_color = ColorTrait("black")
 
@@ -101,15 +101,15 @@
     #: The thickness (in pixels) of each tick.
     tick_weight = Float(1.0)
 
     #: The color of the ticks.
     tick_color = ColorTrait("black")
 
     #: The font of the tick labels.
-    tick_label_font = KivaFont("modern 10")
+    tick_label_font = KivaFont("sans-serif 10")
 
     #: The color of the tick labels.
     tick_label_color = ColorTrait("black")
 
     #: The rotation of the tick labels.
     tick_label_rotate_angle = Float(0)
```

### Comparing `chaco-5.1.1/chaco/axis_view.py` & `chaco-6.0.0/chaco/axis_view.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base.py` & `chaco-6.0.0/chaco/base.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_1d_mapper.py` & `chaco-6.0.0/chaco/base_1d_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_1d_plot.py` & `chaco-6.0.0/chaco/base_1d_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_2d_plot.py` & `chaco-6.0.0/chaco/base_2d_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_candle_plot.py` & `chaco-6.0.0/chaco/base_candle_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_contour_plot.py` & `chaco-6.0.0/chaco/base_contour_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_data_range.py` & `chaco-6.0.0/chaco/base_data_range.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_plot_container.py` & `chaco-6.0.0/chaco/base_plot_container.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/base_xy_plot.py` & `chaco-6.0.0/chaco/base_xy_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/chaco_traits.py` & `chaco-6.0.0/chaco/chaco_traits.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/cmap_image_plot.py` & `chaco-6.0.0/chaco/layers/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 import warnings
 
-from chaco.plots.cmap_image_plot import CMapImagePlot  # noqa: F401
+from chaco.overlays.api import ErrorLayer, StatusLayer, WarningLayer
 
 warnings.warn(
-    "Importing CMapImagePlot from this module is deprecated. Please use "
-    "chaco.api or chaco.plots.api instead. This module will be removed in the "
-    "next major release.",
+    "Importing from chaco.layers.api is deprecated, please import from "
+    "chaco.api or chaco.overlays.api going forward as chaco/layers will be "
+    "removed in a future release.",
     DeprecationWarning,
     stacklevel=2,
 )
```

### Comparing `chaco-5.1.1/chaco/color_mapper.py` & `chaco-6.0.0/chaco/color_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/color_spaces.py` & `chaco-6.0.0/chaco/color_spaces.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/colormap_generators.py` & `chaco-6.0.0/chaco/colormap_generators.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/contour_line_plot.py` & `chaco-6.0.0/chaco/ui/plot_window.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-import warnings
+# Enthought library imports
+from traits.api import Instance, HasTraits
+from traitsui.api import View, Item
+from enable.api import Container
+from enable.api import ComponentEditor
 
-from chaco.plots.contour.contour_line_plot import ContourLinePlot  # noqa: F401
 
-warnings.warn(
-    "Importing ContourLinePlot from this module is deprecated. Please use "
-    "chaco.api or chaco.plots.api instead. This module will be removed in the "
-    "next major release.",
-    DeprecationWarning,
-    stacklevel=2,
-)
+class PlotWindow(HasTraits):
+    plot = Instance(Container)
+
+    traits_view = View(
+        Item(
+            "plot",
+            editor=ComponentEditor(),
+            height=300,
+            width=500,
+            show_label=False,
+        ),
+        title="Chaco Plot",
+        resizable=True,
+    )
```

### Comparing `chaco-5.1.1/chaco/data_frame_plot_data.py` & `chaco-6.0.0/chaco/data_frame_plot_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/data_range_1d.py` & `chaco-6.0.0/chaco/data_range_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,15 @@
                 self._low_value = -inf
             else:
                 self._low_value = self._low_setting
             if self._high_setting in ("auto", "track"):
                 self._high_value = inf
             else:
                 self._high_value = self._high_setting
+            self.updated = (self._low_value, self._high_value)
             return
         else:
             mins, maxes = zip(*bounds_list)
 
             low_start, high_start = calc_bounds(
                 self._low_setting,
                 self._high_setting,
```

### Comparing `chaco-5.1.1/chaco/data_range_2d.py` & `chaco-6.0.0/chaco/data_range_2d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/data_view.py` & `chaco-6.0.0/chaco/data_view.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/default_colormaps.py` & `chaco-6.0.0/chaco/default_colormaps.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/default_colors.py` & `chaco-6.0.0/chaco/default_colors.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/discrete_color_mapper.py` & `chaco-6.0.0/chaco/discrete_color_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/downsample/_lttb.c` & `chaco-6.0.0/chaco/downsample/_lttb.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "include_dirs": [
-            "/tmp/build-env-li4h5_h5/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-k7tbay_7/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "chaco.downsample._lttb",
         "sources": [
             "chaco/downsample/_lttb.pyx"
         ]
     },
     "module_name": "chaco.downsample._lttb"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,16 +90,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -16232,15 +16236,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -16354,15 +16358,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -16618,15 +16622,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -16767,15 +16771,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -18388,28 +18392,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -20965,15 +20969,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21161,15 +21165,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21433,15 +21437,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `chaco-5.1.1/chaco/downsample/_lttb.pyx` & `chaco-6.0.0/chaco/downsample/_lttb.pyx`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/downsample/lttb.py` & `chaco-6.0.0/chaco/downsample/lttb.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/downsample/tests/test_lttb.py` & `chaco-6.0.0/chaco/downsample/tests/test_lttb.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/example_support.py` & `chaco-6.0.0/chaco/example_support.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/_etsdemo_info.py` & `chaco-6.0.0/chaco/examples/_etsdemo_info.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/advanced/asynchronous_updates.py` & `chaco-6.0.0/chaco/examples/demo/advanced/asynchronous_updates.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/advanced/cmap_variable_sized_scatter.py` & `chaco-6.0.0/chaco/examples/demo/advanced/cmap_variable_sized_scatter.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/advanced/data_cube.py` & `chaco-6.0.0/chaco/examples/demo/advanced/data_cube.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/advanced/data_stream.py` & `chaco-6.0.0/chaco/examples/demo/advanced/data_stream.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/advanced/scalar_image_function_inspector.py` & `chaco-6.0.0/chaco/examples/demo/advanced/scalar_image_function_inspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         )
         gridy = linspace(
             self.min_y + ystep / 2, self.max_y - ystep / 2, self.npts_y + 1
         )
         x, y = meshgrid(gridx, gridy)
 
         d = dict(x=x, y=y)
-        exec("from scipy import *", d)
+        exec("from numpy import *", d)
         exec("from scipy.special import *", d)
         try:
             self.zs = eval(self.function, d)
         except NameError:
             # Raised if the function(s) is not available in scipy context (d)
             print("The function name {0} is invalid".format(self.function))
             self.trait_setq(_function=self.function)
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/bar_plot_configurable.py` & `chaco-6.0.0/chaco/examples/demo/basic/bar_plot_configurable.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/bar_plot_stacked.py` & `chaco-6.0.0/chaco/examples/demo/basic/bar_plot_stacked.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/bounded_grids.py` & `chaco-6.0.0/chaco/examples/demo/basic/bounded_grids.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/candle.py` & `chaco-6.0.0/chaco/examples/demo/basic/candle.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/capitol.jpg` & `chaco-6.0.0/chaco/examples/demo/basic/capitol.jpg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cat.jpg` & `chaco-6.0.0/chaco/examples/demo/basic/cat.jpg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cmap_image_aspect_ratio.py` & `chaco-6.0.0/chaco/examples/demo/basic/cmap_image_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cmap_image_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/cmap_image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cmap_image_select.py` & `chaco-6.0.0/chaco/examples/demo/basic/cmap_image_select.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cmap_scatter.py` & `chaco-6.0.0/chaco/examples/demo/basic/cmap_scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     )
 
     # Tweak some of the plot properties
     plot.title = "Colormapped Scatter Plot with Range-selectable Data Points"
     plot.padding = 50
     plot.x_grid.visible = False
     plot.y_grid.visible = False
-    plot.x_axis.font = "modern 16"
-    plot.y_axis.font = "modern 16"
+    plot.x_axis.font = "sans-serif 16"
+    plot.y_axis.font = "sans-serif 16"
 
     # Right now, some of the tools are a little invasive, and we need the
     # actual ColomappedScatterPlot object to give to them
     cmap_renderer = plot.plots["my_plot"][0]
 
     # Attach some tools to the plot
     plot.tools.append(PanTool(plot, constrain_key="shift"))
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/cmap_segment_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/cmap_segment_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     )
 
     # Tweak some of the plot properties
     plot.title = "Colormapped Segment Plot with variable widths"
     plot.padding = 50
     plot.x_grid.visible = False
     plot.y_grid.visible = False
-    plot.x_axis.font = "modern 16"
-    plot.y_axis.font = "modern 16"
+    plot.x_axis.font = "sans-serif 16"
+    plot.y_axis.font = "sans-serif 16"
 
     # Right now, some of the tools are a little invasive, and we need the
     # actual ColomappedSegmentPlot object to give to them
     cmap_renderer = plot.plots["my_plot"][0]
 
     # Attach some tools to the plot
     plot.tools.append(PanTool(plot, constrain_key="shift"))
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/contour_cmap_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/contour_cmap_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/contour_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/contour_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/discrete_cmap_image_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/discrete_cmap_image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/discrete_cmap_scatter.py` & `chaco-6.0.0/chaco/examples/demo/basic/discrete_cmap_scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     )
 
     # Tweak some of the plot properties
     plot.title = "Colormapped Scatter Plot with Range-selectable Data Points"
     plot.padding = 50
     plot.x_grid.visible = False
     plot.y_grid.visible = False
-    plot.x_axis.font = "modern 16"
-    plot.y_axis.font = "modern 16"
+    plot.x_axis.font = "sans-serif 16"
+    plot.y_axis.font = "sans-serif 16"
 
     # Right now, some of the tools are a little invasive, and we need the
     # actual ColomappedScatterPlot object to give to them
     cmap_renderer = plot.plots["my_plot"][0]
 
     # Attach some tools to the plot
     plot.tools.append(PanTool(plot, constrain_key="shift"))
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/draw_layers.py` & `chaco-6.0.0/chaco/examples/demo/basic/draw_layers.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/grid_container.py` & `chaco-6.0.0/chaco/examples/demo/basic/grid_container.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/grid_container_aspect_ratio.py` & `chaco-6.0.0/chaco/examples/demo/basic/grid_container_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/hittest_tool.py` & `chaco-6.0.0/chaco/examples/demo/basic/hittest_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/horizon_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/horizon_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/image_from_file.py` & `chaco-6.0.0/chaco/examples/demo/basic/image_from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     # ---------------------------------------------------------------------------
 
     def init(self, info):
         """Initializes the controls of a user interface.
         Overridden here to assign the 'view' trait.
         """
         self.view = info.object
+        return True
 
     def save(self, ui_info):
         """
         Callback for the 'Save Image' menu option.
         """
         ui = self.view.edit_traits(view="save_file_view")
         if ui.result == True:
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/image_inspector.py` & `chaco-6.0.0/chaco/examples/demo/basic/image_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/image_lasso.py` & `chaco-6.0.0/chaco/examples/demo/basic/image_lasso.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/image_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/inset_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/inset_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/line_drawing.py` & `chaco-6.0.0/chaco/examples/demo/basic/line_drawing.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/line_plot1.py` & `chaco-6.0.0/chaco/examples/demo/basic/line_plot1.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/line_plot_hold.py` & `chaco-6.0.0/chaco/examples/demo/basic/line_plot_hold.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/log_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/log_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/minard_napoleon.py` & `chaco-6.0.0/chaco/examples/demo/basic/minard_napoleon.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/minor_ticks_axis.py` & `chaco-6.0.0/chaco/examples/demo/basic/minor_ticks_axis.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/nans_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/nans_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/pandas_data.py` & `chaco-6.0.0/chaco/examples/demo/basic/pandas_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/polygon_move.py` & `chaco-6.0.0/chaco/examples/demo/basic/polygon_move.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/polygon_plot_demo.py` & `chaco-6.0.0/chaco/examples/demo/basic/polygon_plot_demo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/regression.py` & `chaco-6.0.0/chaco/examples/demo/basic/regression.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_1d.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     plot.plot(
         ("index", "value"),
         type="scatter",
         marker="square",
         index_sort="ascending",
         color="orange",
-        marker_size=3,  # randint(1,5, numpts),
+        marker_size=3,
         bgcolor="white",
         use_backbuffer=True,
     )
 
     # Tweak some of the plot properties
     plot.title = "1D Scatter Plots"
     plot.line_width = 0.5
```

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_alpha.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_alpha.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_custom_marker.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_custom_marker.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_inspector.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_inspector2.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_inspector2.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_rect_select.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_rect_select.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_select.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_select.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_toggle.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_toggle.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scatter_variable_size.py` & `chaco-6.0.0/chaco/examples/demo/basic/scatter_variable_size.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/scrollbar.py` & `chaco-6.0.0/chaco/examples/demo/basic/scrollbar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/segment_plot.py` & `chaco-6.0.0/chaco/examples/demo/basic/segment_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/tabbed_plots.py` & `chaco-6.0.0/chaco/examples/demo/basic/tabbed_plots.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/basic/zoomable_colorbar.py` & `chaco-6.0.0/chaco/examples/demo/basic/zoomable_colorbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     )
 
     # Tweak some of the plot properties
     plot.title = "Colormapped Scatter Plot with Pan/Zoom Color Bar"
     plot.padding = 50
     plot.x_grid.visible = False
     plot.y_grid.visible = False
-    plot.x_axis.font = "modern 16"
-    plot.y_axis.font = "modern 16"
+    plot.x_axis.font = "sans-serif 16"
+    plot.y_axis.font = "sans-serif 16"
 
     # Add pan and zoom to the plot
     plot.tools.append(PanTool(plot, constrain_key="shift"))
     zoom = ZoomTool(plot)
     plot.overlays.append(zoom)
 
     # Create the colorbar, handing in the appropriate range and colormap
```

### Comparing `chaco-5.1.1/chaco/examples/demo/bigdata.py` & `chaco-6.0.0/chaco/examples/demo/bigdata.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/chaco_trait_editor.py` & `chaco-6.0.0/chaco/examples/demo/chaco_trait_editor.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/coordinate_line_overlay_demo.py` & `chaco-6.0.0/chaco/examples/demo/coordinate_line_overlay_demo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/cursor_tool_demo.py` & `chaco-6.0.0/chaco/examples/demo/cursor_tool_demo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/data_labels.py` & `chaco-6.0.0/chaco/examples/demo/data_labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             data_point=(x[20], y[20]),
             label_position="bottom right",
             border_visible=False,
             bgcolor="transparent",
             marker_color="blue",
             marker_line_color="transparent",
             marker="diamond",
-            font="modern 14",
+            font="sans-serif 14",
             arrow_visible=False,
         )
         plot.overlays.append(label2)
 
         label3 = DataLabel(
             component=plot,
             data_point=(x[80], y[80]),
@@ -128,15 +128,15 @@
             border_padding=10,
             marker_color="red",
             marker_size=3,
             label_position=(20, 50),
             label_style="bubble",
             label_text="Something interesting",
             label_format="at x=%(x).2f, y=%(y).2f",
-            font="modern 18",
+            font="sans-serif 18",
             bgcolor=(1, 1, 0.75, 1),
         )
         plot.overlays.append(label4)
         tool4 = DataLabelTool(
             label4, drag_button="right", auto_arrow_root=True
         )
         label4.tools.append(tool4)
@@ -151,15 +151,15 @@
             marker_size=4,
             show_label_coords=False,
             label_style="bubble",
             label_position=(25, 5),
             label_text="Label with\narrow_min_length=20",
             border_visible=False,
             arrow_min_length=20,
-            font="modern 14",
+            font="sans-serif 14",
             bgcolor=(0.75, 0.75, 0.75, 1),
         )
         plot.overlays.append(label5)
         tool5 = DataLabelTool(
             label5, drag_button="right", auto_arrow_root=True
         )
         label5.tools.append(tool5)
```

### Comparing `chaco-5.1.1/chaco/examples/demo/data_view.py` & `chaco-6.0.0/chaco/examples/demo/data_view.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/edit_line.py` & `chaco-6.0.0/chaco/examples/demo/edit_line.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/financial/correlations.py` & `chaco-6.0.0/chaco/examples/demo/financial/correlations.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/financial/stock_prices.py` & `chaco-6.0.0/chaco/examples/demo/financial/stock_prices.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/functionplotter.py` & `chaco-6.0.0/chaco/examples/demo/functionplotter.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/hyetograph.py` & `chaco-6.0.0/chaco/examples/demo/hyetograph.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/image_plot_origin_and_orientation.py` & `chaco-6.0.0/chaco/examples/demo/image_plot_origin_and_orientation.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/multi_line_plot_demo.py` & `chaco-6.0.0/chaco/examples/demo/multi_line_plot_demo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/nonlinear_color_mapping.py` & `chaco-6.0.0/chaco/examples/demo/nonlinear_color_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     colorbar = Property(Instance(ColorBar), observe=["plot"])
 
     traits_view = View(
         HGroup(
             Item("colormap_scale"),
             Item(
                 "power",
-                editor=RangeEditor(low=0.1, high=3.0, format="%4.2f"),
+                editor=RangeEditor(low=0.1, high=3.0, format_str="%4.2f"),
                 visible_when='colormap_scale.startswith("power")',
                 springy=True,
             ),
             Item("colorbar_scale"),
             springy=True,
         ),
         UItem("plot", editor=ComponentEditor()),
```

### Comparing `chaco-5.1.1/chaco/examples/demo/qt_example.py` & `chaco-6.0.0/chaco/examples/demo/qt_example.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/quiver.py` & `chaco-6.0.0/chaco/examples/demo/quiver.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/range_selection_demo.py` & `chaco-6.0.0/chaco/examples/demo/range_selection_demo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/scales_test.py` & `chaco-6.0.0/chaco/examples/demo/scales_test.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/simple_line.py` & `chaco-6.0.0/chaco/examples/demo/simple_line.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/simple_polar.py` & `chaco-6.0.0/chaco/examples/demo/simple_polar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/stacked_axis.py` & `chaco-6.0.0/chaco/examples/demo/stacked_axis.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/status_overlay.py` & `chaco-6.0.0/chaco/examples/demo/status_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/toolbar_plot.py` & `chaco-6.0.0/chaco/examples/demo/toolbar_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/tornado.py` & `chaco-6.0.0/chaco/examples/demo/tornado.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/two_plots.py` & `chaco-6.0.0/chaco/examples/demo/two_plots.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/vanderwaals.py` & `chaco-6.0.0/chaco/examples/demo/vanderwaals.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/vertical_plot.py` & `chaco-6.0.0/chaco/examples/demo/vertical_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/demo/xray_plot.py` & `chaco-6.0.0/chaco/examples/demo/xray_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/examples/tests/test_etsdemo_info.py` & `chaco-6.0.0/chaco/examples/tests/test_etsdemo_info.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/function_data_source.py` & `chaco-6.0.0/chaco/function_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/function_image_data.py` & `chaco-6.0.0/chaco/function_image_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/grid.py` & `chaco-6.0.0/chaco/grid.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/grid_data_source.py` & `chaco-6.0.0/chaco/grid_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/grid_mapper.py` & `chaco-6.0.0/chaco/grid_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/image_data.py` & `chaco-6.0.0/chaco/image_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/image_utils.py` & `chaco-6.0.0/chaco/image_utils.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/label.py` & `chaco-6.0.0/chaco/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     #: The color of the border.
     border_color = black_color_trait
 
     #: Whether or not the border is visible
     border_visible = Bool(True)
 
     #: The font of the label text.
-    font = KivaFont("modern 10")
+    font = KivaFont("sans-serif 10")
 
     #: Number of pixels of margin around the label, for both X and Y dimensions.
     margin = Int(2)
 
     #: Number of pixels of spacing between lines of text.
     line_spacing = Int(5)
```

### Comparing `chaco-5.1.1/chaco/label_axis.py` & `chaco-6.0.0/chaco/label_axis.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/layers/api.py` & `chaco-6.0.0/chaco/tests/test_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-import warnings
+import unittest
 
-from chaco.overlays.api import ErrorLayer, StatusLayer, WarningLayer
+import chaco.api
 
-warnings.warn(
-    "Importing from chaco.layers.api is deprecated, please import from "
-    "chaco.api or chaco.overlays.api going forward as chaco/layers will be "
-    "removed in a future release.",
-    DeprecationWarning,
-    stacklevel=2,
-)
+
+class TestAPI(unittest.TestCase):
+
+    def test_enable_imports(self):
+        """Test for deprecated imports from enable.api"""
+        names = {'marker_trait'}
+        for name in names:
+            with self.subTest(name=name):
+                with self.assertWarns(DeprecationWarning):
+                    getattr(chaco.api, name)
```

### Comparing `chaco-5.1.1/chaco/linear_mapper.py` & `chaco-6.0.0/chaco/linear_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/log_mapper.py` & `chaco-6.0.0/chaco/log_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/multi_array_data_source.py` & `chaco-6.0.0/chaco/multi_array_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/aligned_container_overlay.py` & `chaco-6.0.0/chaco/overlays/aligned_container_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/api.py` & `chaco-6.0.0/chaco/overlays/api.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/colormapped_selection_overlay.py` & `chaco-6.0.0/chaco/overlays/colormapped_selection_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/container_overlay.py` & `chaco-6.0.0/chaco/overlays/container_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/coordinate_line_overlay.py` & `chaco-6.0.0/chaco/overlays/coordinate_line_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/data_label.py` & `chaco-6.0.0/chaco/overlays/data_label.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/databox.py` & `chaco-6.0.0/chaco/overlays/databox.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/lasso_overlay.py` & `chaco-6.0.0/chaco/overlays/lasso_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/layers/data/Dialog-error.svg` & `chaco-6.0.0/chaco/overlays/layers/data/Dialog-error.svg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/layers/data/Dialog-warning.svg` & `chaco-6.0.0/chaco/overlays/layers/data/Dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/layers/data/range_selection.svg` & `chaco-6.0.0/chaco/overlays/layers/data/range_selection.svg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/layers/status_layer.py` & `chaco-6.0.0/chaco/overlays/layers/status_layer.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/layers/svg_range_selection_overlay.py` & `chaco-6.0.0/chaco/overlays/layers/svg_range_selection_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/legend.py` & `chaco-6.0.0/chaco/overlays/legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         scatter[0]._render_icon(gc, x, y, width, height)
 
 
 class Legend(AbstractOverlay):
     """A legend for a plot."""
 
     #: The font to use for the legend text.
-    font = KivaFont("modern 12")
+    font = KivaFont("sans-serif 12")
 
     #: The amount of space between the content of the legend and the border.
     border_padding = Int(10)
 
     #: The border is visible (overrides Enable Component).
     border_visible = True
 
@@ -423,15 +423,15 @@
             labels.append(self._create_label(self.title))
             label_names.append(self.title)
             visible_plots.append(None)
 
         # We need a dummy GC in order to get font metrics
         dummy_gc = font_metrics_provider()
         label_sizes = array(
-            [label.get_width_height(dummy_gc) for label in labels]
+            [label.get_bounding_box(dummy_gc) for label in labels]
         )
 
         if len(label_sizes) > 0:
             max_label_width = max(label_sizes[:, 0])
             total_label_height = (
                 sum(label_sizes[:, 1])
                 + (len(label_sizes) - 1) * self.line_spacing
@@ -461,16 +461,20 @@
             legend_width = self.outer_width
         if "v" not in self.resizable:
             legend_height = self.outer_height
         return [legend_width, legend_height]
 
     def get_label_at(self, x, y):
         """ Returns the label object at (x,y) """
+        icon_space = array([
+            self.icon_spacing + self.icon_bounds[0],
+            self.icon_bounds[1],
+        ])
         for i, pos in enumerate(self._cached_label_positions):
-            size = self._cached_label_sizes[i]
+            size = self._cached_label_sizes[i] + icon_space
             corner = pos + size
             if (pos[0] <= x <= corner[0]) and (pos[1] <= y <= corner[1]):
                 return self._cached_labels[i]
         else:
             return None
 
     def _do_layout(self):
```

### Comparing `chaco-5.1.1/chaco/overlays/plot_label.py` & `chaco-6.0.0/chaco/overlays/plot_label.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/scatter_inspector_overlay.py` & `chaco-6.0.0/chaco/overlays/scatter_inspector_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/simple_inspector_overlay.py` & `chaco-6.0.0/chaco/overlays/simple_inspector_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/tests/test_data_label.py` & `chaco-6.0.0/chaco/overlays/tests/test_data_label.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/tests/test_databox.py` & `chaco-6.0.0/chaco/overlays/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/overlays/text_box_overlay.py` & `chaco-6.0.0/chaco/overlays/text_box_overlay.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     # Configuration traits ####################################################
 
     #: The text to display in the box.
     text = Str
 
     #: The font to use for the text.
-    font = KivaFont("modern 12")
+    font = KivaFont("sans-serif 12")
 
     #: The background color for the box (overrides AbstractOverlay).
     bgcolor = ColorTrait("transparent")
 
     #: The alpha value to apply to **bgcolor**
     alpha = Union(Float(1.0), None)
```

### Comparing `chaco-5.1.1/chaco/overlays/text_grid_overlay.py` & `chaco-6.0.0/chaco/overlays/text_grid_overlay.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     def _text_grid_changed(self, old, new):
         if old is not None:
             self.remove(old)
         if new is not None:
             self.add(new)
 
     def _text_grid_default(self):
-        text_grid = TextGrid(font="modern 12", cell_border_width=0)
+        text_grid = TextGrid(font="sans-serif 12", cell_border_width=0)
         self.add(text_grid)
         return text_grid
```

### Comparing `chaco-5.1.1/chaco/overlays/tooltip.py` & `chaco-6.0.0/chaco/overlays/tooltip.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from chaco.label import Label
 
 
 class ToolTip(AbstractOverlay):
     """An overlay that is a toolip."""
 
     #: The font to render the tooltip.
-    font = KivaFont("modern 10")
+    font = KivaFont("sans-serif 10")
 
     #: The color of the text in the tooltip
     text_color = black_color_trait
 
     #: The ammount of space between the border and the text.
     border_padding = Int(4)
```

### Comparing `chaco-5.1.1/chaco/pdf_graphics_context.py` & `chaco-6.0.0/chaco/pdf_graphics_context.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot.py` & `chaco-6.0.0/chaco/plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_canvas.py` & `chaco-6.0.0/chaco/plot_canvas.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_canvas_toolbar.py` & `chaco-6.0.0/chaco/plot_canvas_toolbar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_component.py` & `chaco-6.0.0/chaco/plot_component.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_containers.py` & `chaco-6.0.0/chaco/plot_containers.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_factory.py` & `chaco-6.0.0/chaco/plot_factory.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plot_graphics_context.py` & `chaco-6.0.0/chaco/plot_graphics_context.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/api.py` & `chaco-6.0.0/chaco/plots/api.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/barplot.py` & `chaco-6.0.0/chaco/plots/barplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from numpy import (
     array,
     compress,
     column_stack,
     empty,
     invert,
-    isnan,
+    isfinite,
     transpose,
     zeros,
 )
 from traits.api import (
     Any,
     Bool,
     Enum,
@@ -267,30 +267,34 @@
                 "Chaco: using empty dataset; index_len=%d, value_len=%d."
                 % (len(index), len(value))
             )
             self._cached_data_pts = array([])
             self._cache_valid = True
             return
 
-        # TODO: Until we code up a better handling of value-based culling that
-        # takes into account starting_value and dataspace bar widths, just use
-        # the index culling for now.
-        # value_range_mask = self.value_mapper.range.mask_data(value)
-        # nan_mask = invert(isnan(index_mask)) & invert(isnan(value_mask))
-        # point_mask = index_mask & value_mask & nan_mask & \
-        #              index_range_mask & value_range_mask
+        # TODO: better accounting for intersection of boxes with visible region
+        # current strategy simply masks the index values and then does a 1D
+        # dilation of the mask.  This will work in many situations but will
+        # fail on extreme zoom in.
+        # Ideally we would work out all the boxes and compute intersections.
 
         index_range_mask = self.index_mapper.range.mask_data(index)
-        nan_mask = invert(isnan(index_mask))
-        point_mask = index_mask & nan_mask & index_range_mask
+        # include points on either side of clipped range (1D dilation)
+        # - not perfect, but better than simple clipping
+        index_range_mask[:-1] |= index_range_mask[1:]
+        index_range_mask[1:] |= index_range_mask[:-1]
+
+        nan_mask = isfinite(index) & isfinite(value)
+        point_mask = index_mask & value_mask & nan_mask & index_range_mask
 
         if self.starting_value is None:
             starting_values = zeros(len(index))
         else:
             starting_values = self.starting_value.get_data()
+            point_mask &= isfinite(starting_values)
 
         if self.bar_width_type == "data":
             half_width = self.bar_width / 2.0
             points = column_stack(
                 (
                     index - half_width,
                     index + half_width,
```

### Comparing `chaco-5.1.1/chaco/plots/candle_plot.py` & `chaco-6.0.0/chaco/plots/candle_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/cmap_image_plot.py` & `chaco-6.0.0/chaco/plots/cmap_image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/color_bar.py` & `chaco-6.0.0/chaco/plots/color_bar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/colormapped_scatterplot.py` & `chaco-6.0.0/chaco/plots/colormapped_scatterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/contour/cntr.c` & `chaco-6.0.0/chaco/plots/contour/cntr.c`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/contour/contour_line_plot.py` & `chaco-6.0.0/chaco/plots/contour/contour_line_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/contour/contour_poly_plot.py` & `chaco-6.0.0/chaco/plots/contour/contour_poly_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/contour/setup.py` & `chaco-6.0.0/chaco/plots/contour/setup.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/contour/tests/test_contour.py` & `chaco-6.0.0/chaco/plots/contour/tests/test_contour.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/errorbar_plot.py` & `chaco-6.0.0/chaco/plots/errorbar_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/filled_line_plot.py` & `chaco-6.0.0/chaco/plots/filled_line_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/horizon_plot.py` & `chaco-6.0.0/chaco/plots/horizon_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/image_plot.py` & `chaco-6.0.0/chaco/plots/image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/jitterplot.py` & `chaco-6.0.0/chaco/plots/jitterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/line_scatterplot_1d.py` & `chaco-6.0.0/chaco/plots/line_scatterplot_1d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/lineplot.py` & `chaco-6.0.0/chaco/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/multi_line_plot.py` & `chaco-6.0.0/chaco/plots/multi_line_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/polar_line_renderer.py` & `chaco-6.0.0/chaco/plots/polar_line_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         return array(
             (self.index_mapper.map_data(x), self.value_mapper.map_data(y))
         )
 
     def _downsample(self):
         return self.map_screen(self._cached_data_pts)
 
-    def _draw_plot(self, *args, **kw):
+    def _draw_plot(self, gc, *args, **kw):
         """Draws the 'plot' layer."""
         self._gather_points()
         self._render(gc, self._cached_data_pts)
 
     def _bounds_changed(self, old, new):
         super()._bounds_changed(old, new)
         self._update_mappers()
```

### Comparing `chaco-5.1.1/chaco/plots/polygon_plot.py` & `chaco-6.0.0/chaco/plots/polygon_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/quiverplot.py` & `chaco-6.0.0/chaco/plots/quiverplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/scatterplot.py` & `chaco-6.0.0/chaco/plots/scatterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/scatterplot_1d.py` & `chaco-6.0.0/chaco/plots/scatterplot_1d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/segment_plot.py` & `chaco-6.0.0/chaco/plots/segment_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_cmap_image_plot.py` & `chaco-6.0.0/chaco/plots/tests/test_cmap_image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_colormapped_scatterplot.py` & `chaco-6.0.0/chaco/plots/tests/test_colormapped_scatterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_errorbarplot.py` & `chaco-6.0.0/chaco/plots/tests/test_errorbarplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_image_plot.py` & `chaco-6.0.0/chaco/plots/tests/test_image_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_jitterplot.py` & `chaco-6.0.0/chaco/plots/tests/test_jitterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_line_scatterplot.py` & `chaco-6.0.0/chaco/plots/tests/test_line_scatterplot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_scatterplot_1d.py` & `chaco-6.0.0/chaco/plots/tests/test_scatterplot_1d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_scatterplot_renderers.py` & `chaco-6.0.0/chaco/plots/tests/test_scatterplot_renderers.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_segment_plot.py` & `chaco-6.0.0/chaco/plots/tests/test_segment_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_text_plot.py` & `chaco-6.0.0/chaco/plots/tests/test_text_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/tests/test_text_plot_1d.py` & `chaco-6.0.0/chaco/plots/tests/test_text_plot_1d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/plots/text_plot.py` & `chaco-6.0.0/chaco/plots/text_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,33 +30,33 @@
 class TextPlot(BaseXYPlot):
     """ A plot that positions textual labels in 2D """
 
     #: text values corresponding to indices
     text = Instance(ArrayDataSource)
 
     #: The font of the tick labels.
-    text_font = KivaFont("modern 10")
+    text_font = KivaFont("sans-serif 10", redraw=True)
 
     #: The color of the tick labels.
-    text_color = black_color_trait
+    text_color = black_color_trait(redraw=True)
 
     #: The rotation of the tick labels.
-    text_rotate_angle = Float(0)
+    text_rotate_angle = Float(0, redraw=True)
 
     #: The margin around the label.
-    text_margin = Int(2)
+    text_margin = Int(2, redraw=True)
 
     #: horizontal position of text relative to target point
-    h_position = Enum("center", "left", "right")
+    h_position = Enum("center", "left", "right", redraw=True)
 
     #: vertical position of text relative to target point
-    v_position = Enum("center", "top", "bottom")
+    v_position = Enum("center", "top", "bottom", redraw=True)
 
     #: offset of text relative to non-index direction in pixels
-    text_offset = Tuple(Float, Float)
+    text_offset = Tuple(Float, Float, redraw=True)
 
     # ------------------------------------------------------------------------
     # Private traits
     # ------------------------------------------------------------------------
 
     #: flag for whether the cache of Label instances is valid
     _label_cache_valid = Bool(False, transient=True)
@@ -169,10 +169,10 @@
 
     @observe("index.data_changed")
     def _invalidate(self, event):
         self._cache_valid = False
         self._screen_cache_valid = False
         self._label_cache_valid = False
 
-    @observe("value.data_changed")
+    @observe("value.data_changed,+redraw")
     def _invalidate_labels(self, event):
         self._label_cache_valid = False
```

### Comparing `chaco-5.1.1/chaco/plots/text_plot_1d.py` & `chaco-6.0.0/chaco/plots/text_plot_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class TextPlot1D(Base1DPlot):
     """ A plot that positions textual labels in 1D """
 
     #: text values corresponding to indices
     value = Instance(ArrayDataSource)
 
     #: The font of the tick labels.
-    text_font = KivaFont("modern 10")
+    text_font = KivaFont("sans-serif 10")
 
     #: The color of the tick labels.
     text_color = black_color_trait
 
     #: The rotation of the tick labels.
     text_rotate_angle = Float(0)
```

### Comparing `chaco-5.1.1/chaco/plotscrollbar.py` & `chaco-6.0.0/chaco/plotscrollbar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/point_data_source.py` & `chaco-6.0.0/chaco/point_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/polar_mapper.py` & `chaco-6.0.0/chaco/polar_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/formatters.py` & `chaco-6.0.0/chaco/scales/formatters.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/safetime.py` & `chaco-6.0.0/chaco/scales/safetime.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/scales.py` & `chaco-6.0.0/chaco/scales/scales.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/tests/test_formatters.py` & `chaco-6.0.0/chaco/scales/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/tests/test_scales.py` & `chaco-6.0.0/chaco/scales/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/tests/test_time_scale.py` & `chaco-6.0.0/chaco/scales/tests/test_time_scale.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/tests/test_time_scale_resolution.py` & `chaco-6.0.0/chaco/scales/tests/test_time_scale_resolution.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales/time_scale.py` & `chaco-6.0.0/chaco/scales/time_scale.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scales_tick_generator.py` & `chaco-6.0.0/chaco/scales_tick_generator.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/scaly_plot.py` & `chaco-6.0.0/chaco/scaly_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/selectable_legend.py` & `chaco-6.0.0/chaco/selectable_legend.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/speedups.py` & `chaco-6.0.0/chaco/speedups.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/svg_graphics_context.py` & `chaco-6.0.0/chaco/svg_graphics_context.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/_tools.py` & `chaco-6.0.0/chaco/tests/_tools.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_2d_case.py` & `chaco-6.0.0/chaco/tests/test_2d_case.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_array_or_none.py` & `chaco-6.0.0/chaco/tests/test_array_or_none.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_array_plot_data.py` & `chaco-6.0.0/chaco/tests/test_array_plot_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_arraydatasource.py` & `chaco-6.0.0/chaco/tests/test_arraydatasource.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_base_utils.py` & `chaco-6.0.0/chaco/tests/test_base_utils.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_border.py` & `chaco-6.0.0/chaco/tests/test_border.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     def test_draw_border_simple(self):
         """Borders should have the correct height and width."""
         size = (5, 5)
         container = Plot(padding=1, border_visible=True)
         container.outer_bounds = list(size)
         gc = PlotGraphicsContext(size)
+        gc.clear()
         gc.render_component(container)
 
         desired = array(
             (
                 (255, 255, 255, 255, 255, 255),
                 (255, 0, 0, 0, 0, 255),
                 (255, 0, 255, 255, 0, 255),
```

### Comparing `chaco-5.1.1/chaco/tests/test_chaco_traits.py` & `chaco-6.0.0/chaco/tests/test_chaco_traits.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_colormapper.py` & `chaco-6.0.0/chaco/tests/test_colormapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_data_frame_plot_data.py` & `chaco-6.0.0/chaco/tests/test_data_frame_plot_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_data_view.py` & `chaco-6.0.0/chaco/tests/test_data_view.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_datarange_1d.py` & `chaco-6.0.0/chaco/tests/test_datarange_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import unittest
 import warnings
 
 from numpy import arange, array, zeros, inf
 from numpy.testing import assert_equal
 
 from traits.api import HasTraits, Instance, Bool, observe
+from traits.testing.api import UnittestTools
 
 from chaco.api import DataRange1D, ArrayDataSource
 
 NAN = float("nan")
 
 
 class Foo(HasTraits):
@@ -31,15 +32,15 @@
     range_updated = Bool(False)
 
     @observe("range.updated")
     def range_changed(self, event):
         self.range_updated = True
 
 
-class DataRangeTestCase(unittest.TestCase):
+class DataRangeTestCase(UnittestTools, unittest.TestCase):
     def test_empty_range(self):
         r = DataRange1D()
         self.assertEqual(r.low, -inf)
         self.assertEqual(r.high, inf)
         self.assertEqual(r.low_setting, "auto")
         self.assertEqual(r.high_setting, "auto")
         r.low = 5.0
@@ -333,7 +334,32 @@
         r.sources.append(ds2)
         self.assertEqual(r.low, -inf)
         self.assertEqual(r.high, 1.0)
 
         r.sources.append(ds1)
         self.assertEqual(r.low, -inf)
         self.assertEqual(r.high, inf)
+
+    def test_sources_changed_auto(self):
+        ds1 = ArrayDataSource(array([3, 4, 5, 6, 7]))
+        ds2 = ArrayDataSource(array([5, 10, 15, 20]))
+        r = DataRange1D()
+        events = []
+        r.observe(events.append, 'updated')
+
+        self.assertEqual(r.low, -inf)
+        self.assertEqual(r.high, inf)
+
+        with self.assertTraitChanges(r, "updated", count=1):
+            r.add(ds1)
+
+        self.assertEqual(events[-1].new, (3, 7))
+        self.assertEqual(r.low, 3)
+        self.assertEqual(r.high, 7)
+
+
+        with self.assertTraitChanges(r, "updated", count=1):
+            r.remove(ds1)
+
+        self.assertEqual(events[-1].new, (-inf, inf))
+        self.assertEqual(r.low, -inf)
+        self.assertEqual(r.high, inf)
```

### Comparing `chaco-5.1.1/chaco/tests/test_datarange_2d.py` & `chaco-6.0.0/chaco/tests/test_datarange_2d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_default_colormaps.py` & `chaco-6.0.0/chaco/tests/test_default_colormaps.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_discrete_colormapper.py` & `chaco-6.0.0/chaco/tests/test_discrete_colormapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_function_data_source.py` & `chaco-6.0.0/chaco/tests/test_function_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_grid_data_source.py` & `chaco-6.0.0/chaco/tests/test_grid_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_grid_mapper.py` & `chaco-6.0.0/chaco/tests/test_grid_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_highlight_tool.py` & `chaco-6.0.0/chaco/tests/test_highlight_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_hittest.py` & `chaco-6.0.0/chaco/tests/test_hittest.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_image_data.py` & `chaco-6.0.0/chaco/tests/test_image_data.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_image_utils.py` & `chaco-6.0.0/chaco/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_instantiation_order.py` & `chaco-6.0.0/chaco/tests/test_instantiation_order.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_linearmapper.py` & `chaco-6.0.0/chaco/tests/test_linearmapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_logmapper.py` & `chaco-6.0.0/chaco/tests/test_logmapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_multi_array_data_source.py` & `chaco-6.0.0/chaco/tests/test_multi_array_data_source.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_plot.py` & `chaco-6.0.0/chaco/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_plot_factory.py` & `chaco-6.0.0/chaco/tests/test_plot_factory.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_plotcontainer.py` & `chaco-6.0.0/chaco/tests/test_plotcontainer.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_speedups.py` & `chaco-6.0.0/chaco/tests/test_speedups.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tests/test_ticks.py` & `chaco-6.0.0/chaco/tests/test_ticks.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/ticks.py` & `chaco-6.0.0/chaco/ticks.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/toolbar_plot.py` & `chaco-6.0.0/chaco/toolbar_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/api.py` & `chaco-6.0.0/chaco/tools/api.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/better_selecting_zoom.py` & `chaco-6.0.0/chaco/tools/better_selecting_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/better_zoom.py` & `chaco-6.0.0/chaco/tools/better_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/broadcaster.py` & `chaco-6.0.0/chaco/tools/broadcaster.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/cursor_tool.py` & `chaco-6.0.0/chaco/tools/cursor_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/data_label_tool.py` & `chaco-6.0.0/chaco/tools/data_label_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/dataprinter.py` & `chaco-6.0.0/chaco/tools/dataprinter.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/drag_zoom.py` & `chaco-6.0.0/chaco/tools/drag_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/draw_points_tool.py` & `chaco-6.0.0/chaco/tools/draw_points_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/highlight_tool.py` & `chaco-6.0.0/chaco/tools/highlight_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/image_inspector_tool.py` & `chaco-6.0.0/chaco/tools/image_inspector_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/lasso_selection.py` & `chaco-6.0.0/chaco/tools/lasso_selection.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/legend_highlighter.py` & `chaco-6.0.0/chaco/tools/legend_highlighter.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,15 @@
 
 
 def get_hit_plots(legend, event):
     if legend is None or not legend.is_in(event.x, event.y):
         return []
 
     try:
-        # FIXME: The size of the legend is not being computed correctly, so
-        # always look at the front of the label where we know we'll get a hit.
-        label = legend.get_label_at(legend.x + 20, event.y)
-
+        label = legend.get_label_at(event.x, event.y)
     except:
         raise
         label = None
 
     if label is None:
         return []
     try:
```

### Comparing `chaco-5.1.1/chaco/tools/legend_tool.py` & `chaco-6.0.0/chaco/tools/legend_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/line_inspector.py` & `chaco-6.0.0/chaco/tools/line_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/line_segment_tool.py` & `chaco-6.0.0/chaco/tools/line_segment_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/move_tool.py` & `chaco-6.0.0/chaco/tools/move_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/pan_tool.py` & `chaco-6.0.0/chaco/tools/pan_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/pan_tool2.py` & `chaco-6.0.0/chaco/tools/pan_tool2.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/point_marker.py` & `chaco-6.0.0/chaco/tools/point_marker.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/range_selection.py` & `chaco-6.0.0/chaco/tools/range_selection.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/range_selection_2d.py` & `chaco-6.0.0/chaco/tools/range_selection_2d.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/range_selection_overlay.py` & `chaco-6.0.0/chaco/tools/range_selection_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/rect_zoom.py` & `chaco-6.0.0/chaco/tools/rect_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/rectangular_selection.py` & `chaco-6.0.0/chaco/tools/rectangular_selection.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/regression_lasso.py` & `chaco-6.0.0/chaco/tools/regression_lasso.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     line_width = Float(2.0)
 
     _label = Instance(
         Label,
         kw=dict(
             bgcolor="white",
             border_color="black",
-            font="modern 14",
+            font="sans-serif 14",
             border_width=1,
         ),
     )
 
     def overlay(self, other_component, gc, view_bounds=None, mode="normal"):
         super().overlay(other_component, gc, view_bounds, mode)
         selection = self.lasso_selection
```

### Comparing `chaco-5.1.1/chaco/tools/save_tool.py` & `chaco-6.0.0/chaco/tools/save_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/scatter_inspector.py` & `chaco-6.0.0/chaco/tools/scatter_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/select_tool.py` & `chaco-6.0.0/chaco/tools/select_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/simple_inspector.py` & `chaco-6.0.0/chaco/tools/simple_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_better_zoom_tool.py` & `chaco-6.0.0/chaco/tools/tests/test_better_zoom_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_cursor_tool.py` & `chaco-6.0.0/chaco/tools/tests/test_cursor_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_data_label_tool.py` & `chaco-6.0.0/chaco/tools/tests/test_data_label_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_image_inspector.py` & `chaco-6.0.0/chaco/tools/tests/test_image_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_pan_tool.py` & `chaco-6.0.0/chaco/tools/tests/test_pan_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_range_selection.py` & `chaco-6.0.0/chaco/tools/tests/test_range_selection.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_range_zoom.py` & `chaco-6.0.0/chaco/tools/tests/test_range_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_rectangular_selection_tool.py` & `chaco-6.0.0/chaco/tools/tests/test_rectangular_selection_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tests/test_scatter_inspector.py` & `chaco-6.0.0/chaco/tools/tests/test_scatter_inspector.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tool_history_mixin.py` & `chaco-6.0.0/chaco/tools/tool_history_mixin.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tool_states.py` & `chaco-6.0.0/chaco/tools/tool_states.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/application-vnd-ms-excel.png` & `chaco-6.0.0/chaco/tools/toolbars/images/application-vnd-ms-excel.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/document-save.png` & `chaco-6.0.0/chaco/tools/toolbars/images/document-save.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/edit-copy.png` & `chaco-6.0.0/chaco/tools/toolbars/images/edit-copy.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/zoom-fit-height.png` & `chaco-6.0.0/chaco/tools/toolbars/images/zoom-fit-height.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/zoom-fit-width.png` & `chaco-6.0.0/chaco/tools/toolbars/images/zoom-fit-width.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/images/zoom-original.png` & `chaco-6.0.0/chaco/tools/toolbars/images/zoom-original.png`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/plot_toolbar.py` & `chaco-6.0.0/chaco/tools/toolbars/plot_toolbar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/toolbars/toolbar_buttons.py` & `chaco-6.0.0/chaco/tools/toolbars/toolbar_buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
         # Restore the toolbar.
         plot_component.add_toolbar()
 
     def _perform_wx(self, width, height, gc):
         import wx
 
-        bitmap = wx.BitmapFromBufferRGBA(
+        bitmap = wx.Bitmap.FromBufferRGBA(
             width + 1, height + 1, gc.bmp_array.flatten()
         )
         data = wx.BitmapDataObject()
         data.SetBitmap(bitmap)
         if wx.TheClipboard.Open():
             wx.TheClipboard.SetData(data)
             wx.TheClipboard.Close()
```

### Comparing `chaco-5.1.1/chaco/tools/tracking_pan_tool.py` & `chaco-6.0.0/chaco/tools/tracking_pan_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/tracking_zoom.py` & `chaco-6.0.0/chaco/tools/tracking_zoom.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/tools/traits_tool.py` & `chaco-6.0.0/chaco/tools/traits_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/transform_color_mapper.py` & `chaco-6.0.0/chaco/transform_color_mapper.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco/ui/axis_ui.py` & `chaco-6.0.0/chaco/ui/axis_ui.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/chaco.egg-info/PKG-INFO` & `chaco-6.0.0/chaco.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaco
-Version: 5.1.1
+Version: 6.0.0
 Summary: interactive 2-dimensional plotting
 Home-page: http://docs.enthought.com/chaco
 Download-URL: https://github.com/enthought/chaco
 Author: Peter Wang, et. al.
 Author-email: info@enthought.com
 Maintainer: ETS Developers
 Maintainer-email: enthought-dev@enthought.com
@@ -27,14 +27,21 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: tests
+Provides-Extra: pyside2
+Provides-Extra: pyside6
+Provides-Extra: pyqt5
+Provides-Extra: pyqt6
+Provides-Extra: wx
+Provides-Extra: null
 License-File: LICENSE.txt
 
 =========================================
 chaco: interactive 2-dimensional plotting
 =========================================
 
 http://www.github.com/enthought/chaco
```

### Comparing `chaco-5.1.1/chaco.egg-info/SOURCES.txt` & `chaco-6.0.0/chaco.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,96 +21,65 @@
 chaco/abstract_plot_data.py
 chaco/abstract_plot_renderer.py
 chaco/api.py
 chaco/array_data_source.py
 chaco/array_plot_data.py
 chaco/axis.py
 chaco/axis_view.py
-chaco/barplot.py
 chaco/base.py
 chaco/base_1d_mapper.py
 chaco/base_1d_plot.py
 chaco/base_2d_plot.py
 chaco/base_candle_plot.py
 chaco/base_contour_plot.py
 chaco/base_data_range.py
 chaco/base_plot_container.py
 chaco/base_xy_plot.py
-chaco/candle_plot.py
 chaco/chaco_traits.py
-chaco/cmap_image_plot.py
-chaco/color_bar.py
 chaco/color_mapper.py
 chaco/color_spaces.py
 chaco/colormap_generators.py
-chaco/colormapped_scatterplot.py
-chaco/colormapped_selection_overlay.py
-chaco/contour_line_plot.py
-chaco/contour_poly_plot.py
 chaco/data_frame_plot_data.py
-chaco/data_label.py
 chaco/data_range_1d.py
 chaco/data_range_2d.py
 chaco/data_view.py
 chaco/default_colormaps.py
 chaco/default_colors.py
 chaco/discrete_color_mapper.py
-chaco/errorbar_plot.py
 chaco/example_support.py
-chaco/filled_line_plot.py
 chaco/function_data_source.py
 chaco/function_image_data.py
 chaco/grid.py
 chaco/grid_data_source.py
 chaco/grid_mapper.py
-chaco/horizon_plot.py
 chaco/image_data.py
-chaco/image_plot.py
 chaco/image_utils.py
-chaco/jitterplot.py
 chaco/label.py
 chaco/label_axis.py
-chaco/lasso_overlay.py
-chaco/legend.py
-chaco/line_scatterplot_1d.py
 chaco/linear_mapper.py
-chaco/lineplot.py
 chaco/log_mapper.py
 chaco/multi_array_data_source.py
-chaco/multi_line_plot.py
 chaco/pdf_graphics_context.py
 chaco/plot.py
 chaco/plot_canvas.py
 chaco/plot_canvas_toolbar.py
 chaco/plot_component.py
 chaco/plot_containers.py
 chaco/plot_factory.py
 chaco/plot_graphics_context.py
-chaco/plot_label.py
 chaco/plotscrollbar.py
 chaco/point_data_source.py
-chaco/polar_line_renderer.py
 chaco/polar_mapper.py
-chaco/polygon_plot.py
-chaco/quiverplot.py
 chaco/scales_tick_generator.py
 chaco/scaly_plot.py
-chaco/scatter_inspector_overlay.py
-chaco/scatterplot.py
-chaco/scatterplot_1d.py
-chaco/segment_plot.py
 chaco/selectable_legend.py
 chaco/speedups.py
 chaco/svg_graphics_context.py
-chaco/text_box_overlay.py
-chaco/text_plot.py
-chaco/text_plot_1d.py
 chaco/ticks.py
 chaco/toolbar_plot.py
-chaco/tooltip.py
 chaco/transform_color_mapper.py
 chaco.egg-info/PKG-INFO
 chaco.egg-info/SOURCES.txt
 chaco.egg-info/dependency_links.txt
 chaco.egg-info/entry_points.txt
 chaco.egg-info/not-zip-safe
 chaco.egg-info/requires.txt
@@ -211,16 +180,14 @@
 chaco/examples/demo/financial/__init__.py
 chaco/examples/demo/financial/correlations.py
 chaco/examples/demo/financial/stock_prices.py
 chaco/examples/tests/__init__.py
 chaco/examples/tests/test_etsdemo_info.py
 chaco/layers/__init__.py
 chaco/layers/api.py
-chaco/layers/status_layer.py
-chaco/layers/svg_range_selection_overlay.py
 chaco/overlays/__init__.py
 chaco/overlays/aligned_container_overlay.py
 chaco/overlays/api.py
 chaco/overlays/colormapped_selection_overlay.py
 chaco/overlays/container_overlay.py
 chaco/overlays/coordinate_line_overlay.py
 chaco/overlays/data_label.py
@@ -270,14 +237,15 @@
 chaco/plots/contour/cntr.c
 chaco/plots/contour/contour_line_plot.py
 chaco/plots/contour/contour_poly_plot.py
 chaco/plots/contour/setup.py
 chaco/plots/contour/tests/__init__.py
 chaco/plots/contour/tests/test_contour.py
 chaco/plots/tests/__init__.py
+chaco/plots/tests/test_barplot.py
 chaco/plots/tests/test_cmap_image_plot.py
 chaco/plots/tests/test_colormapped_scatterplot.py
 chaco/plots/tests/test_errorbarplot.py
 chaco/plots/tests/test_image_plot.py
 chaco/plots/tests/test_jitterplot.py
 chaco/plots/tests/test_line_scatterplot.py
 chaco/plots/tests/test_scatterplot_1d.py
@@ -295,14 +263,15 @@
 chaco/scales/tests/test_formatters.py
 chaco/scales/tests/test_scales.py
 chaco/scales/tests/test_time_scale.py
 chaco/scales/tests/test_time_scale_resolution.py
 chaco/tests/__init__.py
 chaco/tests/_tools.py
 chaco/tests/test_2d_case.py
+chaco/tests/test_api.py
 chaco/tests/test_array_or_none.py
 chaco/tests/test_array_plot_data.py
 chaco/tests/test_arraydatasource.py
 chaco/tests/test_base_utils.py
 chaco/tests/test_border.py
 chaco/tests/test_chaco_traits.py
 chaco/tests/test_colormapper.py
```

### Comparing `chaco-5.1.1/examples/demo/advanced/javascript_hover_tools.py` & `chaco-6.0.0/examples/demo/advanced/javascript_hover_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 your browser to see the output.
 
 Author: Judah De Paula <judah@enthought.com>
 Date: November 21, 2008.
 """
 # Standard library imports
 import os, sys, webbrowser, io
-from base64 import encodestring
+from base64 import encodebytes
 
 # Major library imports
 from PIL import Image
 from numpy import arange, searchsorted, where, array, vstack, linspace
 from scipy.special import jn
 
 # Chaco imports
@@ -533,20 +533,20 @@
 
 def make_palettized_png_str(gc):
     """ Generate a png file in a string, base64 encoded. """
     format = gc.format()[:-2].upper()
     if format != "RGBA":
         gc = gc.convert_pixel_format("rgba32")
     img = Image.frombytes(
-        "RGBA", (gc.width(), gc.height()), gc.bmp_array.tostring()
+        "RGBA", (gc.width(), gc.height()), gc.bmp_array.tobytes()
     )
     img2 = img.convert("P")
     output_buf = io.BytesIO()
     img2.save(output_buf, "png")
-    output = encodestring(output_buf.getvalue())
+    output = encodebytes(output_buf.getvalue())
     output_buf.close()
     return output
 
 
 # ------------------------------------------------------------------------------
 #  Main
 # ------------------------------------------------------------------------------
```

### Comparing `chaco-5.1.1/examples/demo/advanced/spec_waterfall.py` & `chaco-6.0.0/examples/demo/advanced/spec_waterfall.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This plot displays the audio spectrum from the microphone.
 
 Based on updating_plot.py
 """
 # Major library imports
 import pyaudio
 from numpy import zeros, linspace, short, fromstring, transpose, array, empty
-from scipy import fft
+from scipy.fft import fft
 
 # Enthought library imports
 from enable.api import Window, Component, ComponentEditor
 from traits.api import HasTraits, Instance, List
 from traitsui.api import Item, Group, View, Handler
 from pyface.timer.api import Timer
 
@@ -96,15 +96,15 @@
 # ============================================================================
 # Create the Chaco plot.
 # ============================================================================
 
 
 def _create_plot_component(obj):
     # Setup the spectrum plot
-    frequencies = linspace(0.0, float(SAMPLING_RATE) / 2, num=NUM_SAMPLES / 2)
+    frequencies = linspace(0.0, float(SAMPLING_RATE) / 2, num=NUM_SAMPLES // 2)
     obj.spectrum_data = ArrayPlotData(frequency=frequencies)
     empty_amplitude = zeros(NUM_SAMPLES // 2)
     obj.spectrum_data.set_data("amplitude", empty_amplitude)
 
     obj.spectrum_plot = Plot(obj.spectrum_data)
     spec_renderer = obj.spectrum_plot.plot(
         ("frequency", "amplitude"), name="Spectrum", color="red"
```

### Comparing `chaco-5.1.1/examples/demo/advanced/spectrum.py` & `chaco-6.0.0/examples/demo/advanced/spectrum.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/aspect_ratio.py` & `chaco-6.0.0/examples/demo/aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/axis_tool.py` & `chaco-6.0.0/examples/demo/canvas/axis_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/canvas.py` & `chaco-6.0.0/examples/demo/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/cliptest.py` & `chaco-6.0.0/examples/demo/canvas/cliptest.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/data_source_button.py` & `chaco-6.0.0/examples/demo/canvas/data_source_button.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/mp_viewport_pan_tool.py` & `chaco-6.0.0/examples/demo/canvas/mp_viewport_pan_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/mptools.py` & `chaco-6.0.0/examples/demo/canvas/mptools.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     Instance,
     Int,
     Property,
     Tuple,
     CArray,
 )
 
+from enable.api import BaseTool
+
 # Chaco imports
-from chaco.api import BaseTool
 from chaco.chaco_traits import Optional
 from chaco.tools.api import PanTool, DragZoom, LegendTool, RangeSelection
 
 
 BOGUS_BLOB_ID = -1
```

### Comparing `chaco-5.1.1/examples/demo/canvas/plot_clone_tool.py` & `chaco-6.0.0/examples/demo/canvas/plot_clone_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/canvas/transient_plot_overlay.py` & `chaco-6.0.0/examples/demo/canvas/transient_plot_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/data/sample.wav` & `chaco-6.0.0/examples/demo/data/sample.wav`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/depth.py` & `chaco-6.0.0/examples/demo/depth.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/domain_limits.py` & `chaco-6.0.0/examples/demo/domain_limits.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/financial_plot.py` & `chaco-6.0.0/examples/demo/financial_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/financial_plot_dates.py` & `chaco-6.0.0/examples/demo/financial_plot_dates.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/logo.py` & `chaco-6.0.0/examples/demo/logo.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/multi_line_plot.py` & `chaco-6.0.0/examples/demo/multi_line_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/multiaxis.py` & `chaco-6.0.0/examples/demo/multiaxis.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/multiaxis_using_Plot.py` & `chaco-6.0.0/examples/demo/multiaxis_using_Plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/noninteractive.py` & `chaco-6.0.0/examples/demo/noninteractive.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/updating_plot/updating_plot1.py` & `chaco-6.0.0/examples/demo/updating_plot/updating_plot1.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/updating_plot/updating_plot2.py` & `chaco-6.0.0/examples/demo/updating_plot/updating_plot2.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/updating_plot/updating_plot3.py` & `chaco-6.0.0/examples/demo/updating_plot/updating_plot3.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/updating_plot/updating_plot4.py` & `chaco-6.0.0/examples/demo/updating_plot/updating_plot4.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/updating_plot/updating_plot5.py` & `chaco-6.0.0/examples/demo/updating_plot/updating_plot5.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/world_map.py` & `chaco-6.0.0/examples/demo/world_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ### Public Traits ##########################################################
 
     # The plot which will be displayed
     plot = Instance(Plot)
 
     # The URL which points to the world map image to be downloaded
     image_url = Str(
-        "http://eoimages.gsfc.nasa.gov/ve//2433/land_shallow_topo_2048.jpg"
+        "https://eoimages.gsfc.nasa.gov/images/imagerecords/57000/57752/land_shallow_topo_2048.jpg"
     )
 
     ### Private Traits #########################################################
 
     # The path to where the image exists on the filesystem
     image_path = Str()
```

### Comparing `chaco-5.1.1/examples/demo/zoomed_plot/grid_plot_factory.py` & `chaco-6.0.0/examples/demo/zoomed_plot/grid_plot_factory.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/zoomed_plot/wav_to_numeric.py` & `chaco-6.0.0/examples/demo/zoomed_plot/wav_to_numeric.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/zoomed_plot/zoom_overlay.py` & `chaco-6.0.0/examples/demo/zoomed_plot/zoom_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/demo/zoomed_plot/zoom_plot.py` & `chaco-6.0.0/examples/demo/zoomed_plot/zoom_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/connected_orientation.py` & `chaco-6.0.0/examples/tutorials/scipy2008/connected_orientation.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/connected_range.py` & `chaco-6.0.0/examples/tutorials/scipy2008/connected_range.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/connected_single_range.py` & `chaco-6.0.0/examples/tutorials/scipy2008/connected_single_range.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/connected_widgets.py` & `chaco-6.0.0/examples/tutorials/scipy2008/connected_widgets.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/container.py` & `chaco-6.0.0/examples/tutorials/scipy2008/container.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/container_nospace.py` & `chaco-6.0.0/examples/tutorials/scipy2008/container_nospace.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/container_vertical.py` & `chaco-6.0.0/examples/tutorials/scipy2008/container_vertical.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay_dataspace.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay_dataspace.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_overlay_movetool.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_overlay_movetool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_tool.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_tool.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_tool_click.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_tool_click.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/custom_tool_screen.py` & `chaco-6.0.0/examples/tutorials/scipy2008/custom_tool_screen.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/data_chooser.py` & `chaco-6.0.0/examples/tutorials/scipy2008/data_chooser.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/first_plot.py` & `chaco-6.0.0/examples/tutorials/scipy2008/first_plot.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/image.py` & `chaco-6.0.0/examples/tutorials/scipy2008/image.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/overlapping.py` & `chaco-6.0.0/examples/tutorials/scipy2008/overlapping.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/ploteditor.py` & `chaco-6.0.0/examples/tutorials/scipy2008/ploteditor.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/scatter.py` & `chaco-6.0.0/examples/tutorials/scipy2008/scatter.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/tool_chooser.py` & `chaco-6.0.0/examples/tutorials/scipy2008/tool_chooser.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/tools.py` & `chaco-6.0.0/examples/tutorials/scipy2008/tools.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/traits_example.py` & `chaco-6.0.0/examples/tutorials/scipy2008/traits_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy import linspace, sin
 
-from enable.api import ColorTrait
-from chaco.api import ArrayPlotData, Plot, marker_trait
+from enable.api import ColorTrait, marker_trait
+from chaco.api import ArrayPlotData, Plot
 from enable.api import ComponentEditor
 from traits.api import HasTraits, Instance, Int
 from traitsui.api import Group, Item, View
 
 
 class ScatterPlotTraits(HasTraits):
```

### Comparing `chaco-5.1.1/examples/tutorials/scipy2008/traits_image.py` & `chaco-6.0.0/examples/tutorials/scipy2008/traits_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         plotdata = ArrayPlotData(imagedata=z)
         # Create a Plot and associate it with the PlotData
         plot = Plot(plotdata)
         # Create an image plot in the Plot
         self.renderer = plot.img_plot(
             "imagedata",
             name="plot1",
-            xbounds=xgrid,
-            ybounds=ygrid,
+            xbounds=(0, 8),
+            ybounds=(0, 6),
             colormap=viridis,
         )[0]
         self.plot = plot
 
     def _origin_changed(self):
         self.renderer.origin = self.origin
         self.plot.request_redraw()
```

### Comparing `chaco-5.1.1/examples/tutorials/tutor.py` & `chaco-6.0.0/examples/tutorials/tutor.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial1.py` & `chaco-6.0.0/examples/tutorials/tutorial1.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial10.py` & `chaco-6.0.0/examples/tutorials/tutorial10.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial10b.py` & `chaco-6.0.0/examples/tutorials/tutorial10b.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial11.py` & `chaco-6.0.0/examples/tutorials/tutorial11.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial2.py` & `chaco-6.0.0/examples/tutorials/tutorial2.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial2_ipython.py` & `chaco-6.0.0/examples/tutorials/tutorial2_ipython.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial3.py` & `chaco-6.0.0/examples/tutorials/tutorial3.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial8.py` & `chaco-6.0.0/examples/tutorials/tutorial8.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial9.py` & `chaco-6.0.0/examples/tutorials/tutorial9.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorial9b.py` & `chaco-6.0.0/examples/tutorials/tutorial9b.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/tutorials/tutorials.cfg` & `chaco-6.0.0/examples/tutorials/tutorials.cfg`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/grid_plot_container.py` & `chaco-6.0.0/examples/user_guide/grid_plot_container.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/h_plot_container.py` & `chaco-6.0.0/examples/user_guide/h_plot_container.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/h_plot_container_add_multiple_times.py` & `chaco-6.0.0/examples/user_guide/h_plot_container_add_multiple_times.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/h_plot_container_colorbar.py` & `chaco-6.0.0/examples/user_guide/h_plot_container_colorbar.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/overlay_container_inset.py` & `chaco-6.0.0/examples/user_guide/overlay_container_inset.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/plot_types/create_plot_snapshots.py` & `chaco-6.0.0/examples/user_guide/plot_types/create_plot_snapshots.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     "border_visible": True,
     "border_width": AXIS_WIDTH,
 }
 
 AXIS_DEFAULTS = {
     "axis_line_weight": AXIS_WIDTH,
     "tick_weight": AXIS_WIDTH,
-    "tick_label_font": "modern 16",
-    "title_font": "modern 20",
+    "tick_label_font": "sans-serif 16",
+    "title_font": "sans-serif 20",
 }
 
 
 def get_data_sources(x=None, y=None):
     y = np.asarray(y)
 
     if x is None:
@@ -145,17 +145,17 @@
 
 get_line_plot_connected = partial(get_line_plot, "connectedpoints")
 get_line_plot_hold = partial(get_line_plot, "hold")
 get_line_plot_connectedhold = partial(get_line_plot, "connectedhold")
 
 
 def get_scatter_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
-    lower_status = boston["data"][:, -1]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
+    lower_status = diabetes["data"][:, -1]
 
     x, y = get_data_sources(x=lower_status, y=prices)
     x_mapper, y_mapper = get_mappers(x, y)
 
     scatter_plot = ScatterPlot(
         index=x,
         value=y,
@@ -172,18 +172,18 @@
         y_label="Median house prices",
     )
 
     return scatter_plot
 
 
 def get_cmap_scatter_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
-    lower_status = boston["data"][:, -1]
-    nox = boston["data"][:, 4]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
+    lower_status = diabetes["data"][:, -1]
+    nox = diabetes["data"][:, 4]
 
     x, y = get_data_sources(x=lower_status, y=prices)
     x_mapper, y_mapper = get_mappers(x, y)
 
     color_source = ArrayDataSource(nox)
     color_mapper = dc.reverse(dc.RdYlGn)(
         DataRange1D(low=nox.min(), high=nox.max())
@@ -208,19 +208,19 @@
         y_label="Median house prices",
     )
 
     return scatter_plot
 
 
 def get_4d_scatter_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
-    lower_status = boston["data"][:, -1]
-    tax = boston["data"][:, 9]
-    nox = boston["data"][:, 4]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
+    lower_status = diabetes["data"][:, -1]
+    tax = diabetes["data"][:, 9]
+    nox = diabetes["data"][:, 4]
 
     x, y = get_data_sources(x=lower_status, y=prices)
     x_mapper, y_mapper = get_mappers(x, y)
 
     color_source = ArrayDataSource(nox)
     color_mapper = dc.reverse(dc.RdYlGn)(
         DataRange1D(low=nox.min(), high=nox.max())
@@ -251,18 +251,18 @@
         y_label="Median house prices",
     )
 
     return scatter_plot
 
 
 def get_variable_size_scatter_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
-    lower_status = boston["data"][:, -1]
-    tax = boston["data"][:, 9]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
+    lower_status = diabetes["data"][:, -1]
+    tax = diabetes["data"][:, 9]
 
     x, y = get_data_sources(x=lower_status, y=prices)
     x_mapper, y_mapper = get_mappers(x, y)
 
     # normalize between 0 and 10
     marker_size = tax / tax.max() * 10.0
 
@@ -284,16 +284,16 @@
         y_label="Median house prices",
     )
 
     return scatter_plot
 
 
 def get_jitter_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
 
     x, y = get_data_sources(y=prices)
     x_mapper, y_mapper = get_mappers(x, y)
 
     jitter_plot = JitterPlot(
         index=y,
         index_mapper=y_mapper,
@@ -430,36 +430,46 @@
 
     add_axes(image_plot, x_label="x", y_label="y")
 
     return image_plot
 
 
 def get_image_from_file():
-    import os.path
+    # importlib.resources is new in Python 3.7, and
+    # importlib.resources.files is new in Python 3.9,
+    # so for Python < 3.9 we must rely on the 3rd party
+    # importlib_resources package.
+    try:
+        from importlib.resources import as_file, files
+    except ImportError:
+        from importlib_resources import as_file, files
+
+    image_resource = files(
+        'chaco.examples.demo.basic'
+    ).joinpath('capitol.jpg')
+
+    with as_file(image_resource) as filename:
+        image_content = ImageData.fromfile(filename)
+        w, h = image_content.get_width(), image_content.get_height()
+        index = GridDataSource(np.arange(w), np.arange(h))
+        index_mapper = GridMapper(
+            range=DataRange2D(low=(0, 0), high=(w - 1, h - 1))
+        )
+
+        image_plot = ImagePlot(
+            index=index,
+            value=image_content,
+            index_mapper=index_mapper,
+            origin="top left",
+            **PLOT_DEFAULTS
+        )
 
-    filename = os.path.join("..", "..", "demo", "basic", "capitol.jpg")
-    image_source = ImageData.fromfile(filename)
+        add_axes(image_plot, x_label="x", y_label="y")
 
-    w, h = image_source.get_width(), image_source.get_height()
-    index = GridDataSource(np.arange(w), np.arange(h))
-    index_mapper = GridMapper(
-        range=DataRange2D(low=(0, 0), high=(w - 1, h - 1))
-    )
-
-    image_plot = ImagePlot(
-        index=index,
-        value=image_source,
-        index_mapper=index_mapper,
-        origin="top left",
-        **PLOT_DEFAULTS
-    )
-
-    add_axes(image_plot, x_label="x", y_label="y")
-
-    return image_plot
+        return image_plot
 
 
 def get_cmap_image_plot():
     # Create a scalar field to colormap
     NPOINTS = 200
 
     xs = np.linspace(-2 * np.pi, +2 * np.pi, NPOINTS)
@@ -562,16 +572,16 @@
 
     add_axes(polygon_plot, x_label="x", y_label="y")
 
     return polygon_plot
 
 
 def get_bar_plot():
-    boston = datasets.load_boston()
-    prices = boston["target"]
+    diabetes = datasets.load_diabetes()
+    prices = diabetes["target"]
 
     ys, bin_edges = np.histogram(prices, bins=10)
     ys = ys.astype("d") / ys.sum()
     xs = (bin_edges[:-1] + bin_edges[1:]) / 2.0
 
     x, y = get_data_sources(x=xs, y=ys)
     x_mapper, y_mapper = get_mappers(x, y)
```

### Comparing `chaco-5.1.1/examples/user_guide/plot_types/plot_window.py` & `chaco-6.0.0/examples/user_guide/plot_types/plot_window.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/examples/user_guide/power_function_example.py` & `chaco-6.0.0/examples/user_guide/power_function_example.py`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/image_LICENSE.txt` & `chaco-6.0.0/image_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chaco-5.1.1/setup.py` & `chaco-6.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import runpy
 import subprocess
 
 from numpy import get_include
 from setuptools import setup, Extension, find_packages
 from Cython.Build import cythonize
 
-MAJOR = 5
-MINOR = 1
-MICRO = 1
+MAJOR = 6
+MINOR = 0
+MICRO = 0
 PRERELEASE = ""
 IS_RELEASED = True
 
 # If this file is part of a Git export (for example created with "git archive",
 # or downloaded from GitHub), ARCHIVE_COMMIT_HASH gives the full hash of the
 # commit that was exported.
 ARCHIVE_COMMIT_HASH = "$Format:%H$"
```

