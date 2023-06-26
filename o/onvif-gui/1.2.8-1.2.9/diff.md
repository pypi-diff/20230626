# Comparing `tmp/onvif-gui-1.2.8.tar.gz` & `tmp/onvif-gui-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.2.8.tar", last modified: Sun Jun 25 13:42:24 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.9.tar", last modified: Mon Jun 26 15:55:26 2023, max compression
```

## Comparing `onvif-gui-1.2.8.tar` & `onvif-gui-1.2.9.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11558 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)      221 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29897 2023-06-22 16:15:18.000000 onvif-gui-1.2.8/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       68 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      357 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18177 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5800 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5379 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      623 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8119 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9476 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    30158 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3103 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15786 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1360 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/Base-RCNN-FPN.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      201 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      542 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      190 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      663 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7603 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21787 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7460 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9406 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8360 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10433 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22191 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13496 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8008 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    24004 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9205 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9864 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223770 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219193 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39434 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3210 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23487 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      429 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12067 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1991 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      480 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23683 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12980 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      900 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5908 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12431 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3135 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4335 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11154 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6629 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3393 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      673 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      555 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5271 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15825 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2586 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1048 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10628 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16434 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17108 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    24352 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25785 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6546 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19860 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6391 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      524 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      839 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11940 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13541 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10676 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14237 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18704 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10173 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11104 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11575 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4145 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      236 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      860 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8333 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    24347 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9016 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      797 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4195 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13289 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25959 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11428 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12467 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    38578 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11446 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2388 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12723 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1829 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      662 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14854 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5649 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6807 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9269 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    20336 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19356 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2775 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       52 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6205 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8633 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4254 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5807 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1911 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5814 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17508 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1226 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8044 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2667 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1934 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1096 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18576 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11606 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    52426 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/visualizer.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      286 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1824 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2459 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/directoryselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6416 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4194 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1962 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/thresholdslider.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      831 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/waitdialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19633 2023-06-25 13:37:09.000000 onvif-gui-1.2.8/gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5665 2023-06-25 13:31:01.000000 onvif-gui-1.2.8/gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4051 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2484 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5364 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5241 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4640 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      184 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3802 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/audiopanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13667 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14756 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14134 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/settingspanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3806 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/videopanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2021 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13358 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)   207707 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/onvif-gui.ico
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/onvif-gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19236 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/spinner.gif
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/modules/audio/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/audio/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/audio/sample.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/modules/video/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8912 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6322 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3418 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9443 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8944 2023-06-22 16:15:18.000000 onvif-gui-1.2.8/modules/video/segmentv8.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16289 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolov7.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15676 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolov8.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8502 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       44 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1688 2023-06-25 13:36:51.000000 onvif-gui-1.2.8/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1569 2023-06-25 13:36:43.000000 onvif-gui-1.2.8/setup.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1003 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9816 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6304 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    86435 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11177 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/experimental.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    40895 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/yolo.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2320 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/activations.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5771 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/add_nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7321 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/autoanchor.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    57559 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/datasets.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37789 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/general.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4996 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/google_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    76741 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/loss.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9537 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/metrics.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21424 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/plots.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15840 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/torch_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      961 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5019 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6840 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2372 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6944 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3202 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    26204 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4288 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      130 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1628 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/utils/utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11558 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      221 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29897 2023-06-22 16:15:18.000000 onvif-gui-1.2.9/README.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       68 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/checkpoint/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      357 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/checkpoint/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18177 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/checkpoint/c2_model_loading.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5800 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/checkpoint/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5379 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/checkpoint/detection_checkpoint.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/config/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      623 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8119 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/compat.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9476 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/config.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    30158 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/defaults.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3103 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/instantiate.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15786 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/config/lazy.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/configs/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1360 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/Base-RCNN-FPN.yaml
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/configs/COCO-InstanceSegmentation/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      201 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/configs/COCO-Keypoints/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      542 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      190 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/configs/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.480009 onvif-gui-1.2.9/detectron2/data/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      663 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7603 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/benchmark.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21787 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7460 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9406 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8360 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/dataset_mapper.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.484009 onvif-gui-1.2.9/detectron2/data/datasets/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10433 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/builtin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    22191 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/builtin_meta.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13496 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/cityscapes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8008 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24004 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9205 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/coco_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9864 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/lvis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   223770 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   219193 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/lvis_v1_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    39434 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3210 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/pascal_voc.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/datasets/register_coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23487 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/detection_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.484009 onvif-gui-1.2.9/detectron2/data/samplers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      429 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/samplers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12067 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/samplers/distributed_sampler.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1991 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/samplers/grouped_batch_sampler.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.484009 onvif-gui-1.2.9/detectron2/data/transforms/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      480 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/transforms/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14492 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/transforms/augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23683 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/transforms/augmentation_impl.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12980 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/data/transforms/transform.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.484009 onvif-gui-1.2.9/detectron2/layers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      900 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5908 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/aspp.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12431 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/batch_norm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3135 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17492 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/deform_conv.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4335 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11154 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/mask_ops.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6629 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3172 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/roi_align.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3393 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/roi_align_rotated.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      673 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      555 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/shape_spec.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5271 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/layers/wrappers.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.488009 onvif-gui-1.2.9/detectron2/modeling/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1632 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15825 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/anchor_generator.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.488009 onvif-gui-1.2.9/detectron2/modeling/backbone/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2586 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/backbone.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1048 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10628 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16434 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/mvit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17108 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/regnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24352 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/resnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25785 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/swin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6546 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19860 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/backbone/vit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15492 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/box_regression.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6391 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/matcher.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.488009 onvif-gui-1.2.9/detectron2/modeling/meta_arch/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      524 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      839 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11940 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/dense_detector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13541 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/fcos.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10676 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14237 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18704 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10173 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11104 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/mmdet_wrapper.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11575 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/poolers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4145 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/postprocessing.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.488009 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      236 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      860 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8333 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24347 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/rpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9016 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/proposal_generator/rrpn.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.488009 onvif-gui-1.2.9/detectron2/modeling/roi_heads/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      797 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4195 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/box_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13289 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25959 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11428 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12467 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/mask_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    38578 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/roi_heads.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11446 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2388 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/sampling.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12723 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/modeling/test_time_augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1829 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/predictor.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/detectron2/structures/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      662 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14854 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5649 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/image_list.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6807 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/instances.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9269 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/keypoints.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    20336 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/masks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19356 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/structures/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2775 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/tracker.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/detectron2/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       52 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6205 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/analysis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8633 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/collect_env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4254 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/colormap.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5807 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/comm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1911 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/develop.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5814 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17508 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/events.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1226 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/file_io.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8044 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/logger.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2667 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/memory.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1934 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/registry.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1096 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/serialize.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18576 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/testing.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11606 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/video_visualizer.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    52426 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/detectron2/utils/visualizer.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/gui/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/gui/components/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      286 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1824 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/comboselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2459 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/directoryselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2172 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/fileselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6416 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/labelselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4194 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/progress.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1962 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/thresholdslider.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      831 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/components/waitdialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/glwidget.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    20265 2023-06-26 15:53:45.000000 onvif-gui-1.2.9/gui/main.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/gui/onvif/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5665 2023-06-25 13:31:01.000000 onvif-gui-1.2.9/gui/onvif/admintab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4051 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/imagetab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2484 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/logindialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5364 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/networktab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5241 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/ptztab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4640 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/onvif/videotab.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.492009 onvif-gui-1.2.9/gui/panels/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      184 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3802 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/audiopanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13667 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/camerapanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14756 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/filepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14134 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/settingspanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3806 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/panels/videopanel.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/gui/resources/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2021 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/apply.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/apply_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/apply_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/audio.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/audio_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/audio_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_closed.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_closed_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_closed_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_open.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_open_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/branch_open_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/checked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/checked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/checked_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13358 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/darkstyle.qss
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/discover.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/discover_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/discover_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/fast-forward.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/fast-forward_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/fast-forward_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/mute.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/mute_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/mute_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/next.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/next_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/next_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   207707 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/onvif-gui.ico
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/onvif-gui.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/pause.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/pause_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/pause_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/play.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/play_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/play_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/previous.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/previous_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/previous_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-off.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-off_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-off_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-on.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-on_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/radio-on_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/record.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/record_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/record_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/recording.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/recording_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/recording_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/rewind.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/rewind_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/rewind_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_left.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_left_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_left_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_up.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_up_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/small_arrow_up_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19236 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/spinner.gif
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/stop.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/stop_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/stop_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/unchecked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/unchecked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/gui/resources/unchecked_lo.png
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/modules/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/modules/audio/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/audio/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3492 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/audio/sample.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/modules/video/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8912 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/keypoint.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6322 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3418 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/sample.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9443 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/segment.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11487 2023-06-26 15:48:37.000000 onvif-gui-1.2.9/modules/video/segmentv8.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16289 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/yolov7.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15676 2023-06-25 17:47:26.000000 onvif-gui-1.2.9/modules/video/yolov8.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17632 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/modules/video/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/onvif_gui.egg-info/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8502 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/entry_points.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/requires.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       44 2023-06-26 15:55:26.000000 onvif-gui-1.2.9/onvif_gui.egg-info/top_level.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1688 2023-06-26 15:53:58.000000 onvif-gui-1.2.9/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1569 2023-06-26 15:53:53.000000 onvif-gui-1.2.9/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/tracker/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/tracker/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1003 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/tracker/basetrack.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12632 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/tracker/byte_tracker.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9816 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/tracker/kalman_filter.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6304 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/tracker/matching.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/yolov7/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.500009 onvif-gui-1.2.9/yolov7/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    86435 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/models/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11177 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/models/experimental.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    40895 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/models/yolo.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/yolov7/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2320 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/activations.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5771 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/add_nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7321 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/autoanchor.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    57559 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/datasets.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    37789 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/general.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4996 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/google_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    76741 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/loss.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9537 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/metrics.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21424 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/plots.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15840 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolov7/utils/torch_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/yolox/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/yolox/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      961 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5019 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6840 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/darknet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2372 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6944 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/network_blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3202 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/yolo_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    26204 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/yolo_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4288 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/yolo_pafpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/models/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-26 15:55:26.504009 onvif-gui-1.2.9/yolox/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      130 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1628 2023-06-20 17:09:20.000000 onvif-gui-1.2.9/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.2.8/LICENSE` & `onvif-gui-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/PKG-INFO` & `onvif-gui-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.8
+Version: 1.2.9
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.8/README.md` & `onvif-gui-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.9/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.9/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.9/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/__init__.py` & `onvif-gui-1.2.9/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/compat.py` & `onvif-gui-1.2.9/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/config.py` & `onvif-gui-1.2.9/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/defaults.py` & `onvif-gui-1.2.9/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/instantiate.py` & `onvif-gui-1.2.9/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/config/lazy.py` & `onvif-gui-1.2.9/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.9/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.9/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/__init__.py` & `onvif-gui-1.2.9/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/benchmark.py` & `onvif-gui-1.2.9/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/build.py` & `onvif-gui-1.2.9/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/catalog.py` & `onvif-gui-1.2.9/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/common.py` & `onvif-gui-1.2.9/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.9/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.9/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.9/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.9/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.9/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.9/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.9/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.9/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.9/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.9/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.9/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.9/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.9/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/detection_utils.py` & `onvif-gui-1.2.9/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.9/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.9/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.9/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.9/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.9/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/__init__.py` & `onvif-gui-1.2.9/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/aspp.py` & `onvif-gui-1.2.9/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.9/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/blocks.py` & `onvif-gui-1.2.9/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.9/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/losses.py` & `onvif-gui-1.2.9/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.9/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/nms.py` & `onvif-gui-1.2.9/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/roi_align.py` & `onvif-gui-1.2.9/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.9/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.9/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.9/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/layers/wrappers.py` & `onvif-gui-1.2.9/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/__init__.py` & `onvif-gui-1.2.9/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.9/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.9/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.9/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/matcher.py` & `onvif-gui-1.2.9/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.9/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.9/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/poolers.py` & `onvif-gui-1.2.9/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.9/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.9/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.9/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.9/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.9/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.9/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/sampling.py` & `onvif-gui-1.2.9/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.9/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/predictor.py` & `onvif-gui-1.2.9/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/__init__.py` & `onvif-gui-1.2.9/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/boxes.py` & `onvif-gui-1.2.9/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/image_list.py` & `onvif-gui-1.2.9/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/instances.py` & `onvif-gui-1.2.9/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/keypoints.py` & `onvif-gui-1.2.9/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/masks.py` & `onvif-gui-1.2.9/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.9/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/tracker.py` & `onvif-gui-1.2.9/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/analysis.py` & `onvif-gui-1.2.9/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/collect_env.py` & `onvif-gui-1.2.9/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/colormap.py` & `onvif-gui-1.2.9/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/comm.py` & `onvif-gui-1.2.9/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/develop.py` & `onvif-gui-1.2.9/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/env.py` & `onvif-gui-1.2.9/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/events.py` & `onvif-gui-1.2.9/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/file_io.py` & `onvif-gui-1.2.9/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/logger.py` & `onvif-gui-1.2.9/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/memory.py` & `onvif-gui-1.2.9/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/registry.py` & `onvif-gui-1.2.9/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/serialize.py` & `onvif-gui-1.2.9/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/testing.py` & `onvif-gui-1.2.9/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.9/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/detectron2/utils/visualizer.py` & `onvif-gui-1.2.9/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/comboselector.py` & `onvif-gui-1.2.9/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/directoryselector.py` & `onvif-gui-1.2.9/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/fileselector.py` & `onvif-gui-1.2.9/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/labelselector.py` & `onvif-gui-1.2.9/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/progress.py` & `onvif-gui-1.2.9/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/thresholdslider.py` & `onvif-gui-1.2.9/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/components/waitdialog.py` & `onvif-gui-1.2.9/gui/components/waitdialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/glwidget.py` & `onvif-gui-1.2.9/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/main.py` & `onvif-gui-1.2.9/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from gui.panels import CameraPanel, FilePanel, SettingsPanel, VideoPanel, AudioPanel
 from gui.glwidget import GLWidget
 from gui.components import WaitDialog
 from collections import deque
 
 import avio
 
-VERSION = "1.2.8"
+VERSION = "1.2.9"
 
 class MainWindowSignals(QObject):
     started = pyqtSignal(int)
     stopped = pyqtSignal()
     progress = pyqtSignal(float)
     error = pyqtSignal(str)
     showWait = pyqtSignal()
@@ -121,14 +121,15 @@
 
         self.split = QSplitter()
         self.split.addWidget(self.glWidget)
         self.split.addWidget(self.tab)
         self.split.setStretchFactor(0, 10)
         self.split.splitterMoved.connect(self.splitterMoved)
         splitterState = self.settings.value(self.splitKey)
+
         self.setCentralWidget(self.split)
 
         rect = self.settings.value(self.geometryKey)
         if rect is not None:
             if rect.width() > 0 and rect.height() > 0 and rect.x() > 0 and rect.y() > 0:
                 self.setGeometry(rect)
 
@@ -155,14 +156,17 @@
         self.audioConfigure = None
         audioWorkerName = self.audioPanel.cmbWorker.currentText()
         if len(audioWorkerName) > 0:
             self.loadAudioConfigure(audioWorkerName)
 
         if splitterState is not None:
             self.split.restoreState(splitterState)
+        self.splitterCollapsed = False
+        if not self.split.sizes()[1]:
+            self.splitterCollapsed = True
 
         self.tab.setCurrentIndex(int(self.settings.value(self.tabIndexKey, 0)))
 
     def loadVideoConfigure(self, workerName):
         spec = importlib.util.spec_from_file_location("VideoConfigure", self.videoPanel.dirModules.text() + "/" + workerName)
         videoConfigureHook = importlib.util.module_from_spec(spec)
         sys.modules["VideoConfigure"] = videoConfigureHook
@@ -369,14 +373,26 @@
 
     def reconnect(self):
         self.signals.hideWait.emit()
         logger.debug("Attempting to re-connnect")
         self.playMedia(self.uri)
 
     def splitterMoved(self, pos, index):
+        if self.split.sizes()[1]:
+            if self.splitterCollapsed:
+                self.splitterCollapsed = False
+                ci = self.tab.currentIndex()
+                self.tab.setCurrentIndex(0)
+                self.tab.setCurrentIndex(ci)
+                ci = self.cameraPanel.tabOnvif.currentIndex()
+                self.cameraPanel.tabOnvif.setCurrentIndex(0)
+                self.cameraPanel.tabOnvif.setCurrentIndex(ci)
+        else:
+            self.splitterCollapsed = True
+
         self.settings.setValue(self.splitKey, self.split.saveState())
 
     def getLocation(self):
         path = Path(os.path.dirname(__file__))
         return str(path.parent.absolute())
     
     def getVideoFrameRate(self):
```

### Comparing `onvif-gui-1.2.8/gui/onvif/admintab.py` & `onvif-gui-1.2.9/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/onvif/imagetab.py` & `onvif-gui-1.2.9/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/onvif/logindialog.py` & `onvif-gui-1.2.9/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/onvif/networktab.py` & `onvif-gui-1.2.9/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/onvif/ptztab.py` & `onvif-gui-1.2.9/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/onvif/videotab.py` & `onvif-gui-1.2.9/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/panels/audiopanel.py` & `onvif-gui-1.2.9/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/panels/camerapanel.py` & `onvif-gui-1.2.9/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/panels/filepanel.py` & `onvif-gui-1.2.9/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/panels/settingspanel.py` & `onvif-gui-1.2.9/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/panels/videopanel.py` & `onvif-gui-1.2.9/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/LICENSE` & `onvif-gui-1.2.9/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/audio.png` & `onvif-gui-1.2.9/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/audio_hi.png` & `onvif-gui-1.2.9/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/audio_lo.png` & `onvif-gui-1.2.9/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/darkstyle.qss` & `onvif-gui-1.2.9/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/discover.png` & `onvif-gui-1.2.9/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/discover_hi.png` & `onvif-gui-1.2.9/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/discover_lo.png` & `onvif-gui-1.2.9/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/mute.png` & `onvif-gui-1.2.9/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/mute_lo.png` & `onvif-gui-1.2.9/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/onvif-gui.ico` & `onvif-gui-1.2.9/gui/resources/onvif-gui.ico`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/onvif-gui.png` & `onvif-gui-1.2.9/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/recording_lo.png` & `onvif-gui-1.2.9/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/gui/resources/spinner.gif` & `onvif-gui-1.2.9/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/audio/sample.py` & `onvif-gui-1.2.9/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/keypoint.py` & `onvif-gui-1.2.9/modules/video/keypoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/retinanet.py` & `onvif-gui-1.2.9/modules/video/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/sample.py` & `onvif-gui-1.2.9/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/segment.py` & `onvif-gui-1.2.9/modules/video/segment.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/segmentv8.py` & `onvif-gui-1.2.9/modules/video/segmentv8.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,16 +53,15 @@
             self.mw = mw
             self.name = MODULE_NAME
             self.last_ex = ""
 
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
             self.showIDKey = "Module/" + MODULE_NAME + "/showID"
-            self.logCountKey = "Module/" + MODULE_NAME + "/logCount"
-            self.countIntervalKey = "Module/" + MODULE_NAME + "/countInterval"
+            self.showBoxKey = "Module/" + MODULE_NAME + "/showBox"
 
             self.model_names = {"nano" : "yolov8n-seg.pt", "small" : "yolov8s-seg.pt", "medium" : "yolov8m-seg.pt", "large" : "yolov8l-seg.pt", "XL" : "yolov8x-seg.pt"}
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
@@ -72,34 +71,52 @@
             self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440", "1920"), "640", MODULE_NAME)
 
             self.txtModelFile = FileSelector(mw, MODULE_NAME)
             self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
+            self.chkShowBox = QCheckBox("Show Detection Box")
+            self.chkShowBox.setChecked(int(self.mw.settings.value(self.showBoxKey, 0)))
+            self.chkShowBox.stateChanged.connect(self.chkShowBoxClicked)
+
+            self.chkTrack = QCheckBox("Track Objects")
+            self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
+            self.chkTrack.stateChanged.connect(self.chkTrackClicked)
+
+            self.chkShowID = QCheckBox("Show Object ID")
+            self.chkShowID.setChecked(int(self.mw.settings.value(self.showIDKey, 1)))
+            self.chkShowID.stateChanged.connect(self.chkShowIDClicked)
+
+            if not self.chkTrack.isChecked():
+                self.chkShowID.setVisible(False)
+
             number_of_labels = 5
             self.labels = []
             for i in range(number_of_labels):
                 self.labels.append(LabelSelector(mw, MODULE_NAME, i+1))
             pnlLabels = QWidget()
             lytLabels = QGridLayout(pnlLabels)
             lblPanel = QLabel("Select classes to be segmented")
             lblPanel.setAlignment(Qt.AlignmentFlag.AlignCenter)
             lytLabels.addWidget(lblPanel,        0, 0, 1, 1)
             for i in range(number_of_labels):
-                self.labels[i].btnColor.setVisible(False)
+                self.labels[i].btnColor.setVisible(self.chkShowBox.isChecked())
                 lytLabels.addWidget(self.labels[i], i+1, 0, 1, 1)
             lytLabels.setContentsMargins(0, 0, 0, 0)
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkAuto,      0, 0, 1, 2)
             lytMain.addWidget(self.cmbModel,     1, 0, 1, 2)
             lytMain.addWidget(self.txtModelFile, 2, 0, 1, 2)
             lytMain.addWidget(self.cmbRes,       3, 0, 1, 2)
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 2)
+            lytMain.addWidget(self.chkShowBox,   5, 0, 1, 2)
+            lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
+            lytMain.addWidget(self.chkShowID,    6, 1, 1, 1)
             lytMain.addWidget(pnlLabels,         7, 0, 1, 2)
             lytMain.addWidget(QLabel(),          8, 0, 1, 2)
             lytMain.setRowStretch(8, 10)
 
             self.first_pass = True
 
             if len(IMPORT_ERROR) > 0:
@@ -109,14 +126,26 @@
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.cmbModel.setEnabled(self.chkAuto.isChecked())
         self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
 
+    def chkShowBoxClicked(self, state):
+        self.mw.settings.setValue(self.showBoxKey, state)
+        for label in self.labels:
+            label.btnColor.setVisible(state)
+
+    def chkTrackClicked(self, state):
+        self.mw.settings.setValue(self.trackKey, state)
+        self.chkShowID.setVisible(state)
+
+    def chkShowIDClicked(self, state):
+        self.mw.settings.setValue(self.showIDKey, state)
+
     def getModelName(self):
         if self.chkAuto.isChecked():
             return self.model_names[self.cmbModel.currentText()]
         else:
             return self.txtModelFile.text()
         
     def getLabel(self, class_id):
@@ -183,34 +212,56 @@
                     torch.cuda.empty_cache()
                 self.__init__(self.mw)
 
             confthre = self.mw.configure.sldConfThre.value()
             res = int(self.mw.configure.cmbRes.currentText())
 
             composite = None
-            results = self.model(img, stream=True, verbose=False,
-                                 classes=label_filter,
-                                 conf=confthre,
-                                 imgsz=res)
+            results = None
+
+            if self.mw.configure.chkTrack.isChecked():
+                results = self.model.track(img, stream=True, verbose=False,
+                                classes=label_filter, persist=True,
+                                conf=confthre, imgsz=res)
+            else:
+                results = self.model.predict(img, stream=True, verbose=False,
+                                classes=label_filter, conf=confthre, imgsz=res)
             
+            boxes = None
             for result in results:
+                boxes = result.boxes.cpu().numpy()
                 if result.masks is not None:
                     for mask in result.masks:
                         m = torch.squeeze(mask.data)
                         if composite is None:
                             composite = torch.zeros_like(m).cuda()
                         composite += m
 
                     composite = torch.gt(composite, 0)
                     composite = torch.stack((composite, composite, composite), 2).cpu().numpy().astype(np.uint8)
                     composite = cv2.resize(composite, (img.shape[1], img.shape[0]), interpolation=cv2.INTER_LINEAR)
 
             if composite is not None:
                 img *= composite
 
+            if self.mw.configure.chkShowBox.isChecked():
+                if boxes is not None:
+                    for box in boxes:
+                        r = box.xyxy[0].astype(int)
+                        class_id = int(box.cls[0])
+                        class_color = self.mw.configure.getLabel(class_id).color()
+                        if self.mw.configure.chkTrack.isChecked():
+                            id_text = '{}'.format(int(box.id)).zfill(4)
+                            box_color = (int((37 * box.id) % 255), int((17 * box.id) % 255), int((29 * box.id) % 255))
+                            cv2.rectangle(img, r[:2], r[2:], box_color, 2)
+                            if self.mw.configure.chkShowID.isChecked():
+                                cv2.putText(img, id_text, r[:2], cv2.FONT_HERSHEY_PLAIN, 2, class_color, 2)
+                        else:
+                            cv2.rectangle(img, r[:2], r[2:], class_color, 2)
+
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         return torch.hub.get_dir() +  "/checkpoints/" + self.mw.configure.getModelName()
```

### Comparing `onvif-gui-1.2.8/modules/video/yolov7.py` & `onvif-gui-1.2.9/modules/video/yolov7.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/yolov8.py` & `onvif-gui-1.2.9/modules/video/yolov8.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/modules/video/yolox.py` & `onvif-gui-1.2.9/modules/video/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.2.9/onvif_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.2.8
+Version: 1.2.9
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.2.8/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.9/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/pyproject.toml` & `onvif-gui-1.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.2.8"  
+version = "1.2.9"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.2.8/setup.py` & `onvif-gui-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding = 'cp850') as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.2.8",
+    version="1.2.9",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.2.8/tracker/basetrack.py` & `onvif-gui-1.2.9/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/tracker/byte_tracker.py` & `onvif-gui-1.2.9/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/tracker/kalman_filter.py` & `onvif-gui-1.2.9/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/tracker/matching.py` & `onvif-gui-1.2.9/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/models/common.py` & `onvif-gui-1.2.9/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/models/experimental.py` & `onvif-gui-1.2.9/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/models/yolo.py` & `onvif-gui-1.2.9/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/activations.py` & `onvif-gui-1.2.9/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/add_nms.py` & `onvif-gui-1.2.9/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.9/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/datasets.py` & `onvif-gui-1.2.9/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/general.py` & `onvif-gui-1.2.9/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/google_utils.py` & `onvif-gui-1.2.9/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/loss.py` & `onvif-gui-1.2.9/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/metrics.py` & `onvif-gui-1.2.9/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/plots.py` & `onvif-gui-1.2.9/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.9/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/__init__.py` & `onvif-gui-1.2.9/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/build.py` & `onvif-gui-1.2.9/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/darknet.py` & `onvif-gui-1.2.9/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/losses.py` & `onvif-gui-1.2.9/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/network_blocks.py` & `onvif-gui-1.2.9/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.9/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/yolo_head.py` & `onvif-gui-1.2.9/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.9/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/models/yolox.py` & `onvif-gui-1.2.9/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.8/yolox/utils/utils.py` & `onvif-gui-1.2.9/yolox/utils/utils.py`

 * *Files identical despite different names*

