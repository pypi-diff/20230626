# Comparing `tmp/hello2-2.0.8.tar.gz` & `tmp/hello2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-2.0.8.tar", last modified: Wed Jun 21 03:48:36 2023, max compression
+gzip compressed data, was "hello2-2.0.9.tar", last modified: Wed Jun 21 07:59:13 2023, max compression
```

## Comparing `hello2-2.0.8.tar` & `hello2-2.0.9.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-2.0.8/.gitignore
--rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-2.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-2.0.8/LICENSE
--rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-2.0.8/README.md
--rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-2.0.8/docs/Makefile
--rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-2.0.8/docs/make.bat
--rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-2.0.8/docs/requirements.txt
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-2.0.8/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-2.0.8/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-2.0.8/docs/source/conf.py
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-2.0.8/docs/source/hello.data.coco2yolo.rst
--rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-2.0.8/docs/source/hello.data.rst
--rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-2.0.8/docs/source/hello.experimental.albu.detection.rst
--rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-2.0.8/docs/source/hello.experimental.albu.rst
--rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-2.0.8/docs/source/hello.experimental.rst
--rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-2.0.8/docs/source/hello.fiftyone.annotate.rst
--rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-2.0.8/docs/source/hello.fiftyone.brain.rst
--rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-2.0.8/docs/source/hello.fiftyone.coco.rst
--rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-2.0.8/docs/source/hello.fiftyone.coco_utils.rst
--rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-2.0.8/docs/source/hello.fiftyone.connected.rst
--rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-2.0.8/docs/source/hello.fiftyone.copypaste.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-2.0.8/docs/source/hello.fiftyone.core.rst
--rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-2.0.8/docs/source/hello.fiftyone.dataset.rst
--rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-2.0.8/docs/source/hello.fiftyone.dataset_annotate.rst
--rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-2.0.8/docs/source/hello.fiftyone.dataset_detections.rst
--rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.dataset_segmentations.rst
--rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.dataset_yolov5.rst
--rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.dataset_zoo.rst
--rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.evaluate.rst
--rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.evaluate_detections.rst
--rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.evaluate_segmentations.rst
--rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-2.0.8/docs/source/hello.fiftyone.gen_examples.rst
--rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-2.0.8/docs/source/hello.fiftyone.mask_ignore.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-2.0.8/docs/source/hello.fiftyone.miou.rst
--rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-2.0.8/docs/source/hello.fiftyone.patches.rst
--rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-2.0.8/docs/source/hello.fiftyone.rst
--rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-2.0.8/docs/source/hello.fiftyone.tarinfo.rst
--rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-2.0.8/docs/source/hello.fiftyone.unique.rst
--rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-2.0.8/docs/source/hello.fiftyone.utils.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-2.0.8/docs/source/hello.fiftyone.video.rst
--rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-2.0.8/docs/source/hello.fiftyone.view.rst
--rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-2.0.8/docs/source/hello.fvcore.core.rst
--rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-2.0.8/docs/source/hello.fvcore.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-2.0.8/docs/source/hello.io.image.rst
--rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-2.0.8/docs/source/hello.io.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-2.0.8/docs/source/hello.io.utils.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-2.0.8/docs/source/hello.mmdet.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-2.0.8/docs/source/hello.mmdet.flop.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-2.0.8/docs/source/hello.mmdet.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-2.0.8/docs/source/hello.mmdet.log.rst
--rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-2.0.8/docs/source/hello.mmdet.plot.rst
--rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-2.0.8/docs/source/hello.mmdet.rst
--rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-2.0.8/docs/source/hello.mmlab.mmdet3.rst
--rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-2.0.8/docs/source/hello.mmlab.mmseg.rst
--rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-2.0.8/docs/source/hello.mmlab.rst
--rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-2.0.8/docs/source/hello.mmseg.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-2.0.8/docs/source/hello.mmseg.log.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-2.0.8/docs/source/hello.mmseg.lr.rst
--rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-2.0.8/docs/source/hello.mmseg.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-2.0.8/docs/source/hello.nanodet.infer.rst
--rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-2.0.8/docs/source/hello.nanodet.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-2.0.8/docs/source/hello.onnx.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-2.0.8/docs/source/hello.onnx.infer.rst
--rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-2.0.8/docs/source/hello.onnx.rst
--rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-2.0.8/docs/source/hello.rst
--rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-2.0.8/docs/source/hello.transforms.rst
--rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-2.0.8/docs/source/hello.transforms.transforms.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-2.0.8/docs/source/hello.utils.colors.rst
--rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-2.0.8/docs/source/hello.utils.compare.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-2.0.8/docs/source/hello.utils.cuda.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-2.0.8/docs/source/hello.utils.importer.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-2.0.8/docs/source/hello.utils.plots.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-2.0.8/docs/source/hello.utils.points.rst
--rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-2.0.8/docs/source/hello.utils.rst
--rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-2.0.8/docs/source/hello.utils.strtime.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-2.0.8/docs/source/hello.video.align.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-2.0.8/docs/source/hello.video.clip.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-2.0.8/docs/source/hello.video.fisheye.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-2.0.8/docs/source/hello.video.frames.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-2.0.8/docs/source/hello.video.info.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-2.0.8/docs/source/hello.video.resize.rst
--rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-2.0.8/docs/source/hello.video.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-2.0.8/docs/source/hello.video.rtsp.rst
--rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-2.0.8/docs/source/hello.video.rtsp_pull.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-2.0.8/docs/source/hello.video.split.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-2.0.8/docs/source/hello.video.unwarp.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-2.0.8/docs/source/hello.video.utils.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-2.0.8/docs/source/hello.x3m.config.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-2.0.8/docs/source/hello.x3m.preprocess.rst
--rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-2.0.8/docs/source/hello.x3m.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-2.0.8/docs/source/hello.x3m.transforms.rst
--rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-2.0.8/docs/source/index.rst
--rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-2.0.8/docs/source/modules.rst
--rw-r--r--   0        0        0     3270 2023-06-06 04:22:36.459690 hello2-2.0.8/hello/README.md
--rw-r--r--   0        0        0      773 2023-06-21 03:45:16.576795 hello2-2.0.8/hello/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/__main__.py
--rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-2.0.8/hello/data/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/data/__main__.py
--rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-2.0.8/hello/data/coco2yolo.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-2.0.8/hello/experimental/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-2.0.8/hello/experimental/albu/__init__.py
--rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-2.0.8/hello/experimental/albu/detection.py
--rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-2.0.8/hello/fiftyone/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/fiftyone/__main__.py
--rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-2.0.8/hello/fiftyone/annotate.py
--rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-2.0.8/hello/fiftyone/brain.py
--rw-r--r--   0        0        0     8246 2023-06-14 06:42:08.391095 hello2-2.0.8/hello/fiftyone/coco.py
--rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-2.0.8/hello/fiftyone/coco_utils.py
--rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-2.0.8/hello/fiftyone/connected.py
--rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-2.0.8/hello/fiftyone/copypaste.py
--rw-r--r--   0        0        0    19157 2023-06-15 04:03:09.717943 hello2-2.0.8/hello/fiftyone/core.py
--rw-r--r--   0        0        0    20844 2023-06-15 08:19:34.131331 hello2-2.0.8/hello/fiftyone/dataset.py
--rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-2.0.8/hello/fiftyone/dataset_detections.py
--rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-2.0.8/hello/fiftyone/dataset_segmentations.py
--rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-2.0.8/hello/fiftyone/dataset_yolov5.py
--rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-2.0.8/hello/fiftyone/dataset_zoo.py
--rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-2.0.8/hello/fiftyone/evaluate.py
--rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-2.0.8/hello/fiftyone/evaluate_detections.py
--rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-2.0.8/hello/fiftyone/evaluate_segmentations.py
--rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/fiftyone/examples/README.md
--rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-2.0.8/hello/fiftyone/examples/examples.py
--rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-2.0.8/hello/fiftyone/examples/utils.py
--rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-2.0.8/hello/fiftyone/gen_examples.py
--rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-2.0.8/hello/fiftyone/mask_ignore.py
--rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-2.0.8/hello/fiftyone/miou.py
--rw-r--r--   0        0        0      164 2023-06-08 07:23:27.040658 hello2-2.0.8/hello/fiftyone/novabot/README.md
--rw-r--r--   0        0        0     4003 2023-06-14 08:35:33.468173 hello2-2.0.8/hello/fiftyone/novabot/big_test.py
--rw-r--r--   0        0        0      942 2023-06-15 07:20:02.952865 hello2-2.0.8/hello/fiftyone/novabot/cal_data.py
--rw-r--r--   0        0        0     6250 2023-06-14 04:03:54.435176 hello2-2.0.8/hello/fiftyone/novabot/det_annotate.py
--rw-r--r--   0        0        0     5309 2023-06-14 04:11:05.194991 hello2-2.0.8/hello/fiftyone/novabot/det_big_train.py
--rw-r--r--   0        0        0     1669 2023-06-14 03:43:11.095705 hello2-2.0.8/hello/fiftyone/novabot/seg_base.py
--rw-r--r--   0        0        0     2045 2023-06-15 07:15:02.202995 hello2-2.0.8/hello/fiftyone/novabot/tag_data.py
--rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-2.0.8/hello/fiftyone/patches.py
--rw-r--r--   0        0        0     9350 2023-06-14 06:41:26.931115 hello2-2.0.8/hello/fiftyone/tarinfo.py
--rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-2.0.8/hello/fiftyone/unique.py
--rw-r--r--   0        0        0     8304 2023-06-15 08:24:13.821210 hello2-2.0.8/hello/fiftyone/utils.py
--rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-2.0.8/hello/fiftyone/video.py
--rw-r--r--   0        0        0    10699 2023-06-14 07:43:28.909510 hello2-2.0.8/hello/fiftyone/view.py
--rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-2.0.8/hello/fvcore/README.md
--rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-2.0.8/hello/fvcore/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-2.0.8/hello/fvcore/core.py
--rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-2.0.8/hello/io/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-2.0.8/hello/io/image.py
--rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-2.0.8/hello/io/utils.py
--rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-2.0.8/hello/mmdet/__init__.py
--rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-2.0.8/hello/mmdet/__main__.py
--rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-2.0.8/hello/mmdet/export.py
--rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-2.0.8/hello/mmdet/flop.py
--rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-2.0.8/hello/mmdet/infer.py
--rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-2.0.8/hello/mmdet/log.py
--rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-2.0.8/hello/mmdet/plot.py
--rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-2.0.8/hello/mmlab/__init__.py
--rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-2.0.8/hello/mmlab/__main__.py
--rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-2.0.8/hello/mmlab/mmdet3.py
--rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-2.0.8/hello/mmlab/mmseg.py
--rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-2.0.8/hello/mmseg/__init__.py
--rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-2.0.8/hello/mmseg/__main__.py
--rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-2.0.8/hello/mmseg/infer.py
--rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-2.0.8/hello/mmseg/log.py
--rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-2.0.8/hello/mmseg/lr.py
--rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-2.0.8/hello/nanodet/__init__.py
--rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-2.0.8/hello/nanodet/__main__.py
--rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-2.0.8/hello/nanodet/infer.py
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-2.0.8/hello/onnx/__init__.py
--rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-2.0.8/hello/onnx/examples/README.md
--rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-2.0.8/hello/onnx/examples/test_sigmoid.py
--rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-2.0.8/hello/onnx/export.py
--rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-2.0.8/hello/onnx/infer.py
--rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-2.0.8/hello/transforms/README.md
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-2.0.8/hello/transforms/__init__.py
--rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-2.0.8/hello/transforms/transforms.py
--rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-2.0.8/hello/utils/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-2.0.8/hello/utils/colors.py
--rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-2.0.8/hello/utils/compare.py
--rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-2.0.8/hello/utils/cuda.py
--rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-2.0.8/hello/utils/importer.py
--rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-2.0.8/hello/utils/plots.py
--rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-2.0.8/hello/utils/points.py
--rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-2.0.8/hello/utils/strtime.py
--rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-2.0.8/hello/video/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/video/__main__.py
--rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-2.0.8/hello/video/align.py
--rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-2.0.8/hello/video/clip.py
--rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-2.0.8/hello/video/fisheye.py
--rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-2.0.8/hello/video/info.py
--rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-2.0.8/hello/video/resize.py
--rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-2.0.8/hello/video/rtsp.py
--rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-2.0.8/hello/video/rtsp_pull.py
--rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-2.0.8/hello/video/split.py
--rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-2.0.8/hello/video/unwarp.py
--rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-2.0.8/hello/video/utils.py
--rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-2.0.8/hello/x3m/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.8/hello/x3m/__main__.py
--rw-r--r--   0        0        0     4843 2023-06-21 01:21:14.617945 hello2-2.0.8/hello/x3m/config.py
--rw-r--r--   0        0        0     3335 2023-06-21 03:35:25.746873 hello2-2.0.8/hello/x3m/mmseg/single_cls.py
--rw-r--r--   0        0        0     6232 2023-06-21 03:35:38.436872 hello2-2.0.8/hello/x3m/nanodet/best_one.py
--rw-r--r--   0        0        0     5310 2023-06-21 03:47:59.306774 hello2-2.0.8/hello/x3m/nanodet/one_fast.py
--rw-r--r--   0        0        0     3280 2023-06-06 08:46:57.526337 hello2-2.0.8/hello/x3m/preprocess.py
--rw-r--r--   0        0        0     8170 2023-06-20 08:59:23.075922 hello2-2.0.8/hello/x3m/transforms.py
--rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-2.0.8/hello_c/CMakeLists.txt
--rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-2.0.8/hello_c/README.md
--rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-2.0.8/hello_c/main.cpp
--rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-2.0.8/hello_c/trace_model.py
--rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-2.0.9/.gitignore
+-rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-2.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-2.0.9/LICENSE
+-rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-2.0.9/README.md
+-rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-2.0.9/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-2.0.9/docs/make.bat
+-rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-2.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-2.0.9/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-2.0.9/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-2.0.9/docs/source/conf.py
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-2.0.9/docs/source/hello.data.coco2yolo.rst
+-rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-2.0.9/docs/source/hello.data.rst
+-rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-2.0.9/docs/source/hello.experimental.albu.detection.rst
+-rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-2.0.9/docs/source/hello.experimental.albu.rst
+-rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-2.0.9/docs/source/hello.experimental.rst
+-rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-2.0.9/docs/source/hello.fiftyone.annotate.rst
+-rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-2.0.9/docs/source/hello.fiftyone.brain.rst
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-2.0.9/docs/source/hello.fiftyone.coco.rst
+-rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-2.0.9/docs/source/hello.fiftyone.coco_utils.rst
+-rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-2.0.9/docs/source/hello.fiftyone.connected.rst
+-rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-2.0.9/docs/source/hello.fiftyone.copypaste.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-2.0.9/docs/source/hello.fiftyone.core.rst
+-rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-2.0.9/docs/source/hello.fiftyone.dataset.rst
+-rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-2.0.9/docs/source/hello.fiftyone.dataset_annotate.rst
+-rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-2.0.9/docs/source/hello.fiftyone.dataset_detections.rst
+-rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.dataset_segmentations.rst
+-rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.dataset_yolov5.rst
+-rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.dataset_zoo.rst
+-rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.evaluate.rst
+-rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.evaluate_detections.rst
+-rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.evaluate_segmentations.rst
+-rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-2.0.9/docs/source/hello.fiftyone.gen_examples.rst
+-rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-2.0.9/docs/source/hello.fiftyone.mask_ignore.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-2.0.9/docs/source/hello.fiftyone.miou.rst
+-rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-2.0.9/docs/source/hello.fiftyone.patches.rst
+-rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-2.0.9/docs/source/hello.fiftyone.rst
+-rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-2.0.9/docs/source/hello.fiftyone.tarinfo.rst
+-rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-2.0.9/docs/source/hello.fiftyone.unique.rst
+-rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-2.0.9/docs/source/hello.fiftyone.utils.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-2.0.9/docs/source/hello.fiftyone.video.rst
+-rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-2.0.9/docs/source/hello.fiftyone.view.rst
+-rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-2.0.9/docs/source/hello.fvcore.core.rst
+-rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-2.0.9/docs/source/hello.fvcore.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-2.0.9/docs/source/hello.io.image.rst
+-rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-2.0.9/docs/source/hello.io.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-2.0.9/docs/source/hello.io.utils.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-2.0.9/docs/source/hello.mmdet.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-2.0.9/docs/source/hello.mmdet.flop.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-2.0.9/docs/source/hello.mmdet.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-2.0.9/docs/source/hello.mmdet.log.rst
+-rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-2.0.9/docs/source/hello.mmdet.plot.rst
+-rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-2.0.9/docs/source/hello.mmdet.rst
+-rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-2.0.9/docs/source/hello.mmlab.mmdet3.rst
+-rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-2.0.9/docs/source/hello.mmlab.mmseg.rst
+-rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-2.0.9/docs/source/hello.mmlab.rst
+-rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-2.0.9/docs/source/hello.mmseg.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-2.0.9/docs/source/hello.mmseg.log.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-2.0.9/docs/source/hello.mmseg.lr.rst
+-rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-2.0.9/docs/source/hello.mmseg.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-2.0.9/docs/source/hello.nanodet.infer.rst
+-rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-2.0.9/docs/source/hello.nanodet.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-2.0.9/docs/source/hello.onnx.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-2.0.9/docs/source/hello.onnx.infer.rst
+-rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-2.0.9/docs/source/hello.onnx.rst
+-rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-2.0.9/docs/source/hello.rst
+-rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-2.0.9/docs/source/hello.transforms.rst
+-rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-2.0.9/docs/source/hello.transforms.transforms.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-2.0.9/docs/source/hello.utils.colors.rst
+-rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-2.0.9/docs/source/hello.utils.compare.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-2.0.9/docs/source/hello.utils.cuda.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-2.0.9/docs/source/hello.utils.importer.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-2.0.9/docs/source/hello.utils.plots.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-2.0.9/docs/source/hello.utils.points.rst
+-rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-2.0.9/docs/source/hello.utils.rst
+-rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-2.0.9/docs/source/hello.utils.strtime.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-2.0.9/docs/source/hello.video.align.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-2.0.9/docs/source/hello.video.clip.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-2.0.9/docs/source/hello.video.fisheye.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-2.0.9/docs/source/hello.video.frames.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-2.0.9/docs/source/hello.video.info.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-2.0.9/docs/source/hello.video.resize.rst
+-rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-2.0.9/docs/source/hello.video.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-2.0.9/docs/source/hello.video.rtsp.rst
+-rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-2.0.9/docs/source/hello.video.rtsp_pull.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-2.0.9/docs/source/hello.video.split.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-2.0.9/docs/source/hello.video.unwarp.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-2.0.9/docs/source/hello.video.utils.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-2.0.9/docs/source/hello.x3m.config.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-2.0.9/docs/source/hello.x3m.preprocess.rst
+-rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-2.0.9/docs/source/hello.x3m.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-2.0.9/docs/source/hello.x3m.transforms.rst
+-rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-2.0.9/docs/source/index.rst
+-rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-2.0.9/docs/source/modules.rst
+-rw-r--r--   0        0        0     3270 2023-06-06 04:22:36.459690 hello2-2.0.9/hello/README.md
+-rw-r--r--   0        0        0      773 2023-06-21 07:55:18.084802 hello2-2.0.9/hello/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/__main__.py
+-rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-2.0.9/hello/data/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/data/__main__.py
+-rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-2.0.9/hello/data/coco2yolo.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-2.0.9/hello/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-2.0.9/hello/experimental/albu/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-2.0.9/hello/experimental/albu/detection.py
+-rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-2.0.9/hello/fiftyone/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/fiftyone/__main__.py
+-rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-2.0.9/hello/fiftyone/annotate.py
+-rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-2.0.9/hello/fiftyone/brain.py
+-rw-r--r--   0        0        0     8246 2023-06-14 06:42:08.391095 hello2-2.0.9/hello/fiftyone/coco.py
+-rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-2.0.9/hello/fiftyone/coco_utils.py
+-rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-2.0.9/hello/fiftyone/connected.py
+-rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-2.0.9/hello/fiftyone/copypaste.py
+-rw-r--r--   0        0        0    19157 2023-06-15 04:03:09.717943 hello2-2.0.9/hello/fiftyone/core.py
+-rw-r--r--   0        0        0    20844 2023-06-15 08:19:34.131331 hello2-2.0.9/hello/fiftyone/dataset.py
+-rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-2.0.9/hello/fiftyone/dataset_detections.py
+-rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-2.0.9/hello/fiftyone/dataset_segmentations.py
+-rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-2.0.9/hello/fiftyone/dataset_yolov5.py
+-rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-2.0.9/hello/fiftyone/dataset_zoo.py
+-rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-2.0.9/hello/fiftyone/evaluate.py
+-rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-2.0.9/hello/fiftyone/evaluate_detections.py
+-rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-2.0.9/hello/fiftyone/evaluate_segmentations.py
+-rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/fiftyone/examples/README.md
+-rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-2.0.9/hello/fiftyone/examples/examples.py
+-rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-2.0.9/hello/fiftyone/examples/utils.py
+-rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-2.0.9/hello/fiftyone/gen_examples.py
+-rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-2.0.9/hello/fiftyone/mask_ignore.py
+-rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-2.0.9/hello/fiftyone/miou.py
+-rw-r--r--   0        0        0      164 2023-06-08 07:23:27.040658 hello2-2.0.9/hello/fiftyone/novabot/README.md
+-rw-r--r--   0        0        0     4003 2023-06-14 08:35:33.468173 hello2-2.0.9/hello/fiftyone/novabot/big_test.py
+-rw-r--r--   0        0        0      942 2023-06-15 07:20:02.952865 hello2-2.0.9/hello/fiftyone/novabot/cal_data.py
+-rw-r--r--   0        0        0     6250 2023-06-14 04:03:54.435176 hello2-2.0.9/hello/fiftyone/novabot/det_annotate.py
+-rw-r--r--   0        0        0     5309 2023-06-14 04:11:05.194991 hello2-2.0.9/hello/fiftyone/novabot/det_big_train.py
+-rw-r--r--   0        0        0     1669 2023-06-14 03:43:11.095705 hello2-2.0.9/hello/fiftyone/novabot/seg_base.py
+-rw-r--r--   0        0        0     2045 2023-06-15 07:15:02.202995 hello2-2.0.9/hello/fiftyone/novabot/tag_data.py
+-rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-2.0.9/hello/fiftyone/patches.py
+-rw-r--r--   0        0        0     9350 2023-06-14 06:41:26.931115 hello2-2.0.9/hello/fiftyone/tarinfo.py
+-rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-2.0.9/hello/fiftyone/unique.py
+-rw-r--r--   0        0        0     8304 2023-06-15 08:24:13.821210 hello2-2.0.9/hello/fiftyone/utils.py
+-rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-2.0.9/hello/fiftyone/video.py
+-rw-r--r--   0        0        0    10699 2023-06-14 07:43:28.909510 hello2-2.0.9/hello/fiftyone/view.py
+-rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-2.0.9/hello/fvcore/README.md
+-rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-2.0.9/hello/fvcore/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-2.0.9/hello/fvcore/core.py
+-rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-2.0.9/hello/io/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-2.0.9/hello/io/image.py
+-rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-2.0.9/hello/io/utils.py
+-rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-2.0.9/hello/mmdet/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-2.0.9/hello/mmdet/__main__.py
+-rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-2.0.9/hello/mmdet/export.py
+-rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-2.0.9/hello/mmdet/flop.py
+-rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-2.0.9/hello/mmdet/infer.py
+-rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-2.0.9/hello/mmdet/log.py
+-rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-2.0.9/hello/mmdet/plot.py
+-rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-2.0.9/hello/mmlab/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-2.0.9/hello/mmlab/__main__.py
+-rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-2.0.9/hello/mmlab/mmdet3.py
+-rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-2.0.9/hello/mmlab/mmseg.py
+-rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-2.0.9/hello/mmseg/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-2.0.9/hello/mmseg/__main__.py
+-rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-2.0.9/hello/mmseg/infer.py
+-rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-2.0.9/hello/mmseg/log.py
+-rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-2.0.9/hello/mmseg/lr.py
+-rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-2.0.9/hello/nanodet/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-2.0.9/hello/nanodet/__main__.py
+-rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-2.0.9/hello/nanodet/infer.py
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-2.0.9/hello/onnx/__init__.py
+-rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-2.0.9/hello/onnx/examples/README.md
+-rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-2.0.9/hello/onnx/examples/test_sigmoid.py
+-rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-2.0.9/hello/onnx/export.py
+-rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-2.0.9/hello/onnx/infer.py
+-rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-2.0.9/hello/transforms/README.md
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-2.0.9/hello/transforms/__init__.py
+-rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-2.0.9/hello/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-2.0.9/hello/utils/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-2.0.9/hello/utils/colors.py
+-rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-2.0.9/hello/utils/compare.py
+-rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-2.0.9/hello/utils/cuda.py
+-rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-2.0.9/hello/utils/importer.py
+-rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-2.0.9/hello/utils/plots.py
+-rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-2.0.9/hello/utils/points.py
+-rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-2.0.9/hello/utils/strtime.py
+-rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-2.0.9/hello/video/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/video/__main__.py
+-rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-2.0.9/hello/video/align.py
+-rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-2.0.9/hello/video/clip.py
+-rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-2.0.9/hello/video/fisheye.py
+-rw-r--r--   0        0        0     1720 2023-06-21 07:55:52.344797 hello2-2.0.9/hello/video/info.py
+-rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-2.0.9/hello/video/resize.py
+-rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-2.0.9/hello/video/rtsp.py
+-rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-2.0.9/hello/video/rtsp_pull.py
+-rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-2.0.9/hello/video/split.py
+-rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-2.0.9/hello/video/unwarp.py
+-rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-2.0.9/hello/video/utils.py
+-rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-2.0.9/hello/x3m/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-2.0.9/hello/x3m/__main__.py
+-rw-r--r--   0        0        0     4843 2023-06-21 01:21:14.617945 hello2-2.0.9/hello/x3m/config.py
+-rw-r--r--   0        0        0     3335 2023-06-21 03:35:25.746873 hello2-2.0.9/hello/x3m/mmseg/single_cls.py
+-rw-r--r--   0        0        0     6232 2023-06-21 03:35:38.436872 hello2-2.0.9/hello/x3m/nanodet/best_one.py
+-rw-r--r--   0        0        0     5310 2023-06-21 03:47:59.306774 hello2-2.0.9/hello/x3m/nanodet/one_fast.py
+-rw-r--r--   0        0        0     3280 2023-06-06 08:46:57.526337 hello2-2.0.9/hello/x3m/preprocess.py
+-rw-r--r--   0        0        0     8170 2023-06-20 08:59:23.075922 hello2-2.0.9/hello/x3m/transforms.py
+-rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-2.0.9/hello_c/CMakeLists.txt
+-rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-2.0.9/hello_c/README.md
+-rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-2.0.9/hello_c/main.cpp
+-rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-2.0.9/hello_c/trace_model.py
+-rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-2.0.9/PKG-INFO
```

### Comparing `hello2-2.0.8/.gitignore` & `hello2-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/.readthedocs.yaml` & `hello2-2.0.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/LICENSE` & `hello2-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/docs/Makefile` & `hello2-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/docs/make.bat` & `hello2-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/docs/source/conf.py` & `hello2-2.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/docs/source/hello.fiftyone.rst` & `hello2-2.0.9/docs/source/hello.fiftyone.rst`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/docs/source/index.rst` & `hello2-2.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/README.md` & `hello2-2.0.9/hello/README.md`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/__init__.py` & `hello2-2.0.9/hello/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 help_doc_str = """\
 usage: hello [--version] [--help]
 
 shell command:
     hello -h
     hello-data -h
```

### Comparing `hello2-2.0.8/hello/data/coco2yolo.py` & `hello2-2.0.9/hello/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/__init__.py` & `hello2-2.0.9/hello/fiftyone/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/annotate.py` & `hello2-2.0.9/hello/fiftyone/annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/brain.py` & `hello2-2.0.9/hello/fiftyone/brain.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/coco.py` & `hello2-2.0.9/hello/fiftyone/coco.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/coco_utils.py` & `hello2-2.0.9/hello/fiftyone/coco_utils.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/connected.py` & `hello2-2.0.9/hello/fiftyone/connected.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/core.py` & `hello2-2.0.9/hello/fiftyone/core.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/dataset.py` & `hello2-2.0.9/hello/fiftyone/dataset.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/dataset_detections.py` & `hello2-2.0.9/hello/fiftyone/dataset_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/dataset_segmentations.py` & `hello2-2.0.9/hello/fiftyone/dataset_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/dataset_yolov5.py` & `hello2-2.0.9/hello/fiftyone/dataset_yolov5.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/dataset_zoo.py` & `hello2-2.0.9/hello/fiftyone/dataset_zoo.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/evaluate.py` & `hello2-2.0.9/hello/fiftyone/evaluate.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/evaluate_detections.py` & `hello2-2.0.9/hello/fiftyone/evaluate_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/evaluate_segmentations.py` & `hello2-2.0.9/hello/fiftyone/evaluate_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/examples/examples.py` & `hello2-2.0.9/hello/fiftyone/examples/examples.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/examples/utils.py` & `hello2-2.0.9/hello/fiftyone/examples/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/gen_examples.py` & `hello2-2.0.9/hello/fiftyone/gen_examples.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/mask_ignore.py` & `hello2-2.0.9/hello/fiftyone/mask_ignore.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/miou.py` & `hello2-2.0.9/hello/fiftyone/miou.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/big_test.py` & `hello2-2.0.9/hello/fiftyone/novabot/big_test.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/cal_data.py` & `hello2-2.0.9/hello/fiftyone/novabot/cal_data.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/det_annotate.py` & `hello2-2.0.9/hello/fiftyone/novabot/det_annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/det_big_train.py` & `hello2-2.0.9/hello/fiftyone/novabot/det_big_train.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/seg_base.py` & `hello2-2.0.9/hello/fiftyone/novabot/seg_base.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/novabot/tag_data.py` & `hello2-2.0.9/hello/fiftyone/novabot/tag_data.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/patches.py` & `hello2-2.0.9/hello/fiftyone/patches.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/tarinfo.py` & `hello2-2.0.9/hello/fiftyone/tarinfo.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/unique.py` & `hello2-2.0.9/hello/fiftyone/unique.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/utils.py` & `hello2-2.0.9/hello/fiftyone/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/video.py` & `hello2-2.0.9/hello/fiftyone/video.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fiftyone/view.py` & `hello2-2.0.9/hello/fiftyone/view.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/fvcore/core.py` & `hello2-2.0.9/hello/fvcore/core.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/io/image.py` & `hello2-2.0.9/hello/io/image.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/io/utils.py` & `hello2-2.0.9/hello/io/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmdet/__init__.py` & `hello2-2.0.9/hello/mmdet/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmdet/flop.py` & `hello2-2.0.9/hello/mmdet/flop.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmdet/infer.py` & `hello2-2.0.9/hello/mmdet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmdet/log.py` & `hello2-2.0.9/hello/mmdet/log.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmdet/plot.py` & `hello2-2.0.9/hello/mmdet/plot.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmlab/__init__.py` & `hello2-2.0.9/hello/mmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmlab/mmseg.py` & `hello2-2.0.9/hello/mmlab/mmseg.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmseg/__init__.py` & `hello2-2.0.9/hello/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmseg/infer.py` & `hello2-2.0.9/hello/mmseg/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmseg/log.py` & `hello2-2.0.9/hello/mmseg/log.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/mmseg/lr.py` & `hello2-2.0.9/hello/mmseg/lr.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/nanodet/infer.py` & `hello2-2.0.9/hello/nanodet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/onnx/examples/test_sigmoid.py` & `hello2-2.0.9/hello/onnx/examples/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/onnx/export.py` & `hello2-2.0.9/hello/onnx/export.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/onnx/infer.py` & `hello2-2.0.9/hello/onnx/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/transforms/README.md` & `hello2-2.0.9/hello/transforms/README.md`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/transforms/transforms.py` & `hello2-2.0.9/hello/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/utils/colors.py` & `hello2-2.0.9/hello/utils/colors.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/utils/compare.py` & `hello2-2.0.9/hello/utils/compare.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/utils/cuda.py` & `hello2-2.0.9/hello/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/utils/plots.py` & `hello2-2.0.9/hello/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/utils/points.py` & `hello2-2.0.9/hello/utils/points.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/__init__.py` & `hello2-2.0.9/hello/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/align.py` & `hello2-2.0.9/hello/video/align.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/clip.py` & `hello2-2.0.9/hello/video/clip.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/fisheye.py` & `hello2-2.0.9/hello/video/fisheye.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/info.py` & `hello2-2.0.9/hello/video/info.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,41 +12,43 @@
     for f in sorted(Path(input_dir).glob("**/*")):
         if f.suffix in suffix_set:
             video_paths.append(f.as_posix())
 
     return video_paths
 
 
-def print_info(video_path):
+def get_info(video_path):
     cap = cv.VideoCapture(video_path)
-
     fps = int(cap.get(cv.CAP_PROP_FPS))
     count = int(cap.get(cv.CAP_PROP_FRAME_COUNT))
     width = int(cap.get(cv.CAP_PROP_FRAME_WIDTH))
     height = int(cap.get(cv.CAP_PROP_FRAME_HEIGHT))
+    cap.release()
 
     video_info = ", ".join(Path(video_path).parts[-2:])
-    print(f"{video_info}, seconds={count//fps:04d}, size={width}x{height}, {fps=}")
-
-    cap.release()
+    return f"{video_info}, seconds={count//fps:04d}, size={width}x{height}, {fps=}"
 
 
 def func(input_dir):
     input_dir = Path(input_dir)
 
     if input_dir.is_file():
         video_paths = [input_dir.as_posix()]
         input_dir = input_dir.parent
     else:
         video_paths = find_videos(input_dir)
 
+    data = []
     for video_path in video_paths:
-        print_info(video_path)
+        data.append(get_info(video_path))
+
+    _sum = sum([int(t.split(",")[2].split("=")[1]) for t in data])
+    data.append(f"\n{_sum}s, {_sum//60:04d}:{_sum%60:02d}")
 
-    return "\n[END]"
+    return "\n".join(data)
 
 
 def parse_args(args=None):
     from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
     parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("input_dir", type=str,
```

### Comparing `hello2-2.0.8/hello/video/resize.py` & `hello2-2.0.9/hello/video/resize.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/rtsp.py` & `hello2-2.0.9/hello/video/rtsp.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/rtsp_pull.py` & `hello2-2.0.9/hello/video/rtsp_pull.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/split.py` & `hello2-2.0.9/hello/video/split.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/unwarp.py` & `hello2-2.0.9/hello/video/unwarp.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/video/utils.py` & `hello2-2.0.9/hello/video/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/__init__.py` & `hello2-2.0.9/hello/x3m/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/config.py` & `hello2-2.0.9/hello/x3m/config.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/mmseg/single_cls.py` & `hello2-2.0.9/hello/x3m/mmseg/single_cls.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/nanodet/best_one.py` & `hello2-2.0.9/hello/x3m/nanodet/best_one.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/nanodet/one_fast.py` & `hello2-2.0.9/hello/x3m/nanodet/one_fast.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/preprocess.py` & `hello2-2.0.9/hello/x3m/preprocess.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello/x3m/transforms.py` & `hello2-2.0.9/hello/x3m/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello_c/CMakeLists.txt` & `hello2-2.0.9/hello_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello_c/README.md` & `hello2-2.0.9/hello_c/README.md`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/hello_c/main.cpp` & `hello2-2.0.9/hello_c/main.cpp`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/pyproject.toml` & `hello2-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hello2-2.0.8/PKG-INFO` & `hello2-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello2
-Version: 2.0.8
+Version: 2.0.9
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scikit-image
```

