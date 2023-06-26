# Comparing `tmp/fastmri-0.2.0.tar.gz` & `tmp/fastmri-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmri-0.2.0.tar", last modified: Fri Jun 17 20:04:20 2022, max compression
+gzip compressed data, was "fastmri-0.3.0.tar", last modified: Mon Jun 26 17:17:58 2023, max compression
```

## Comparing `fastmri-0.2.0.tar` & `fastmri-0.3.0.tar`

### file list

```diff
@@ -1,175 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.250835 fastmri-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-17 20:04:08.000000 fastmri-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.234835 fastmri-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.238835 fastmri-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/ISSUE_TEMPLATE/Bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/ISSUE_TEMPLATE/Feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/ISSUE_TEMPLATE/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.238835 fastmri-0.2.0/.github/old_discussion_posts/
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/old_discussion_posts/2020_challenge_launch.md
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/old_discussion_posts/fastmri_test_set.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.238835 fastmri-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-06-17 20:04:08.000000 fastmri-0.2.0/.github/workflows/publish-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-06-17 20:04:08.000000 fastmri-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-17 20:04:08.000000 fastmri-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-06-17 20:04:08.000000 fastmri-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-06-17 20:04:08.000000 fastmri-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)    26582 2022-06-17 20:04:08.000000 fastmri-0.2.0/LIST_OF_PAPERS.md
--rw-r--r--   0 runner    (1001) docker     (121)    13956 2022-06-17 20:04:20.250835 fastmri-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12965 2022-06-17 20:04:08.000000 fastmri-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.238835 fastmri-0.2.0/banding_removal/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.238835 fastmri-0.2.0/banding_removal/fastmri/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26231 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/args.py
--rw-r--r--   0 runner    (1001) docker     (121)     9492 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/base_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7412 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/checkpointing_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/common/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/image_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    12515 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/subsample.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/common/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/test/test_subsample.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/data/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10330 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/data/mri_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/data/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    20503 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/data/volume_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     9136 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/distributed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/learning_rate_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/logging_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/model/
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_prev.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_wide.py
--rw-r--r--   0 runner    (1001) docker     (121)     7677 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/torchvision_resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     7687 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/classifiers/unpooled_resnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/public_unet.py
--rw-r--r--   0 runner    (1001) docker     (121)    12507 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/model/var_net.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/optimizer/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/orientation_adversary/
--rw-r--r--   0 runner    (1001) docker     (121)    10890 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/orientation_adversary/adversary_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/orientation_adversary/test_adversary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/parameter_group_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/spawn_dist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/ssim_loss_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13166 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/training_loop_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/transform_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/transforms/kspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/transforms/orientation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/fastmri/var_net/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/var_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/var_net/var_net_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/fastmri/visualization_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/banding_removal/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/scripts/pretrain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/scripts/pretrain_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-06-17 20:04:08.000000 fastmri-0.2.0/banding_removal/scripts/train_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastMRI_tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/fastmri/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-17 20:04:19.000000 fastmri-0.2.0/fastmri/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/coil_combine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri/data/
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21895 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/mri_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    18509 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/subsample.py
--rw-r--r--   0 runner    (1001) docker     (121)    22493 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/data/volume_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/fftc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri/models/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23346 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/models/adaptive_varnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    17693 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/models/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (121)    10632 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/models/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri/pl_modules/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/pl_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16742 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/pl_modules/data_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     9497 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/pl_modules/mri_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/pl_modules/unet_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     7188 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/pl_modules/varnet_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.242835 fastmri-0.2.0/fastmri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13956 2022-06-17 20:04:19.000000 fastmri-0.2.0/fastmri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5420 2022-06-17 20:04:20.000000 fastmri-0.2.0/fastmri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 20:04:19.000000 fastmri-0.2.0/fastmri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-06-17 20:04:19.000000 fastmri-0.2.0/fastmri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-17 20:04:20.000000 fastmri-0.2.0/fastmri.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/adaptive_varnet/
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    11091 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/eval_pretrained_adaptive_varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24684 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/adaptive_varnet_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    24425 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/varnet_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/subsample.py
--rw-r--r--   0 runner    (1001) docker     (121)    25692 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/train_adaptive_varnet_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/adaptive_varnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/annotation/
--rw-r--r--   0 runner    (1001) docker     (121)   685937 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/annotation/fastmri_plus_viz.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/cs/
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/cs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/cs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/cs/cs_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/cs/run_bart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/unet/
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/run_pretrained_unet_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/train_unet_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.246835 fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_brain_leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_mc_leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_sc_leaderboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.250835 fastmri-0.2.0/fastmri_examples/varnet/
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/run_pretrained_varnet_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/train_varnet_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.250835 fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_brain_leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_knee_leaderboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.250835 fastmri-0.2.0/fastmri_examples/zero_filled/
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/zero_filled/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/zero_filled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-06-17 20:04:08.000000 fastmri-0.2.0/fastmri_examples/zero_filled/run_zero_filled.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-17 20:04:08.000000 fastmri-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-06-17 20:04:20.250835 fastmri-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-17 20:04:08.000000 fastmri-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:04:20.250835 fastmri-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/create_temp_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-06-17 20:04:08.000000 fastmri-0.2.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.544846 fastmri-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 17:17:44.000000 fastmri-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.512845 fastmri-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.516845 fastmri-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/ISSUE_TEMPLATE/Bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/ISSUE_TEMPLATE/Feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.516845 fastmri-0.3.0/.github/old_discussion_posts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/old_discussion_posts/2020_challenge_launch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/old_discussion_posts/fastmri_test_set.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.516845 fastmri-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-26 17:17:44.000000 fastmri-0.3.0/.github/workflows/publish-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-26 17:17:44.000000 fastmri-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-26 17:17:44.000000 fastmri-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-26 17:17:44.000000 fastmri-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 17:17:44.000000 fastmri-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-06-26 17:17:44.000000 fastmri-0.3.0/LIST_OF_PAPERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-06-26 17:17:58.544846 fastmri-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-06-26 17:17:44.000000 fastmri-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.520846 fastmri-0.3.0/banding_removal/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.520846 fastmri-0.3.0/banding_removal/fastmri/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/base_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/checkpointing_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.520846 fastmri-0.3.0/banding_removal/fastmri/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/image_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/subsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.520846 fastmri-0.3.0/banding_removal/fastmri/common/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/test/test_subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/data/mri_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/data/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/data/volume_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/distributed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/learning_rate_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/logging_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_prev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_wide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/torchvision_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/classifiers/unpooled_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/public_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/model/var_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/orientation_adversary/
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/orientation_adversary/adversary_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/orientation_adversary/test_adversary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/parameter_group_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/spawn_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/ssim_loss_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/training_loop_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/transform_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/transforms/kspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/transforms/orientation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/fastmri/var_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/var_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/var_net/var_net_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/fastmri/visualization_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.524845 fastmri-0.3.0/banding_removal/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/scripts/pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/scripts/pretrain_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-26 17:17:44.000000 fastmri-0.3.0/banding_removal/scripts/train_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastMRI_tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.528846 fastmri-0.3.0/fastmri/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/coil_combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.528846 fastmri-0.3.0/fastmri/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23526 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/mri_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22497 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/data/volume_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/fftc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.528846 fastmri-0.3.0/fastmri/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/models/adaptive_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/models/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/models/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.528846 fastmri-0.3.0/fastmri/pl_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/pl_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17578 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/pl_modules/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/pl_modules/mri_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/pl_modules/unet_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/pl_modules/varnet_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.528846 fastmri-0.3.0/fastmri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 17:17:58.000000 fastmri-0.3.0/fastmri.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/RadiologyJohnson2022/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/RadiologyJohnson2022/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/RadiologyJohnson2022/RunInference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/adaptive_varnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/eval_pretrained_adaptive_varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24684 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/adaptive_varnet_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/varnet_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25692 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/train_adaptive_varnet_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/adaptive_varnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)   685937 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/annotation/fastmri_plus_viz.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.532846 fastmri-0.3.0/fastmri_examples/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/cs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/cs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/cs/cs_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/cs/run_bart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.536846 fastmri-0.3.0/fastmri_examples/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/run_pretrained_unet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/train_unet_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.536846 fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_brain_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_mc_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_sc_leaderboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.536846 fastmri-0.3.0/fastmri_examples/varnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/run_pretrained_varnet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/train_varnet_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.536846 fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_brain_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_knee_leaderboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.536846 fastmri-0.3.0/fastmri_examples/zero_filled/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/zero_filled/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/zero_filled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_examples/zero_filled/run_zero_filled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.516845 fastmri-0.3.0/fastmri_raw_data_manifest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.544846 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_batch_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_batch_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_batch_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_full_batch_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_full_batch_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_test_full_batch_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14442 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14355 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_train_batch_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_val_batch_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_val_batch_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/brain_multicoil_val_batch_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_train_batch_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_train_batch_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_train_batch_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_train_batch_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_train_batch_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_multicoil_val.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_singlecoil_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_singlecoil_train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-26 17:17:44.000000 fastmri-0.3.0/fastmri_raw_data_manifest/v2.0/knee_singlecoil_val.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 17:17:44.000000 fastmri-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-26 17:17:58.548846 fastmri-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 17:17:44.000000 fastmri-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:17:58.544846 fastmri-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/create_temp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-26 17:17:44.000000 fastmri-0.3.0/tests/test_transforms.py
```

### Comparing `fastmri-0.2.0/.github/old_discussion_posts/2020_challenge_launch.md` & `fastmri-0.3.0/.github/old_discussion_posts/2020_challenge_launch.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/.github/old_discussion_posts/fastmri_test_set.md` & `fastmri-0.3.0/.github/old_discussion_posts/fastmri_test_set.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/.github/workflows/build-and-test.yml` & `fastmri-0.3.0/.github/workflows/build-and-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   build:
     name: Build
     strategy:
       max-parallel: 4
       matrix:
         platform: [ubuntu-latest]
-        python-version: [3.8]
+        python-version: ["3.8", "3.10"]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
@@ -37,15 +37,15 @@
 
   lint-and-test:
     name: Lint and Test
     strategy:
       max-parallel: 4
       matrix:
         platform: [ubuntu-latest]
-        python-version: [3.8]
+        python-version: ["3.8", "3.10"]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
```

### Comparing `fastmri-0.2.0/.github/workflows/publish-package.yml` & `fastmri-0.3.0/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/CONTRIBUTING.md` & `fastmri-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/LICENSE.md` & `fastmri-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/LIST_OF_PAPERS.md` & `fastmri-0.3.0/LIST_OF_PAPERS.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 5. Knoll, F.\*, Murrell, T.\*, Sriram, A.\*, Yakubova, N., Zbontar, J., Rabbat, M., ... & Recht, M. P. (2020). [Advancing machine learning for MR image reconstruction with an open competition: Overview of the 2019 fastMRI challenge](#advancing-machine-learning-for-mr-image-reconstruction-with-an-open-competition-overview-of-the-2019-fastmri-challenge). *Magnetic Resonance in Medicine*, 84(6), pages 3054-3070.
 6. Sriram, A., Zbontar, J., Murrell, T., Zitnick, C. L., Defazio, A., & Sodickson, D. K. (2020). [GrappaNet: Combining parallel imaging with deep learning for multi-coil MRI reconstruction](#grappanet-combining-parallel-imaging-with-deep-learning-for-multi-coil-mri-reconstruction). In *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition*, pages 14315-14322.
 7. Recht, M. P., Zbontar, J., Sodickson, D. K., Knoll, F., Yakubova, N., Sriram, A., ... & Zitnick, C. L. (2020). [Using Deep Learning to Accelerate Knee MRI at 3T: Results of an Interchangeability Study](#using-deep-learning-to-accelerate-knee-mri-at-3t-results-of-an-interchangeability-study). *American Journal of Roentgenology*, 215(6), pages 1421-1429.
 8. Pineda, L., Basu, S., Romero, A., Calandra, R., & Drozdzal, M. (2020). [Active MR k-space Sampling with Reinforcement Learning](#active-mr-k-space-sampling-with-reinforcement-learning). In *International Conference on Medical Image Computing and Computer-Assisted Intervention*, pages 23-33.
 9. Sriram, A.\*, Zbontar, J.\*, Murrell, T., Defazio, A., Zitnick, C. L., Yakubova, N., ... & Johnson, P. (2020). [End-to-End Variational Networks for Accelerated MRI Reconstruction](#end-to-end-variational-networks-for-accelerated-mri-reconstruction). In *International Conference on Medical Image Computing and Computer-Assisted Intervention*, pages 64-73.
 10. Defazio, A., Murrell, T., & Recht, M. P. (2020). [MRI Banding Removal via Adversarial Training](#mri-banding-removal-via-adversarial-training). In *Advances in Neural Information Processing Systems*, 33, pages 7660-7670.
 11. Muckley, M. J.\*, Riemenschneider, B.\*, Radmanesh, A., Kim, S., Jeong, G., Ko, J., ... & Knoll, F. (2021). [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction](#results-of-the-2020-fastmri-challenge-for-machine-learning-mr-image-reconstruction). *IEEE Transactions on Medical Imaging*, 40(9), pages 2306-2317.
-12. Johnson, P. M., Jeong, G., Hammernik, K., Schlemper, J., Qin, C., Duan, J., ..., & Knoll, F. [Evaluation of the Robustness of Learned MR Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the fastMRI Challenge](#evaluation-of-the-robustness-of-learned-mr-image-reconstruction-to-systematic-deviations-between-training-and-test-data-for-the-models-from-the-fastmri-challenge). In *MICCAI Machine Learning for Medical Image Reconstruction Workshop*, pages 25–34, 2021.
-13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://arxiv.org/abs/2203.16392). *Accepted at MIDL, 2022*, to appear.
+12. Johnson, P. M., Jeong, G., Hammernik, K., Schlemper, J., Qin, C., Duan, J., ..., & Knoll, F. (2021). [Evaluation of the Robustness of Learned MR Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the fastMRI Challenge](#evaluation-of-the-robustness-of-learned-mr-image-reconstruction-to-systematic-deviations-between-training-and-test-data-for-the-models-from-the-fastmri-challenge). In *MICCAI Machine Learning for Medical Image Reconstruction Workshop*, pages 25–34.
+13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](#on-learning-adaptive-acquisition-policies-for-undersampled-multi-coil-mri-reconstruction). In * *International Conference on Medical Imaging with Deep Learning*, pages 63-85.
+14. Radmanesh, A.\*, Muckley, M. J.\*, Murrell, T., Lindsey, E., Sriram, A., Knoll, F., ... & Lui, Y. W. (2022). [Exploring the Acceleration Limits of Deep Learning VarNet-based Two-dimensional Brain MRI](#exploring-the-acceleration-limits-of-deep-learning-varnet-based-two-dimensional-brain-mri). *Radiology: Artificial Intelligence*, 4(6), page e210313.
+15. Johnson, Patricia M., Lin, D. J., Zbontar, J., Zitnick, C. L., Sriram, A., Mucklye, M., ..., & Knoll, F. (2023). [Deep learning reconstruction enables prospectively accelerated clinical knee MRI](#deep-learning-reconstruction-enables-prospectively-accelerated-clinical-knee-mri) *Radiology*, page 220425.
 
 ## fastMRI: An open dataset and benchmarks for accelerated MRI
 
 [arXiv](https://arxiv.org/abs/1811.08839) [Code](https://github.com/facebookresearch/fastMRI) [Website](https://fastmri.org)
 
 Accelerating Magnetic Resonance Imaging (MRI) by taking fewer measurements has the potential to reduce medical costs, minimize stress to patients and make MRI possible in applications where it is currently prohibitively slow or expensive. We introduce the fastMRI dataset, a large-scale collection of both raw MR measurements and clinical MR images, that can be used for training and evaluation of machine-learning approaches to MR image reconstruction. By introducing standardized evaluation criteria and a freely-accessible dataset, our goal is to help the community make rapid advances in the state of the art for MR image reconstruction. We also provide a self-contained introduction to MRI for machine learning researchers with no medical imaging background.
 
@@ -263,23 +265,93 @@
     title={Evaluation of the Robustness of Learned {MR} Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the {fastMRI} Challenge},
     booktitle={International Workshop on Machine Learning for Medical Image Reconstruction},
     year={2021},
     pages={25--34},
 }
 ```
 
-
 ## On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction
 
-[publication](https://arxiv.org/abs/2203.16392)
+[publication](https://proceedings.mlr.press/v172/bakker22a)
 
 Most current approaches to undersampled multi-coil MRI reconstruction focus on learning the reconstruction model for a fixed, equidistant acquisition trajectory. In this paper, we study the problem of joint learning of the reconstruction model together with acquisition policies. To this end, we extend the End-to-End Variational Network with learnable acquisition policies that can adapt to different data points. We validate our model on a coil-compressed version of the large scale undersampled multi-coil fastMRI dataset using two undersampling factors: 4× and 8×. Our experiments show on-par performance with the learnable non-adaptive and handcrafted equidistant strategies at 4×, and an observed improvement of more than 2% in SSIM at 8× acceleration, suggesting that potentially-adaptive k-space acquisition trajectories can improve reconstructed image quality for larger acceleration factors. However, and perhaps surprisingly, our best performing policies learn to be explicitly non-adaptive.
 
 ```BibTeX
-@article{bakker2022adaptive,
+@inproceedings{bakker2022adaptive,
     title={On learning adaptive acquisition policies for undersampled multi-coil {MRI} reconstruction},
     author={Tim Bakker and Matthew Muckley and Adriana Romero-Soriano and Michal Drozdzal and Luis Pineda},
-    journal={Proceedings of Machine Learning Research (MIDL)},
-    pages={to appear},
+    booktitle={Proceedings of Machine Learning Research (MIDL)},
     year={2022},
 }
-```
+```
+
+## Exploring the Acceleration Limits of Deep Learning VarNet-based Two-dimensional Brain MRI
+
+[publication](https://doi.org/10.1148/ryai.210313)
+
+**Purpose**
+
+To explore the limits of deep learning-based brain MRI reconstruction and identify useful acceleration ranges for general-purpose imaging and potential screening.
+
+**Materials and Methods**
+
+In this retrospective study conducted from 2019 through 2021, a model was trained for reconstruction on 5,847 brain MRIs. Performance was evaluated across a wide range of accelerations (up to 100-fold along a single phase-encoded direction for two-dimensional [2D] slices) on the fastMRI test set collected by New York University, consisting of 558 image volumes. In a sample of 69 volumes, reconstructions were classified by radiologists for identifying two clinical thresholds: 1) general-purpose diagnostic imaging and 2) potential use in a screening protocol. A Monte Carlo procedure was developed for estimating reconstruction error with only undersampled data. The model was evaluated on both in-domain and out-of-domain data. Confidence intervals were calculated using the percentile bootstrap method.
+
+**Results**
+
+Radiologists rated 100% of 69 volumes as having sufficient image quality for general-purpose imaging at up to 4× acceleration and 65 of 69 (94%) of volumes as having sufficient image quality for screening at up to 14× acceleration. The Monte Carlo procedure estimated ground truth peak signal-to-noise ratio and mean squared error with coefficients of determination greater than 0.5 at all accelerations. Out-of-distribution experiments demonstrated the model’s ability to produce images substantially distinct from the training set, even at 100× acceleration.
+
+**Conclusion**
+
+For 2D brain images using deep learning-based reconstruction, maximum acceleration for potential screening was 3–4 times higher than that for diagnostic general-purpose imaging.
+
+```BibTeX
+@article{radmanesh2022exploring,
+  title={Exploring the Acceleration Limits of Deep Learning {VarNet}-based Two-dimensional Brain {MRI}},
+  author={Radmanesh, Alireza and Muckley, Matthew J and Murrell, Tullie and Lindsey, Emma and Sriram, Anuroop and Knoll, Florian and Sodickson, Daniel K and Lui, Yvonne W},
+  journal={Radiology: Artificial Intelligence},
+  volume={4},
+  number={6},
+  pages={e210313},
+  year={2022},
+  publisher={Radiological Society of North America}
+}
+```
+
+## Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI
+
+[publication](https://doi.org/10.1148/radiol.220425) [Code](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/RadiologyJohnson2022)
+
+**Abstract**
+
+Compared with conventional reconstruction, deep learning reconstruction of prospectively accelerated knee MRI enabled an almost twofold scan time reduction, improved image quality, and had equivalent diagnostic utility.
+
+**Background**
+
+MRI is a powerful diagnostic tool with a long acquisition time. Recently, deep learning (DL) methods have provided accelerated high-quality image reconstructions from undersampled data, but it is unclear if DL image reconstruction can be reliably translated to everyday clinical practice.
+
+**Purpose**
+
+To determine the diagnostic equivalence of prospectively accelerated DL-reconstructed knee MRI compared with conventional accelerated MRI for evaluating internal derangement of the knee in a clinical setting.
+
+**Materials and Methods**
+
+A DL reconstruction model was trained with images from 298 clinical 3-T knee examinations. In a prospective analysis, patients clinically referred for knee MRI underwent a conventional accelerated knee MRI protocol at 3 T followed by an accelerated DL protocol between January 2020 and February 2021. The equivalence of the DL reconstruction of the images relative to the conventional images for the detection of an abnormality was assessed in terms of interchangeability. Each examination was reviewed by six musculoskeletal radiologists. Analyses pertaining to the detection of meniscal or ligament tears and bone marrow or cartilage abnormalities were based on four-point ordinal scores for the likelihood of an abnormality. Additionally, the protocols were compared with use of four-point ordinal scores for each aspect of image quality: overall image quality, presence of artifacts, sharpness, and signal-to-noise ratio.
+
+**Results**
+
+A total of 170 participants (mean age ± SD, 45 years ± 16; 76 men) were evaluated. The DL-reconstructed images were determined to be of diagnostic equivalence with the conventional images for detection of abnormalities. The overall image quality score, averaged over six readers, was significantly better (P < .001) for the DL than for the conventional images.
+
+**Conclusion**
+
+In a clinical setting, deep learning reconstruction enabled a nearly twofold reduction in scan time for a knee MRI and was diagnostically equivalent with the conventional protocol.
+
+```BibTeX
+@article{johnson2023deep,
+    title={Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI},
+    author={Johnson, Patricia M. and Lin, Dana J. and Zbontar, Jure and Zitnick, C. Lawrence and Sriram, Anuroop and Muckley, Matthew and Babb, James S. and Kline, Mitchell and Ciavarra, Gina and Alaia, Erin and Samim, Mohammad and Walter, William R. and Calderon, Liz and Pock, Thomas and Sodickson, Daniel K. and Recht, Michael P. and Knoll, Florian},
+    journal = {Radiology},
+    pages = {220425},
+    year = {2023},
+    doi = {10.1148/radiol.220425},
+}
+```
```

### Comparing `fastmri-0.2.0/PKG-INFO` & `fastmri-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,13 @@
-Metadata-Version: 2.1
-Name: fastmri
-Version: 0.2.0
-Summary: A large-scale dataset of both raw MRI measurements and clinical MRI images.
-Author: Meta/NYU fastMRI Team
-Author-email: fastmri@fb.com
-License: MIT
-Project-URL: Homepage, https://fastmri.org/
-Project-URL: Source, https://github.com/facebookresearch/fastMRI
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-License-File: LICENSE.md
-
 # fastMRI
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/fastMRI/blob/master/LICENSE.md)
 [![Build and Test](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml)
 
-[Website and Leaderboards](https://fastMRI.org) |
+[Website](https://fastMRI.org) |
 [Dataset](https://fastmri.med.nyu.edu/) |
 [GitHub](https://github.com/facebookresearch/fastMRI) |
 [Publications](#list-of-papers)
 
 Accelerating Magnetic Resonance Imaging (MRI) by acquiring fewer measurements
 has the potential to reduce medical costs, minimize stress to patients and make
 MR imaging possible in applications where it is currently prohibitively slow or
@@ -52,22 +27,25 @@
 publications of the fastMRI project.
 
 ## Documentation
 
 ### The fastMRI Dataset
 
 There are multiple publications describing different subcomponents of the data
-(e.g., brain vs. knee) and associated baselines.
+(e.g., brain vs. knee) and associated baselines. All of the fastMRI data can be
+downloaded from the [fastMRI dataset page](https://fastmri.med.nyu.edu/).
 
 * **Project Summary, Datasets, Baselines:** [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI ({J. Zbontar*, F. Knoll*, A. Sriram*} et al., 2018)](https://arxiv.org/abs/1811.08839)
 
 * **Knee Data:** [fastMRI: A Publicly Available Raw k-Space and DICOM Dataset of Knee Images for Accelerated MR Image Reconstruction Using Machine Learning ({F. Knoll*, J. Zbontar*} et al., 2020)](https://doi.org/10.1148/ryai.2020190007)
 
 * **Brain Dataset Properties:** [Supplemental Material](https://ieeexplore.ieee.org/ielx7/42/9526230/9420272/supp1-3075856.pdf?arnumber=9420272) of [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction ({M. Muckley*, B. Riemenschneider*} et al., 2021)](https://doi.org/10.1109/TMI.2021.3075856)
 
+* **Prostate Data:** [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://arxiv.org/abs/2304.09254)
+
 ### Code Repository
 
 For code documentation, most functions and classes have accompanying docstrings
 that you can access via the `help` function in IPython. For example:
 
 ```python
 from fastmri.data import SliceDataset
@@ -139,20 +117,24 @@
   * [U-Net: Convolutional networks for biomedical image segmentation (O. Ronneberger et al., 2015)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/)
 
 * **Sampling, Reconstruction and Artifact Correction**
 
   * [Offset Sampling Improves Deep Learning based Accelerated MRI Reconstructions by Exploiting Symmetry (A. Defazio, 2019)](https://github.com/facebookresearch/fastMRI/blob/8abe6eaeeb3d4504f26dc77adffb02a4be41d6f4/fastmri/data/subsample.py#L344-L475)
   * [End-to-End Variational Networks for Accelerated MRI Reconstruction ({A. Sriram*, J. Zbontar*} et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/varnet/)
   * [MRI Banding Removal via Adversarial Training (A. Defazio, et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/banding_removal)
+  * [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI (P. Johnson et al., 2023)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/RadiologyJohnson2022)
 
 * **Active Acquisition**
   * (external repository) [Reducing uncertainty in undersampled MRI reconstruction with active acquisition (Z. Zhang et al., 2019)](https://github.com/facebookresearch/active-mri-acquisition/tree/master/activemri/experimental/cvpr19_models)
   * (external repository) [Active MR k-space Sampling with Reinforcement Learning (L. Pineda et al., 2020)](https://github.com/facebookresearch/active-mri-acquisition)
   * [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction (T. Bakker et al., 2022)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/adaptive_varnet/)
 
+* **Prostate Data**
+  * (external respository) [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://github.com/cai2r/fastMRI_prostate)
+
 ## Testing
 
 Run `pytest tests`. By default integration tests that use the fastMRI data are
 skipped. If you would like to run these tests, set `SKIP_INTEGRATIONS` to
 `False` in the [conftest](https://github.com/facebookresearch/fastMRI/tree/master/tests/conftest.py).
 
 ## Training a model
@@ -164,43 +146,54 @@
 
 Please look at
 [this U-Net demo script](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/train_unet_demo.py) for an
 example of how to train a model using the PyTorch Lightning framework.
 
 ## Submitting to the Leaderboard
 
-Run your model on the provided test data and create a zip file containing your
-predictions. `fastmri` has a `save_reconstructions` function that saves the
-data in the correct format.
-
-Upload the zip file to any publicly accessible cloud storage (e.g. Amazon S3,
-Dropbox etc). Submit a link to the zip file on the
-[challenge website](https://fastmri.org/submit). You will need to create an
-account before submitting.
+**NOTICE:** As documented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293),
+the fastmri.org domain was transferred from Meta ownership to NYU ownership on
+2023-04-17, and NYU has not yet rebuilt the site. Until the site and
+leaderbaords are rebuilt by NYU, leaderboards will be unavailable. Mitigations
+are presented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293).
 
 ## License
 
 fastMRI is MIT licensed, as found in the [LICENSE file](https://github.com/facebookresearch/fastMRI/tree/master/LICENSE.md).
 
 ## Cite
 
 If you use the fastMRI data or code in your project, please cite the arXiv
 paper:
 
 ```BibTeX
-@inproceedings{zbontar2018fastMRI,
+@misc{zbontar2018fastMRI,
     title={{fastMRI}: An Open Dataset and Benchmarks for Accelerated {MRI}},
     author={Jure Zbontar and Florian Knoll and Anuroop Sriram and Tullie Murrell and Zhengnan Huang and Matthew J. Muckley and Aaron Defazio and Ruben Stern and Patricia Johnson and Mary Bruno and Marc Parente and Krzysztof J. Geras and Joe Katsnelson and Hersh Chandarana and Zizhao Zhang and Michal Drozdzal and Adriana Romero and Michael Rabbat and Pascal Vincent and Nafissa Yakubova and James Pinkerton and Duo Wang and Erich Owens and C. Lawrence Zitnick and Michael P. Recht and Daniel K. Sodickson and Yvonne W. Lui},
     journal = {ArXiv e-prints},
     archivePrefix = "arXiv",
     eprint = {1811.08839},
     year={2018}
 }
 ```
 
+If you use the fastMRI prostate data or code in your project, please cite that
+paper:
+
+```BibTeX
+@misc{tibrewala2023fastmri,
+  title={{FastMRI Prostate}: A Publicly Available, Biparametric {MRI} Dataset to Advance Machine Learning for Prostate Cancer Imaging},
+  author={Tibrewala, Radhika and Dutt, Tarun and Tong, Angela and Ginocchio, Luke and Keerthivasan, Mahesh B and Baete, Steven H and Chopra, Sumit and Lui, Yvonne W and Sodickson, Daniel K and Chandarana, Hersh and Johnson, Patricia M},
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint={2304.09254},
+  year={2023}
+}
+```
+
 ## List of Papers
 
 The following lists titles of papers from the fastMRI project. The
 corresponding abstracts, as well as links to preprints and code can be found
 [here](https://github.com/facebookresearch/fastMRI/tree/master/LIST_OF_PAPERS.md).
 
 1. Zbontar, J.\*, Knoll, F.\*, Sriram, A.\*, Murrell, T., Huang, Z., Muckley, M. J., ... & Lui, Y. W. (2018). [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI](https://arxiv.org/abs/1811.08839). *arXiv preprint arXiv:1811.08839*.
@@ -211,8 +204,11 @@
 6. Sriram, A., Zbontar, J., Murrell, T., Zitnick, C. L., Defazio, A., & Sodickson, D. K. (2020). [GrappaNet: Combining parallel imaging with deep learning for multi-coil MRI reconstruction](https://openaccess.thecvf.com/content_CVPR_2020/html/Sriram_GrappaNet_Combining_Parallel_Imaging_With_Deep_Learning_for_Multi-Coil_MRI_CVPR_2020_paper.html). In *CVPR*, pages 14315-14322.
 7. Recht, M. P., Zbontar, J., Sodickson, D. K., Knoll, F., Yakubova, N., Sriram, A., ... & Zitnick, C. L. (2020). [Using Deep Learning to Accelerate Knee MRI at 3T: Results of an Interchangeability Study](https://doi.org/10.2214/AJR.20.23313). *American Journal of Roentgenology*, 215(6), pages 1421-1429.
 8. Pineda, L., Basu, S., Romero, A., Calandra, R., & Drozdzal, M. (2020). [Active MR k-space Sampling with Reinforcement Learning](https://doi.org/10.1007/978-3-030-59713-9_3). In *MICCAI*, pages 23-33.
 9. Sriram, A.\*, Zbontar, J.\*, Murrell, T., Defazio, A., Zitnick, C. L., Yakubova, N., ... & Johnson, P. (2020). [End-to-End Variational Networks for Accelerated MRI Reconstruction](https://doi.org/10.1007/978-3-030-59713-9_7). In *MICCAI*, pages 64-73.
 10. Defazio, A., Murrell, T., & Recht, M. P. (2020). [MRI Banding Removal via Adversarial Training](https://papers.nips.cc/paper/2020/hash/567b8f5f423af15818a068235807edc0-Abstract.html). In *Advances in Neural Information Processing Systems*, 33, pages 7660-7670.
 11. Muckley, M. J.\*, Riemenschneider, B.\*, Radmanesh, A., Kim, S., Jeong, G., Ko, J., ... & Knoll, F. (2021). [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction](https://doi.org/10.1109/TMI.2021.3075856). *IEEE Transactions on Medical Imaging*, 40(9), pages 2306-2317.
 12. Johnson, P. M., Jeong, G., Hammernik, K., Schlemper, J., Qin, C., Duan, J., ..., & Knoll, F. (2021). [Evaluation of the Robustness of Learned MR Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the fastMRI Challenge](https://doi.org/10.1007/978-3-030-88552-6_3). In *MICCAI MLMIR Workshop*, pages 25–34,
-13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://arxiv.org/abs/2203.16392). *In MIDL*. Accepted.
+13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://proceedings.mlr.press/v172/bakker22a). In *MIDL*, pages 63-85.
+14. Radmanesh, A.\*, Muckley, M. J.\*, Murrell, T., Lindsey, E., Sriram, A., Knoll, F., ... & Lui, Y. W. (2022). [Exploring the Acceleration Limits of Deep Learning VarNet-based Two-dimensional Brain MRI](https://doi.org/10.1148/ryai.210313). *Radiology: Artificial Intelligence*, 4(6), page e210313.
+15. Johnson, P.M., Lin, D.J., Zbontar, J., Zitnick, C.L., Sriram, A., Muckley, M., Babb, J.S., Kline, M., Ciavarra, G., Alaia, E., ..., & Knoll, F. (2023). [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI](https://doi.org/10.1148/radiol.220425). *Radiology*, 307(2), page e220425.
+16. Tibrewala, R., Dutt, T., Tong, A., Ginocchio, L., Keerthivasan, M.B., Baete, S.H., Lui, Y.W., Sodickson, D.K., Chandarana, H., Johnson, P.M. (2023). [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging](https://arxiv.org/abs/2304.09254). *arXiv preprint, arXiv:2034.09254*.
```

### Comparing `fastmri-0.2.0/README.md` & `fastmri-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,38 @@
+Metadata-Version: 2.1
+Name: fastmri
+Version: 0.3.0
+Summary: A large-scale dataset of both raw MRI measurements and clinical MRI images.
+Author: Meta/NYU fastMRI Team
+Author-email: fastmri@fb.com
+License: MIT
+Project-URL: Homepage, https://fastmri.org/
+Project-URL: Source, https://github.com/facebookresearch/fastMRI
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
+License-File: LICENSE.md
+
 # fastMRI
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/fastMRI/blob/master/LICENSE.md)
 [![Build and Test](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml)
 
-[Website and Leaderboards](https://fastMRI.org) |
+[Website](https://fastMRI.org) |
 [Dataset](https://fastmri.med.nyu.edu/) |
 [GitHub](https://github.com/facebookresearch/fastMRI) |
 [Publications](#list-of-papers)
 
 Accelerating Magnetic Resonance Imaging (MRI) by acquiring fewer measurements
 has the potential to reduce medical costs, minimize stress to patients and make
 MR imaging possible in applications where it is currently prohibitively slow or
@@ -27,22 +52,25 @@
 publications of the fastMRI project.
 
 ## Documentation
 
 ### The fastMRI Dataset
 
 There are multiple publications describing different subcomponents of the data
-(e.g., brain vs. knee) and associated baselines.
+(e.g., brain vs. knee) and associated baselines. All of the fastMRI data can be
+downloaded from the [fastMRI dataset page](https://fastmri.med.nyu.edu/).
 
 * **Project Summary, Datasets, Baselines:** [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI ({J. Zbontar*, F. Knoll*, A. Sriram*} et al., 2018)](https://arxiv.org/abs/1811.08839)
 
 * **Knee Data:** [fastMRI: A Publicly Available Raw k-Space and DICOM Dataset of Knee Images for Accelerated MR Image Reconstruction Using Machine Learning ({F. Knoll*, J. Zbontar*} et al., 2020)](https://doi.org/10.1148/ryai.2020190007)
 
 * **Brain Dataset Properties:** [Supplemental Material](https://ieeexplore.ieee.org/ielx7/42/9526230/9420272/supp1-3075856.pdf?arnumber=9420272) of [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction ({M. Muckley*, B. Riemenschneider*} et al., 2021)](https://doi.org/10.1109/TMI.2021.3075856)
 
+* **Prostate Data:** [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://arxiv.org/abs/2304.09254)
+
 ### Code Repository
 
 For code documentation, most functions and classes have accompanying docstrings
 that you can access via the `help` function in IPython. For example:
 
 ```python
 from fastmri.data import SliceDataset
@@ -114,20 +142,24 @@
   * [U-Net: Convolutional networks for biomedical image segmentation (O. Ronneberger et al., 2015)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/)
 
 * **Sampling, Reconstruction and Artifact Correction**
 
   * [Offset Sampling Improves Deep Learning based Accelerated MRI Reconstructions by Exploiting Symmetry (A. Defazio, 2019)](https://github.com/facebookresearch/fastMRI/blob/8abe6eaeeb3d4504f26dc77adffb02a4be41d6f4/fastmri/data/subsample.py#L344-L475)
   * [End-to-End Variational Networks for Accelerated MRI Reconstruction ({A. Sriram*, J. Zbontar*} et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/varnet/)
   * [MRI Banding Removal via Adversarial Training (A. Defazio, et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/banding_removal)
+  * [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI (P. Johnson et al., 2023)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/RadiologyJohnson2022)
 
 * **Active Acquisition**
   * (external repository) [Reducing uncertainty in undersampled MRI reconstruction with active acquisition (Z. Zhang et al., 2019)](https://github.com/facebookresearch/active-mri-acquisition/tree/master/activemri/experimental/cvpr19_models)
   * (external repository) [Active MR k-space Sampling with Reinforcement Learning (L. Pineda et al., 2020)](https://github.com/facebookresearch/active-mri-acquisition)
   * [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction (T. Bakker et al., 2022)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/adaptive_varnet/)
 
+* **Prostate Data**
+  * (external respository) [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://github.com/cai2r/fastMRI_prostate)
+
 ## Testing
 
 Run `pytest tests`. By default integration tests that use the fastMRI data are
 skipped. If you would like to run these tests, set `SKIP_INTEGRATIONS` to
 `False` in the [conftest](https://github.com/facebookresearch/fastMRI/tree/master/tests/conftest.py).
 
 ## Training a model
@@ -139,43 +171,54 @@
 
 Please look at
 [this U-Net demo script](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/train_unet_demo.py) for an
 example of how to train a model using the PyTorch Lightning framework.
 
 ## Submitting to the Leaderboard
 
-Run your model on the provided test data and create a zip file containing your
-predictions. `fastmri` has a `save_reconstructions` function that saves the
-data in the correct format.
-
-Upload the zip file to any publicly accessible cloud storage (e.g. Amazon S3,
-Dropbox etc). Submit a link to the zip file on the
-[challenge website](https://fastmri.org/submit). You will need to create an
-account before submitting.
+**NOTICE:** As documented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293),
+the fastmri.org domain was transferred from Meta ownership to NYU ownership on
+2023-04-17, and NYU has not yet rebuilt the site. Until the site and
+leaderbaords are rebuilt by NYU, leaderboards will be unavailable. Mitigations
+are presented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293).
 
 ## License
 
 fastMRI is MIT licensed, as found in the [LICENSE file](https://github.com/facebookresearch/fastMRI/tree/master/LICENSE.md).
 
 ## Cite
 
 If you use the fastMRI data or code in your project, please cite the arXiv
 paper:
 
 ```BibTeX
-@inproceedings{zbontar2018fastMRI,
+@misc{zbontar2018fastMRI,
     title={{fastMRI}: An Open Dataset and Benchmarks for Accelerated {MRI}},
     author={Jure Zbontar and Florian Knoll and Anuroop Sriram and Tullie Murrell and Zhengnan Huang and Matthew J. Muckley and Aaron Defazio and Ruben Stern and Patricia Johnson and Mary Bruno and Marc Parente and Krzysztof J. Geras and Joe Katsnelson and Hersh Chandarana and Zizhao Zhang and Michal Drozdzal and Adriana Romero and Michael Rabbat and Pascal Vincent and Nafissa Yakubova and James Pinkerton and Duo Wang and Erich Owens and C. Lawrence Zitnick and Michael P. Recht and Daniel K. Sodickson and Yvonne W. Lui},
     journal = {ArXiv e-prints},
     archivePrefix = "arXiv",
     eprint = {1811.08839},
     year={2018}
 }
 ```
 
+If you use the fastMRI prostate data or code in your project, please cite that
+paper:
+
+```BibTeX
+@misc{tibrewala2023fastmri,
+  title={{FastMRI Prostate}: A Publicly Available, Biparametric {MRI} Dataset to Advance Machine Learning for Prostate Cancer Imaging},
+  author={Tibrewala, Radhika and Dutt, Tarun and Tong, Angela and Ginocchio, Luke and Keerthivasan, Mahesh B and Baete, Steven H and Chopra, Sumit and Lui, Yvonne W and Sodickson, Daniel K and Chandarana, Hersh and Johnson, Patricia M},
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint={2304.09254},
+  year={2023}
+}
+```
+
 ## List of Papers
 
 The following lists titles of papers from the fastMRI project. The
 corresponding abstracts, as well as links to preprints and code can be found
 [here](https://github.com/facebookresearch/fastMRI/tree/master/LIST_OF_PAPERS.md).
 
 1. Zbontar, J.\*, Knoll, F.\*, Sriram, A.\*, Murrell, T., Huang, Z., Muckley, M. J., ... & Lui, Y. W. (2018). [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI](https://arxiv.org/abs/1811.08839). *arXiv preprint arXiv:1811.08839*.
@@ -186,8 +229,11 @@
 6. Sriram, A., Zbontar, J., Murrell, T., Zitnick, C. L., Defazio, A., & Sodickson, D. K. (2020). [GrappaNet: Combining parallel imaging with deep learning for multi-coil MRI reconstruction](https://openaccess.thecvf.com/content_CVPR_2020/html/Sriram_GrappaNet_Combining_Parallel_Imaging_With_Deep_Learning_for_Multi-Coil_MRI_CVPR_2020_paper.html). In *CVPR*, pages 14315-14322.
 7. Recht, M. P., Zbontar, J., Sodickson, D. K., Knoll, F., Yakubova, N., Sriram, A., ... & Zitnick, C. L. (2020). [Using Deep Learning to Accelerate Knee MRI at 3T: Results of an Interchangeability Study](https://doi.org/10.2214/AJR.20.23313). *American Journal of Roentgenology*, 215(6), pages 1421-1429.
 8. Pineda, L., Basu, S., Romero, A., Calandra, R., & Drozdzal, M. (2020). [Active MR k-space Sampling with Reinforcement Learning](https://doi.org/10.1007/978-3-030-59713-9_3). In *MICCAI*, pages 23-33.
 9. Sriram, A.\*, Zbontar, J.\*, Murrell, T., Defazio, A., Zitnick, C. L., Yakubova, N., ... & Johnson, P. (2020). [End-to-End Variational Networks for Accelerated MRI Reconstruction](https://doi.org/10.1007/978-3-030-59713-9_7). In *MICCAI*, pages 64-73.
 10. Defazio, A., Murrell, T., & Recht, M. P. (2020). [MRI Banding Removal via Adversarial Training](https://papers.nips.cc/paper/2020/hash/567b8f5f423af15818a068235807edc0-Abstract.html). In *Advances in Neural Information Processing Systems*, 33, pages 7660-7670.
 11. Muckley, M. J.\*, Riemenschneider, B.\*, Radmanesh, A., Kim, S., Jeong, G., Ko, J., ... & Knoll, F. (2021). [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction](https://doi.org/10.1109/TMI.2021.3075856). *IEEE Transactions on Medical Imaging*, 40(9), pages 2306-2317.
 12. Johnson, P. M., Jeong, G., Hammernik, K., Schlemper, J., Qin, C., Duan, J., ..., & Knoll, F. (2021). [Evaluation of the Robustness of Learned MR Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the fastMRI Challenge](https://doi.org/10.1007/978-3-030-88552-6_3). In *MICCAI MLMIR Workshop*, pages 25–34,
-13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://arxiv.org/abs/2203.16392). *In MIDL*. Accepted.
+13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://proceedings.mlr.press/v172/bakker22a). In *MIDL*, pages 63-85.
+14. Radmanesh, A.\*, Muckley, M. J.\*, Murrell, T., Lindsey, E., Sriram, A., Knoll, F., ... & Lui, Y. W. (2022). [Exploring the Acceleration Limits of Deep Learning VarNet-based Two-dimensional Brain MRI](https://doi.org/10.1148/ryai.210313). *Radiology: Artificial Intelligence*, 4(6), page e210313.
+15. Johnson, P.M., Lin, D.J., Zbontar, J., Zitnick, C.L., Sriram, A., Muckley, M., Babb, J.S., Kline, M., Ciavarra, G., Alaia, E., ..., & Knoll, F. (2023). [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI](https://doi.org/10.1148/radiol.220425). *Radiology*, 307(2), page e220425.
+16. Tibrewala, R., Dutt, T., Tong, A., Ginocchio, L., Keerthivasan, M.B., Baete, S.H., Lui, Y.W., Sodickson, D.K., Chandarana, H., Johnson, P.M. (2023). [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging](https://arxiv.org/abs/2304.09254). *arXiv preprint, arXiv:2034.09254*.
```

### Comparing `fastmri-0.2.0/banding_removal/README.md` & `fastmri-0.3.0/banding_removal/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/args.py` & `fastmri-0.3.0/banding_removal/fastmri/args.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/base_trainer.py` & `fastmri-0.3.0/banding_removal/fastmri/base_trainer.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/checkpointing_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/checkpointing_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/common/evaluate.py` & `fastmri-0.3.0/banding_removal/fastmri/common/evaluate.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/common/image_grid.py` & `fastmri-0.3.0/banding_removal/fastmri/common/image_grid.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/common/subsample.py` & `fastmri-0.3.0/banding_removal/fastmri/common/subsample.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/common/test/test_subsample.py` & `fastmri-0.3.0/banding_removal/fastmri/common/test/test_subsample.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/common/utils.py` & `fastmri-0.3.0/banding_removal/fastmri/common/utils.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/data/mri_data.py` & `fastmri-0.3.0/banding_removal/fastmri/data/mri_data.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/data/test_transforms.py` & `fastmri-0.3.0/banding_removal/fastmri/data/test_transforms.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/data/transforms.py` & `fastmri-0.3.0/banding_removal/fastmri/data/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -484,39 +484,14 @@
         Returns shape: height x width x 2
     """
     assert data.shape[-3] == 2
     real = data[..., 0, :, :]
     imaginary = data[..., 1, :, :]
     return torch.stack([real, imaginary], dim=-1)
 
-
-def complex_whiten(complex_image, eps=1e-10):
-    real = complex_image[:, :, 0]
-    imag = complex_image[:, :, 1]
-
-    # Center around mean.
-    centered_complex_image = complex_image - complex_image.mean()
-
-    # Determine covariance between real and imaginary.
-    n = real.nelement()
-    real_real = (real.mul(real).sum() - real.mean().mul(real.mean())) / n
-    real_imag = (real.mul(imag).sum() - real.mean().mul(imag.mean())) / n
-    imag_imag = (imag.mul(imag).sum() - imag.mean().mul(imag.mean())) / n
-    V = torch.Tensor([[real_real, real_imag], [real_imag, imag_imag]])
-
-    # Remove correlation by rotating around covariance eigenvectors.
-    eig_values, eig_vecs = torch.eig(V, eigenvectors=True)
-    whitened_image = torch.matmul(centered_complex_image, eig_vecs)
-
-    # Scale by eigenvalues for unit variance.
-    whitened_image[:, :, 0] = whitened_image[:, :, 0] / (eig_values[0, 0] + eps).sqrt()
-    whitened_image[:, :, 1] = whitened_image[:, :, 1] / (eig_values[1, 0] + eps).sqrt()
-    return whitened_image
-
-
 # Helper functions
 
 def roll(x, shift, dim):
     """
     Similar to np.roll but applies to PyTorch Tensors
     """
     if isinstance(shift, (tuple, list)):
```

### Comparing `fastmri-0.2.0/banding_removal/fastmri/data/volume_sampler.py` & `fastmri-0.3.0/banding_removal/fastmri/data/volume_sampler.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/distributed_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/distributed_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/learning_rate_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/learning_rate_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/logging_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/logging_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/__init__.py` & `fastmri-0.3.0/banding_removal/fastmri/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_prev.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_prev.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_simple.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_simple.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/resnet_r1_wide.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/resnet_r1_wide.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/torchvision_resnet.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/torchvision_resnet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/classifiers/unpooled_resnet.py` & `fastmri-0.3.0/banding_removal/fastmri/model/classifiers/unpooled_resnet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/public_unet.py` & `fastmri-0.3.0/banding_removal/fastmri/model/public_unet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/model/var_net.py` & `fastmri-0.3.0/banding_removal/fastmri/model/var_net.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/optimizer/__init__.py` & `fastmri-0.3.0/banding_removal/fastmri/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/orientation_adversary/adversary_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/orientation_adversary/adversary_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/orientation_adversary/test_adversary.py` & `fastmri-0.3.0/banding_removal/fastmri/orientation_adversary/test_adversary.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/parameter_group_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/parameter_group_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/run.py` & `fastmri-0.3.0/banding_removal/fastmri/run.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/spawn_dist.py` & `fastmri-0.3.0/banding_removal/fastmri/spawn_dist.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/ssim_loss_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/ssim_loss_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/trainer.py` & `fastmri-0.3.0/banding_removal/fastmri/trainer.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/training_loop_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/training_loop_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/transform_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/transform_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/transforms/__init__.py` & `fastmri-0.3.0/banding_removal/fastmri/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/transforms/kspace.py` & `fastmri-0.3.0/banding_removal/fastmri/transforms/kspace.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/transforms/orientation.py` & `fastmri-0.3.0/banding_removal/fastmri/transforms/orientation.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/var_net/var_net_trainer.py` & `fastmri-0.3.0/banding_removal/fastmri/var_net/var_net_trainer.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/fastmri/visualization_mixin.py` & `fastmri-0.3.0/banding_removal/fastmri/visualization_mixin.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/scripts/pretrain.py` & `fastmri-0.3.0/banding_removal/scripts/pretrain.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/scripts/pretrain_dev.py` & `fastmri-0.3.0/banding_removal/scripts/pretrain_dev.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/scripts/train.py` & `fastmri-0.3.0/banding_removal/scripts/train.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/banding_removal/scripts/train_dev.py` & `fastmri-0.3.0/banding_removal/scripts/train_dev.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastMRI_tutorial.ipynb` & `fastmri-0.3.0/fastMRI_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/__init__.py` & `fastmri-0.3.0/fastmri/__init__.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/coil_combine.py` & `fastmri-0.3.0/fastmri/coil_combine.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/data/README.md` & `fastmri-0.3.0/fastmri/data/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/data/mri_data.py` & `fastmri-0.3.0/fastmri/data/mri_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,36 @@
 """
 
 import logging
 import os
 import pickle
 import random
 import xml.etree.ElementTree as etree
+from copy import deepcopy
 from pathlib import Path
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 from warnings import warn
 
 import h5py
 import numpy as np
 import pandas as pd
 import requests
 import torch
 import yaml
+from tqdm import tqdm
 
 
 def et_query(
     root: etree.Element,
     qlist: Sequence[str],
     namespace: str = "http://www.ismrm.org/ISMRMRD",
 ) -> str:
@@ -96,14 +108,20 @@
     else:
         with open(data_config_file, "r") as f:
             data_dir = yaml.safe_load(f)[key]
 
     return Path(data_dir)
 
 
+class FastMRIRawDataSample(NamedTuple):
+    fname: Path
+    slice_ind: int
+    metadata: Dict[str, Any]
+
+
 class CombinedSliceDataset(torch.utils.data.Dataset):
     """
     A container for combining slice datasets.
     """
 
     def __init__(
         self,
@@ -111,14 +129,15 @@
         challenges: Sequence[str],
         transforms: Optional[Sequence[Optional[Callable]]] = None,
         sample_rates: Optional[Sequence[Optional[float]]] = None,
         volume_sample_rates: Optional[Sequence[Optional[float]]] = None,
         use_dataset_cache: bool = False,
         dataset_cache_file: Union[str, Path, os.PathLike] = "dataset_cache.pkl",
         num_cols: Optional[Tuple[int]] = None,
+        raw_sample_filter: Optional[Callable] = None,
     ):
         """
         Args:
             roots: Paths to the datasets.
             challenges: "singlecoil" or "multicoil" depending on which
                 challenge to use.
             transforms: Optional; A sequence of callable objects that
@@ -138,14 +157,17 @@
                 but not both.
             use_dataset_cache: Whether to cache dataset metadata. This is very
                 useful for large datasets like the brain data.
             dataset_cache_file: Optional; A file in which to cache dataset
                 information for faster load times.
             num_cols: Optional; If provided, only slices with the desired
                 number of columns will be considered.
+            raw_sample_filter: Optional; A callable object that takes an raw_sample
+                metadata as input and returns a boolean indicating whether the
+                raw_sample should be included in the dataset.
         """
         if sample_rates is not None and volume_sample_rates is not None:
             raise ValueError(
                 "either set sample_rates (sample by slices) or volume_sample_rates (sample by volumes) but not both"
             )
         if transforms is None:
             transforms = [None] * len(roots)
@@ -161,30 +183,31 @@
             == len(volume_sample_rates)
         ):
             raise ValueError(
                 "Lengths of roots, transforms, challenges, sample_rates do not match"
             )
 
         self.datasets = []
-        self.examples: List[Tuple[Path, int, Dict[str, object]]] = []
+        self.raw_samples: List[FastMRIRawDataSample] = []
         for i in range(len(roots)):
             self.datasets.append(
                 SliceDataset(
                     root=roots[i],
                     transform=transforms[i],
                     challenge=challenges[i],
                     sample_rate=sample_rates[i],
                     volume_sample_rate=volume_sample_rates[i],
                     use_dataset_cache=use_dataset_cache,
                     dataset_cache_file=dataset_cache_file,
                     num_cols=num_cols,
+                    raw_sample_filter=raw_sample_filter,
                 )
             )
 
-            self.examples = self.examples + self.datasets[-1].examples
+            self.raw_samples = self.raw_samples + self.datasets[-1].raw_samples
 
     def __len__(self):
         return sum(len(dataset) for dataset in self.datasets)
 
     def __getitem__(self, i):
         for dataset in self.datasets:
             if i < len(dataset):
@@ -204,14 +227,15 @@
         challenge: str,
         transform: Optional[Callable] = None,
         use_dataset_cache: bool = False,
         sample_rate: Optional[float] = None,
         volume_sample_rate: Optional[float] = None,
         dataset_cache_file: Union[str, Path, os.PathLike] = "dataset_cache.pkl",
         num_cols: Optional[Tuple[int]] = None,
+        raw_sample_filter: Optional[Callable] = None,
     ):
         """
         Args:
             root: Path to the dataset.
             challenge: "singlecoil" or "multicoil" depending on which challenge
                 to use.
             transform: Optional; A callable object that pre-processes the raw
@@ -228,14 +252,17 @@
                 of the volumes should be loaded. Defaults to 1 if no value is given.
                 When creating a sampled dataset either set sample_rate (sample by slices)
                 or volume_sample_rate (sample by volumes) but not both.
             dataset_cache_file: Optional; A file in which to cache dataset
                 information for faster load times.
             num_cols: Optional; If provided, only slices with the desired
                 number of columns will be considered.
+            raw_sample_filter: Optional; A callable object that takes an raw_sample
+                metadata as input and returns a boolean indicating whether the
+                raw_sample should be included in the dataset.
         """
         if challenge not in ("singlecoil", "multicoil"):
             raise ValueError('challenge should be either "singlecoil" or "multicoil"')
 
         if sample_rate is not None and volume_sample_rate is not None:
             raise ValueError(
                 "either set sample_rate (sample by slices) or volume_sample_rate (sample by volumes) but not both"
@@ -243,15 +270,19 @@
 
         self.dataset_cache_file = Path(dataset_cache_file)
 
         self.transform = transform
         self.recons_key = (
             "reconstruction_esc" if challenge == "singlecoil" else "reconstruction_rss"
         )
-        self.examples = []
+        self.raw_samples = []
+        if raw_sample_filter is None:
+            self.raw_sample_filter = lambda raw_sample: True
+        else:
+            self.raw_sample_filter = raw_sample_filter
 
         # set default sampling mode if none given
         if sample_rate is None:
             sample_rate = 1.0
         if volume_sample_rate is None:
             volume_sample_rate = 1.0
 
@@ -265,45 +296,51 @@
         # check if our dataset is in the cache
         # if there, use that metadata, if not, then regenerate the metadata
         if dataset_cache.get(root) is None or not use_dataset_cache:
             files = list(Path(root).iterdir())
             for fname in sorted(files):
                 metadata, num_slices = self._retrieve_metadata(fname)
 
-                self.examples += [
-                    (fname, slice_ind, metadata) for slice_ind in range(num_slices)
-                ]
+                new_raw_samples = []
+                for slice_ind in range(num_slices):
+                    raw_sample = FastMRIRawDataSample(fname, slice_ind, metadata)
+                    if self.raw_sample_filter(raw_sample):
+                        new_raw_samples.append(raw_sample)
+
+                self.raw_samples += new_raw_samples
 
             if dataset_cache.get(root) is None and use_dataset_cache:
-                dataset_cache[root] = self.examples
+                dataset_cache[root] = self.raw_samples
                 logging.info(f"Saving dataset cache to {self.dataset_cache_file}.")
                 with open(self.dataset_cache_file, "wb") as cache_f:
                     pickle.dump(dataset_cache, cache_f)
         else:
             logging.info(f"Using dataset cache from {self.dataset_cache_file}.")
-            self.examples = dataset_cache[root]
+            self.raw_samples = dataset_cache[root]
 
         # subsample if desired
         if sample_rate < 1.0:  # sample by slice
-            random.shuffle(self.examples)
-            num_examples = round(len(self.examples) * sample_rate)
-            self.examples = self.examples[:num_examples]
+            random.shuffle(self.raw_samples)
+            num_raw_samples = round(len(self.raw_samples) * sample_rate)
+            self.raw_samples = self.raw_samples[:num_raw_samples]
         elif volume_sample_rate < 1.0:  # sample by volume
-            vol_names = sorted(list(set([f[0].stem for f in self.examples])))
+            vol_names = sorted(list(set([f[0].stem for f in self.raw_samples])))
             random.shuffle(vol_names)
             num_volumes = round(len(vol_names) * volume_sample_rate)
             sampled_vols = vol_names[:num_volumes]
-            self.examples = [
-                example for example in self.examples if example[0].stem in sampled_vols
+            self.raw_samples = [
+                raw_sample
+                for raw_sample in self.raw_samples
+                if raw_sample[0].stem in sampled_vols
             ]
 
         if num_cols:
-            self.examples = [
+            self.raw_samples = [
                 ex
-                for ex in self.examples
+                for ex in self.raw_samples
                 if ex[2]["encoding_size"][1] in num_cols  # type: ignore
             ]
 
     def _retrieve_metadata(self, fname):
         with h5py.File(fname, "r") as hf:
             et_root = etree.fromstring(hf["ismrmrd_header"][()])
 
@@ -325,28 +362,29 @@
             enc_limits_max = int(et_query(et_root, lims + ["maximum"])) + 1
 
             padding_left = enc_size[1] // 2 - enc_limits_center
             padding_right = padding_left + enc_limits_max
 
             num_slices = hf["kspace"].shape[0]
 
-        metadata = {
-            "padding_left": padding_left,
-            "padding_right": padding_right,
-            "encoding_size": enc_size,
-            "recon_size": recon_size,
-        }
+            metadata = {
+                "padding_left": padding_left,
+                "padding_right": padding_right,
+                "encoding_size": enc_size,
+                "recon_size": recon_size,
+                **hf.attrs,
+            }
 
         return metadata, num_slices
 
     def __len__(self):
-        return len(self.examples)
+        return len(self.raw_samples)
 
     def __getitem__(self, i: int):
-        fname, dataslice, metadata = self.examples[i]
+        fname, dataslice, metadata = self.raw_samples[i]
 
         with h5py.File(fname, "r") as hf:
             kspace = hf["kspace"][dataslice]
 
             mask = np.asarray(hf["mask"]) if "mask" in hf else None
 
             target = hf[self.recons_key][dataslice] if self.recons_key in hf else None
@@ -364,15 +402,15 @@
 
 class AnnotatedSliceDataset(SliceDataset):
     """
     A PyTorch Dataset that provides access to MR image slices with annotation.
 
     This is a subclass from SliceDataset that incorporates functionality of the fastMRI+ dataset.
     It can be used to download the csv file from fastMRI+ based on the specified version using git hash.
-    It parses the csv and links it to samples in SliceDataset as annotated_examples.
+    It parses the csv and links it to samples in SliceDataset as annotated_raw_samples.
 
     Github: https://github.com/microsoft/fastmri-plus
     Paper: https://arxiv.org/abs/2109.03812
     """
 
     def __init__(
         self,
@@ -429,15 +467,15 @@
             use_dataset_cache,
             sample_rate,
             volume_sample_rate,
             dataset_cache_file,
             num_cols,
         )
 
-        self.annotated_examples = []
+        annotated_raw_samples: List[FastMRIRawDataSample] = []
 
         if subsplit not in ("knee", "brain"):
             raise ValueError('subsplit should be either "knee" or "brain"')
         if multiple_annotation_policy not in ("first", "random", "all"):
             raise ValueError(
                 'multiple_annotation_policy should be "single", "random", or "all"'
             )
@@ -447,100 +485,116 @@
         annotation_path = Path(os.getcwd(), ".annotation_cache", annotation_name)
         if not annotation_path.is_file():
             annotation_path = self.download_csv(
                 annotation_version, subsplit, annotation_path
             )
         annotations_csv = pd.read_csv(annotation_path)
 
-        for example in self.examples:
-            fname, slice_ind, metadata = example
+        for raw_sample in self.raw_samples:
+            fname, slice_ind, metadata = raw_sample
+            metadata = deepcopy(metadata)
+            maxy = metadata["recon_size"][0]
 
             # using filename and slice to find desired annotation
             annotations_df = annotations_csv[
                 (annotations_csv["file"] == fname.stem)
                 & (annotations_csv["slice"] == slice_ind)
             ]
-            annotations_list = annotations_df.itertuples(index=True, name="Pandas")
-
-            # if annotation (filename or slice) not found, fill in empty values
-            if len(annotations_df) == 0:
-                annotation = self.get_annotation(True, None)
-                metadata["annotation"] = annotation
-                self.annotated_examples.append(
-                    list([fname, slice_ind, metadata.copy()])
-                )
 
-            elif len(annotations_df) == 1:
-                rows = list(annotations_list)[0]
-                annotation = self.get_annotation(False, rows)
-                metadata["annotation"] = annotation
-                self.annotated_examples.append(
-                    list([fname, slice_ind, metadata.copy()])
-                )
-
-            else:
-                # only use the first annotation
-                if multiple_annotation_policy == "first":
-                    rows = list(annotations_list)[0]
-                    annotation = self.get_annotation(False, rows)
+            if len(annotations_df) > 1 and multiple_annotation_policy == "all":
+                # multiple annotations
+                # extend raw samples to have tow copies of the same slice,
+                # one for each annotation
+                for ind in range(len(annotations_df)):
+                    row = annotations_df.iloc[ind]
+                    annotation = self.get_annotation(row, maxy)
                     metadata["annotation"] = annotation
-                    self.annotated_examples.append(
-                        list([fname, slice_ind, metadata.copy()])
+                    annotated_raw_samples.append(
+                        FastMRIRawDataSample(fname, slice_ind, metadata)
                     )
-
-                # use an annotation at random
+            else:
+                # only add one annotation
+                if len(annotations_df) == 0:
+                    # no annotation found
+                    rows = None
+                elif len(annotations_df) == 1 or multiple_annotation_policy == "first":
+                    # only use the first annotation
+                    rows = annotations_df.iloc[0]
                 elif multiple_annotation_policy == "random":
+                    # use an annotation at random
                     random_number = torch.randint(len(annotations_df) - 1, (1,))
-                    rows = list(annotations_list)[random_number]
-                    annotation = self.get_annotation(False, rows)
-                    metadata["annotation"] = annotation
-                    self.annotated_examples.append(
-                        list([fname, slice_ind, metadata.copy()])
-                    )
+                    rows = annotations_df.iloc[random_number]
 
-                # extend examples to have tow copies of the same slice, one for each annotation
-                elif multiple_annotation_policy == "all":
-                    for rows in annotations_list:
-                        annotation = self.get_annotation(False, rows)
-                        metadata["annotation"] = annotation
-                        self.annotated_examples.append(
-                            list([fname, slice_ind, metadata.copy()])
-                        )
+                metadata["annotation"] = self.get_annotation(rows, maxy)
+                annotated_raw_samples.append(
+                    FastMRIRawDataSample(fname, slice_ind, metadata)
+                )
 
-    def get_annotation(self, empty_value, row):
-        if empty_value is True:
+        self.raw_samples = annotated_raw_samples
+
+    def get_annotation(self, row: Optional[pd.Series], maxy: int):
+        if row is None:
             annotation = {
                 "fname": "",
                 "slice": "",
                 "study_level": "",
                 "x": -1,
                 "y": -1,
                 "width": -1,
                 "height": -1,
                 "label": "",
             }
+        elif row.study_level == "Yes":
+            annotation = {
+                "fname": str(row.file),
+                "slice": "",
+                "study_level": "Yes",
+                "x": -1,
+                "y": -1,
+                "width": -1,
+                "height": -1,
+                "label": str(row.label),
+            }
         else:
             annotation = {
                 "fname": str(row.file),
                 "slice": int(row.slice),
                 "study_level": str(row.study_level),
                 "x": int(row.x),
-                "y": 320 - int(row.y) - int(row.height) - 1,
+                "y": maxy - int(row.y) - int(row.height),
                 "width": int(row.width),
                 "height": int(row.height),
                 "label": str(row.label),
             }
         return annotation
 
     def download_csv(self, version, subsplit, path):
         # request file by git hash and mri type
-        url = f"https://raw.githubusercontent.com/microsoft/fastmri-plus/{version}/Annotations/{subsplit}.csv"
-        request = requests.get(url, timeout=10, stream=True)
+        if version is None:
+            url = (
+                "https://raw.githubusercontent.com/microsoft/fastmri-plus/"
+                f"main/Annotations/{subsplit}.csv"
+            )
+        else:
+            url = (
+                "https://raw.githubusercontent.com/microsoft/fastmri-plus/"
+                f"{version}/Annotations/{subsplit}.csv"
+            )
+        response = requests.get(url, timeout=10, stream=True)
 
         # create temporary folders
         Path(".annotation_cache").mkdir(parents=True, exist_ok=True)
 
+        total_size_in_bytes = int(response.headers.get("content-length", 0))
+        progress_bar = tqdm(
+            desc="Downloading annotations",
+            total=total_size_in_bytes,
+            unit="iB",
+            unit_scale=True,
+        )
+
         # download csv from github and save it locally
         with open(path, "wb") as fh:
-            for chunk in request.iter_content(1024 * 1024):
+            for chunk in response.iter_content(1024 * 1024):
+                progress_bar.update(len(chunk))
                 fh.write(chunk)
         return path
```

### Comparing `fastmri-0.2.0/fastmri/data/subsample.py` & `fastmri-0.3.0/fastmri/data/subsample.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/data/transforms.py` & `fastmri-0.3.0/fastmri/data/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             mask: The generated mask.
             num_low_frequencies: The number of low-resolution frequency samples
                 in the mask.
     """
     shape = (1,) * len(data.shape[:-3]) + tuple(data.shape[-3:])
     mask, num_low_frequencies = mask_func(shape, offset, seed)
     if padding is not None:
-        mask[:, :, : padding[0]] = 0
-        mask[:, :, padding[1] :] = 0  # padding value inclusive on right of zeros
+        mask[..., : padding[0], :] = 0
+        mask[..., padding[1] :, :] = 0  # padding value inclusive on right of zeros
 
     masked_data = data * mask + 0.0  # the + 0.0 removes the sign of the zeros
 
     return masked_data, mask, num_low_frequencies
 
 
 def mask_center(x: torch.Tensor, mask_from: int, mask_to: int) -> torch.Tensor:
```

### Comparing `fastmri-0.2.0/fastmri/data/volume_sampler.py` & `fastmri-0.3.0/fastmri/data/volume_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,31 +59,31 @@
         self.rank = rank
         self.epoch = 0
         self.shuffle = shuffle
         self.seed = seed
 
         # get all file names and split them based on number of processes
         self.all_volume_names = sorted(
-            set(str(example[0]) for example in self.dataset.examples)
+            set(str(raw_sample[0]) for raw_sample in self.dataset.raw_samples)
         )
         self.all_volumes_split: List[List[str]] = []
         for rank_num in range(self.num_replicas):
             self.all_volumes_split.append(
                 [
                     self.all_volume_names[i]
                     for i in range(
                         rank_num, len(self.all_volume_names), self.num_replicas
                     )
                 ]
             )
 
         # get slice indices for each file name
         rank_indices: List[List[int]] = [[] for _ in range(self.num_replicas)]
-        for i, example in enumerate(self.dataset.examples):
-            vname = str(example[0])
+        for i, raw_sample in enumerate(self.dataset.raw_samples):
+            vname = str(raw_sample[0])
             for rank_num in range(self.num_replicas):
                 if vname in self.all_volumes_split[rank_num]:
                     rank_indices[rank_num].append(i)
                     break
 
         # need to send equal number of samples to each process - take the max
         self.num_samples = max(len(indices) for indices in rank_indices)
```

### Comparing `fastmri-0.2.0/fastmri/evaluate.py` & `fastmri-0.3.0/fastmri/evaluate.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/fftc.py` & `fastmri-0.3.0/fastmri/fftc.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/losses.py` & `fastmri-0.3.0/fastmri/losses.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/math.py` & `fastmri-0.3.0/fastmri/math.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/models/adaptive_varnet.py` & `fastmri-0.3.0/fastmri/models/adaptive_varnet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/models/policy.py` & `fastmri-0.3.0/fastmri/models/policy.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/models/unet.py` & `fastmri-0.3.0/fastmri/models/unet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/models/varnet.py` & `fastmri-0.3.0/fastmri/models/varnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         else:
             num_low_frequencies_tensor = num_low_frequencies * torch.ones(
                 mask.shape[0], dtype=mask.dtype, device=mask.device
             )
 
         pad = (mask.shape[-2] - num_low_frequencies_tensor + 1) // 2
 
-        return pad, num_low_frequencies_tensor
+        return pad.type(torch.long), num_low_frequencies_tensor.type(torch.long)
 
     def forward(
         self,
         masked_kspace: torch.Tensor,
         mask: torch.Tensor,
         num_low_frequencies: Optional[int] = None,
     ) -> torch.Tensor:
```

### Comparing `fastmri-0.2.0/fastmri/pl_modules/data_module.py` & `fastmri-0.3.0/fastmri/pl_modules/data_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,17 @@
         test_path: Optional[Path] = None,
         sample_rate: Optional[float] = None,
         val_sample_rate: Optional[float] = None,
         test_sample_rate: Optional[float] = None,
         volume_sample_rate: Optional[float] = None,
         val_volume_sample_rate: Optional[float] = None,
         test_volume_sample_rate: Optional[float] = None,
+        train_filter: Optional[Callable] = None,
+        val_filter: Optional[Callable] = None,
+        test_filter: Optional[Callable] = None,
         use_dataset_cache_file: bool = True,
         batch_size: int = 1,
         num_workers: int = 4,
         distributed_sampler: bool = False,
     ):
         """
         Args:
@@ -130,14 +133,19 @@
                 not set, it defaults to 1.0. To subsample the dataset either
                 set sample_rate (sample by slice) or volume_sample_rate (sample
                 by volume), but not both.
             val_volume_sample_rate: Same as volume_sample_rate, but for val
                 split.
             test_volume_sample_rate: Same as volume_sample_rate, but for val
                 split.
+            train_filter: A callable which takes as input a training example
+                metadata, and returns whether it should be part of the training
+                dataset.
+            val_filter: Same as train_filter, but for val split.
+            test_filter: Same as train_filter, but for test split.
             use_dataset_cache_file: Whether to cache dataset metadata. This is
                 very useful for large datasets like the brain data.
             batch_size: Batch size.
             num_workers: Number of workers for PyTorch dataloader.
             distributed_sampler: Whether to use a distributed sampler. This
                 should be set to True if training with ddp.
         """
@@ -164,14 +172,17 @@
         self.test_path = test_path
         self.sample_rate = sample_rate
         self.val_sample_rate = val_sample_rate
         self.test_sample_rate = test_sample_rate
         self.volume_sample_rate = volume_sample_rate
         self.val_volume_sample_rate = val_volume_sample_rate
         self.test_volume_sample_rate = test_volume_sample_rate
+        self.train_filter = train_filter
+        self.val_filter = val_filter
+        self.test_filter = test_filter
         self.use_dataset_cache_file = use_dataset_cache_file
         self.batch_size = batch_size
         self.num_workers = num_workers
         self.distributed_sampler = distributed_sampler
 
     def _create_data_loader(
         self,
@@ -184,34 +195,37 @@
             is_train = True
             sample_rate = self.sample_rate if sample_rate is None else sample_rate
             volume_sample_rate = (
                 self.volume_sample_rate
                 if volume_sample_rate is None
                 else volume_sample_rate
             )
+            raw_sample_filter = self.train_filter
         else:
             is_train = False
             if data_partition == "val":
                 sample_rate = (
                     self.val_sample_rate if sample_rate is None else sample_rate
                 )
                 volume_sample_rate = (
                     self.val_volume_sample_rate
                     if volume_sample_rate is None
                     else volume_sample_rate
                 )
+                raw_sample_filter = self.val_filter
             elif data_partition == "test":
                 sample_rate = (
                     self.test_sample_rate if sample_rate is None else sample_rate
                 )
                 volume_sample_rate = (
                     self.test_volume_sample_rate
                     if volume_sample_rate is None
                     else volume_sample_rate
                 )
+                raw_sample_filter = self.test_filter
 
         # if desired, combine train and val together for the train split
         dataset: Union[SliceDataset, CombinedSliceDataset]
         if is_train and self.combine_train_val:
             data_paths = [
                 self.data_path / f"{self.challenge}_train",
                 self.data_path / f"{self.challenge}_val",
@@ -226,28 +240,30 @@
             dataset = CombinedSliceDataset(
                 roots=data_paths,
                 transforms=data_transforms,
                 challenges=challenges,
                 sample_rates=sample_rates,
                 volume_sample_rates=volume_sample_rates,
                 use_dataset_cache=self.use_dataset_cache_file,
+                raw_sample_filter=raw_sample_filter,
             )
         else:
             if data_partition in ("test", "challenge") and self.test_path is not None:
                 data_path = self.test_path
             else:
                 data_path = self.data_path / f"{self.challenge}_{data_partition}"
 
             dataset = SliceDataset(
                 root=data_path,
                 transform=data_transform,
                 sample_rate=sample_rate,
                 volume_sample_rate=volume_sample_rate,
                 challenge=self.challenge,
                 use_dataset_cache=self.use_dataset_cache_file,
+                raw_sample_filter=raw_sample_filter,
             )
 
         # ensure that entire volumes go to the same GPU in the ddp setting
         sampler = None
 
         if self.distributed_sampler:
             if is_train:
```

### Comparing `fastmri-0.2.0/fastmri/pl_modules/mri_module.py` & `fastmri-0.3.0/fastmri/pl_modules/mri_module.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/pl_modules/unet_module.py` & `fastmri-0.3.0/fastmri/pl_modules/unet_module.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/pl_modules/varnet_module.py` & `fastmri-0.3.0/fastmri/pl_modules/varnet_module.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri/utils.py` & `fastmri-0.3.0/fastmri/utils.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri.egg-info/PKG-INFO` & `fastmri-0.3.0/fastmri.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmri
-Version: 0.2.0
+Version: 0.3.0
 Summary: A large-scale dataset of both raw MRI measurements and clinical MRI images.
 Author: Meta/NYU fastMRI Team
 Author-email: fastmri@fb.com
 License: MIT
 Project-URL: Homepage, https://fastmri.org/
 Project-URL: Source, https://github.com/facebookresearch/fastMRI
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 License-File: LICENSE.md
 
 # fastMRI
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/fastMRI/blob/master/LICENSE.md)
 [![Build and Test](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/fastMRI/actions/workflows/build-and-test.yml)
 
-[Website and Leaderboards](https://fastMRI.org) |
+[Website](https://fastMRI.org) |
 [Dataset](https://fastmri.med.nyu.edu/) |
 [GitHub](https://github.com/facebookresearch/fastMRI) |
 [Publications](#list-of-papers)
 
 Accelerating Magnetic Resonance Imaging (MRI) by acquiring fewer measurements
 has the potential to reduce medical costs, minimize stress to patients and make
 MR imaging possible in applications where it is currently prohibitively slow or
@@ -52,22 +52,25 @@
 publications of the fastMRI project.
 
 ## Documentation
 
 ### The fastMRI Dataset
 
 There are multiple publications describing different subcomponents of the data
-(e.g., brain vs. knee) and associated baselines.
+(e.g., brain vs. knee) and associated baselines. All of the fastMRI data can be
+downloaded from the [fastMRI dataset page](https://fastmri.med.nyu.edu/).
 
 * **Project Summary, Datasets, Baselines:** [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI ({J. Zbontar*, F. Knoll*, A. Sriram*} et al., 2018)](https://arxiv.org/abs/1811.08839)
 
 * **Knee Data:** [fastMRI: A Publicly Available Raw k-Space and DICOM Dataset of Knee Images for Accelerated MR Image Reconstruction Using Machine Learning ({F. Knoll*, J. Zbontar*} et al., 2020)](https://doi.org/10.1148/ryai.2020190007)
 
 * **Brain Dataset Properties:** [Supplemental Material](https://ieeexplore.ieee.org/ielx7/42/9526230/9420272/supp1-3075856.pdf?arnumber=9420272) of [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction ({M. Muckley*, B. Riemenschneider*} et al., 2021)](https://doi.org/10.1109/TMI.2021.3075856)
 
+* **Prostate Data:** [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://arxiv.org/abs/2304.09254)
+
 ### Code Repository
 
 For code documentation, most functions and classes have accompanying docstrings
 that you can access via the `help` function in IPython. For example:
 
 ```python
 from fastmri.data import SliceDataset
@@ -139,20 +142,24 @@
   * [U-Net: Convolutional networks for biomedical image segmentation (O. Ronneberger et al., 2015)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/)
 
 * **Sampling, Reconstruction and Artifact Correction**
 
   * [Offset Sampling Improves Deep Learning based Accelerated MRI Reconstructions by Exploiting Symmetry (A. Defazio, 2019)](https://github.com/facebookresearch/fastMRI/blob/8abe6eaeeb3d4504f26dc77adffb02a4be41d6f4/fastmri/data/subsample.py#L344-L475)
   * [End-to-End Variational Networks for Accelerated MRI Reconstruction ({A. Sriram*, J. Zbontar*} et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/varnet/)
   * [MRI Banding Removal via Adversarial Training (A. Defazio, et al., 2020)](https://github.com/facebookresearch/fastMRI/tree/master/banding_removal)
+  * [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI (P. Johnson et al., 2023)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/RadiologyJohnson2022)
 
 * **Active Acquisition**
   * (external repository) [Reducing uncertainty in undersampled MRI reconstruction with active acquisition (Z. Zhang et al., 2019)](https://github.com/facebookresearch/active-mri-acquisition/tree/master/activemri/experimental/cvpr19_models)
   * (external repository) [Active MR k-space Sampling with Reinforcement Learning (L. Pineda et al., 2020)](https://github.com/facebookresearch/active-mri-acquisition)
   * [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction (T. Bakker et al., 2022)](https://github.com/facebookresearch/fastMRI/tree/main/fastmri_examples/adaptive_varnet/)
 
+* **Prostate Data**
+  * (external respository) [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging (Tibrewala et al., 2023)](https://github.com/cai2r/fastMRI_prostate)
+
 ## Testing
 
 Run `pytest tests`. By default integration tests that use the fastMRI data are
 skipped. If you would like to run these tests, set `SKIP_INTEGRATIONS` to
 `False` in the [conftest](https://github.com/facebookresearch/fastMRI/tree/master/tests/conftest.py).
 
 ## Training a model
@@ -164,43 +171,54 @@
 
 Please look at
 [this U-Net demo script](https://github.com/facebookresearch/fastMRI/tree/master/fastmri_examples/unet/train_unet_demo.py) for an
 example of how to train a model using the PyTorch Lightning framework.
 
 ## Submitting to the Leaderboard
 
-Run your model on the provided test data and create a zip file containing your
-predictions. `fastmri` has a `save_reconstructions` function that saves the
-data in the correct format.
-
-Upload the zip file to any publicly accessible cloud storage (e.g. Amazon S3,
-Dropbox etc). Submit a link to the zip file on the
-[challenge website](https://fastmri.org/submit). You will need to create an
-account before submitting.
+**NOTICE:** As documented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293),
+the fastmri.org domain was transferred from Meta ownership to NYU ownership on
+2023-04-17, and NYU has not yet rebuilt the site. Until the site and
+leaderbaords are rebuilt by NYU, leaderboards will be unavailable. Mitigations
+are presented in [Discussion 293](https://github.com/facebookresearch/fastMRI/discussions/293).
 
 ## License
 
 fastMRI is MIT licensed, as found in the [LICENSE file](https://github.com/facebookresearch/fastMRI/tree/master/LICENSE.md).
 
 ## Cite
 
 If you use the fastMRI data or code in your project, please cite the arXiv
 paper:
 
 ```BibTeX
-@inproceedings{zbontar2018fastMRI,
+@misc{zbontar2018fastMRI,
     title={{fastMRI}: An Open Dataset and Benchmarks for Accelerated {MRI}},
     author={Jure Zbontar and Florian Knoll and Anuroop Sriram and Tullie Murrell and Zhengnan Huang and Matthew J. Muckley and Aaron Defazio and Ruben Stern and Patricia Johnson and Mary Bruno and Marc Parente and Krzysztof J. Geras and Joe Katsnelson and Hersh Chandarana and Zizhao Zhang and Michal Drozdzal and Adriana Romero and Michael Rabbat and Pascal Vincent and Nafissa Yakubova and James Pinkerton and Duo Wang and Erich Owens and C. Lawrence Zitnick and Michael P. Recht and Daniel K. Sodickson and Yvonne W. Lui},
     journal = {ArXiv e-prints},
     archivePrefix = "arXiv",
     eprint = {1811.08839},
     year={2018}
 }
 ```
 
+If you use the fastMRI prostate data or code in your project, please cite that
+paper:
+
+```BibTeX
+@misc{tibrewala2023fastmri,
+  title={{FastMRI Prostate}: A Publicly Available, Biparametric {MRI} Dataset to Advance Machine Learning for Prostate Cancer Imaging},
+  author={Tibrewala, Radhika and Dutt, Tarun and Tong, Angela and Ginocchio, Luke and Keerthivasan, Mahesh B and Baete, Steven H and Chopra, Sumit and Lui, Yvonne W and Sodickson, Daniel K and Chandarana, Hersh and Johnson, Patricia M},
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint={2304.09254},
+  year={2023}
+}
+```
+
 ## List of Papers
 
 The following lists titles of papers from the fastMRI project. The
 corresponding abstracts, as well as links to preprints and code can be found
 [here](https://github.com/facebookresearch/fastMRI/tree/master/LIST_OF_PAPERS.md).
 
 1. Zbontar, J.\*, Knoll, F.\*, Sriram, A.\*, Murrell, T., Huang, Z., Muckley, M. J., ... & Lui, Y. W. (2018). [fastMRI: An Open Dataset and Benchmarks for Accelerated MRI](https://arxiv.org/abs/1811.08839). *arXiv preprint arXiv:1811.08839*.
@@ -211,8 +229,11 @@
 6. Sriram, A., Zbontar, J., Murrell, T., Zitnick, C. L., Defazio, A., & Sodickson, D. K. (2020). [GrappaNet: Combining parallel imaging with deep learning for multi-coil MRI reconstruction](https://openaccess.thecvf.com/content_CVPR_2020/html/Sriram_GrappaNet_Combining_Parallel_Imaging_With_Deep_Learning_for_Multi-Coil_MRI_CVPR_2020_paper.html). In *CVPR*, pages 14315-14322.
 7. Recht, M. P., Zbontar, J., Sodickson, D. K., Knoll, F., Yakubova, N., Sriram, A., ... & Zitnick, C. L. (2020). [Using Deep Learning to Accelerate Knee MRI at 3T: Results of an Interchangeability Study](https://doi.org/10.2214/AJR.20.23313). *American Journal of Roentgenology*, 215(6), pages 1421-1429.
 8. Pineda, L., Basu, S., Romero, A., Calandra, R., & Drozdzal, M. (2020). [Active MR k-space Sampling with Reinforcement Learning](https://doi.org/10.1007/978-3-030-59713-9_3). In *MICCAI*, pages 23-33.
 9. Sriram, A.\*, Zbontar, J.\*, Murrell, T., Defazio, A., Zitnick, C. L., Yakubova, N., ... & Johnson, P. (2020). [End-to-End Variational Networks for Accelerated MRI Reconstruction](https://doi.org/10.1007/978-3-030-59713-9_7). In *MICCAI*, pages 64-73.
 10. Defazio, A., Murrell, T., & Recht, M. P. (2020). [MRI Banding Removal via Adversarial Training](https://papers.nips.cc/paper/2020/hash/567b8f5f423af15818a068235807edc0-Abstract.html). In *Advances in Neural Information Processing Systems*, 33, pages 7660-7670.
 11. Muckley, M. J.\*, Riemenschneider, B.\*, Radmanesh, A., Kim, S., Jeong, G., Ko, J., ... & Knoll, F. (2021). [Results of the 2020 fastMRI Challenge for Machine Learning MR Image Reconstruction](https://doi.org/10.1109/TMI.2021.3075856). *IEEE Transactions on Medical Imaging*, 40(9), pages 2306-2317.
 12. Johnson, P. M., Jeong, G., Hammernik, K., Schlemper, J., Qin, C., Duan, J., ..., & Knoll, F. (2021). [Evaluation of the Robustness of Learned MR Image Reconstruction to Systematic Deviations Between Training and Test Data for the Models from the fastMRI Challenge](https://doi.org/10.1007/978-3-030-88552-6_3). In *MICCAI MLMIR Workshop*, pages 25–34,
-13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://arxiv.org/abs/2203.16392). *In MIDL*. Accepted.
+13. Bakker, T., Muckley, M.J., Romero-Soriano, A., Drozdzal, M. & Pineda, L. (2022). [On learning adaptive acquisition policies for undersampled multi-coil MRI reconstruction](https://proceedings.mlr.press/v172/bakker22a). In *MIDL*, pages 63-85.
+14. Radmanesh, A.\*, Muckley, M. J.\*, Murrell, T., Lindsey, E., Sriram, A., Knoll, F., ... & Lui, Y. W. (2022). [Exploring the Acceleration Limits of Deep Learning VarNet-based Two-dimensional Brain MRI](https://doi.org/10.1148/ryai.210313). *Radiology: Artificial Intelligence*, 4(6), page e210313.
+15. Johnson, P.M., Lin, D.J., Zbontar, J., Zitnick, C.L., Sriram, A., Muckley, M., Babb, J.S., Kline, M., Ciavarra, G., Alaia, E., ..., & Knoll, F. (2023). [Deep Learning Reconstruction Enables Prospectively Accelerated Clinical Knee MRI](https://doi.org/10.1148/radiol.220425). *Radiology*, 307(2), page e220425.
+16. Tibrewala, R., Dutt, T., Tong, A., Ginocchio, L., Keerthivasan, M.B., Baete, S.H., Lui, Y.W., Sodickson, D.K., Chandarana, H., Johnson, P.M. (2023). [FastMRI Prostate: A Publicly Available, Biparametric MRI Dataset to Advance Machine Learning for Prostate Cancer Imaging](https://arxiv.org/abs/2304.09254). *arXiv preprint, arXiv:2034.09254*.
```

### Comparing `fastmri-0.2.0/fastmri.egg-info/requires.txt` & `fastmri-0.3.0/fastmri.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 PyYAML>=5.3.1
 torchmetrics>=0.5.1
 pandas>=1.3.4
 
 [dev]
 black==22.3.0
 flake8==4.0.1
-mypy==0.961
+mypy==1.1.1
 pytest==7.1.2
 types-pyyaml==5.4.10
 types-requests==2.27.6
 types-urllib3==1.26.6
 
 [tests]
 black==22.3.0
 flake8==4.0.1
 h5py==3.7.0
 isort==5.10.1
-mypy==0.961
-numpy==1.22.3
+mypy==1.1.1
+numpy==1.23.5
 pandas==1.4.2
 pandas-stubs==1.2.0.61
 pytest==7.1.2
 pytorch_lightning==1.6.4
 PyYAML==6.0
 runstats==2.0.0
 scikit_image==0.19.3
```

### Comparing `fastmri-0.2.0/fastmri_examples/README.md` & `fastmri-0.3.0/fastmri_examples/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/README.md` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/eval_pretrained_adaptive_varnet.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/eval_pretrained_adaptive_varnet.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/adaptive_varnet_module.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/adaptive_varnet_module.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/metrics.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/metrics.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/pl_modules/varnet_module.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/pl_modules/varnet_module.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/subsample.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/subsample.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/adaptive_varnet/train_adaptive_varnet_demo.py` & `fastmri-0.3.0/fastmri_examples/adaptive_varnet/train_adaptive_varnet_demo.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/annotation/fastmri_plus_viz.ipynb` & `fastmri-0.3.0/fastmri_examples/annotation/fastmri_plus_viz.ipynb`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/cs/README.md` & `fastmri-0.3.0/fastmri_examples/cs/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/cs/run_bart.py` & `fastmri-0.3.0/fastmri_examples/cs/run_bart.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/README.md` & `fastmri-0.3.0/fastmri_examples/unet/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/run_pretrained_unet_inference.py` & `fastmri-0.3.0/fastmri_examples/unet/run_pretrained_unet_inference.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/train_unet_demo.py` & `fastmri-0.3.0/fastmri_examples/unet/train_unet_demo.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_brain_leaderboard.py` & `fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_brain_leaderboard.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_mc_leaderboard.py` & `fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_mc_leaderboard.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_sc_leaderboard.py` & `fastmri-0.3.0/fastmri_examples/unet/unet_reproduce_20201111.py/unet_knee_sc_leaderboard.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/varnet/README.md` & `fastmri-0.3.0/fastmri_examples/varnet/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/varnet/run_pretrained_varnet_inference.py` & `fastmri-0.3.0/fastmri_examples/varnet/run_pretrained_varnet_inference.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/varnet/train_varnet_demo.py` & `fastmri-0.3.0/fastmri_examples/varnet/train_varnet_demo.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_brain_leaderboard.py` & `fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_brain_leaderboard.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_knee_leaderboard.py` & `fastmri-0.3.0/fastmri_examples/varnet/varnet_reproduce_20201111/varnet_knee_leaderboard.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/zero_filled/README.md` & `fastmri-0.3.0/fastmri_examples/zero_filled/README.md`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/fastmri_examples/zero_filled/run_zero_filled.py` & `fastmri-0.3.0/fastmri_examples/zero_filled/run_zero_filled.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/setup.cfg` & `fastmri-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,26 @@
 packages = find:
 python_requires = >=3.8
 
 [options.extras_require]
 dev = 
 	black==22.3.0
 	flake8==4.0.1
-	mypy==0.961
+	mypy==1.1.1
 	pytest==7.1.2
 	types-pyyaml==5.4.10
 	types-requests==2.27.6
 	types-urllib3==1.26.6
 tests = 
 	black==22.3.0
 	flake8==4.0.1
 	h5py==3.7.0
 	isort==5.10.1
-	mypy==0.961
-	numpy==1.22.3
+	mypy==1.1.1
+	numpy==1.23.5
 	pandas==1.4.2
 	pandas-stubs==1.2.0.61
 	pytest==7.1.2
 	pytorch_lightning==1.6.4
 	PyYAML==6.0
 	runstats==2.0.0
 	scikit_image==0.19.3
```

### Comparing `fastmri-0.2.0/tests/conftest.py` & `fastmri-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/tests/create_temp_data.py` & `fastmri-0.3.0/tests/create_temp_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,23 +88,27 @@
 
                 enc_limits_center = enc_size[1] // 2 + 1
                 enc_limits_max = enc_size[1] - 2
 
                 padding_left = enc_size[1] // 2 - enc_limits_center
                 padding_right = padding_left + enc_limits_max
 
-                metadata[str(fname)] = (
-                    {
-                        "padding_left": padding_left,
-                        "padding_right": padding_right,
-                        "encoding_size": enc_size,
-                        "recon_size": recon_size,
-                    },
-                    num_slices,
-                )
+                acquisition = "CORPD_FBK" if dataset == "knee_data" else "AXT1"
+
+                metadata_dict = {
+                    "padding_left": padding_left,
+                    "padding_right": padding_right,
+                    "encoding_size": enc_size,
+                    "recon_size": recon_size,
+                    "acquisition": acquisition,
+                }
+                if split.split("_")[-1] in ("test", "challenge"):
+                    metadata_dict["acceleration"] = 4
+
+                metadata[str(fname)] = (metadata_dict, num_slices)
 
                 fcount += 1
 
     return path / "knee_data", path / "brain_data", metadata
 
 
 def create_temp_annotation(path):
```

### Comparing `fastmri-0.2.0/tests/test_data.py` & `fastmri-0.3.0/tests/test_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Copyright (c) Facebook, Inc. and its affiliates.
 
 This source code is licensed under the MIT license found in the
 LICENSE file in the root directory of this source tree.
 """
 
+import pytest
+
 from fastmri.data.mri_data import (
     AnnotatedSliceDataset,
     CombinedSliceDataset,
     SliceDataset,
 )
 
 
@@ -37,14 +39,49 @@
             )
 
             assert len(dataset) > 0
             assert dataset[0] is not None
             assert dataset[-1] is not None
 
 
+@pytest.mark.parametrize(
+    "acquisition, is_full",
+    [
+        ("CORPD_FBK", True),
+        ("CORPDFS_FBK", False),
+    ],
+)
+def test_filtered_slice_datasets(
+    fastmri_mock_dataset, monkeypatch, acquisition, is_full
+):
+    knee_path, brain_path, metadata = fastmri_mock_dataset
+
+    def retrieve_metadata_mock(a, fname):
+        return metadata[str(fname)]
+
+    def raw_sample_filter(raw_sample):
+        return raw_sample.metadata["acquisition"] == acquisition
+
+    monkeypatch.setattr(SliceDataset, "_retrieve_metadata", retrieve_metadata_mock)
+
+    for challenge in ("multicoil", "singlecoil"):
+        for split in ("train", "val", "test", "challenge"):
+            dataset = SliceDataset(
+                knee_path / f"{challenge}_{split}",
+                transform=None,
+                challenge=challenge,
+                raw_sample_filter=raw_sample_filter,
+            )
+
+            if is_full:
+                assert len(dataset) > 0
+            else:
+                assert len(dataset) == 0
+
+
 def test_combined_slice_dataset(fastmri_mock_dataset, monkeypatch):
     knee_path, brain_path, metadata = fastmri_mock_dataset
 
     def retrieve_metadata_mock(a, fname):
         return metadata[str(fname)]
 
     monkeypatch.setattr(SliceDataset, "_retrieve_metadata", retrieve_metadata_mock)
```

### Comparing `fastmri-0.2.0/tests/test_integrations.py` & `fastmri-0.3.0/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/tests/test_math.py` & `fastmri-0.3.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/tests/test_models.py` & `fastmri-0.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/tests/test_modules.py` & `fastmri-0.3.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `fastmri-0.2.0/tests/test_transforms.py` & `fastmri-0.3.0/tests/test_transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,47 @@
     assert mask.shape == expected_mask.shape
     assert np.all(expected_mask.numpy() == mask.numpy())
     assert np.all(np.where(mask.numpy() == 0, 0, output.numpy()) == output.numpy())
     assert num_low_frequencies == expected_num_low_frequencies
 
 
 @pytest.mark.parametrize(
+    "shape, center_fractions, accelerations",
+    [([150, 75, 2], [0.08], [4]), ([120, 60, 2], [0.04, 0.08], [8, 4])],
+)
+def test_apply_mask_with_padding(shape, center_fractions, accelerations):
+    state = np.random.get_state()
+
+    padding = [3, shape[-2] - 3]
+    mask_func = RandomMaskFunc(center_fractions, accelerations)
+    expected_mask, expected_num_low_frequencies = mask_func(shape, seed=123)
+    assert expected_num_low_frequencies in [
+        round(cf * shape[-2]) for cf in center_fractions
+    ]
+    x = create_input(shape)
+    output, mask, num_low_frequencies = transforms.apply_mask(
+        x,
+        mask_func,
+        seed=123,
+        padding=padding,
+    )
+
+    assert (state[1] == np.random.get_state()[1]).all()
+    assert output.shape == x.shape
+    assert mask.shape == expected_mask.shape
+    assert np.unique(mask.numpy()).tolist() == [0.0, 1.0]
+    assert np.all(
+        expected_mask[..., padding[0] : padding[1], :].numpy()
+        == mask[..., padding[0] : padding[1], :].numpy()
+    )
+    assert np.all(np.where(mask.numpy() == 0, 0, output.numpy()) == output.numpy())
+    assert num_low_frequencies == expected_num_low_frequencies
+
+
+@pytest.mark.parametrize(
     "mask_type",
     ["random", "equispaced", "equispaced_fraction", "magic", "magic_fraction"],
 )
 def test_mask_types(mask_type):
     shape_list = ((4, 32, 32, 2), (2, 64, 32, 2), (1, 33, 24, 2))
     center_fraction_list = ([0.08], [0.04], [0.04, 0.08])
     acceleration_list = ([4], [8], [4, 8])
```

