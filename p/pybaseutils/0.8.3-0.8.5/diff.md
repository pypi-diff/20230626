# Comparing `tmp/pybaseutils-0.8.3.tar.gz` & `tmp/pybaseutils-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.8.3.tar", last modified: Mon Jun 19 03:45:15 2023, max compression
+gzip compressed data, was "dist/pybaseutils-0.8.5.tar", last modified: Mon Jun 26 02:20:57 2023, max compression
```

## Comparing `pybaseutils-0.8.3.tar` & `pybaseutils-0.8.5.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.513464 pybaseutils-0.8.3/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.3/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-19 03:45:15.513141 pybaseutils-0.8.3/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.3/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.469735 pybaseutils-0.8.3/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-06-19 03:45:11.000000 pybaseutils-0.8.3/pybaseutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/base64_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.472683 pybaseutils-0.8.3/pybaseutils/base_audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.3/pybaseutils/base_audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.3/pybaseutils/base_audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.474600 pybaseutils-0.8.3/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.3/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.3/pybaseutils/config_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.476933 pybaseutils-0.8.3/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.3/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.3/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6101 2023-06-01 06:52:32.000000 pybaseutils-0.8.3/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9722 2023-06-07 03:32:53.000000 pybaseutils-0.8.3/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.479453 pybaseutils-0.8.3/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32586 2023-06-19 03:44:02.000000 pybaseutils-0.8.3/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.480002 pybaseutils-0.8.3/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    97190 2023-06-14 03:03:27.000000 pybaseutils-0.8.3/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.3/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.483197 pybaseutils-0.8.3/pybaseutils/maker/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/maker/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/maker/maker_voc.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.486149 pybaseutils-0.8.3/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.3/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.487406 pybaseutils-0.8.3/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.3/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.3/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.3/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.3/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.488263 pybaseutils-0.8.3/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.3/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.3/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.3/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.471917 pybaseutils-0.8.3/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3491 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.3/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-06-19 03:45:15.000000 pybaseutils-0.8.3/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-06-19 03:45:15.513545 pybaseutils-0.8.3/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.3/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.501545 pybaseutils-0.8.3/test_py/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.3/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.507081 pybaseutils-0.8.3/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.3/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.3/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.3/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.3/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.3/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.3/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.3/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.3/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.3/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      544 2023-06-16 03:40:08.000000 pybaseutils-0.8.3/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.3/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.3/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.3/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.3/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.3/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.3/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.3/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2943 2023-06-15 00:54:20.000000 pybaseutils-0.8.3/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.3/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.3/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.3/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.3/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      779 2023-06-05 05:36:00.000000 pybaseutils-0.8.3/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.3/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2440 2023-06-15 00:55:49.000000 pybaseutils-0.8.3/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.3/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.508115 pybaseutils-0.8.3/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.3/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.3/test_py/detector/detect_face_person.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.509747 pybaseutils-0.8.3/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.3/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.3/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.3/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-19 03:45:15.512319 pybaseutils-0.8.3/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.3/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.3/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.3/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.3/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.3/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.368254 pybaseutils-0.8.5/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.5/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-26 02:20:57.368025 pybaseutils-0.8.5/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.5/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.316336 pybaseutils-0.8.5/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-06-26 02:20:49.000000 pybaseutils-0.8.5/pybaseutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/base64_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.321150 pybaseutils-0.8.5/pybaseutils/base_audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.5/pybaseutils/base_audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4870 2023-06-20 02:36:58.000000 pybaseutils-0.8.5/pybaseutils/base_audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1841 2023-06-20 03:14:56.000000 pybaseutils-0.8.5/pybaseutils/base_audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.323783 pybaseutils-0.8.5/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.5/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.5/pybaseutils/config_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.326985 pybaseutils-0.8.5/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.5/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.5/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-0.8.5/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9734 2023-06-21 02:44:02.000000 pybaseutils-0.8.5/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.330403 pybaseutils-0.8.5/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32585 2023-06-19 09:57:39.000000 pybaseutils-0.8.5/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.331143 pybaseutils-0.8.5/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    97190 2023-06-14 03:03:27.000000 pybaseutils-0.8.5/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.5/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.335382 pybaseutils-0.8.5/pybaseutils/maker/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/maker/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/maker/maker_voc.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.339211 pybaseutils-0.8.5/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.5/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.340948 pybaseutils-0.8.5/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.5/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.5/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/pycpp/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.5/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.5/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.342152 pybaseutils-0.8.5/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.5/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.5/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.5/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.319202 pybaseutils-0.8.5/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3558 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.5/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-06-26 02:20:57.368324 pybaseutils-0.8.5/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.5/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.357799 pybaseutils-0.8.5/test_py/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.5/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.363364 pybaseutils-0.8.5/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.5/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.5/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.5/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.5/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.5/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.5/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.5/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.5/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.5/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1259 2023-06-20 02:37:41.000000 pybaseutils-0.8.5/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1263 2023-06-21 00:19:31.000000 pybaseutils-0.8.5/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.5/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.5/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.5/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.5/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.5/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.5/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2943 2023-06-15 00:54:20.000000 pybaseutils-0.8.5/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.5/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.5/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.5/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.5/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      834 2023-06-21 01:39:59.000000 pybaseutils-0.8.5/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2888 2023-06-25 08:37:27.000000 pybaseutils-0.8.5/test_py/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.5/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2440 2023-06-15 00:55:49.000000 pybaseutils-0.8.5/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.5/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.364264 pybaseutils-0.8.5/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.5/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.5/test_py/detector/detect_face_person.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.365608 pybaseutils-0.8.5/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.5/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.5/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.5/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.367507 pybaseutils-0.8.5/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.5/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.5/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.5/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.5/test_py/performance.py
```

### Comparing `pybaseutils-0.8.3/LICENCE` & `pybaseutils-0.8.5/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/PKG-INFO` & `pybaseutils-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.3
+Version: 0.8.5
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.3/README.md` & `pybaseutils-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/base64_utils.py` & `pybaseutils-0.8.5/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/base_audio/audio_utils.py` & `pybaseutils-0.8.5/pybaseutils/base_audio/audio_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*-coding: utf-8 -*-
 """
     @Author : 
     @E-mail : 
     @Date   : 2023-05-11 10:36:28
     @Brief  : pip install ffmpy -i https://pypi.douban.com/simple
               https://blog.csdn.net/zhiweihongyan1/article/details/121735158
+              安装依赖项:见install.sh
 """
 import os
 import base64
 import io
 import soundfile
 import numpy as np
 import copy
@@ -139,12 +140,12 @@
     return video_out
 
 
 if __name__ == '__main__':
     # video_file = "../data/video/kunkun_cut.mp4"
     # audio_file = "../data/video/kunkun_cut.mp3"
     # extract_video_audio(video_file, audio_file)
-
-    video_file = "../data/video/test-video.mp4"
-    audio_file = "../data/video/kunkun_cut.mp3"
-    video_out = "../data/video/test-video-result.mp4"
+    video_file = "../../data/video/test-video.mp4"
+    audio_file = "../../data/video/kunkun_cut.mp3"
+    video_out = "../../data/video/test-video-result.mp4"
+    playsound(audio_file)
     merge_video_audio(video_file, audio_file, video_out)
```

### Comparing `pybaseutils-0.8.3/pybaseutils/batch_utils.py` & `pybaseutils-0.8.5/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.5/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.5/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.5/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/color_utils.py` & `pybaseutils-0.8.5/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/config_utils.py` & `pybaseutils-0.8.5/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/coords_utils.py` & `pybaseutils-0.8.5/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.5/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cvutils/monitor.py` & `pybaseutils-0.8.5/pybaseutils/cvutils/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,26 +91,29 @@
         """
         diff = np.asarray(diff_map).reshape(-1)
         diff = -np.sort(-diff)  # 降序排序
         diff = diff[:tok]  # 提取tok的差异较大的特征
         dist = np.sum(diff) / tok  # 计算平均绝对误差作为相似度(距离)
         return dist
 
-    def get_frame_similarity(self, frame1, frame2, measurement="l1", size=(), vis=False):
+    def get_frame_similarity(self, frame1, frame2, measurement="l1", size=(), blur=True, vis=False):
         """
         比较两帧图像的相似度(距离)
         :param frame1: 输入frame1图像
         :param frame2: 输入frame2图像
         :param measurement: 相似度(距离)度量方法,l1: 平均绝对误差作为相似度(距离),l2: 均方差作为相似距离
         :param vis: <bool> 默认为False,是否显示差异图
         :return: <float>相似度(距离)
         """
         if size:
             frame1 = cv2.resize(frame1, dsize=size)
             frame2 = cv2.resize(frame2, dsize=size)
+        if blur:
+            frame1 = cv2.blur(frame1, ksize=(5, 5))
+            frame2 = cv2.blur(frame2, ksize=(5, 5))
         frame1 = np.asarray(frame1, dtype=np.float32) / 255.0
         frame2 = np.asarray(frame2, dtype=np.float32) / 255.0
         diff_map = self.get_diff_map(frame1, frame2)
         if measurement == "l1":
             dist = self.cal_diff_map_similarity_l1(diff_map)
         elif measurement == "l2":
             dist = self.cal_diff_map_similarity_l2(diff_map)
```

### Comparing `pybaseutils-0.8.3/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.5/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.5/pybaseutils/cvutils/video_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     count = 0
     frames = []
     while True:
         if count % interval == 0 and count >= 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
-            if not isSuccess or count > num_frames: break
+            if not isSuccess or 0 < num_frames < count: break
             if func:
                 frame = func(frame)
             if vis:
                 image_utils.cv_show_image("frame", frame, use_rgb=False, delay=30)
             frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
             frames.append(frame)
         count += 1
@@ -72,21 +72,20 @@
     """
     name = os.path.basename(video_file).split(".")[0]
     if not out_dir:  out_dir = os.path.join(os.path.dirname(video_file), name)
     video_cap = get_video_capture(video_file)
     width, height, num_frames, fps = get_video_info(video_cap)
     if not os.path.exists(out_dir): os.makedirs(out_dir)
     count = 0
-    while count < num_frames:
+    while True:
         if count % interval == 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
-            if not isSuccess:
-                break
+            if not isSuccess or 0 < num_frames < count: break
             if func:
                 frame = func(frame)
             if vis:
                 image_utils.cv_show_image("frame", frame, use_rgb=False, delay=30)
             frame_file = os.path.join(out_dir, "{}_{:0=4d}.jpg".format(name, count))
             cv2.imwrite(frame_file, frame)
         count += 1
@@ -108,21 +107,20 @@
     name = os.path.basename(video_file).split(".")[0]
     if not out_dir:  out_dir = os.path.join(os.path.dirname(video_file), name)
     video_cap = get_video_capture(video_file)
     width, height, num_frames, fps = get_video_info(video_cap)
     if not os.path.exists(out_dir): os.makedirs(out_dir)
     count = 0
     last_frame = None
-    while count < num_frames:
+    while True:
         if count % interval == 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, curr_frame = video_cap.read()
-            if not isSuccess:
-                break
+            if not isSuccess or 0 < num_frames < count: break
             if func: curr_frame = func(curr_frame)
             if last_frame is None:
                 last_frame = curr_frame.copy()
             diff = sm.get_frame_similarity(curr_frame, last_frame, size=(256, 256), vis=False)
             if diff > thresh:
                 frame_file = os.path.join(out_dir, "{}_{:0=4d}.jpg".format(name, count))
                 last_frame = curr_frame.copy()
@@ -196,16 +194,15 @@
     count = 0
     while True:
         # if count % interval == 0:
         if count % interval == 0 and count > 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
-            if not isSuccess:
-                break
+            if not isSuccess or 0 < num_frames < count: break
             if vis: image_utils.cv_show_image("frame", frame, use_rgb=False, delay=delay)
             video_writer.write(frame)
         count += 1
     video_cap.release()
     video_writer.release()
 
 
@@ -233,16 +230,15 @@
         # freq = int(fps / detect_freq)
         count = 0
         while True:
             if count % interval == 0:
                 # 设置抽帧的位置
                 video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
                 isSuccess, frame = video_cap.read()
-                if not isSuccess:
-                    break
+                if not isSuccess or 0 < num_frames < count: break
                 frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
                 frame = self.task(frame)
                 if save_video:
                     video_writer.write(frame)
             count += 1
         video_cap.release()
```

### Comparing `pybaseutils-0.8.3/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.5/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.5/pybaseutils/dataloader/parser_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.5/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.5/pybaseutils/dataloader/parser_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/file_utils.py` & `pybaseutils-0.8.5/pybaseutils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     :return: txt的数据列表
     Python中有三个去除头尾字符、空白符的函数，它们依次为:
     strip： 用来去除头尾字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     lstrip：用来去除开头字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     rstrip：用来去除结尾字符、空白符(包括\n、\r、\t、' '，即：换行、回车、制表符、空格)
     注意：这些函数都只会删除头和尾的字符，中间的不会删除。
     """
-    with open(filename, mode="rb", encoding='utf-8') as f:
+    with open(filename, mode="r", encoding='utf-8') as f:
         content_list = f.readlines()
         if split is None:
             content_list = [content.rstrip() for content in content_list]
             return content_list
         else:
             content_list = [content.rstrip().split(split) for content in content_list]
         if convertNum:
```

### Comparing `pybaseutils-0.8.3/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.5/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/font_utils.py` & `pybaseutils-0.8.5/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.5/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.5/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/image_utils.py` & `pybaseutils-0.8.5/pybaseutils/image_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/json_utils.py` & `pybaseutils-0.8.5/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/log.py` & `pybaseutils-0.8.5/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/logger.py` & `pybaseutils-0.8.5/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.5/pybaseutils/maker/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.5/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.5/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.5/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.5/pybaseutils/maker/maker_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.5/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.5/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.5/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.5/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.5/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.5/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.5/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.5/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/plot_utils.py` & `pybaseutils-0.8.5/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.5/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.5/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/setup_config.py` & `pybaseutils-0.8.5/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/thread_utils.py` & `pybaseutils-0.8.5/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/time_utils.py` & `pybaseutils-0.8.5/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.5/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.5/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.5/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/word_utils.py` & `pybaseutils-0.8.5/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/worker.py` & `pybaseutils-0.8.5/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.5/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.5/pybaseutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.3
+Version: 0.8.5
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.3/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.5/pybaseutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 pybaseutils.egg-info/PKG-INFO
 pybaseutils.egg-info/SOURCES.txt
 pybaseutils.egg-info/dependency_links.txt
 pybaseutils.egg-info/not-zip-safe
 pybaseutils.egg-info/top_level.txt
 pybaseutils/base_audio/__init__.py
 pybaseutils/base_audio/audio_utils.py
+pybaseutils/base_audio/pyaudio_utils.py
 pybaseutils/cluster/__init__.py
 pybaseutils/cluster/kmean.py
 pybaseutils/cluster/maxmin_distance.py
 pybaseutils/cluster/similarity.py
 pybaseutils/cvutils/__init__.py
 pybaseutils/cvutils/corner_utils.py
 pybaseutils/cvutils/monitor.py
@@ -83,14 +84,15 @@
 test_py/demo_mouse.py
 test_py/demo_pandas.py
 test_py/demo_plot.py
 test_py/demo_standard_image .py
 test_py/demo_standard_video .py
 test_py/demo_taichi.py
 test_py/demo_video.py
+test_py/demo_video_aije.py
 test_py/demo_voc_crop.py
 test_py/demo_voc_vis.py
 test_py/demo_word_similar.py
 test_py/demo_worker1.py
 test_py/demo_worker2.py
 test_py/kafka_worker.py
 test_py/men_tracemalloc.py
```

### Comparing `pybaseutils-0.8.3/setup.py` & `pybaseutils-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/class_names.py` & `pybaseutils-0.8.5/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/AffectNet.py` & `pybaseutils-0.8.5/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.5/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.5/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.5/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/CCPD.py` & `pybaseutils-0.8.5/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.5/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/TT100K.py` & `pybaseutils-0.8.5/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.5/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.5/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.5/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo2.py` & `pybaseutils-0.8.5/test_py/demo2.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,10 +30,10 @@
 
     @staticmethod
     def hex2rgb(h):  # rgb order (PIL)
         return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
 
 
 if __name__ == "__main__":
-    c = Colors()
-    print(c)
-    
+    image_file = "test.png"
+    image = cv2.imread(image_file)
+    image_utils.cv_show_image("image",image)
```

### Comparing `pybaseutils-0.8.3/test_py/demo_async_await2.py` & `pybaseutils-0.8.5/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_copy_files.py` & `pybaseutils-0.8.5/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.5/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_ffmpy.py` & `pybaseutils-0.8.5/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_get_file_list.py` & `pybaseutils-0.8.5/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_gif.py` & `pybaseutils-0.8.5/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_gif_video.py` & `pybaseutils-0.8.5/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_metrics.py` & `pybaseutils-0.8.5/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_mouse.py` & `pybaseutils-0.8.5/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_pandas.py` & `pybaseutils-0.8.5/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_plot.py` & `pybaseutils-0.8.5/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_standard_image .py` & `pybaseutils-0.8.5/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_standard_video .py` & `pybaseutils-0.8.5/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_taichi.py` & `pybaseutils-0.8.5/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_voc_crop.py` & `pybaseutils-0.8.5/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_voc_vis.py` & `pybaseutils-0.8.5/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_word_similar.py` & `pybaseutils-0.8.5/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_worker1.py` & `pybaseutils-0.8.5/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/demo_worker2.py` & `pybaseutils-0.8.5/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/detector/detect_face_person.py` & `pybaseutils-0.8.5/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/flask_demo/server.py` & `pybaseutils-0.8.5/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/kafka_worker.py` & `pybaseutils-0.8.5/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/men_tracemalloc.py` & `pybaseutils-0.8.5/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.3/test_py/performance.py` & `pybaseutils-0.8.5/test_py/performance.py`

 * *Files identical despite different names*

