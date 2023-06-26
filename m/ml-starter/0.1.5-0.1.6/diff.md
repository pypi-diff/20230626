# Comparing `tmp/ml-starter-0.1.5.tar.gz` & `tmp/ml-starter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.5.tar", last modified: Sun Jun 25 22:32:29 2023, max compression
+gzip compressed data, was "ml-starter-0.1.6.tar", last modified: Mon Jun 26 06:11:16 2023, max compression
```

## Comparing `ml-starter-0.1.5.tar` & `ml-starter-0.1.6.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.549038 ml-starter-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 22:32:12.000000 ml-starter-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 22:32:12.000000 ml-starter-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 22:32:29.549038 ml-starter-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-25 22:32:12.000000 ml-starter-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.533038 ml-starter-0.1.5/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.533038 ml-starter-0.1.5/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.533038 ml-starter-0.1.5/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.537038 ml-starter-0.1.5/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.541038 ml-starter-0.1.5/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.545038 ml-starter-0.1.5/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.545038 ml-starter-0.1.5/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.549038 ml-starter-0.1.5/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.549038 ml-starter-0.1.5/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-25 22:32:12.000000 ml-starter-0.1.5/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:32:29.549038 ml-starter-0.1.5/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 22:32:29.000000 ml-starter-0.1.5/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-25 22:32:29.000000 ml-starter-0.1.5/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:32:29.000000 ml-starter-0.1.5/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 22:32:29.000000 ml-starter-0.1.5/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 22:32:29.000000 ml-starter-0.1.5/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 22:32:12.000000 ml-starter-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-25 22:32:12.000000 ml-starter-0.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 22:32:12.000000 ml-starter-0.1.5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 22:32:12.000000 ml-starter-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-25 22:32:29.549038 ml-starter-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 22:32:12.000000 ml-starter-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.171654 ml-starter-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 06:11:04.000000 ml-starter-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 06:11:04.000000 ml-starter-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 06:11:16.171654 ml-starter-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 06:11:04.000000 ml-starter-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.155653 ml-starter-0.1.6/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.155653 ml-starter-0.1.6/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.155653 ml-starter-0.1.6/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.155653 ml-starter-0.1.6/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.155653 ml-starter-0.1.6/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.159653 ml-starter-0.1.6/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.159653 ml-starter-0.1.6/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.159653 ml-starter-0.1.6/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.159653 ml-starter-0.1.6/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.159653 ml-starter-0.1.6/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.163653 ml-starter-0.1.6/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.167654 ml-starter-0.1.6/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.167654 ml-starter-0.1.6/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.171654 ml-starter-0.1.6/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.171654 ml-starter-0.1.6/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-26 06:11:04.000000 ml-starter-0.1.6/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:16.171654 ml-starter-0.1.6/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 06:11:16.000000 ml-starter-0.1.6/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-26 06:11:16.000000 ml-starter-0.1.6/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:11:16.000000 ml-starter-0.1.6/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 06:11:16.000000 ml-starter-0.1.6/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 06:11:16.000000 ml-starter-0.1.6/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 06:11:04.000000 ml-starter-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 06:11:04.000000 ml-starter-0.1.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 06:11:04.000000 ml-starter-0.1.6/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 06:11:04.000000 ml-starter-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 06:11:16.171654 ml-starter-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 06:11:04.000000 ml-starter-0.1.6/setup.py
```

### Comparing `ml-starter-0.1.5/LICENSE` & `ml-starter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/PKG-INFO` & `ml-starter-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.5
+Version: 0.1.6
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.5/README.md` & `ml-starter-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/api.py` & `ml-starter-0.1.6/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     "SupervisedLearningTaskConfig",
     "SupervisedLearningTrainer",
     "SupervisedLearningTrainerConfig",
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
     "test_environment",
+    "test_task",
     "timeout",
     "Timer",
     "TokenReader",
     "TokenWriter",
     "transforms",
     "VideoFileDataset",
     "WorkerPool",
@@ -235,15 +236,14 @@
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
 from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
 from ml.tasks.datasets.multi_iter import MultiIterDataset
 from ml.tasks.datasets.samplers import ChunkSampler
 from ml.tasks.datasets.streaming import StreamingDataset, StreamingDatasetNoIndex
-from ml.tasks.datasets.utils import test_dataset
 from ml.tasks.datasets.video_file import VideoFileDataset
 from ml.tasks.environments.base import Environment
 from ml.tasks.environments.utils import test_environment
 from ml.tasks.environments.worker import (
     AsyncEnvironmentWorker,
     AsyncWorkerPool,
     BaseEnvironmentWorker,
@@ -288,14 +288,15 @@
 from ml.utils.image import read_gif, write_gif
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
 from ml.utils.parallel import init_parallelism, parallel_group_info, parallelism_is_initialized, reset_parallelism
 from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
+from ml.utils.testing import test_dataset, test_task
 from ml.utils.timer import Timer, timeout
 from ml.utils.tokens import TokenReader, TokenWriter
 from ml.utils.torch_distributed import (
     MultiprocessConfig,
     get_distributed_backend,
     init_and_run,
     init_dist,
```

### Comparing `ml-starter-0.1.5/ml/core/common_types.py` & `ml-starter-0.1.6/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/core/config.py` & `ml-starter-0.1.6/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/core/env.py` & `ml-starter-0.1.6/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/core/registry.py` & `ml-starter-0.1.6/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/core/state.py` & `ml-starter-0.1.6/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/launchers/base.py` & `ml-starter-0.1.6/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/launchers/mp.py` & `ml-starter-0.1.6/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/launchers/slurm.py` & `ml-starter-0.1.6/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/launchers/torchrun.py` & `ml-starter-0.1.6/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/loggers/base.py` & `ml-starter-0.1.6/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/loggers/meter.py` & `ml-starter-0.1.6/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/loggers/multi.py` & `ml-starter-0.1.6/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/loggers/stdout.py` & `ml-starter-0.1.6/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/loggers/tensorboard.py` & `ml-starter-0.1.6/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/base.py` & `ml-starter-0.1.6/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/constant.py` & `ml-starter-0.1.6/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.6/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.6/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/linear.py` & `ml-starter-0.1.6/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.6/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.6/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/activations.py` & `ml-starter-0.1.6/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/base.py` & `ml-starter-0.1.6/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/embeddings.py` & `ml-starter-0.1.6/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/init.py` & `ml-starter-0.1.6/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/kmeans.py` & `ml-starter-0.1.6/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/lora.py` & `ml-starter-0.1.6/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/norms.py` & `ml-starter-0.1.6/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/models/parallel.py` & `ml-starter-0.1.6/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/adam.py` & `ml-starter-0.1.6/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/adamw.py` & `ml-starter-0.1.6/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/adan.py` & `ml-starter-0.1.6/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/base.py` & `ml-starter-0.1.6/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/common.py` & `ml-starter-0.1.6/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/lion.py` & `ml-starter-0.1.6/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/sgd.py` & `ml-starter-0.1.6/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/optimizers/shampoo.py` & `ml-starter-0.1.6/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/scripts/cli.py` & `ml-starter-0.1.6/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/scripts/stage.py` & `ml-starter-0.1.6/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/scripts/train.py` & `ml-starter-0.1.6/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/base.py` & `ml-starter-0.1.6/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.6/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.6/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/collate.py` & `ml-starter-0.1.6/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.6/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.6/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.6/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.6/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.6/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.6/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/environments/base.py` & `ml-starter-0.1.6/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/environments/utils.py` & `ml-starter-0.1.6/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/environments/worker.py` & `ml-starter-0.1.6/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/losses/reduce.py` & `ml-starter-0.1.6/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/rl/base.py` & `ml-starter-0.1.6/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/rl/replay.py` & `ml-starter-0.1.6/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/tasks/sl/base.py` & `ml-starter-0.1.6/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/base.py` & `ml-starter-0.1.6/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/learning.py` & `ml-starter-0.1.6/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/compile.py` & `ml-starter-0.1.6/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.6/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.6/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.6/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.6/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.6/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.6/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.6/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.6/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.6/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/rl.py` & `ml-starter-0.1.6/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/trainers/sl.py` & `ml-starter-0.1.6/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/argparse.py` & `ml-starter-0.1.6/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/atomic.py` & `ml-starter-0.1.6/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/audio.py` & `ml-starter-0.1.6/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/augmentation.py` & `ml-starter-0.1.6/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/caching.py` & `ml-starter-0.1.6/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/checkpoint.py` & `ml-starter-0.1.6/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/cli.py` & `ml-starter-0.1.6/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/colors.py` & `ml-starter-0.1.6/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/data.py` & `ml-starter-0.1.6/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/datetime.py` & `ml-starter-0.1.6/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/device/auto.py` & `ml-starter-0.1.6/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/device/base.py` & `ml-starter-0.1.6/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/device/cpu.py` & `ml-starter-0.1.6/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/device/gpu.py` & `ml-starter-0.1.6/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/device/metal.py` & `ml-starter-0.1.6/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/distributed.py` & `ml-starter-0.1.6/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/image.py` & `ml-starter-0.1.6/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/io.py` & `ml-starter-0.1.6/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/large_models.py` & `ml-starter-0.1.6/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/logging.py` & `ml-starter-0.1.6/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/meter.py` & `ml-starter-0.1.6/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/parallel.py` & `ml-starter-0.1.6/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/staging.py` & `ml-starter-0.1.6/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/timer.py` & `ml-starter-0.1.6/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/tokens.py` & `ml-starter-0.1.6/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/torch_distributed.py` & `ml-starter-0.1.6/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/triton/kmeans.py` & `ml-starter-0.1.6/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/triton/lion.py` & `ml-starter-0.1.6/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml/utils/video.py` & `ml-starter-0.1.6/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.6/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.5
+Version: 0.1.6
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.5/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.6/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 ml/tasks/datasets/clippify.py
 ml/tasks/datasets/collate.py
 ml/tasks/datasets/error_handling.py
 ml/tasks/datasets/multi_iter.py
 ml/tasks/datasets/samplers.py
 ml/tasks/datasets/streaming.py
 ml/tasks/datasets/transforms.py
-ml/tasks/datasets/utils.py
 ml/tasks/datasets/video_file.py
 ml/tasks/environments/__init__.py
 ml/tasks/environments/base.py
 ml/tasks/environments/utils.py
 ml/tasks/environments/worker.py
 ml/tasks/losses/__init__.py
 ml/tasks/losses/reduce.py
@@ -120,14 +119,15 @@
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/parallel.py
 ml/utils/random.py
 ml/utils/staging.py
+ml/utils/testing.py
 ml/utils/timer.py
 ml/utils/tokens.py
 ml/utils/torch_distributed.py
 ml/utils/video.py
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
```

### Comparing `ml-starter-0.1.5/pyproject.toml` & `ml-starter-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.5/setup.py` & `ml-starter-0.1.6/setup.py`

 * *Files identical despite different names*

