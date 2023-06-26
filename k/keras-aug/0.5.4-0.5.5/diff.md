# Comparing `tmp/keras-aug-0.5.4.tar.gz` & `tmp/keras-aug-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-aug-0.5.4.tar", last modified: Thu Jun  8 12:17:55 2023, max compression
+gzip compressed data, was "keras-aug-0.5.5.tar", last modified: Mon Jun 26 05:06:19 2023, max compression
```

## Comparing `keras-aug-0.5.4.tar` & `keras-aug-0.5.5.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.722174 keras-aug-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-08 12:17:18.000000 keras-aug-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-08 12:17:55.722174 keras-aug-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-06-08 12:17:18.000000 keras-aug-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.690173 keras-aug-0.5.4/keras_aug/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.694173 keras-aug-0.5.4/keras_aug/core/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.694173 keras-aug-0.5.4/keras_aug/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/uniform_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.694173 keras-aug-0.5.4/keras_aug/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.698173 keras-aug-0.5.4/keras_aug/layers/__internal__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/base_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/graph_xla_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/mixed_precision_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/output_common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/with_bounding_boxes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/__internal__/with_ragged_image_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.698173 keras-aug-0.5.4/keras_aug/layers/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.698173 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/aug_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/rand_augment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.702173 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23246 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_rotate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.706173 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_clahe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_clahe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gamma_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_hsv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_posterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_posterize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_solarize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.706173 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/cut_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mix_up_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17535 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mosaic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.710173 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_cutout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_erase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_erase_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.710173 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_apply_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_choice_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/repeated_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/augmentation/utility/repeated_augment_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.710173 keras-aug-0.5.4/keras_aug/layers/base/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/base/vectorized_base_random_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22094 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/base/vectorized_base_random_layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.710173 keras-aug-0.5.4/keras_aug/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.714173 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/resize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.718173 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/equalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/equalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/grayscale_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/invert.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/invert_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/normalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/rescale_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.718173 keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.718173 keras-aug-0.5.4/keras_aug/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/augmentation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/bounding_box_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 12:17:18.000000 keras-aug-0.5.4/keras_aug/utils/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:17:55.694173 keras-aug-0.5.4/keras_aug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-08 12:17:55.000000 keras-aug-0.5.4/keras_aug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-08 12:17:55.000000 keras-aug-0.5.4/keras_aug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:17:55.000000 keras-aug-0.5.4/keras_aug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 12:17:55.000000 keras-aug-0.5.4/keras_aug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 12:17:55.000000 keras-aug-0.5.4/keras_aug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-08 12:17:18.000000 keras-aug-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:17:55.722174 keras-aug-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-26 05:05:50.000000 keras-aug-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-26 05:06:19.525474 keras-aug-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-06-26 05:05:50.000000 keras-aug-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/__internal__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/graph_xla_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/mixed_precision_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/output_common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/with_bounding_boxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/__internal__/with_ragged_image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.509474 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.513474 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22094 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.517474 keras-aug-0.5.5/keras_aug/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.521474 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.521474 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.525474 keras-aug-0.5.5/keras_aug/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/augmentation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/bounding_box_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 05:05:50.000000 keras-aug-0.5.5/keras_aug/utils/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:06:19.505474 keras-aug-0.5.5/keras_aug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 05:06:19.000000 keras-aug-0.5.5/keras_aug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-26 05:05:50.000000 keras-aug-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:06:19.525474 keras-aug-0.5.5/setup.cfg
```

### Comparing `keras-aug-0.5.4/LICENSE` & `keras-aug-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/PKG-INFO` & `keras-aug-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `keras-aug-0.5.4/README.md` & `keras-aug-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/conftest.py` & `keras-aug-0.5.5/keras_aug/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/__init__.py` & `keras-aug-0.5.5/keras_aug/core/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/constant_factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/constant_factor_sampler_test.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/normal_factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/normal_factor_sampler_test.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/uniform_factor_sampler.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py` & `keras-aug-0.5.5/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/__init__.py` & `keras-aug-0.5.5/keras_aug/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/base_layer.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/base_layer_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/base_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/config_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/config_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/graph_xla_mode_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/graph_xla_mode_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         {"value_range": (0, 255), "factor": 0.1},
         True,
     ),
     (
         "RandomCLAHE",
         layers.RandomCLAHE,
         {"value_range": (0, 255), "factor": (2, 10), "tile_grid_size": (4, 4)},
-        True,
+        False,
     ),
     (
         "RandomColorJitter",
         layers.RandomColorJitter,
         {
             "value_range": (0, 255),
             "brightness_factor": 0.1,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/mixed_precision_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/with_ragged_image_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import inspect
 
 import tensorflow as tf
 from absl.testing import parameterized
-from keras_cv import bounding_box
-from tensorflow import keras
 
 from keras_aug import layers
 from keras_aug.layers import augmentation
 from keras_aug.layers import preprocessing
 from keras_aug.utils.augmentation import BOUNDING_BOXES
 from keras_aug.utils.augmentation import IMAGES
 from keras_aug.utils.augmentation import LABELS
@@ -15,25 +13,25 @@
 #   (
 #       name,
 #       layer_cls,
 #       args,
 #       is_bbox_compatible,
 #   )
 # all configurations should be expanded for readability
-GENERAL_TESTS = [
+CONSISTENT_OUTPUTS_LAYERS = [
     (
         "AugMix",
         layers.AugMix,
         {"value_range": (0, 255)},
         False,
     ),
     (
         "RandAugment",
         layers.RandAugment,
-        {"value_range": (0, 255)},
+        {"value_range": (0, 255), "seed": 2023},
         True,
     ),
     (
         "TrivialAugmentWide",
         layers.TrivialAugmentWide,
         {"value_range": (0, 255)},
         True,
@@ -49,55 +47,26 @@
             "zoom_width_factor": 0.1,
             "shear_height_factor": 0.1,
             "shear_width_factor": 0.1,
         },
         True,
     ),
     (
-        "RandomCrop",
-        layers.RandomCrop,
-        {"height": 2, "width": 2},
-        True,
-    ),
-    (
-        "RandomCropAndResize",
-        layers.RandomCropAndResize,
-        {
-            "height": 2,
-            "width": 2,
-            "crop_area_factor": (0.8, 1.0),
-            "aspect_ratio_factor": (3 / 4, 4 / 3),
-        },
-        True,
-    ),
-    (
         "RandomFlip",
         layers.RandomFlip,
         {"mode": "horizontal"},
         True,
     ),
     (
-        "RandomResize",
-        layers.RandomResize,
-        {"heights": [2]},
-        True,
-    ),
-    (
         "RandomRotate",
         layers.RandomRotate,
         {"factor": 10},
         True,
     ),
     (
-        "RandomZoomAndCrop",
-        layers.RandomZoomAndCrop,
-        {"height": 2, "width": 2, "scale_factor": (0.8, 1.25)},
-        True,
-    ),
-    (
         "ChannelShuffle",
         layers.ChannelShuffle,
         {"groups": 3},
         True,
     ),
     (
         "RandomBlur",
@@ -110,15 +79,15 @@
         layers.RandomChannelShift,
         {"value_range": (0, 255), "factor": 0.1},
         True,
     ),
     (
         "RandomCLAHE",
         layers.RandomCLAHE,
-        {"value_range": (0, 255), "factor": (2, 10), "tile_grid_size": (4, 4)},
+        {"value_range": (0, 255)},
         True,
     ),
     (
         "RandomColorJitter",
         layers.RandomColorJitter,
         {
             "value_range": (0, 255),
@@ -180,35 +149,14 @@
             "value_range": (0, 255),
             "threshold_factor": 10,
             "addition_factor": 10,
         },
         True,
     ),
     (
-        "CutMix",
-        layers.CutMix,
-        {"alpha": 1.0},
-        False,
-    ),
-    (
-        "MixUp",
-        layers.MixUp,
-        {},
-        True,
-    ),
-    (
-        "Mosaic",
-        layers.Mosaic,
-        {
-            "height": 100,
-            "width": 100,
-        },
-        True,
-    ),
-    (
         "RandomChannelDropout",
         layers.RandomChannelDropout,
         {},
         True,
     ),
     (
         "RandomCutout",
@@ -229,29 +177,49 @@
             "size_factor": (0.5, 1.0),
             "ratio_factor": (0.6, 0.6),
             "rotation_factor": (-10, 10),
         },
         True,
     ),
     (
-        "CenterCrop",
-        layers.CenterCrop,
-        {"height": 2, "width": 2},
+        "RandomApply",
+        layers.RandomApply,
+        {"layer": layers.RandomChannelDropout()},
         True,
     ),
     (
-        "PadIfNeeded",
-        layers.PadIfNeeded,
-        {"min_height": 2, "min_width": 2},
+        "RandomChoice",
+        layers.RandomChoice,
+        {
+            "layers": [
+                layers.RandomChannelDropout(),
+                layers.RandomChannelDropout(),
+            ]
+        },
         True,
     ),
     (
-        "Resize",
-        layers.Resize,
-        {"height": 2, "width": 2},
+        "RepeatedAugment",
+        layers.RepeatedAugment,
+        {
+            "layers": [
+                layers.RandomColorJitter(
+                    value_range=(0, 255), brightness_factor=(1.5, 1.5)
+                ),
+                layers.RandomColorJitter(
+                    value_range=(0, 255), contrast_factor=(1.5, 1.5)
+                ),
+            ]
+        },
+        True,
+    ),
+    (
+        "PadIfNeeded",
+        layers.PadIfNeeded,
+        {"min_height": 2, "min_width": 2},
         True,
     ),
     (
         "AutoContrast",
         layers.AutoContrast,
         {"value_range": (0, 255)},
         True,
@@ -296,85 +264,112 @@
         "SanitizeBoundingBox",
         layers.SanitizeBoundingBox,
         {"min_size": 10},
         True,
     ),
 ]
 
-BUILD_IN_RUNTIME = [
+FORCE_DENSE_IMAGES_LAYERS = [
     (
-        "RandomApply",
-        layers.RandomApply,
-        {"name": "layer", "value": "single", "args": {}},
-        layers.RandomChannelDropout,
-        {},
+        "RandomCrop",
+        layers.RandomCrop,
+        {"height": 2, "width": 2},
+        True,
     ),
     (
-        "RandomApplyBatchwise",
-        layers.RandomApply,
-        {"name": "layer", "value": "single", "args": {"batchwise": True}},
-        layers.RandomChannelDropout,
-        {},
+        "RandomCropAndResize",
+        layers.RandomCropAndResize,
+        {
+            "height": 2,
+            "width": 2,
+            "crop_area_factor": (0.8, 1.0),
+            "aspect_ratio_factor": (3 / 4, 4 / 3),
+        },
+        True,
     ),
     (
-        "RandomChoice",
-        layers.RandomChoice,
-        {"name": "layers", "value": "multiple", "args": {}},
-        layers.RandomChannelDropout,
-        {},
+        "RandomResize",
+        layers.RandomResize,
+        {"heights": [2]},
+        True,
     ),
     (
-        "RandomChoiceBatchwise",
-        layers.RandomChoice,
-        {"name": "layers", "value": "multiple", "args": {"batchwise": True}},
-        layers.RandomChannelDropout,
-        {},
+        "RandomZoomAndCrop",
+        layers.RandomZoomAndCrop,
+        {"height": 2, "width": 2, "scale_factor": (0.8, 1.25)},
+        True,
     ),
     (
-        "RepeatedAugment",
-        layers.RepeatedAugment,
-        {"name": "layers", "value": "multiple", "args": {}},
-        layers.RandomColorJitter,
-        {"value_range": (0, 255), "brightness_factor": (1.5, 1.5)},
+        "Mosaic",
+        layers.Mosaic,
+        {
+            "height": 2,
+            "width": 2,
+        },
+        True,
+    ),
+    (
+        "CenterCrop",
+        layers.CenterCrop,
+        {"height": 2, "width": 2},
+        True,
+    ),
+    (
+        "Resize",
+        layers.Resize,
+        {"height": 2, "width": 2},
+        True,
     ),
 ]
 
+NO_RAGGED_IMAGES_SUPPORT = [
+    (
+        "CutMix",
+        layers.CutMix,
+        {"alpha": 1.0},
+        False,
+    ),
+    (
+        "MixUp",
+        layers.MixUp,
+        {},
+        True,
+    ),
+]
 
-class MixedPrecisionTest(tf.test.TestCase, parameterized.TestCase):
+
+class WithRaggedImageTest(tf.test.TestCase, parameterized.TestCase):
     def test_all_2d_aug_layers_included(self):
         base_cls = layers.VectorizedBaseRandomLayer
         cls_spaces = [augmentation, preprocessing]
         all_2d_aug_layers = []
         for cls_space in cls_spaces:
             all_2d_aug_layers.extend(
                 inspect.getmembers(cls_space, predicate=inspect.isclass)
             )
         all_2d_aug_layer_names = set(
             item[0]
             for item in all_2d_aug_layers
             if issubclass(item[1], base_cls)
         )
 
-        general_names = set(item[0] for item in GENERAL_TESTS)
-        build_names = set(item[0] for item in BUILD_IN_RUNTIME)
-        all_test_names = general_names.union(build_names)
+        cosistent_names = set(item[0] for item in CONSISTENT_OUTPUTS_LAYERS)
+        dense_names = set(item[0] for item in FORCE_DENSE_IMAGES_LAYERS)
+        no_ragged_names = set(item[0] for item in NO_RAGGED_IMAGES_SUPPORT)
+        all_test_names = cosistent_names.union(dense_names).union(
+            no_ragged_names
+        )
 
         for name in all_2d_aug_layer_names:
             self.assertIn(name, all_test_names, msg=f"{name} not found")
 
-    @parameterized.named_parameters(*GENERAL_TESTS)
-    def test_run_in_mixed_precision(self, layer_cls, args, is_bbox_compatible):
-        keras.mixed_precision.set_global_policy("mixed_float16")
-        images = tf.cast(
-            tf.random.uniform(shape=(2, 32, 32, 3)) * 255.0,
-            dtype=tf.float64,
-        )
-        labels = tf.cast(
-            tf.random.uniform(shape=(2, 1)) * 10.0, dtype=tf.float64
-        )
+    @parameterized.named_parameters(*CONSISTENT_OUTPUTS_LAYERS)
+    def test_consistent_images(self, layer_cls, args, is_bbox_compatible):
+        images = tf.ragged.stack([tf.ones((5, 5, 3)), tf.ones((8, 8, 3))])
+        labels = tf.ragged.stack([tf.ones((1,)), tf.ones((1,))])
         bounding_boxes = {
             "boxes": tf.ragged.constant(
                 [
                     [[10, 10, 20, 20], [100, 100, 150, 150]],
                     [[200, 200, 400, 400]],
                 ],
                 dtype=tf.float32,
@@ -393,51 +388,71 @@
             }
         else:
             layer = layer_cls(**args)
             inputs = {IMAGES: images, LABELS: labels}
 
         outputs = layer(inputs)
 
+        self.assertTrue(isinstance(outputs[IMAGES], tf.RaggedTensor))
+
+    @parameterized.named_parameters(*FORCE_DENSE_IMAGES_LAYERS)
+    def test_force_dense_images(self, layer_cls, args, is_bbox_compatible):
+        images = tf.ragged.stack([tf.ones((5, 5, 3)), tf.ones((8, 8, 3))])
+        labels = tf.ragged.stack([tf.ones((1,)), tf.ones((1,))])
+        bounding_boxes = {
+            "boxes": tf.ragged.constant(
+                [
+                    [[10, 10, 20, 20], [100, 100, 150, 150]],
+                    [[200, 200, 400, 400]],
+                ],
+                dtype=tf.float32,
+            ),
+            "classes": tf.ragged.constant([[0, 1], [2]], dtype=tf.float32),
+        }
         if is_bbox_compatible:
-            self.assertDTypeEqual(outputs[IMAGES], tf.float16)
-            dense_bounding_boxes = bounding_box.to_dense(
-                outputs[BOUNDING_BOXES]
-            )
-            self.assertDTypeEqual(dense_bounding_boxes["boxes"], tf.float16)
+            try:
+                layer = layer_cls(**args, bounding_box_format="xyxy")
+            except TypeError:
+                layer = layer_cls(**args)
+            inputs = {
+                IMAGES: images,
+                LABELS: labels,
+                BOUNDING_BOXES: bounding_boxes,
+            }
         else:
-            self.assertDTypeEqual(outputs[IMAGES], tf.float16)
+            layer = layer_cls(**args)
+            inputs = {IMAGES: images, LABELS: labels}
 
-    @parameterized.named_parameters(*BUILD_IN_RUNTIME)
-    def test_run_in_mixed_precision_and_build_in_runtime(
-        self, layer_cls, args, build_layer_cls, build_args
-    ):
-        keras.mixed_precision.set_global_policy("mixed_float16")
-        images = tf.cast(
-            tf.random.uniform(shape=(4, 32, 32, 3)) * 255.0,
-            dtype=tf.float64,
-        )
-        labels = tf.cast(
-            tf.random.uniform(shape=(4, 1)) * 10.0, dtype=tf.float64
-        )
-        name = args["name"]
-        value = args["value"]
-        other_args = args["args"]
-        if value == "single":
-            build_layers = build_layer_cls(**build_args)
-        elif value == "multiple":
-            build_layers = [
-                build_layer_cls(**build_args),
-                build_layer_cls(**build_args),
-            ]
+        outputs = layer(inputs)
+
+        self.assertTrue(isinstance(outputs[IMAGES], tf.Tensor))
+
+    @parameterized.named_parameters(*NO_RAGGED_IMAGES_SUPPORT)
+    def test_no_ragged_images(self, layer_cls, args, is_bbox_compatible):
+        images = tf.ragged.stack([tf.ones((5, 5, 3)), tf.ones((8, 8, 3))])
+        labels = tf.ragged.stack([tf.ones((1,)), tf.ones((1,))])
+        bounding_boxes = {
+            "boxes": tf.ragged.constant(
+                [
+                    [[10, 10, 20, 20], [100, 100, 150, 150]],
+                    [[200, 200, 400, 400]],
+                ],
+                dtype=tf.float32,
+            ),
+            "classes": tf.ragged.constant([[0, 1], [2]], dtype=tf.float32),
+        }
+        if is_bbox_compatible:
+            try:
+                layer = layer_cls(**args, bounding_box_format="xyxy")
+            except TypeError:
+                layer = layer_cls(**args)
+            inputs = {
+                IMAGES: images,
+                LABELS: labels,
+                BOUNDING_BOXES: bounding_boxes,
+            }
         else:
-            raise NotImplementedError()
-        args = {name: build_layers, **other_args}
-        layer = layer_cls(**args)
-
-        outputs = layer({IMAGES: images, LABELS: labels})
-
-        self.assertDTypeEqual(outputs[IMAGES], tf.float16)
-
-    @classmethod
-    def tearDownClass(cls) -> None:
-        # Do not affect other tests
-        keras.mixed_precision.set_global_policy("float32")
+            layer = layer_cls(**args)
+            inputs = {IMAGES: images, LABELS: labels}
+
+        with self.assertRaises(ValueError):
+            layer(inputs)
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/output_common_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/output_common_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -354,43 +354,23 @@
     layers.RandomZoomAndCrop,
     layers.Mosaic,
     layers.RepeatedAugment,
     layers.CenterCrop,
     layers.Resize,
 ]
 
-NO_BFLOAT16 = [
-    # tf.raw_ops.ImageProjectiveTransformV3 is not supported with bfloat16
-    layers.AugMix,
-    layers.RandAugment,
-    layers.TrivialAugmentWide,
-    layers.RandomAffine,
-    layers.RandomCrop,
-    layers.RandomCropAndResize,
-    layers.RandomRotate,
-    layers.CutMix,  # tf.random.stateless_gamma
-    layers.MixUp,  # tf.random.stateless_gamma
-]
-
 NO_UINT8 = [
     layers.AugMix,  # alpha
     layers.RandAugment,  # stateless_random_uniform
     layers.TrivialAugmentWide,  # stateless_random_uniform
-    layers.RandomAffine,  # stateless_random_uniform
-    layers.RandomCrop,  # stateless_random_uniform
-    layers.RandomRotate,  # stateless_random_uniform
-    layers.RandomZoomAndCrop,  # stateless_random_uniform
     layers.RandomSharpness,  # stateless_random_uniform
     layers.RandomSolarize,  # stateless_random_uniform
     layers.CutMix,  # tf.convert_to_tensor
     layers.MixUp,  # tf.convert_to_tensor
-    layers.Mosaic,  # stateless_random_uniform
     layers.RandomCutout,  # tf.where with -1 (invalid bbox)
-    layers.RandomErase,  # stateless_random_uniform
-    layers.RandomGridMask,  # tf.sqrt
     layers.RandomHSV,  # stateless_random_uniform
     layers.RandomChannelShift,  # stateless_random_uniform
     layers.RandomColorJitter,  # stateless_random_uniform
     layers.RandomGamma,  # stateless_random_uniform
     layers.RandomGaussianBlur,  # tf.nn.depthwise_conv2d
     layers.RandomJpegQuality,  # preprocessing_utils.transform_value_range
     layers.AutoContrast,  # tf.convert_to_tensor
@@ -533,22 +513,17 @@
 
         # float16
         layer = layer_cls(**copied_args, dtype=tf.float16)
         results = layer(inputs)
         self.assertDTypeEqual(results[IMAGES], tf.float16)
 
         # bfloat16
-        if layer_cls not in NO_BFLOAT16:
-            layer = layer_cls(**copied_args, dtype=tf.bfloat16)
-            results = layer(inputs)
-            self.assertDTypeEqual(results[IMAGES], tf.bfloat16)
-        else:
-            with self.assertRaises(tf.errors.InvalidArgumentError):
-                layer = layer_cls(**copied_args, dtype=tf.bfloat16)
-                layer(inputs)
+        layer = layer_cls(**copied_args, dtype=tf.bfloat16)
+        results = layer(inputs)
+        self.assertDTypeEqual(results[IMAGES], tf.bfloat16)
 
         # uint8
         if layer_cls not in NO_UINT8:
             layer = layer_cls(**copied_args, dtype=tf.uint8)
             results = layer(inputs)
             self.assertDTypeEqual(results[IMAGES], tf.uint8)
         else:
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/__internal__/with_bounding_boxes_test.py` & `keras-aug-0.5.5/keras_aug/layers/__internal__/with_bounding_boxes_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/__init__.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/auto/aug_mix.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,32 +81,31 @@
             value_range=self.value_range, dtype=self.compute_dtype
         )
         self.equalize = layers.Equalize(
             value_range=self.value_range, dtype=self.compute_dtype
         )
 
     def get_random_transformation_batch(self, batch_size, **kwargs):
+        # cast to float32 to avoid numerical issue
         # sample from dirichlet
-        alpha = (
-            tf.ones([self.num_chains], dtype=self.compute_dtype) * self.alpha
-        )
+        alpha = tf.ones([self.num_chains], dtype=tf.float32) * self.alpha
         chain_mixing_weights = stateless_random_dirichlet(
             (batch_size, self.num_chains),
             seed=self._random_generator.make_seed_for_stateless_op(),
             alpha=alpha,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         # sample from beta
         weight_sample = stateless_random_beta(
             (batch_size, 1),
             seed_alpha=self._random_generator.make_seed_for_stateless_op(),
             seed_beta=self._random_generator.make_seed_for_stateless_op(),
             alpha=self.alpha,
             beta=self.alpha,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         return {
             "chain_mixing_weights": chain_mixing_weights,
             "weight_sample": weight_sample,
         }
 
     def augment_ragged_image(self, image, transformation, **kwargs):
@@ -142,16 +141,20 @@
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
     def aug_mix_single_image(self, inputs):
         image = inputs.get(IMAGES, None)
         transformation = inputs.get("transformations", None)
 
-        chain_mixing_weights = transformation["chain_mixing_weights"]
-        weight_sample = transformation["weight_sample"]
+        chain_mixing_weights = tf.cast(
+            transformation["chain_mixing_weights"], dtype=self.compute_dtype
+        )
+        weight_sample = tf.cast(
+            transformation["weight_sample"], dtype=self.compute_dtype
+        )
 
         result = tf.zeros_like(image, dtype=image.dtype)
         curr_chain = tf.constant([0], dtype=tf.int32)
         image, chain_mixing_weights, curr_chain, result = tf.while_loop(
             lambda image, chain_mixing_weights, curr_chain, result: tf.less(
                 curr_chain, self.num_chains
             ),
@@ -252,19 +255,23 @@
         angle = tf.expand_dims(
             self.severity(shape=(1,), dtype=tf.float32) * 30, axis=0
         )
         height = tf.expand_dims(tf.shape(image)[H_AXIS : H_AXIS + 1], axis=0)
         width = tf.expand_dims(tf.shape(image)[W_AXIS : W_AXIS + 1], axis=0)
         height = tf.cast(height, dtype=tf.float32)
         width = tf.cast(width, dtype=tf.float32)
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if image.dtype == tf.bfloat16:
+            image = tf.cast(image, dtype=tf.float32)
         image = preprocessing_utils.transform(
             tf.expand_dims(image, axis=0),
             augmentation_utils.get_rotation_matrix(angle, height, width),
         )
-        return tf.squeeze(image, axis=0)
+        image = tf.squeeze(image, axis=0)
+        return tf.cast(image, dtype=self.compute_dtype)
 
     def solarize(self, image):
         threshold = tf.cast(
             tf.cast(self.severity() * 255, tf.int32), image.dtype
         )
         image = tf.where(image < threshold, image, 255 - image)
         return image
@@ -276,19 +283,23 @@
             transform = tf.convert_to_tensor(
                 [1.0, factor, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0]
             )
         else:
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, 0.0, factor, 1.0, 0.0, 0.0, 0.0]
             )
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if image.dtype == tf.bfloat16:
+            image = tf.cast(image, dtype=tf.float32)
         image = preprocessing_utils.transform(
             tf.expand_dims(image, axis=0),
             tf.expand_dims(transform, axis=0),
         )
-        return tf.squeeze(image, axis=0)
+        image = tf.squeeze(image, axis=0)
+        return tf.cast(image, dtype=self.compute_dtype)
 
     def translate(self, image, along_x=True):
         shape = tf.cast(tf.shape(image), tf.float32)
         if along_x:
             size = shape[1]
         else:
             size = shape[0]
@@ -298,19 +309,23 @@
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, factor, 0.0, 1.0, 0.0, 0.0, 0.0]
             )
         else:
             transform = tf.convert_to_tensor(
                 [1.0, 0.0, 0.0, 0.0, 1.0, factor, 0.0, 0.0]
             )
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if image.dtype == tf.bfloat16:
+            image = tf.cast(image, dtype=tf.float32)
         image = preprocessing_utils.transform(
             tf.expand_dims(image, axis=0),
             tf.expand_dims(transform, axis=0),
         )
-        return tf.squeeze(image, axis=0)
+        image = tf.squeeze(image, axis=0)
+        return tf.cast(image, dtype=self.compute_dtype)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "value_range": self.value_range,
                 "severity": self.severity,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/auto/aug_mix_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/aug_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/auto/rand_augment.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/auto/rand_augment_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/rand_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/auto/trivial_augment_wide.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/auto/trivial_augment_wide.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_affine.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,54 +208,53 @@
             self.shear_width_factor, not_working_value=0.0
         )
         self._enable_shear = _enable_shear_height or _enable_shear_width
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
+        # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
         factor_shape = (batch_size, 1)
         # dummy
-        angles = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        translation_heights = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        translation_widths = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        zoom_heights = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        zoom_widths = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        shear_heights = tf.zeros(factor_shape, dtype=self.compute_dtype)
-        shear_widths = tf.zeros(factor_shape, dtype=self.compute_dtype)
+        angles = tf.zeros(factor_shape, dtype=tf.float32)
+        translation_heights = tf.zeros(factor_shape, dtype=tf.float32)
+        translation_widths = tf.zeros(factor_shape, dtype=tf.float32)
+        zoom_heights = tf.zeros(factor_shape, dtype=tf.float32)
+        zoom_widths = tf.zeros(factor_shape, dtype=tf.float32)
+        shear_heights = tf.zeros(factor_shape, dtype=tf.float32)
+        shear_widths = tf.zeros(factor_shape, dtype=tf.float32)
 
         if self._enable_rotation:
-            angles = self.rotation_factor(
-                factor_shape, dtype=self.compute_dtype
-            )
+            angles = self.rotation_factor(factor_shape, dtype=tf.float32)
         if self._enable_translation:
             translation_heights = self.translation_height_factor(
-                factor_shape, dtype=self.compute_dtype
+                factor_shape, dtype=tf.float32
             )
             translation_widths = self.translation_width_factor(
-                factor_shape, dtype=self.compute_dtype
+                factor_shape, dtype=tf.float32
             )
         if self._enable_zoom:
             zoom_heights = self.zoom_height_factor(
-                factor_shape, dtype=self.compute_dtype
+                factor_shape, dtype=tf.float32
             )
             if self.same_zoom_factor:
                 zoom_widths = zoom_heights
             else:
                 zoom_widths = self.zoom_width_factor(
-                    factor_shape, dtype=self.compute_dtype
+                    factor_shape, dtype=tf.float32
                 )
         if self._enable_shear:
             shear_heights = self.shear_height_factor(
-                factor_shape, dtype=self.compute_dtype
+                factor_shape, dtype=tf.float32
             )
             shear_widths = self.shear_width_factor(
-                factor_shape, dtype=self.compute_dtype
+                factor_shape, dtype=tf.float32
             )
 
         angles = angles / 360.0 * 2.0 * math.pi
         translations = tf.concat(
             [translation_widths, translation_heights], axis=1
         )
         zooms = tf.concat([zoom_widths, zoom_heights], axis=1)
@@ -263,19 +262,19 @@
 
         # start from identity matrixes:
         #     [[1 0 0]
         #      [0 1 0]
         #      [0 0 1]]
         identity_matrixes = tf.concat(
             [
-                tf.ones((batch_size, 1), dtype=self.compute_dtype),
-                tf.zeros((batch_size, 3), dtype=self.compute_dtype),
-                tf.ones((batch_size, 1), dtype=self.compute_dtype),
-                tf.zeros((batch_size, 3), dtype=self.compute_dtype),
-                tf.ones((batch_size, 1), dtype=self.compute_dtype),
+                tf.ones((batch_size, 1), dtype=tf.float32),
+                tf.zeros((batch_size, 3), dtype=tf.float32),
+                tf.ones((batch_size, 1), dtype=tf.float32),
+                tf.zeros((batch_size, 3), dtype=tf.float32),
+                tf.ones((batch_size, 1), dtype=tf.float32),
             ],
             axis=1,
         )
         combined_matrixes = tf.reshape(identity_matrixes, (batch_size, 3, 3))
         # process zoom
         if self._enable_zoom:
             zoom_matrixes = augmentation_utils.get_zoom_matrix(
@@ -315,55 +314,59 @@
         )
         image = self.augment_images(
             images=image, transformations=transformation, **kwargs
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
-        original_shape = images.shape
+        ori_shape = images.shape
         batch_size = tf.shape(images)[0]
         combined_matrixes = transformations["combined_matrixes"]
         combined_matrixes = tf.reshape(
             combined_matrixes, shape=(batch_size, -1)
         )
         combined_matrixes = combined_matrixes[:, :-1]
 
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if images.dtype == tf.bfloat16:
+            images = tf.cast(images, dtype=tf.float32)
         images = preprocessing_utils.transform(
             images,
-            tf.cast(combined_matrixes, dtype=tf.float32),  # must be float32
+            combined_matrixes,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
             interpolation=self.interpolation,
         )
-        images = tf.ensure_shape(images, shape=original_shape)
-        return images
+        images = tf.ensure_shape(images, shape=ori_shape)
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
     def augment_bounding_boxes(
         self, bounding_boxes, transformations, raw_images=None, **kwargs
     ):
         if self.bounding_box_format is None:
             raise ValueError(
                 "`RandomAffine()` was called with bounding boxes,"
                 "but no `bounding_box_format` was specified in the constructor."
                 "Please specify a bounding box format in the constructor. i.e."
                 "`RandomAffine(bounding_box_format='xyxy')`"
             )
+        # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            raw_images, dtype=self.compute_dtype
+            raw_images, dtype=tf.float32
         )
         bounding_boxes = bounding_box.to_dense(bounding_boxes)
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source=self.bounding_box_format,
             target="xyxy",
             images=raw_images,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         boxes = bounding_boxes["boxes"]
         original_bounding_boxes = bounding_boxes.copy()
         # process rotations
         if self._enable_rotation:
             origin_x = widths / 2
             origin_y = heights / 2
@@ -495,25 +498,28 @@
         batch_size = tf.shape(segmentation_masks)[0]
         combined_matrixes = transformations["combined_matrixes"]
         combined_matrixes = tf.reshape(
             combined_matrixes, shape=(batch_size, -1)
         )
         combined_matrixes = combined_matrixes[:, :-1]
 
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if segmentation_masks.dtype == tf.bfloat16:
+            segmentation_masks = tf.cast(segmentation_masks, dtype=tf.float32)
         segmentation_masks = preprocessing_utils.transform(
             segmentation_masks,
-            tf.cast(combined_matrixes, dtype=tf.float32),  # must be float32
+            combined_matrixes,
             fill_mode=self.fill_mode,
             fill_value=0,
             interpolation="nearest",
         )
         segmentation_masks = tf.ensure_shape(
             segmentation_masks, shape=original_shape
         )
-        return segmentation_masks
+        return tf.cast(segmentation_masks, dtype=self.compute_dtype)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "rotation_factor": self.rotation_factor,
                 "translation_height_factor": self.translation_height_factor,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_affine_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_affine_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,20 @@
         # set force_output_dense_images=True because the output images must
         # have same shape (B, height, width, C)
         self.force_output_dense_images = True
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
+        # cast to float32 to avoid numerical issue
         tops = self._random_generator.random_uniform(
-            shape=(batch_size, 1), minval=0, maxval=1, dtype=self.compute_dtype
+            shape=(batch_size, 1), minval=0, maxval=1, dtype=tf.float32
         )
         lefts = self._random_generator.random_uniform(
-            shape=(batch_size, 1), minval=0, maxval=1, dtype=self.compute_dtype
+            shape=(batch_size, 1), minval=0, maxval=1, dtype=tf.float32
         )
         return {"crop_tops": tops, "crop_lefts": lefts}
 
     def compute_ragged_image_signature(self, images):
         ragged_spec = tf.RaggedTensorSpec(
             shape=(self.height, self.width, images.shape[-1]),
             ragged_rank=1,
@@ -105,15 +106,15 @@
             tf.math.logical_and(h_diffs >= 0, w_diffs >= 0),
             self.crop_images(images, transformations),
             self.resize_images(images, interpolation=self.interpolation),
         )
         images = tf.ensure_shape(
             images, shape=(None, self.height, self.width, None)
         )
-        return images
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
     def augment_bounding_boxes(
         self,
         bounding_boxes,
@@ -215,36 +216,40 @@
             tf.math.logical_and(h_diffs >= 0, w_diffs >= 0),
             self.crop_images(segmentation_masks, transformations),
             self.resize_images(segmentation_masks, interpolation="nearest"),
         )
         segmentation_masks = tf.ensure_shape(
             segmentation_masks, shape=(None, self.height, self.width, None)
         )
-        return segmentation_masks
+        return tf.cast(segmentation_masks, dtype=self.compute_dtype)
 
     def crop_images(self, images, transformations):
         batch_size = tf.shape(images)[0]
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
         tops = transformations["crop_tops"]
         lefts = transformations["crop_lefts"]
         x1s = lefts * (widths - self.width)
         y1s = tops * (heights - self.height)
         x2s = x1s + self.width
         y2s = y1s + self.height
         # normalize
         x1s /= widths
         y1s /= heights
         x2s /= widths
         y2s /= heights
         boxes = tf.concat([y1s, x1s, y2s, x2s], axis=-1)
+
+        # tf.image.crop_and_resize not support bfloat16
+        if images.dtype == tf.bfloat16:
+            images = tf.cast(images, dtype=tf.float32)
         images = tf.image.crop_and_resize(
             images,
-            tf.cast(boxes, dtype=tf.float32),  # must be tf.float32
+            boxes,
             tf.range(batch_size),
             [self.height, self.width],
             method="nearest",
         )
         return tf.cast(images, dtype=self.compute_dtype)
 
     def resize_images(self, images, interpolation="bilinear"):
@@ -256,15 +261,15 @@
             raise ValueError(f"Unsupported interpolation: {interpolation}")
         return tf.cast(images, dtype=self.compute_dtype)
 
     def crop_bounding_boxes(self, images, boxes, transformation):
         tops = transformation["crop_tops"]
         lefts = transformation["crop_lefts"]
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
 
         # compute offsets for xyxy bounding_boxes
         top_offsets = tf.cast(
             tf.math.round(tops * (heights - self.height)),
             dtype=self.compute_dtype,
         )
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,18 @@
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
         batch_size = tf.shape(images)[0]
         boxes = transformations
         indices = tf.range(batch_size)
+
+        # tf.image.crop_and_resize not support bfloat16
+        if images.dtype == tf.bfloat16:
+            images = tf.cast(images, dtype=tf.float32)
         images = tf.image.crop_and_resize(
             images,  # image shape: [B, H, W, C]
             boxes,  # boxes: (B, 4) in this case; represents area
             # to be cropped from the original image
             indices,  # box_indices: maps boxes to images along batch axis
             [self.height, self.width],  # output size
             method=self.interpolation,
@@ -238,14 +242,18 @@
 
     def augment_segmentation_masks(
         self, segmentation_masks, transformations, **kwargs
     ):
         batch_size = tf.shape(segmentation_masks)[0]
         boxes = transformations
         indices = tf.range(batch_size)
+
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if segmentation_masks.dtype == tf.bfloat16:
+            segmentation_masks = tf.cast(segmentation_masks, dtype=tf.float32)
         segmentation_masks = tf.image.crop_and_resize(
             segmentation_masks,  # image shape: [B, H, W, C]
             boxes,  # boxes: (B, 4) in this case; represents area
             # to be cropped from the original image
             indices,  # box_indices: maps boxes to images along batch axis
             [self.height, self.width],  # output size
             method="nearest",
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_crop_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_flip.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_flip_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_resize.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_resize_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_rotate.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,18 +69,19 @@
         self.fill_value = fill_value
         self.bounding_box_format = bounding_box_format
         self.seed = seed
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
+        # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
-        angles = self.factor(shape=(batch_size, 1), dtype=self.compute_dtype)
+        angles = self.factor(shape=(batch_size, 1), dtype=tf.float32)
         angles = angles / 360.0 * 2.0 * math.pi
         rotation_matrixes = augmentation_utils.get_rotation_matrix(
             angles, heights, widths, to_square=True
         )
         # (batch_size, 3, 3)
         return {
             "angles": angles,
@@ -101,47 +102,52 @@
         original_shape = images.shape
         batch_size = tf.shape(images)[0]
         rotation_matrixes = transformations["rotation_matrixes"]
         rotation_matrixes = tf.reshape(
             rotation_matrixes, shape=(batch_size, -1)
         )
         rotation_matrixes = rotation_matrixes[:, :-1]
+
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if images.dtype == tf.bfloat16:
+            images = tf.cast(images, dtype=tf.float32)
         images = preprocessing_utils.transform(
             images,
-            tf.cast(rotation_matrixes, dtype=tf.float32),  # must be tf.float32
+            rotation_matrixes,
             fill_mode=self.fill_mode,
             fill_value=self.fill_value,
             interpolation=self.interpolation,
         )
         images = tf.ensure_shape(images, shape=original_shape)
-        return images
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def augment_labels(self, labels, transformations, **kwargs):
         return labels
 
     def augment_bounding_boxes(
         self, bounding_boxes, transformations, raw_images=None, **kwargs
     ):
         if self.bounding_box_format is None:
             raise ValueError(
                 "`RandomAffine()` was called with bounding boxes,"
                 "but no `bounding_box_format` was specified in the constructor."
                 "Please specify a bounding box format in the constructor. i.e."
                 "`RandomAffine(bounding_box_format='xyxy')`"
             )
+        # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            raw_images, dtype=self.compute_dtype
+            raw_images, dtype=tf.float32
         )
         bounding_boxes = bounding_box.to_dense(bounding_boxes)
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source=self.bounding_box_format,
             target="xyxy",
             images=raw_images,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         boxes = bounding_boxes["boxes"]
 
         # process rotations
         origin_x = widths / 2
         origin_y = heights / 2
         angles = -transformations["angles"]
@@ -210,25 +216,29 @@
         original_shape = segmentation_masks.shape
         batch_size = tf.shape(segmentation_masks)[0]
         rotation_matrixes = transformations["rotation_matrixes"]
         rotation_matrixes = tf.reshape(
             rotation_matrixes, shape=(batch_size, -1)
         )
         rotation_matrixes = rotation_matrixes[:, :-1]
+
+        # tf.raw_ops.ImageProjectiveTransformV3 not support bfloat16
+        if segmentation_masks.dtype == tf.bfloat16:
+            segmentation_masks = tf.cast(segmentation_masks, dtype=tf.float32)
         segmentation_masks = preprocessing_utils.transform(
             segmentation_masks,
             rotation_matrixes,
             fill_mode=self.fill_mode,
             fill_value=0,
             interpolation="nearest",
         )
         segmentation_masks = tf.ensure_shape(
             segmentation_masks, shape=original_shape
         )
-        return segmentation_masks
+        return tf.cast(segmentation_masks, dtype=self.compute_dtype)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "factor": self.factor,
                 "fill_mode": self.fill_mode,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_rotate_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_rotate_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,37 +102,38 @@
         self.padding_value = padding_value
         self.bounding_box_format = bounding_box_format
         self.seed = seed
 
         crop_size = tf.expand_dims(
             tf.stack([self.crop_height, self.crop_width]), axis=0
         )
-        self.crop_size = tf.cast(crop_size, dtype=self.compute_dtype)
+        self.crop_size = tf.cast(crop_size, dtype=tf.float32)
         self.force_output_dense_images = True
 
     def compute_ragged_image_signature(self, images):
         ragged_spec = tf.RaggedTensorSpec(
             shape=(self.height, self.width, images.shape[-1]),
             ragged_rank=1,
             dtype=self.compute_dtype,
         )
         return ragged_spec
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
+        # cast to float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
 
         # image_scales
         image_shapes = tf.concat((heights, widths), axis=-1)
         scaled_sizes = tf.round(
             image_shapes
-            * self.scale_factor(shape=(batch_size, 1), dtype=self.compute_dtype)
+            * self.scale_factor(shape=(batch_size, 1), dtype=tf.float32)
         )
         scales = tf.where(
             tf.less(
                 scaled_sizes[..., 0:1] / image_shapes[..., 0:1],
                 scaled_sizes[..., 1:] / image_shapes[..., 1:],
             ),
             scaled_sizes[..., 0:1] / image_shapes[..., 0:1],
@@ -143,17 +144,17 @@
 
         # offsets
         max_offsets = scaled_sizes - self.crop_size
         max_offsets = tf.where(
             tf.less(max_offsets, 0), tf.zeros_like(max_offsets), max_offsets
         )
         offsets = max_offsets * self._random_generator.random_uniform(
-            shape=(batch_size, 2), minval=0, maxval=1, dtype=self.compute_dtype
+            shape=(batch_size, 2), minval=0, maxval=1, dtype=tf.float32
         )
-        offsets = tf.cast(offsets, tf.int32)
+        offsets = tf.cast(offsets, dtype=tf.int32)
 
         # paddings
         new_heights = tf.cast(scaled_sizes[..., 0:1], dtype=tf.int32)
         new_widths = tf.cast(scaled_sizes[..., 1:], dtype=tf.int32)
         tops = tf.where(
             new_heights < self.crop_height,
             tf.cast((self.crop_height - new_heights) / 2, tf.int32),
@@ -228,28 +229,29 @@
         if self.bounding_box_format is None:
             raise ValueError(
                 "`RandomZoomAndCrop()` was called with bounding boxes,"
                 "but no `bounding_box_format` was specified in the constructor."
                 "Please specify a bounding box format in the constructor. i.e."
                 "`RandomZoomAndCrop(..., bounding_box_format='xyxy')`"
             )
+        # cast to float32 to avoid numerical issue
         bounding_boxes = bounding_box.to_dense(bounding_boxes)
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source=self.bounding_box_format,
             target="yxyx",
             images=raw_images,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
 
         image_scales = tf.cast(
-            transformations["image_scales"], self.compute_dtype
+            transformations["image_scales"], dtype=tf.float32
         )
-        offsets = tf.cast(transformations["offsets"], self.compute_dtype)
-        paddings = tf.cast(transformations["paddings"], self.compute_dtype)
+        offsets = tf.cast(transformations["offsets"], dtype=tf.float32)
+        paddings = tf.cast(transformations["paddings"], dtype=tf.float32)
         padding_offsets = tf.concat(
             [paddings[..., 0:1], paddings[..., 2:3]], axis=-1
         )
 
         # Adjusts box coordinates based on image_scale and offset.
         bounding_boxes = bounding_boxes.copy()
         yxyx = bounding_boxes["boxes"]
@@ -264,14 +266,15 @@
             images=images,
         )
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source="yxyx",
             target=self.bounding_box_format,
             images=images,
+            dtype=self.compute_dtype,
         )
         return bounding_boxes
 
     def compute_ragged_segmentation_mask_signature(self, segmentation_masks):
         return tf.RaggedTensorSpec(
             shape=(self.height, self.width, segmentation_masks.shape[-1]),
             ragged_rank=1,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/channel_shuffle.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_blur.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_blur_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_channel_shift.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_clahe.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,22 @@
         )
         return tf.squeeze(image, axis=0)
 
     def augment_images(self, images, transformations, **kwargs):
         images = preprocessing_utils.transform_value_range(
             images, self.value_range, (0, 255), dtype=self.compute_dtype
         )
-        inputs_for_RandomCLAHE_single_image = {
+        inputs_for_clahe_single_image = {
             "images": images,
             "clip_limits": transformations,
         }
-        images = tf.vectorized_map(
-            self.RandomCLAHE_single_image,
-            inputs_for_RandomCLAHE_single_image,
+        images = tf.map_fn(
+            self.clahe_single_image,
+            inputs_for_clahe_single_image,
+            fn_output_signature=self.compute_dtype,
         )
         images = preprocessing_utils.transform_value_range(
             images, (0, 255), self.value_range, dtype=self.compute_dtype
         )
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
@@ -100,15 +101,15 @@
         )
         clipped_px_count = tf.math.reduce_sum(hists - clipped_hists, axis=0)
         clipped_hists = tf.cast(clipped_hists, tf.float32)
         clipped_px_count = tf.cast(clipped_px_count, tf.float32)
         clipped_hists = clipped_hists + tf.math.truediv(clipped_px_count, 256)
         return clipped_hists
 
-    def RandomCLAHE_single_image(self, inputs):
+    def clahe_single_image(self, inputs):
         image = inputs.get("images", None)
         clip_limit = inputs.get("clip_limits", None)
 
         original_2d_shape = (tf.shape(image)[0], tf.shape(image)[1])
         original_dtype = image.dtype
 
         # Need image in int32 format for later gather_nd ops
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_clahe_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_clahe_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         args.update({"value_range": (0, 100)})
         layer = layers.RandomCLAHE(**args)
 
         output = layer(image)
 
         self.assertNotAllClose(image, output)
 
-    def test_RandomCLAHE_output(self):
+    def test_random_clahe_output(self):
         image_shape = (4, 8, 8, 3)
         image = tf.random.uniform(shape=image_shape) * 255.0
         image = tf.cast(image, dtype=tf.uint8)
         args = self.regular_args.copy()
         args.update({"factor": (1, 1), "tile_grid_size": (1, 1)})
         layer = layers.RandomCLAHE(**args)
         equalized = equalize(image)
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_color_jitter.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,40 +174,45 @@
     def adjust_brightness(self, images, transformations):
         brightness_factors = transformations["brightness_factors"]
         images *= brightness_factors
         images = tf.clip_by_value(images, 0, 255)
         return images
 
     def adjust_contrast(self, images, transformations):
-        contrast_factors = transformations["contrast_factors"]
+        # cast to float32 to avoid numerical issue
+        contrast_factors = tf.cast(
+            transformations["contrast_factors"], dtype=tf.float32
+        )
+        images = tf.cast(images, dtype=tf.float32)
         degenerates = augmentation_utils.rgb_to_grayscale(images)
         degenerates = tf.reduce_mean(degenerates, axis=(1, 2, 3), keepdims=True)
         images = augmentation_utils.blend(degenerates, images, contrast_factors)
         images = tf.clip_by_value(images, 0, 255)
-        return images
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def adjust_saturation(self, images, transformations):
         saturation_factors = transformations["saturation_factors"]
         degenerates = augmentation_utils.rgb_to_grayscale(images)
         images = augmentation_utils.blend(
             degenerates, images, saturation_factors, (0, 255)
         )
         images = tf.clip_by_value(images, 0, 255)
         return images
 
     def adjust_hue(self, images, transformations):
-        images = tf.image.rgb_to_hsv(images)
-        hue_factors = transformations["hue_factors"]
+        # cast to float32 to avoid numerical issue
+        images = tf.image.rgb_to_hsv(tf.cast(images, dtype=tf.float32))
+        hue_factors = tf.cast(transformations["hue_factors"], dtype=tf.float32)
         h_channels = tf.math.floormod(images[..., 0:1] + hue_factors, 1.0)
         images = tf.concat(
             [h_channels, images[..., 1:2], images[..., 2:3]], axis=-1
         )
         images = tf.image.hsv_to_rgb(images)
         images = tf.clip_by_value(images, 0, 255)
-        return images
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "value_range": self.value_range,
                 "brightness_factor": self.brightness_factor,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gamma.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gamma_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gamma_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_hsv.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,22 +150,24 @@
     ):
         return segmentation_masks
 
     def augment_keypoints(self, keypoints, transformations, **kwargs):
         return keypoints
 
     def adjust_hue(self, images, transformations):
-        images = tf.image.rgb_to_hsv(images)
-        hue_factors = transformations["hue_factors"]
+        # cast to float32 to avoid numerical issue
+        images = tf.image.rgb_to_hsv(tf.cast(images, dtype=tf.float32))
+        hue_factors = tf.cast(transformations["hue_factors"], dtype=tf.float32)
         h_channels = tf.math.floormod(images[..., 0:1] + hue_factors, 1.0)
         images = tf.concat(
             [h_channels, images[..., 1:2], images[..., 2:3]], axis=-1
         )
         images = tf.image.hsv_to_rgb(images)
-        return images
+        images = tf.clip_by_value(images, 0, 255)
+        return tf.cast(images, dtype=self.compute_dtype)
 
     def adjust_saturation(self, images, transformations):
         saturation_factors = transformations["saturation_factors"]
         degenerates = augmentation_utils.rgb_to_grayscale(images)
         images = augmentation_utils.blend(
             degenerates, images, saturation_factors, (0, 255)
         )
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_hsv_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_hsv_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_posterize.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_posterize_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_posterize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_sharpness.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_sharpness_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_sharpness_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_solarize.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/intensity/random_solarize_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/intensity/random_solarize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/cut_mix.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,42 +45,36 @@
         # set force_no_unwrap_ragged_image_call=True because CutMix needs
         # to process images in batch.
         self.force_no_unwrap_ragged_image_call = True
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
-        height = tf.cast(tf.shape(images)[H_AXIS], dtype=self.compute_dtype)
-        width = tf.cast(tf.shape(images)[W_AXIS], dtype=self.compute_dtype)
+        height = tf.cast(tf.shape(images)[H_AXIS], dtype=tf.float32)
+        width = tf.cast(tf.shape(images)[W_AXIS], dtype=tf.float32)
         permutation_order = self._random_generator.random_uniform(
             (batch_size,),
             minval=0,
             maxval=batch_size,
             dtype=tf.int32,
         )
         lambda_samples = stateless_random_beta(
             (batch_size,),
             seed_alpha=self._random_generator.make_seed_for_stateless_op(),
             seed_beta=self._random_generator.make_seed_for_stateless_op(),
             alpha=self.alpha,
             beta=self.alpha,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         ratios = tf.math.sqrt(1.0 - lambda_samples)
-        height = tf.cast(tf.shape(images)[H_AXIS], dtype=self.compute_dtype)
-        width = tf.cast(tf.shape(images)[W_AXIS], dtype=self.compute_dtype)
         cut_heights = tf.cast(ratios * height, dtype=tf.int32)
         cut_widths = tf.cast(ratios * width, dtype=tf.int32)
-        center_xs = self._random_generator.random_uniform(
-            shape=(batch_size,), dtype=self.compute_dtype
-        )
+        center_xs = self._random_generator.random_uniform(shape=(batch_size,))
         center_xs = tf.cast(center_xs * width, dtype=tf.int32)
-        center_ys = self._random_generator.random_uniform(
-            shape=(batch_size,), dtype=self.compute_dtype
-        )
+        center_ys = self._random_generator.random_uniform(shape=(batch_size,))
         center_ys = tf.cast(center_ys * height, dtype=tf.int32)
         return {
             "permutation_order": permutation_order,
             "center_xs": center_xs,
             "center_ys": center_ys,
             "cut_heights": cut_heights,
             "cut_widths": cut_widths,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/cut_mix_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/cut_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mix_up.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,46 +40,51 @@
         self.seed = seed
 
         # set force_no_unwrap_ragged_image_call=True because MixUp needs
         # to process images in batch.
         self.force_no_unwrap_ragged_image_call = True
 
     def get_random_transformation_batch(self, batch_size, **kwargs):
+        # cast to float32 to avoid numerical issue
         permutation_order = tf.argsort(
             self._random_generator.random_uniform((batch_size,)), axis=-1
         )
         lambda_samples = stateless_random_beta(
             (batch_size, 1, 1, 1),
             seed_alpha=self._random_generator.make_seed_for_stateless_op(),
             seed_beta=self._random_generator.make_seed_for_stateless_op(),
             alpha=self.alpha,
             beta=self.alpha,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         return {
             "permutation_order": permutation_order,
             "lambda_samples": lambda_samples,
         }
 
     def augment_images(self, images, transformations, **kwargs):
         if isinstance(images, tf.RaggedTensor):
             raise ValueError(
                 "MixUp expects dense images. Received: images type: "
                 f"{type(images)}"
             )
         permutation_order = transformations["permutation_order"]
-        lambda_samples = transformations["lambda_samples"]
+        lambda_samples = tf.cast(
+            transformations["lambda_samples"], dtype=self.compute_dtype
+        )
         mixup_images = tf.gather(images, permutation_order)
         mixup_images = tf.cast(mixup_images, dtype=self.compute_dtype)
         images = lambda_samples * images + (1.0 - lambda_samples) * mixup_images
         return images
 
     def augment_labels(self, labels, transformations, **kwargs):
         permutation_order = transformations["permutation_order"]
-        lambda_samples = transformations["lambda_samples"]
+        lambda_samples = tf.cast(
+            transformations["lambda_samples"], dtype=self.compute_dtype
+        )
         labels = tf.cast(labels, dtype=self.compute_dtype)
         mixup_labels = tf.gather(labels, permutation_order)
         lambda_samples = tf.reshape(lambda_samples, [-1, 1])
         labels = lambda_samples * labels + (1.0 - lambda_samples) * mixup_labels
         return labels
 
     def augment_bounding_boxes(self, bounding_boxes, transformations, **kwargs):
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mix_up_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mix_up_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mosaic.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,16 @@
         # concatenate the batches with permutation order to get all 4 images of
         # the mosaic
         permutation_order = tf.concat(
             [tf.expand_dims(tf.range(batch_size), axis=-1), permutation_order],
             axis=-1,
         )
 
-        mosaic_centers_x = self.center_sampler(
-            shape=(batch_size,), dtype=self.compute_dtype
-        )
-        mosaic_centers_y = self.center_sampler(
-            shape=(batch_size,), dtype=self.compute_dtype
-        )
+        mosaic_centers_x = self.center_sampler(shape=(batch_size,))
+        mosaic_centers_y = self.center_sampler(shape=(batch_size,))
         mosaic_centers = tf.stack((mosaic_centers_x, mosaic_centers_y), axis=-1)
 
         return {
             "permutation_order": permutation_order,
             "mosaic_centers": mosaic_centers,
         }
 
@@ -129,20 +125,21 @@
         images = tf.ensure_shape(
             images,
             shape=(ori_shape[0], self.height, self.width, ori_shape[-1]),
         )
         return images
 
     def augment_labels(self, labels, transformations, images=None, **kwargs):
+        # cast to float32 to avoid numerical issue
         is_ragged_labels = isinstance(labels, tf.RaggedTensor)
         if is_ragged_labels:
             labels = labels.to_tensor()
-        labels = tf.cast(labels, dtype=self.compute_dtype)
+        labels = tf.cast(labels, dtype=tf.float32)
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
         # updates labels for one output mosaic
         permutation_order = transformations["permutation_order"]
         labels_for_mosaic = tf.gather(labels, permutation_order)
 
         mosaic_centers = transformations["mosaic_centers"]
         center_xs = tf.expand_dims(mosaic_centers[..., 0], axis=-1) * widths
@@ -161,30 +158,30 @@
             labels_for_mosaic[:, 0] * top_left_ratio
             + labels_for_mosaic[:, 1] * top_right_ratio
             + labels_for_mosaic[:, 2] * bottom_left_ratio
             + labels_for_mosaic[:, 3] * bottom_right_ratio
         )
         if is_ragged_labels:
             labels = tf.RaggedTensor.from_tensor(labels)
-        return labels
+        return tf.cast(labels, dtype=self.compute_dtype)
 
     def augment_bounding_boxes(
         self, bounding_boxes, transformations, raw_images=None, **kwargs
     ):
         batch_size = tf.shape(raw_images)[0]
         heights, widths = augmentation_utils.get_images_shape(
-            raw_images, dtype=self.compute_dtype
+            raw_images, dtype=tf.float32
         )
         bounding_boxes = bounding_box.to_dense(bounding_boxes)
         bounding_boxes = bounding_box.convert_format(
             bounding_boxes,
             source=self.bounding_box_format,
             target="xyxy",
             images=raw_images,
-            dtype=self.compute_dtype,
+            dtype=tf.float32,
         )
         boxes, classes = bounding_boxes["boxes"], bounding_boxes["classes"]
 
         # values to translate the boxes by in the mosaic image
         mosaic_centers = transformations["mosaic_centers"]
         mosaic_centers_x = tf.expand_dims(
             mosaic_centers[..., 0] * self.width, axis=-1
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/mix/mosaic_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/mix/mosaic_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_channel_dropout.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_cutout.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_cutout_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_cutout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_erase.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,44 +75,42 @@
 
         self.max_attemp = 10
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
         areas = heights * widths
 
         is_success = False
         for _ in range(self.max_attemp):
             if not is_success:
-                erasing_areas = self.area_factor(
-                    shape=(batch_size, 1), dtype=self.compute_dtype
-                )
+                erasing_areas = self.area_factor(shape=(batch_size, 1))
                 erasing_areas = erasing_areas * areas
                 erasing_aspect_ratios = self.aspect_ratio_factor(
-                    shape=(batch_size, 1), dtype=self.compute_dtype
+                    shape=(batch_size, 1)
                 )
                 erasing_heights = tf.round(
                     tf.sqrt(erasing_areas * erasing_aspect_ratios)
                 )
                 erasing_widths = tf.round(
                     tf.sqrt(erasing_areas / erasing_aspect_ratios)
                 )
                 if tf.reduce_all(
                     tf.less(erasing_widths, widths)
                 ) and tf.reduce_all(tf.less(erasing_heights, heights)):
                     is_success = True
 
         center_xs = self._random_generator.random_uniform(
-            shape=(batch_size, 1), minval=0, maxval=1, dtype=self.compute_dtype
+            shape=(batch_size, 1), minval=0, maxval=1, dtype=tf.float32
         )
         center_ys = self._random_generator.random_uniform(
-            shape=(batch_size, 1), minval=0, maxval=1, dtype=self.compute_dtype
+            shape=(batch_size, 1), minval=0, maxval=1, dtype=tf.float32
         )
         center_xs = tf.round(center_xs * (widths - erasing_widths))
         center_xs = tf.cast(center_xs + erasing_widths / 2, dtype=tf.int32)
         center_ys = tf.round(center_ys * (heights - erasing_heights))
         center_ys = tf.cast(center_ys + erasing_heights / 2, dtype=tf.int32)
 
         return {
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_erase_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_erase_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_grid_mask.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,45 +99,38 @@
                 '"gaussian_noise", or "random". Got '
                 f"`fill_mode`={fill_mode}"
             )
 
     def get_random_transformation_batch(
         self, batch_size, images=None, **kwargs
     ):
+        # all operations run in tf.float32 to avoid numerical issue
         heights, widths = augmentation_utils.get_images_shape(
-            images, dtype=self.compute_dtype
+            images, dtype=tf.float32
         )
 
         # mask side length
         input_diagonal_lens = tf.sqrt(tf.square(widths) + tf.square(heights))
         mask_side_lens = tf.math.ceil(input_diagonal_lens)
 
         # grid unit size
         smaller_side_lens = tf.where(heights < widths, heights, widths)
-        unit_ratios = self.size_factor(
-            shape=(batch_size, 1), dtype=self.compute_dtype
-        )
+        unit_ratios = self.size_factor(shape=(batch_size, 1))
         unit_sizes = unit_ratios * smaller_side_lens
         unit_sizes = tf.maximum(unit_sizes, 2)  # prevent too small units
-        ratios = self.ratio_factor(
-            shape=(batch_size, 1), dtype=self.compute_dtype
-        )
+        ratios = self.ratio_factor(shape=(batch_size, 1))
         rectangle_side_lens = ratios * unit_sizes
 
         # sample x and y offset for grid units randomly between 0 and unit_size
-        delta_xs = self._random_generator.random_uniform(
-            shape=(batch_size, 1), dtype=self.compute_dtype
-        )
-        delta_ys = self._random_generator.random_uniform(
-            shape=(batch_size, 1), dtype=self.compute_dtype
-        )
+        delta_xs = self._random_generator.random_uniform(shape=(batch_size, 1))
+        delta_ys = self._random_generator.random_uniform(shape=(batch_size, 1))
         delta_xs = delta_xs * unit_sizes
         delta_ys = delta_ys * unit_sizes
 
-        # randomly rotate mask (must be tf.float32)
+        # randomly rotate mask
         angles = self.rotation_factor(shape=(batch_size, 1))
         angles = angles / 360.0 * 2.0 * math.pi
 
         return {
             "mask_side_lens": mask_side_lens,
             "rectangle_side_lens": rectangle_side_lens,
             "unit_sizes": unit_sizes,
```

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_apply.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_apply_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_apply_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_choice.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/random_choice_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/random_choice_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/repeated_augment.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/augmentation/utility/repeated_augment_test.py` & `keras-aug-0.5.5/keras_aug/layers/augmentation/utility/repeated_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/base/vectorized_base_random_layer.py` & `keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/base/vectorized_base_random_layer_test.py` & `keras-aug-0.5.5/keras_aug/layers/base/vectorized_base_random_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/__init__.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/center_crop.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/center_crop_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/pad_if_needed.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/resize.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/geometry/resize_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/geometry/resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/auto_contrast.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/equalize.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/equalize_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/equalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/grayscale.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/grayscale_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/grayscale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/identity.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/identity_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/invert.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/invert.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/normalize.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/normalize_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/normalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/rescale.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/intensity/rescale_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/intensity/rescale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py` & `keras-aug-0.5.5/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/augmentation.py` & `keras-aug-0.5.5/keras_aug/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/augmentation_test.py` & `keras-aug-0.5.5/keras_aug/utils/augmentation_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/bounding_box.py` & `keras-aug-0.5.5/keras_aug/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/bounding_box_test.py` & `keras-aug-0.5.5/keras_aug/utils/bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/demo.py` & `keras-aug-0.5.5/keras_aug/utils/demo.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug/utils/distribution.py` & `keras-aug-0.5.5/keras_aug/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/keras_aug.egg-info/PKG-INFO` & `keras-aug-0.5.5/keras_aug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `keras-aug-0.5.4/keras_aug.egg-info/SOURCES.txt` & `keras-aug-0.5.5/keras_aug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.4/pyproject.toml` & `keras-aug-0.5.5/pyproject.toml`

 * *Files identical despite different names*

