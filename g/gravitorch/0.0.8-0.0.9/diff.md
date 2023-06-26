# Comparing `tmp/gravitorch-0.0.8.tar.gz` & `tmp/gravitorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitorch-0.0.8.tar", max compression
+gzip compressed data, was "gravitorch-0.0.9.tar", max compression
```

## Comparing `gravitorch-0.0.8.tar` & `gravitorch-0.0.9.tar`

### file list

```diff
@@ -1,320 +1,324 @@
--rw-r--r--   0        0        0     1501 2023-03-15 04:40:33.874553 gravitorch-0.0.8/LICENSE
--rw-r--r--   0        0        0     2799 2023-03-15 04:40:33.874553 gravitorch-0.0.8/README.md
--rw-r--r--   0        0        0     4974 2023-03-15 04:40:33.878553 gravitorch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       99 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/cli/__init__.py
--rw-r--r--   0        0        0     2337 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/cli/run.py
--rw-r--r--   0        0        0     1321 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/constants.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/__init__.py
--rw-r--r--   0        0        0      325 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/core/__init__.py
--rw-r--r--   0        0        0     3121 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/core/advanced.py
--rw-r--r--   0        0        0     2739 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/core/base.py
--rw-r--r--   0        0        0     2950 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/core/vanilla.py
--rw-r--r--   0        0        0      544 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/dataloader/__init__.py
--rw-r--r--   0        0        0     1289 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/dataloader/base.py
--rw-r--r--   0        0        0     8934 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/dataloader/pytorch.py
--rw-r--r--   0        0        0     1214 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/dataloader/utils.py
--rw-r--r--   0        0        0      600 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datapipe/__init__.py
--rw-r--r--   0        0        0     4872 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datapipe/base.py
--rw-r--r--   0        0        0     2427 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datapipe/random.py
--rw-r--r--   0        0        0    19752 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datapipe/sequential.py
--rw-r--r--   0        0        0      280 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datasource/__init__.py
--rw-r--r--   0        0        0     2002 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datasource/base.py
--rw-r--r--   0        0        0     2010 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/datasource/vanilla.py
--rw-r--r--   0        0        0      327 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/__init__.py
--rw-r--r--   0        0        0     1563 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/base.py
--rw-r--r--   0        0        0     1231 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/utils.py
--rw-r--r--   0        0        0     3508 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/vanilla.py
--rw-r--r--   0        0        0      361 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/model/base.py
--rw-r--r--   0        0        0     3570 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/model/ddp.py
--rw-r--r--   0        0        0     2874 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/model/vanilla.py
--rw-r--r--   0        0        0      526 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/__init__.py
--rw-r--r--   0        0        0     1177 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/base.py
--rw-r--r--   0        0        0     1102 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/noo.py
--rw-r--r--   0        0        0     1222 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/utils.py
--rw-r--r--   0        0        0     2319 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/vanilla.py
--rw-r--r--   0        0        0     4616 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/creators/optimizer/zero.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/__init__.py
--rw-r--r--   0        0        0      361 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datacreators/__init__.py
--rw-r--r--   0        0        0     1542 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datacreators/base.py
--rw-r--r--   0        0        0     3039 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datacreators/caching.py
--rw-r--r--   0        0        0     4989 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datacreators/hypercube_vertex.py
--rw-r--r--   0        0        0      136 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/__init__.py
--rw-r--r--   0        0        0      664 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/__init__.py
--rw-r--r--   0        0        0      725 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/base.py
--rw-r--r--   0        0        0     5377 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/packed_sequence.py
--rw-r--r--   0        0        0     6261 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/padded_sequence.py
--rw-r--r--   0        0        0      785 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/utils.py
--rw-r--r--   0        0        0     3631 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/dataloaders/samplers.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/__init__.py
--rw-r--r--   0        0        0     1535 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/__init__.py
--rw-r--r--   0        0        0     6094 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/batching.py
--rw-r--r--   0        0        0     2026 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/dictionary.py
--rw-r--r--   0        0        0     3927 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/factory.py
--rw-r--r--   0        0        0     1947 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/length.py
--rw-r--r--   0        0        0     2691 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/path.py
--rw-r--r--   0        0        0     4042 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/saving.py
--rw-r--r--   0        0        0    12044 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/shuffling.py
--rw-r--r--   0        0        0     1786 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/source.py
--rw-r--r--   0        0        0      674 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/__init__.py
--rw-r--r--   0        0        0     3546 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/demo_map_style.py
--rw-r--r--   0        0        0     1761 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/factory.py
--rw-r--r--   0        0        0     1193 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/image_folder.py
--rw-r--r--   0        0        0     3380 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/in_memory.py
--rw-r--r--   0        0        0      976 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/mnist.py
--rw-r--r--   0        0        0      828 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/datasets/utils.py
--rw-r--r--   0        0        0      792 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/__init__.py
--rw-r--r--   0        0        0     1685 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/base.py
--rw-r--r--   0        0        0     2714 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/distributed.py
--rw-r--r--   0        0        0     1764 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/even.py
--rw-r--r--   0        0        0     1665 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/fixed_size.py
--rw-r--r--   0        0        0     1761 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/sequential.py
--rw-r--r--   0        0        0     2203 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/shuffling.py
--rw-r--r--   0        0        0      574 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/data/partitioners/trivial.py
--rw-r--r--   0        0        0      759 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/__init__.py
--rw-r--r--   0        0        0     6217 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/base.py
--rw-r--r--   0        0        0    13081 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/datapipe.py
--rw-r--r--   0        0        0     4300 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/dataset.py
--rw-r--r--   0        0        0     6316 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/imagenet.py
--rw-r--r--   0        0        0     2552 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/mnist.py
--rw-r--r--   0        0        0     1798 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/datasources/utils.py
--rw-r--r--   0        0        0     2163 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/__init__.py
--rw-r--r--   0        0        0     3257 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/_constants.py
--rw-r--r--   0        0        0     4217 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/auto.py
--rw-r--r--   0        0        0     7624 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/comm.py
--rw-r--r--   0        0        0     6998 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/ddp.py
--rw-r--r--   0        0        0     5920 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/distributed/utils.py
--rw-r--r--   0        0        0      305 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/engines/__init__.py
--rw-r--r--   0        0        0    13392 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/engines/alpha.py
--rw-r--r--   0        0        0    23151 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/engines/base.py
--rw-r--r--   0        0        0     1136 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/engines/events.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/experimental/__init__.py
--rw-r--r--   0        0        0     3529 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/experimental/object_ops.py
--rw-r--r--   0        0        0     2868 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/handlers/__init__.py
--rw-r--r--   0        0        0      515 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/handlers/base.py
--rw-r--r--   0        0        0     4547 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/handlers/cudamem.py
--rw-r--r--   0        0        0     9692 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/handlers/early_stopping.py
--rw-r--r--   0        0        0     7662 2023-03-15 04:40:33.882553 gravitorch-0.0.8/src/gravitorch/handlers/engine_loader.py
--rw-r--r--   0        0        0    10220 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/engine_saver.py
--rw-r--r--   0        0        0     4586 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/lr_monitor.py
--rw-r--r--   0        0        0     3293 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/lr_scheduler.py
--rw-r--r--   0        0        0     4911 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/lr_scheduler_updater.py
--rw-r--r--   0        0        0     1926 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/model.py
--rw-r--r--   0        0        0     2209 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/model_architecture.py
--rw-r--r--   0        0        0     1830 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/model_initializer.py
--rw-r--r--   0        0        0     2317 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/model_parameter.py
--rw-r--r--   0        0        0     5298 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/model_state_dict_loader.py
--rw-r--r--   0        0        0     5771 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/optimizer_monitor.py
--rw-r--r--   0        0        0     2555 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/optimizer_state.py
--rw-r--r--   0        0        0     1803 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/sysinfo.py
--rw-r--r--   0        0        0     4023 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/handlers/utils.py
--rw-r--r--   0        0        0        0 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/__init__.py
--rw-r--r--   0        0        0      689 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/__init__.py
--rw-r--r--   0        0        0     5581 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/accelerate.py
--rw-r--r--   0        0        0     3675 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/amp.py
--rw-r--r--   0        0        0     1361 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/base.py
--rw-r--r--   0        0        0     6679 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/basic.py
--rw-r--r--   0        0        0     2292 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/conditions.py
--rw-r--r--   0        0        0     1345 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/factory.py
--rw-r--r--   0        0        0      935 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/noop.py
--rw-r--r--   0        0        0     4448 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/evaluation/vanilla.py
--rw-r--r--   0        0        0      477 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/__init__.py
--rw-r--r--   0        0        0     1264 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/base.py
--rw-r--r--   0        0        0     2119 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/batch_saving.py
--rw-r--r--   0        0        0     1196 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/factory.py
--rw-r--r--   0        0        0      660 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/noop.py
--rw-r--r--   0        0        0     1528 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/observers/sequential.py
--rw-r--r--   0        0        0      647 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/__init__.py
--rw-r--r--   0        0        0     7836 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/accelerate.py
--rw-r--r--   0        0        0     5165 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/amp.py
--rw-r--r--   0        0        0     1445 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/base.py
--rw-r--r--   0        0        0     6994 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/basic.py
--rw-r--r--   0        0        0     1279 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/factory.py
--rw-r--r--   0        0        0      916 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/noop.py
--rw-r--r--   0        0        0     6289 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/loops/training/vanilla.py
--rw-r--r--   0        0        0      567 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/lr_schedulers/__init__.py
--rw-r--r--   0        0        0     2339 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/lr_schedulers/base.py
--rw-r--r--   0        0        0     5021 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/lr_schedulers/creation.py
--rw-r--r--   0        0        0     1438 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/lr_schedulers/invsqrt.py
--rw-r--r--   0        0        0      228 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/__init__.py
--rw-r--r--   0        0        0      910 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/base.py
--rw-r--r--   0        0        0      460 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/criteria/__init__.py
--rw-r--r--   0        0        0     3852 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/criteria/packed_seq.py
--rw-r--r--   0        0        0     6567 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/criteria/padded_seq.py
--rw-r--r--   0        0        0     3500 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/criteria/vanilla.py
--rw-r--r--   0        0        0     3435 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/criteria/weighted_sum.py
--rw-r--r--   0        0        0     1647 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/__init__.py
--rw-r--r--   0        0        0     2400 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/base.py
--rw-r--r--   0        0        0     4007 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/base_epoch.py
--rw-r--r--   0        0        0      540 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/classification/__init__.py
--rw-r--r--   0        0        0     7618 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/classification/accuracy.py
--rw-r--r--   0        0        0    10346 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/classification/confusion_matrix.py
--rw-r--r--   0        0        0     1885 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/classification/cross_entropy.py
--rw-r--r--   0        0        0      905 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/__init__.py
--rw-r--r--   0        0        0     2784 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/absolute_error.py
--rw-r--r--   0        0        0     6399 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/absolute_relative_error.py
--rw-r--r--   0        0        0     3255 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/log_cosh_error.py
--rw-r--r--   0        0        0     3867 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/nmse.py
--rw-r--r--   0        0        0     4255 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/squared_error.py
--rw-r--r--   0        0        0     8815 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/regression/squared_log_error.py
--rw-r--r--   0        0        0     3013 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/sequential.py
--rw-r--r--   0        0        0    19766 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/state.py
--rw-r--r--   0        0        0     6162 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/transform.py
--rw-r--r--   0        0        0    11238 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/metrics/vanilla.py
--rw-r--r--   0        0        0      593 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/networks/__init__.py
--rw-r--r--   0        0        0     3595 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/networks/image_classification.py
--rw-r--r--   0        0        0     4786 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/networks/lenet.py
--rw-r--r--   0        0        0     9848 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/networks/mlp.py
--rw-r--r--   0        0        0     3903 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/networks/mnist.py
--rw-r--r--   0        0        0      865 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/utils/__init__.py
--rw-r--r--   0        0        0     3245 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/utils/architecture.py
--rw-r--r--   0        0        0     2325 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/utils/setup_and_attach.py
--rw-r--r--   0        0        0    17803 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/utils/summary.py
--rw-r--r--   0        0        0     6707 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/utils/testing.py
--rw-r--r--   0        0        0     7453 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/models/vanilla.py
--rw-r--r--   0        0        0     3926 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/__init__.py
--rw-r--r--   0        0        0     2215 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/activations.py
--rw-r--r--   0        0        0     4217 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/alpha_activations.py
--rw-r--r--   0        0        0     3748 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/barron_loss.py
--rw-r--r--   0        0        0     3307 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/clamp.py
--rw-r--r--   0        0        0      654 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/creators.py
--rw-r--r--   0        0        0      108 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/experimental/__init__.py
--rw-r--r--   0        0        0     3015 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/experimental/exponential_nll.py
--rw-r--r--   0        0        0     2637 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/exu.py
--rw-r--r--   0        0        0     1990 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/flatten.py
--rw-r--r--   0        0        0     5583 2023-03-15 04:40:33.886553 gravitorch-0.0.8/src/gravitorch/nn/focal_loss.py
--rw-r--r--   0        0        0    11107 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/fourier_feature.py
--rw-r--r--   0        0        0      982 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/__init__.py
--rw-r--r--   0        0        0     4172 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/barron_loss.py
--rw-r--r--   0        0        0     3113 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/error.py
--rw-r--r--   0        0        0      123 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/experimental/__init__.py
--rw-r--r--   0        0        0     2064 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/experimental/exponential_nll.py
--rw-r--r--   0        0        0     2529 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/loss_helpers.py
--rw-r--r--   0        0        0    11355 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/functional/robust_loss.py
--rw-r--r--   0        0        0     8536 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/fusion.py
--rw-r--r--   0        0        0     1014 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/__init__.py
--rw-r--r--   0        0        0      731 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/base.py
--rw-r--r--   0        0        0     7758 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/const.py
--rw-r--r--   0        0        0     1117 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/factory.py
--rw-r--r--   0        0        0     7980 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/kaiming.py
--rw-r--r--   0        0        0      586 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/noop.py
--rw-r--r--   0        0        0     4654 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/normal.py
--rw-r--r--   0        0        0     1304 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/sequential.py
--rw-r--r--   0        0        0     5136 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/init/xavier.py
--rw-r--r--   0        0        0      994 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/residual.py
--rw-r--r--   0        0        0     8779 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/robust_loss.py
--rw-r--r--   0        0        0    19758 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/scalar_encoding.py
--rw-r--r--   0        0        0     8184 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/shift_scale.py
--rw-r--r--   0        0        0    10592 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/transforms.py
--rw-r--r--   0        0        0     1763 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/__init__.py
--rw-r--r--   0        0        0     1270 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/factory.py
--rw-r--r--   0        0        0    13588 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/module_helpers.py
--rw-r--r--   0        0        0     4833 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/parameter.py
--rw-r--r--   0        0        0    10744 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/state_dict.py
--rw-r--r--   0        0        0     5830 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/summary.py
--rw-r--r--   0        0        0     6847 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/utils/testing.py
--rw-r--r--   0        0        0     3852 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/nn/warmup_seq_loss.py
--rw-r--r--   0        0        0      247 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/optimizers/__init__.py
--rw-r--r--   0        0        0     2733 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/optimizers/factory.py
--rw-r--r--   0        0        0      878 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/optimizers/noop.py
--rw-r--r--   0        0        0     3574 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/optimizers/utils.py
--rw-r--r--   0        0        0      546 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/__init__.py
--rw-r--r--   0        0        0     1056 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/base.py
--rw-r--r--   0        0        0     1846 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/distributed.py
--rw-r--r--   0        0        0     2700 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/logging.py
--rw-r--r--   0        0        0    12276 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/pytorch.py
--rw-r--r--   0        0        0     1308 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/rsrc/sysinfo.py
--rw-r--r--   0        0        0      517 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/__init__.py
--rw-r--r--   0        0        0      403 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/base.py
--rw-r--r--   0        0        0     4873 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/evaluation.py
--rw-r--r--   0        0        0     1528 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/no_repeat.py
--rw-r--r--   0        0        0     1459 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/resource.py
--rw-r--r--   0        0        0     5002 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/training.py
--rw-r--r--   0        0        0     2832 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/runners/utils.py
--rw-r--r--   0        0        0      839 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/testing/__init__.py
--rw-r--r--   0        0        0     1716 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/testing/_pytest.py
--rw-r--r--   0        0        0     6927 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/testing/dummy.py
--rw-r--r--   0        0        0      354 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/__init__.py
--rw-r--r--   0        0        0      395 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/__init__.py
--rw-r--r--   0        0        0      480 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/base.py
--rw-r--r--   0        0        0      818 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/jsona.py
--rw-r--r--   0        0        0     1125 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/picklea.py
--rw-r--r--   0        0        0      840 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/pytorcha.py
--rw-r--r--   0        0        0      757 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/artifacts/text.py
--rw-r--r--   0        0        0     7435 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/asset.py
--rw-r--r--   0        0        0     6050 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/cudamem.py
--rw-r--r--   0        0        0     1296 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/__init__.py
--rw-r--r--   0        0        0     1240 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/base.py
--rw-r--r--   0        0        0     7881 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/continuous.py
--rw-r--r--   0        0        0     2609 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/discrete.py
--rw-r--r--   0        0        0     4280 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/float_tensor.py
--rw-r--r--   0        0        0     1853 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/float_value.py
--rw-r--r--   0        0        0      819 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/integer.py
--rw-r--r--   0        0        0     2314 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/long_tensor.py
--rw-r--r--   0        0        0      677 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/noop.py
--rw-r--r--   0        0        0     2536 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/sequence.py
--rw-r--r--   0        0        0     1279 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/data_summary/utils.py
--rw-r--r--   0        0        0      679 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/__init__.py
--rw-r--r--   0        0        0      469 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/auto.py
--rw-r--r--   0        0        0      710 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/base.py
--rw-r--r--   0        0        0     1890 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/manual.py
--rw-r--r--   0        0        0      759 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/noop.py
--rw-r--r--   0        0        0     1326 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/device_placement/utils.py
--rw-r--r--   0        0        0      349 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/engine_states/__init__.py
--rw-r--r--   0        0        0    13888 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/engine_states/base.py
--rw-r--r--   0        0        0     1178 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/engine_states/utils.py
--rw-r--r--   0        0        0     3696 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/engine_states/vanilla.py
--rw-r--r--   0        0        0      670 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/events/__init__.py
--rw-r--r--   0        0        0     3539 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/events/conditions.py
--rw-r--r--   0        0        0     4769 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/events/event_handlers.py
--rw-r--r--   0        0        0    10937 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/events/manager.py
--rw-r--r--   0        0        0      818 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/__init__.py
--rw-r--r--   0        0        0    32543 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/base.py
--rw-r--r--   0        0        0     6659 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/noop.py
--rw-r--r--   0        0        0      897 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/steps.py
--rw-r--r--   0        0        0    11680 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/tensorboard.py
--rw-r--r--   0        0        0     2306 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/utils.py
--rw-r--r--   0        0        0      873 2023-03-15 04:40:33.890553 gravitorch-0.0.8/src/gravitorch/utils/factory.py
--rw-r--r--   0        0        0    16295 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/format.py
--rw-r--r--   0        0        0      764 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/__init__.py
--rw-r--r--   0        0        0    15554 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/base.py
--rw-r--r--   0        0        0     7197 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/comparable.py
--rw-r--r--   0        0        0     4707 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/comparator.py
--rw-r--r--   0        0        0     3039 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/generic.py
--rw-r--r--   0        0        0     7748 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/manager.py
--rw-r--r--   0        0        0     4510 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/history/utils.py
--rw-r--r--   0        0        0     1301 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/info.py
--rw-r--r--   0        0        0     4847 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/integrations.py
--rw-r--r--   0        0        0     9824 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/io.py
--rw-r--r--   0        0        0     1078 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/logging.py
--rw-r--r--   0        0        0     3265 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/mapping.py
--rw-r--r--   0        0        0      801 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/__init__.py
--rw-r--r--   0        0        0     6295 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/average.py
--rw-r--r--   0        0        0    44596 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/confusion_matrix.py
--rw-r--r--   0        0        0      179 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/exceptions.py
--rw-r--r--   0        0        0     6744 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/moving_average.py
--rw-r--r--   0        0        0    11018 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/scalar.py
--rw-r--r--   0        0        0    30892 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/meters/tensor.py
--rw-r--r--   0        0        0     3492 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/metric_tracker.py
--rw-r--r--   0        0        0     7302 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/module_manager.py
--rw-r--r--   0        0        0     1689 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/parameter.py
--rw-r--r--   0        0        0     6888 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/partitioning.py
--rw-r--r--   0        0        0     5511 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/path.py
--rw-r--r--   0        0        0      386 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/profilers/__init__.py
--rw-r--r--   0        0        0      840 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/profilers/base.py
--rw-r--r--   0        0        0      880 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/profilers/noop.py
--rw-r--r--   0        0        0     4497 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/profilers/pytorch.py
--rw-r--r--   0        0        0     1079 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/profilers/utils.py
--rw-r--r--   0        0        0    10720 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/seed.py
--rw-r--r--   0        0        0      572 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/sequence.py
--rw-r--r--   0        0        0     5719 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/summary.py
--rw-r--r--   0        0        0     2965 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/sysinfo.py
--rw-r--r--   0        0        0     1046 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/tensor/__init__.py
--rw-r--r--   0        0        0     5820 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/tensor/flatted.py
--rw-r--r--   0        0        0     4377 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/tensor/math_ops.py
--rw-r--r--   0        0        0     8515 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/tensor/misc.py
--rw-r--r--   0        0        0     9170 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/tensor/recursive_ops.py
--rw-r--r--   0        0        0     9335 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/timing.py
--rw-r--r--   0        0        0     2509 2023-03-15 04:40:33.894553 gravitorch-0.0.8/src/gravitorch/utils/torch_device.py
--rw-r--r--   0        0        0     4476 1970-01-01 00:00:00.000000 gravitorch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-03-27 03:54:22.084780 gravitorch-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2799 2023-03-27 03:54:22.084780 gravitorch-0.0.9/README.md
+-rw-r--r--   0        0        0     5070 2023-03-27 03:54:22.088780 gravitorch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/cli/__init__.py
+-rw-r--r--   0        0        0     2337 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/cli/run.py
+-rw-r--r--   0        0        0     1321 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/constants.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/__init__.py
+-rw-r--r--   0        0        0      325 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/core/__init__.py
+-rw-r--r--   0        0        0     3121 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/core/advanced.py
+-rw-r--r--   0        0        0     2739 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/core/base.py
+-rw-r--r--   0        0        0     2950 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/core/vanilla.py
+-rw-r--r--   0        0        0      544 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/dataloader/__init__.py
+-rw-r--r--   0        0        0     1289 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/dataloader/base.py
+-rw-r--r--   0        0        0     8934 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/dataloader/pytorch.py
+-rw-r--r--   0        0        0     1214 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/dataloader/utils.py
+-rw-r--r--   0        0        0      600 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datapipe/__init__.py
+-rw-r--r--   0        0        0     4862 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datapipe/base.py
+-rw-r--r--   0        0        0     2427 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datapipe/random.py
+-rw-r--r--   0        0        0    19682 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datapipe/sequential.py
+-rw-r--r--   0        0        0      280 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datasource/__init__.py
+-rw-r--r--   0        0        0     2002 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datasource/base.py
+-rw-r--r--   0        0        0     2010 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/datasource/vanilla.py
+-rw-r--r--   0        0        0      327 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0     1563 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/base.py
+-rw-r--r--   0        0        0     1231 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/utils.py
+-rw-r--r--   0        0        0     3508 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/vanilla.py
+-rw-r--r--   0        0        0      457 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/model/__init__.py
+-rw-r--r--   0        0        0     1898 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/model/base.py
+-rw-r--r--   0        0        0     1632 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/model/compiled.py
+-rw-r--r--   0        0        0     3570 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/model/ddp.py
+-rw-r--r--   0        0        0     2874 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/model/vanilla.py
+-rw-r--r--   0        0        0      526 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/__init__.py
+-rw-r--r--   0        0        0     1177 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/base.py
+-rw-r--r--   0        0        0     1102 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/noo.py
+-rw-r--r--   0        0        0     1222 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/utils.py
+-rw-r--r--   0        0        0     2319 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/vanilla.py
+-rw-r--r--   0        0        0     4616 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/creators/optimizer/zero.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/__init__.py
+-rw-r--r--   0        0        0      361 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datacreators/__init__.py
+-rw-r--r--   0        0        0     1542 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datacreators/base.py
+-rw-r--r--   0        0        0     3039 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datacreators/caching.py
+-rw-r--r--   0        0        0     4989 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datacreators/hypercube_vertex.py
+-rw-r--r--   0        0        0      136 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/__init__.py
+-rw-r--r--   0        0        0      664 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/base.py
+-rw-r--r--   0        0        0     5377 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/packed_sequence.py
+-rw-r--r--   0        0        0     6261 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/padded_sequence.py
+-rw-r--r--   0        0        0      785 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/utils.py
+-rw-r--r--   0        0        0     3631 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/dataloaders/samplers.py
+-rw-r--r--   0        0        0      674 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3546 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/demo_map_style.py
+-rw-r--r--   0        0        0     1761 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/factory.py
+-rw-r--r--   0        0        0     1193 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/image_folder.py
+-rw-r--r--   0        0        0     3380 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/in_memory.py
+-rw-r--r--   0        0        0      976 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/mnist.py
+-rw-r--r--   0        0        0      828 2023-03-27 03:54:22.088780 gravitorch-0.0.9/src/gravitorch/data/datasets/utils.py
+-rw-r--r--   0        0        0      792 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/__init__.py
+-rw-r--r--   0        0        0     1685 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/base.py
+-rw-r--r--   0        0        0     2714 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/distributed.py
+-rw-r--r--   0        0        0     1764 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/even.py
+-rw-r--r--   0        0        0     1665 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/fixed_size.py
+-rw-r--r--   0        0        0     1761 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/sequential.py
+-rw-r--r--   0        0        0     2203 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/shuffling.py
+-rw-r--r--   0        0        0      574 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/data/partitioners/trivial.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/__init__.py
+-rw-r--r--   0        0        0     1434 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/__init__.py
+-rw-r--r--   0        0        0     6071 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/batching.py
+-rw-r--r--   0        0        0     2026 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/dictionary.py
+-rw-r--r--   0        0        0     3897 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/factory.py
+-rw-r--r--   0        0        0     1942 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/length.py
+-rw-r--r--   0        0        0     2691 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/path.py
+-rw-r--r--   0        0        0     4042 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/saving.py
+-rw-r--r--   0        0        0    12024 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/shuffling.py
+-rw-r--r--   0        0        0     1786 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datapipes/iter/source.py
+-rw-r--r--   0        0        0      759 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/__init__.py
+-rw-r--r--   0        0        0     6217 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/base.py
+-rw-r--r--   0        0        0    13056 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/datapipe.py
+-rw-r--r--   0        0        0     4300 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/dataset.py
+-rw-r--r--   0        0        0     6316 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/imagenet.py
+-rw-r--r--   0        0        0     2552 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/mnist.py
+-rw-r--r--   0        0        0     1798 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/datasources/utils.py
+-rw-r--r--   0        0        0     2163 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/__init__.py
+-rw-r--r--   0        0        0     3257 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/_constants.py
+-rw-r--r--   0        0        0     4217 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/auto.py
+-rw-r--r--   0        0        0     7644 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/comm.py
+-rw-r--r--   0        0        0     6998 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/ddp.py
+-rw-r--r--   0        0        0     5920 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/distributed/utils.py
+-rw-r--r--   0        0        0      305 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/engines/__init__.py
+-rw-r--r--   0        0        0    13386 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/engines/alpha.py
+-rw-r--r--   0        0        0    23121 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/engines/base.py
+-rw-r--r--   0        0        0     1136 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/engines/events.py
+-rw-r--r--   0        0        0      652 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/events/__init__.py
+-rw-r--r--   0        0        0     3539 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/events/conditions.py
+-rw-r--r--   0        0        0     4769 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/events/event_handlers.py
+-rw-r--r--   0        0        0    10871 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/events/manager.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/experimental/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/experimental/batchloader/__init__.py
+-rw-r--r--   0        0        0      282 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/experimental/batchloader/base.py
+-rw-r--r--   0        0        0      977 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/experimental/batchloader/iterable.py
+-rw-r--r--   0        0        0     3529 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/experimental/object_ops.py
+-rw-r--r--   0        0        0     2868 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/__init__.py
+-rw-r--r--   0        0        0      515 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/base.py
+-rw-r--r--   0        0        0     4541 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/cudamem.py
+-rw-r--r--   0        0        0     9686 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/early_stopping.py
+-rw-r--r--   0        0        0     7656 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/engine_loader.py
+-rw-r--r--   0        0        0    10214 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/engine_saver.py
+-rw-r--r--   0        0        0     4580 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/lr_monitor.py
+-rw-r--r--   0        0        0     3293 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/lr_scheduler.py
+-rw-r--r--   0        0        0     4905 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/lr_scheduler_updater.py
+-rw-r--r--   0        0        0     1920 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/model.py
+-rw-r--r--   0        0        0     2203 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/model_architecture.py
+-rw-r--r--   0        0        0     1824 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/model_initializer.py
+-rw-r--r--   0        0        0     2311 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/model_parameter.py
+-rw-r--r--   0        0        0     5292 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/model_state_dict_loader.py
+-rw-r--r--   0        0        0     5765 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/optimizer_monitor.py
+-rw-r--r--   0        0        0     2549 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/optimizer_state.py
+-rw-r--r--   0        0        0     1797 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/sysinfo.py
+-rw-r--r--   0        0        0     4011 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/handlers/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/__init__.py
+-rw-r--r--   0        0        0      689 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/__init__.py
+-rw-r--r--   0        0        0     5581 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/accelerate.py
+-rw-r--r--   0        0        0     3675 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/amp.py
+-rw-r--r--   0        0        0     1361 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/base.py
+-rw-r--r--   0        0        0     6679 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/basic.py
+-rw-r--r--   0        0        0     2292 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/conditions.py
+-rw-r--r--   0        0        0     1345 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/factory.py
+-rw-r--r--   0        0        0      935 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/noop.py
+-rw-r--r--   0        0        0     4448 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/evaluation/vanilla.py
+-rw-r--r--   0        0        0      477 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/__init__.py
+-rw-r--r--   0        0        0     1264 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/base.py
+-rw-r--r--   0        0        0     2119 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/batch_saving.py
+-rw-r--r--   0        0        0     1196 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/factory.py
+-rw-r--r--   0        0        0      660 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/noop.py
+-rw-r--r--   0        0        0     1528 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/observers/sequential.py
+-rw-r--r--   0        0        0      647 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/__init__.py
+-rw-r--r--   0        0        0     7834 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/accelerate.py
+-rw-r--r--   0        0        0     5163 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/amp.py
+-rw-r--r--   0        0        0     1445 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/base.py
+-rw-r--r--   0        0        0     6530 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/basic.py
+-rw-r--r--   0        0        0     1279 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/factory.py
+-rw-r--r--   0        0        0      916 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/noop.py
+-rw-r--r--   0        0        0     6287 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/loops/training/vanilla.py
+-rw-r--r--   0        0        0      567 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/lr_schedulers/__init__.py
+-rw-r--r--   0        0        0     2339 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/lr_schedulers/base.py
+-rw-r--r--   0        0        0     5021 2023-03-27 03:54:22.092780 gravitorch-0.0.9/src/gravitorch/lr_schedulers/creation.py
+-rw-r--r--   0        0        0     1438 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/lr_schedulers/invsqrt.py
+-rw-r--r--   0        0        0      228 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/__init__.py
+-rw-r--r--   0        0        0      910 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/base.py
+-rw-r--r--   0        0        0      460 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/criteria/__init__.py
+-rw-r--r--   0        0        0     3852 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/criteria/packed_seq.py
+-rw-r--r--   0        0        0     6567 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/criteria/padded_seq.py
+-rw-r--r--   0        0        0     3500 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/criteria/vanilla.py
+-rw-r--r--   0        0        0     3435 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/criteria/weighted_sum.py
+-rw-r--r--   0        0        0     1647 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/__init__.py
+-rw-r--r--   0        0        0     2400 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/base.py
+-rw-r--r--   0        0        0     4001 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/base_epoch.py
+-rw-r--r--   0        0        0      540 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/classification/__init__.py
+-rw-r--r--   0        0        0     7618 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/classification/accuracy.py
+-rw-r--r--   0        0        0    10346 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/classification/confusion_matrix.py
+-rw-r--r--   0        0        0     1885 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/classification/cross_entropy.py
+-rw-r--r--   0        0        0      905 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/__init__.py
+-rw-r--r--   0        0        0     2784 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/absolute_error.py
+-rw-r--r--   0        0        0     6399 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/absolute_relative_error.py
+-rw-r--r--   0        0        0     3255 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/log_cosh_error.py
+-rw-r--r--   0        0        0     3867 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/nmse.py
+-rw-r--r--   0        0        0     4255 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/squared_error.py
+-rw-r--r--   0        0        0     8815 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/regression/squared_log_error.py
+-rw-r--r--   0        0        0     3013 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/sequential.py
+-rw-r--r--   0        0        0    19766 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/state.py
+-rw-r--r--   0        0        0     6162 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/transform.py
+-rw-r--r--   0        0        0    11238 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/metrics/vanilla.py
+-rw-r--r--   0        0        0      593 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/networks/__init__.py
+-rw-r--r--   0        0        0     3595 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/networks/image_classification.py
+-rw-r--r--   0        0        0     4786 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/networks/lenet.py
+-rw-r--r--   0        0        0     9848 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/networks/mlp.py
+-rw-r--r--   0        0        0     3903 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/networks/mnist.py
+-rw-r--r--   0        0        0      865 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/utils/__init__.py
+-rw-r--r--   0        0        0     3245 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/utils/architecture.py
+-rw-r--r--   0        0        0     2325 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/utils/setup_and_attach.py
+-rw-r--r--   0        0        0    17803 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/utils/summary.py
+-rw-r--r--   0        0        0     6707 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/utils/testing.py
+-rw-r--r--   0        0        0     7453 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/models/vanilla.py
+-rw-r--r--   0        0        0     3946 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/__init__.py
+-rw-r--r--   0        0        0     2215 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/activations.py
+-rw-r--r--   0        0        0     4217 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/alpha_activations.py
+-rw-r--r--   0        0        0     3748 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/barron_loss.py
+-rw-r--r--   0        0        0     3307 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/clamp.py
+-rw-r--r--   0        0        0      654 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/creators.py
+-rw-r--r--   0        0        0      108 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/experimental/__init__.py
+-rw-r--r--   0        0        0     3015 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/experimental/exponential_nll.py
+-rw-r--r--   0        0        0     2637 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/exu.py
+-rw-r--r--   0        0        0     1990 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/flatten.py
+-rw-r--r--   0        0        0     5583 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/focal_loss.py
+-rw-r--r--   0        0        0    11107 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/fourier_feature.py
+-rw-r--r--   0        0        0      982 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/__init__.py
+-rw-r--r--   0        0        0     4172 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/barron_loss.py
+-rw-r--r--   0        0        0     3113 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/error.py
+-rw-r--r--   0        0        0      123 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/experimental/__init__.py
+-rw-r--r--   0        0        0     2064 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/experimental/exponential_nll.py
+-rw-r--r--   0        0        0     2529 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/loss_helpers.py
+-rw-r--r--   0        0        0    11355 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/functional/robust_loss.py
+-rw-r--r--   0        0        0     8536 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/fusion.py
+-rw-r--r--   0        0        0     1014 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/__init__.py
+-rw-r--r--   0        0        0      731 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/base.py
+-rw-r--r--   0        0        0     7758 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/const.py
+-rw-r--r--   0        0        0     1117 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/factory.py
+-rw-r--r--   0        0        0     7980 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/kaiming.py
+-rw-r--r--   0        0        0      586 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/noop.py
+-rw-r--r--   0        0        0     4654 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/normal.py
+-rw-r--r--   0        0        0     1304 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/sequential.py
+-rw-r--r--   0        0        0     5136 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/init/xavier.py
+-rw-r--r--   0        0        0      994 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/residual.py
+-rw-r--r--   0        0        0     8779 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/robust_loss.py
+-rw-r--r--   0        0        0    19758 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/scalar_encoding.py
+-rw-r--r--   0        0        0     8184 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/shift_scale.py
+-rw-r--r--   0        0        0    11498 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/transforms.py
+-rw-r--r--   0        0        0     1763 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/__init__.py
+-rw-r--r--   0        0        0     1270 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/factory.py
+-rw-r--r--   0        0        0    13588 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/module_helpers.py
+-rw-r--r--   0        0        0     4833 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/parameter.py
+-rw-r--r--   0        0        0    10744 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/state_dict.py
+-rw-r--r--   0        0        0     5830 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/summary.py
+-rw-r--r--   0        0        0     6847 2023-03-27 03:54:22.096780 gravitorch-0.0.9/src/gravitorch/nn/utils/testing.py
+-rw-r--r--   0        0        0     3852 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/nn/warmup_seq_loss.py
+-rw-r--r--   0        0        0      247 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/optimizers/__init__.py
+-rw-r--r--   0        0        0     2733 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/optimizers/factory.py
+-rw-r--r--   0        0        0      878 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/optimizers/noop.py
+-rw-r--r--   0        0        0     3574 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/optimizers/utils.py
+-rw-r--r--   0        0        0      702 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/__init__.py
+-rw-r--r--   0        0        0     1056 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/base.py
+-rw-r--r--   0        0        0     1846 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/distributed.py
+-rw-r--r--   0        0        0     2700 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/logging.py
+-rw-r--r--   0        0        0    17326 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/pytorch.py
+-rw-r--r--   0        0        0     1308 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/rsrc/sysinfo.py
+-rw-r--r--   0        0        0      517 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/__init__.py
+-rw-r--r--   0        0        0      403 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/base.py
+-rw-r--r--   0        0        0     4873 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/evaluation.py
+-rw-r--r--   0        0        0     1528 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/no_repeat.py
+-rw-r--r--   0        0        0     1459 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/resource.py
+-rw-r--r--   0        0        0     5002 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/training.py
+-rw-r--r--   0        0        0     2832 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/runners/utils.py
+-rw-r--r--   0        0        0      891 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/testing/__init__.py
+-rw-r--r--   0        0        0     1934 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/testing/_pytest.py
+-rw-r--r--   0        0        0     6927 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/testing/dummy.py
+-rw-r--r--   0        0        0      348 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/__init__.py
+-rw-r--r--   0        0        0      395 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/__init__.py
+-rw-r--r--   0        0        0      480 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/base.py
+-rw-r--r--   0        0        0      818 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/jsona.py
+-rw-r--r--   0        0        0     1125 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/picklea.py
+-rw-r--r--   0        0        0      840 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/pytorcha.py
+-rw-r--r--   0        0        0      757 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/artifacts/text.py
+-rw-r--r--   0        0        0     7435 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/asset.py
+-rw-r--r--   0        0        0     6050 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/cudamem.py
+-rw-r--r--   0        0        0     1296 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/__init__.py
+-rw-r--r--   0        0        0     1240 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/base.py
+-rw-r--r--   0        0        0     7881 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/continuous.py
+-rw-r--r--   0        0        0     2609 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/discrete.py
+-rw-r--r--   0        0        0     4280 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/float_tensor.py
+-rw-r--r--   0        0        0     1853 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/float_value.py
+-rw-r--r--   0        0        0      819 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/integer.py
+-rw-r--r--   0        0        0     2314 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/long_tensor.py
+-rw-r--r--   0        0        0      677 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/noop.py
+-rw-r--r--   0        0        0     2536 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/sequence.py
+-rw-r--r--   0        0        0     1279 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/data_summary/utils.py
+-rw-r--r--   0        0        0     2483 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device.py
+-rw-r--r--   0        0        0      679 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/__init__.py
+-rw-r--r--   0        0        0      469 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/auto.py
+-rw-r--r--   0        0        0      710 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/base.py
+-rw-r--r--   0        0        0     1890 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/manual.py
+-rw-r--r--   0        0        0      759 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/noop.py
+-rw-r--r--   0        0        0     1326 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/device_placement/utils.py
+-rw-r--r--   0        0        0      349 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/engine_states/__init__.py
+-rw-r--r--   0        0        0    13888 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/engine_states/base.py
+-rw-r--r--   0        0        0     1178 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/engine_states/utils.py
+-rw-r--r--   0        0        0     3696 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/engine_states/vanilla.py
+-rw-r--r--   0        0        0      818 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/__init__.py
+-rw-r--r--   0        0        0    32543 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/base.py
+-rw-r--r--   0        0        0     6659 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/noop.py
+-rw-r--r--   0        0        0      897 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/steps.py
+-rw-r--r--   0        0        0    11680 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/tensorboard.py
+-rw-r--r--   0        0        0     2306 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/utils.py
+-rw-r--r--   0        0        0      873 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/factory.py
+-rw-r--r--   0        0        0    16295 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/format.py
+-rw-r--r--   0        0        0      764 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/__init__.py
+-rw-r--r--   0        0        0    15554 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/base.py
+-rw-r--r--   0        0        0     7197 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/comparable.py
+-rw-r--r--   0        0        0     4707 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/comparator.py
+-rw-r--r--   0        0        0     3039 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/generic.py
+-rw-r--r--   0        0        0     7748 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/manager.py
+-rw-r--r--   0        0        0     4510 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/history/utils.py
+-rw-r--r--   0        0        0     1301 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/info.py
+-rw-r--r--   0        0        0     5568 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/integrations.py
+-rw-r--r--   0        0        0     9824 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/io.py
+-rw-r--r--   0        0        0     1078 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/logging.py
+-rw-r--r--   0        0        0     3265 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/mapping.py
+-rw-r--r--   0        0        0      801 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/__init__.py
+-rw-r--r--   0        0        0     6295 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/average.py
+-rw-r--r--   0        0        0    44596 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/confusion_matrix.py
+-rw-r--r--   0        0        0      179 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/exceptions.py
+-rw-r--r--   0        0        0     6744 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/moving_average.py
+-rw-r--r--   0        0        0    11018 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/scalar.py
+-rw-r--r--   0        0        0    30892 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/meters/tensor.py
+-rw-r--r--   0        0        0     3492 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/metric_tracker.py
+-rw-r--r--   0        0        0     7302 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/module_manager.py
+-rw-r--r--   0        0        0     1689 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/parameter.py
+-rw-r--r--   0        0        0     6888 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/partitioning.py
+-rw-r--r--   0        0        0     5511 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/path.py
+-rw-r--r--   0        0        0      386 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/profilers/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/profilers/base.py
+-rw-r--r--   0        0        0      880 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/profilers/noop.py
+-rw-r--r--   0        0        0     4497 2023-03-27 03:54:22.100780 gravitorch-0.0.9/src/gravitorch/utils/profilers/pytorch.py
+-rw-r--r--   0        0        0     1079 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/profilers/utils.py
+-rw-r--r--   0        0        0    10720 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/seed.py
+-rw-r--r--   0        0        0      572 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/sequence.py
+-rw-r--r--   0        0        0     5719 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/summary.py
+-rw-r--r--   0        0        0     2965 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/sysinfo.py
+-rw-r--r--   0        0        0     1046 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/tensor/__init__.py
+-rw-r--r--   0        0        0     5820 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/tensor/flatted.py
+-rw-r--r--   0        0        0     4377 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/tensor/math_ops.py
+-rw-r--r--   0        0        0     8515 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/tensor/misc.py
+-rw-r--r--   0        0        0     9170 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/tensor/recursive_ops.py
+-rw-r--r--   0        0        0     9335 2023-03-27 03:54:22.104780 gravitorch-0.0.9/src/gravitorch/utils/timing.py
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 gravitorch-0.0.9/PKG-INFO
```

### Comparing `gravitorch-0.0.8/LICENSE` & `gravitorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/README.md` & `gravitorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/pyproject.toml` & `gravitorch-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gravitorch"
-version = "0.0.8"
+version = "0.0.9"
 description = "Warning: API is not stable"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 #homepage = "https://github.com/durandtibo/gravitorch"
 #repository = "https://github.com/durandtibo/gravitorch"
 keywords = ["gravitorch"]
 
@@ -30,33 +30,35 @@
 hydra-core = "^1.3"
 numpy = "^1.24"
 objectory = "^0.0"
 psutil = "^5.9"
 python = "^3.9"
 pytorch-ignite = "^0.4"
 tabulate = "^0.9"
-torch = "^1.13"
+torch = "^2.0"
 tqdm = "^4.64"
 
 # Optional dependencies
-accelerate = { version = "^0.17", optional = true }
+accelerate = { version = "^0.18", optional = true }
 colorlog = { version = "^6.7", optional = true }
 matplotlib = { version = "^3.7", optional = true }
 pillow = { version = "^9.3", optional = true }
 tensorboard = { version = "^2.11", optional = true }
-torchvision = { version = "^0.14", optional = true }
+torchdata = { version = "^0.6", optional = true }
+torchvision = { version = "^0.15", optional = true }
 
 [tool.poetry.extras]
 all = [
     "accelerate",
     "colorlog",
     "matplotlib",
     "pillow",
     "tensorboard",
     "torch-tb-profiler",
+    "torchdata",
     "torchvision",
 ]
 tb = ["tensorboard", "torch-tb-profiler"]
 vision = ["pillow", "torchvision"]
 
 [tool.poetry.group.exp]
 optional = true
@@ -70,15 +72,15 @@
 codecov = "^2.1"
 coverage = { extras = ["toml"], version = "^6.5" }
 pre-commit = "^2.20"
 pylint = "^2.15"
 pytest = "^7.2"
 pytest-cov = "^4.0"
 pytest-timeout = "^2.1"
-ruff = "^0.0"
+ruff = "^0.0.257"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
@@ -100,14 +102,15 @@
 log_level = "DEBUG"
 addopts = "--color yes --durations 10 -rf"
 # Configuration of the short test summary info https://docs.pytest.org/en/stable/usage.html#detailed-summary-report
 filterwarnings = [
     'ignore::DeprecationWarning:tensorboard.*',
     'ignore::DeprecationWarning:torch.utils.tensorboard.*',
 ]
+timeout_func_only = false
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310"]
 include = '\.pyi?$'
 
 [tool.pylint.FORMAT]
```

### Comparing `gravitorch-0.0.8/src/gravitorch/cli/run.py` & `gravitorch-0.0.9/src/gravitorch/cli/run.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/constants.py` & `gravitorch-0.0.9/src/gravitorch/constants.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/core/advanced.py` & `gravitorch-0.0.9/src/gravitorch/creators/core/advanced.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/core/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/core/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/core/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/creators/core/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/dataloader/__init__.py` & `gravitorch-0.0.9/src/gravitorch/creators/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/dataloader/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/dataloader/pytorch.py` & `gravitorch-0.0.9/src/gravitorch/creators/dataloader/pytorch.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/dataloader/utils.py` & `gravitorch-0.0.9/src/gravitorch/creators/dataloader/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datapipe/__init__.py` & `gravitorch-0.0.9/src/gravitorch/creators/datapipe/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datapipe/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/datapipe/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,28 +96,28 @@
         >>> from gravitorch.creators.datapipe import setup_iter_datapipe_creator
         # Set up an ``IterDataPipe`` creator from an ``IterDataPipe`` creator i.e. do nothing ;)
         >>> from gravitorch.creators.datapipe import SequentialIterDataPipeCreator
         >>> creator = setup_iter_datapipe_creator(
         ...     SequentialIterDataPipeCreator(
         ...         config=[
         ...             {
-        ...                 OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapperIterDataPipe",
+        ...                 OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapperIterDataPipe",
         ...                 "data": [1, 2, 3, 4],
         ...             }
         ...         ],
         ...     )
         ... )
         # Set up an ``IterDataPipe`` creator from its config
         >>> from objectory import OBJECT_TARGET
         >>> creator = setup_iter_datapipe_creator(
         ...     {
         ...         OBJECT_TARGET: "gravitorch.creators.datapipe.SequentialIterDataPipeCreator",
         ...         "config": [
         ...             {
-        ...                 OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapperIterDataPipe",
+        ...                 OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapperIterDataPipe",
         ...                 "data": [1, 2, 3, 4],
         ...             }
         ...         ],
         ...     }
         ... )
     """
     if isinstance(creator, dict):
```

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datapipe/random.py` & `gravitorch-0.0.9/src/gravitorch/creators/datapipe/random.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datapipe/sequential.py` & `gravitorch-0.0.9/src/gravitorch/creators/datapipe/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,46 +74,46 @@
 
             >>> from torch.utils.data import IterDataPipe
             >>> from objectory import OBJECT_TARGET
             >>> from gravitorch.creators.datapipe import SequentialIterDataPipeCreator
             # Create an IterDataPipe object using a single IterDataPipe object and no source input
             >>> creator = SequentialIterDataPipeCreator(
             ...     {
-            ...         OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+            ...         OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
             ...         "data": [1, 2, 3, 4],
             ...     }
             ... )
             >>> datapipe: IterDataPipe = creator.create()
             >>> tuple(datapipe)
             (1, 2, 3, 4)
             # Equivalent to
             >>> creator = SequentialIterDataPipeCreator(
             ...     [
             ...         {
-            ...             OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+            ...             OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
             ...             "data": [1, 2, 3, 4],
             ...         },
             ...     ]
             ... )
             >>> datapipe: IterDataPipe = creator.create()
             >>> tuple(datapipe)
             (1, 2, 3, 4)
             # It is possible to use the source_inputs to create the same IterDataPipe object.
             # The data is given by the source_inputs
             >>> creator = SequentialIterDataPipeCreator(
-            ...     config={OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper"},
+            ...     config={OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper"},
             ... )
             >>> datapipe: IterDataPipe = creator.create(source_inputs=([1, 2, 3, 4],))
             >>> tuple(datapipe)
             (1, 2, 3, 4)
             # Create an IterDataPipe object using two IterDataPipe objects and no source input
             >>> creator = SequentialIterDataPipeCreator(
             ...     [
             ...         {
-            ...             OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+            ...             OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
             ...             "data": [1, 2, 3, 4],
             ...         },
             ...         {
             ...             OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher",
             ...             "batch_size": 2,
             ...         },
             ...     ]
@@ -127,15 +127,15 @@
             ...     config=[
             ...         {
             ...             OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher",
             ...             "batch_size": 2,
             ...         },
             ...     ],
             ... )
-            >>> from gravitorch.data.datapipes.iter import SourceWrapper
+            >>> from gravitorch.datapipes.iter import SourceWrapper
             >>> datapipe: IterDataPipe = creator.create(
             ...     source_inputs=[SourceWrapper(data=[1, 2, 3, 4])]
             ... )
             >>> tuple(datapipe)
             ([1, 2], [3, 4])
             # It is possible to create a sequential ``IterDataPipe`` object that takes several
             # IterDataPipe objects as input.
@@ -225,54 +225,54 @@
 
         >>> from torch.utils.data import IterDataPipe
         >>> from objectory import OBJECT_TARGET
         >>> from gravitorch.creators.datapipe.sequential import create_sequential_iter_datapipe
         # Create an IterDataPipe object using a single IterDataPipe object and no source input
         >>> datapipe: IterDataPipe = create_sequential_iter_datapipe(
         ...     {
-        ...         OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...         OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
         ...         "data": [1, 2, 3, 4],
         ...     }
         ... )
         >>> tuple(datapipe)
         (1, 2, 3, 4)
         # Equivalent to
         >>> datapipe: IterDataPipe = create_sequential_iter_datapipe(
         ...     [
         ...         {
-        ...             OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...     ]
         ... )
         >>> tuple(datapipe)
         (1, 2, 3, 4)
         # It is possible to use the source_inputs to create the same IterDataPipe object.
         # The data is given by the source_inputs
         >>> datapipe: IterDataPipe = create_sequential_iter_datapipe(
-        ...     config={OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper"},
+        ...     config={OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper"},
         ...     source_inputs=([1, 2, 3, 4],),
         ... )
         >>> tuple(datapipe)
         (1, 2, 3, 4)
         # Create an IterDataPipe object using two IterDataPipe objects and no source input
         >>> datapipe: IterDataPipe = create_sequential_iter_datapipe(
         ...     [
         ...         {
-        ...             OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...         {OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher", "batch_size": 2},
         ...     ]
         ... )
         >>> tuple(datapipe)
         ([1, 2], [3, 4])
         # It is possible to use the source_inputs to create the same IterDataPipe object.
         # A source IterDataPipe object is specified by using source_inputs
-        >>> from gravitorch.data.datapipes.iter import SourceWrapper
+        >>> from gravitorch.datapipes.iter import SourceWrapper
         >>> datapipe: IterDataPipe = create_sequential_iter_datapipe(
         ...     config=[
         ...         {OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher", "batch_size": 2},
         ...     ],
         ...     source_inputs=[SourceWrapper(data=[1, 2, 3, 4])],
         ... )
         >>> tuple(datapipe)
@@ -366,55 +366,55 @@
             ...     SequentialIterDataPipeCreator,
             ... )
             # Create an IterDataPipe object using a single IterDataPipe creator and no source input
             >>> creator = SequentialCreatorIterDataPipeCreator(
             ...     [
             ...         SequentialIterDataPipeCreator(
             ...             {
-            ...                 OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+            ...                 OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
             ...                 "data": [1, 2, 3, 4],
             ...             },
             ...         ),
             ...     ]
             ... )
             >>> datapipe: IterDataPipe = creator.create()
             >>> tuple(datapipe)
             (1, 2, 3, 4)
             # It is possible to use the source_inputs to create the same IterDataPipe object.
             # The data is given by the source_inputs
             >>> creator = SequentialCreatorIterDataPipeCreator(
             ...     [
             ...         SequentialIterDataPipeCreator(
-            ...             {OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper"},
+            ...             {OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper"},
             ...         ),
             ...     ]
             ... )
             >>> datapipe: IterDataPipe = creator.create(source_inputs=([1, 2, 3, 4],))
             >>> tuple(datapipe)
             (1, 2, 3, 4)
             # Create an IterDataPipe object using two IterDataPipe creators and no source input
             >>> creator = SequentialCreatorIterDataPipeCreator(
             ...     [
             ...         SequentialIterDataPipeCreator(
-            ...             {OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper"},
+            ...             {OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper"},
             ...         ),
             ...         SequentialIterDataPipeCreator(
             ...             {
             ...                 OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher",
             ...                 "batch_size": 2,
             ...             },
             ...         ),
             ...     ]
             ... )
             >>> datapipe: IterDataPipe = creator.create()
             >>> tuple(datapipe)
             ([1, 2], [3, 4])
             # It is possible to use the source_inputs to create the same IterDataPipe object.
             # A source IterDataPipe object is specified by using source_inputs
-            >>> from gravitorch.data.datapipes.iter import SourceWrapper
+            >>> from gravitorch.datapipes.iter import SourceWrapper
             >>> creator = SequentialCreatorIterDataPipeCreator(
             ...     creators=[
             ...         SequentialIterDataPipeCreator(
             ...             {
             ...                 OBJECT_TARGET: "torch.utils.data.datapipes.iter.Batcher",
             ...                 "batch_size": 2,
             ...             },
```

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datasource/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/datasource/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/datasource/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/creators/datasource/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/utils.py` & `gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/lr_scheduler/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/creators/lr_scheduler/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/model/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/model/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/model/ddp.py` & `gravitorch-0.0.9/src/gravitorch/creators/model/ddp.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/model/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/creators/model/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/__init__.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/base.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/noo.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/noo.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/utils.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/creators/optimizer/zero.py` & `gravitorch-0.0.9/src/gravitorch/creators/optimizer/zero.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datacreators/base.py` & `gravitorch-0.0.9/src/gravitorch/data/datacreators/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datacreators/caching.py` & `gravitorch-0.0.9/src/gravitorch/data/datacreators/caching.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datacreators/hypercube_vertex.py` & `gravitorch-0.0.9/src/gravitorch/data/datacreators/hypercube_vertex.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/__init__.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/base.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/packed_sequence.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/packed_sequence.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/padded_sequence.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/padded_sequence.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/collators/utils.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/collators/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/dataloaders/samplers.py` & `gravitorch-0.0.9/src/gravitorch/data/dataloaders/samplers.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/__init__.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,26 @@
     "PyTorchSaver",
     "SourceWrapper",
     "TensorDictShuffler",
     "TupleBatcher",
     "setup_iter_datapipe",
 ]
 
-from gravitorch.data.datapipes.iter.batching import (
-    DictBatcherIterDataPipe as DictBatcher,
-)
-from gravitorch.data.datapipes.iter.batching import (
-    TupleBatcherIterDataPipe as TupleBatcher,
-)
-from gravitorch.data.datapipes.iter.dictionary import (
+from gravitorch.datapipes.iter.batching import DictBatcherIterDataPipe as DictBatcher
+from gravitorch.datapipes.iter.batching import TupleBatcherIterDataPipe as TupleBatcher
+from gravitorch.datapipes.iter.dictionary import (
     DictOfListConverterIterDataPipe as DictOfListConverter,
 )
-from gravitorch.data.datapipes.iter.dictionary import (
+from gravitorch.datapipes.iter.dictionary import (
     ListOfDictConverterIterDataPipe as ListOfDictConverter,
 )
-from gravitorch.data.datapipes.iter.factory import setup_iter_datapipe
-from gravitorch.data.datapipes.iter.length import LooperIterDataPipe as Looper
-from gravitorch.data.datapipes.iter.path import DirFilterIterDataPipe as DirFilter
-from gravitorch.data.datapipes.iter.path import FileFilterIterDataPipe as FileFilter
-from gravitorch.data.datapipes.iter.path import PathListerIterDataPipe as PathLister
-from gravitorch.data.datapipes.iter.saving import PickleSaverIterDataPipe as PickleSaver
-from gravitorch.data.datapipes.iter.saving import (
-    PyTorchSaverIterDataPipe as PyTorchSaver,
-)
-from gravitorch.data.datapipes.iter.shuffling import (
+from gravitorch.datapipes.iter.factory import setup_iter_datapipe
+from gravitorch.datapipes.iter.length import LooperIterDataPipe as Looper
+from gravitorch.datapipes.iter.path import DirFilterIterDataPipe as DirFilter
+from gravitorch.datapipes.iter.path import FileFilterIterDataPipe as FileFilter
+from gravitorch.datapipes.iter.path import PathListerIterDataPipe as PathLister
+from gravitorch.datapipes.iter.saving import PickleSaverIterDataPipe as PickleSaver
+from gravitorch.datapipes.iter.saving import PyTorchSaverIterDataPipe as PyTorchSaver
+from gravitorch.datapipes.iter.shuffling import (
     TensorDictShufflerIterDataPipe as TensorDictShuffler,
 )
-from gravitorch.data.datapipes.iter.source import (
-    SourceWrapperIterDataPipe as SourceWrapper,
-)
+from gravitorch.datapipes.iter.source import SourceWrapperIterDataPipe as SourceWrapper
```

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/batching.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/batching.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 from collections.abc import Hashable, Iterator, Sequence
 from typing import Union
 
 import torch
 from torch import Tensor
 from torch.utils.data import IterDataPipe
 
-from gravitorch.data.datapipes.iter.shuffling import (
-    shuffle_tensor_mapping,
-    shuffle_tensors,
-)
-from gravitorch.data.datapipes.iter.source import SourceWrapperIterDataPipe
+from gravitorch.datapipes.iter.shuffling import shuffle_tensor_mapping, shuffle_tensors
+from gravitorch.datapipes.iter.source import SourceWrapperIterDataPipe
 from gravitorch.utils.format import str_indent
 from gravitorch.utils.mapping import get_first_value
 from gravitorch.utils.seed import get_torch_generator
 from gravitorch.utils.summary import concise_summary
 
 logger = logging.getLogger(__name__)
```

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/dictionary.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/dictionary.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/factory.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
         ValueError if the ``IterDataPipe`` configuration sequence is
             empty.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter.factory import create_sequential_iter_datapipe
+        >>> from gravitorch.datapipes.iter.factory import create_sequential_iter_datapipe
         >>> datapipe = create_sequential_iter_datapipe(
         ...     [
         ...         {
-        ...             '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...     ],
         ... )
         >>> tuple(datapipe)
         (1, 2, 3, 4)
         >>> datapipe = create_sequential_iter_datapipe(
         ...     [
         ...         {
-        ...             '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...         {'_target_': "torch.utils.data.datapipes.iter.Batcher", "batch_size": 2},
         ...     ]
         ... )
         >>> tuple(datapipe)
         ([1, 2], [3, 4])
@@ -84,29 +84,29 @@
         ``IterDataPipe``: The last ``IterDataPipe`` of the sequence
             (a.k.a. sink).
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter import setup_iter_datapipe
+        >>> from gravitorch.datapipes.iter import setup_iter_datapipe
         >>> datapipe = setup_iter_datapipe(
         ...     [
         ...         {
-        ...             '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...     ],
         ... )
         >>> tuple(datapipe)
         (1, 2, 3, 4)
         >>> datapipe = setup_iter_datapipe(
         ...     [
         ...         {
-        ...             '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...             '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...             "data": [1, 2, 3, 4],
         ...         },
         ...         {'_target_': "torch.utils.data.datapipes.iter.Batcher", "batch_size": 2},
         ...     ]
         ... )
         >>> tuple(datapipe)
         ([1, 2], [3, 4])
```

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/length.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/length.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             the source iterable DataPipe.
         length (int): Specifies the length of the DataPipe.
 
      Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter import Looper, SourceWrapper
+        >>> from gravitorch.datapipes.iter import Looper, SourceWrapper
         >>> dp = Looper(SourceWrapper([1, 2, 3, 4]), length=10)
         >>> list(dp)
         [1, 2, 3, 4, 1, 2, 3, 4, 1, 2]
         >>> dp = Looper(SourceWrapper([1, 2, 3, 4, 5, 6]), length=4)
         >>> list(dp)
         [1, 2, 3, 4]
     """
```

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/path.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/path.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/saving.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/saving.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/shuffling.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/shuffling.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             Default: ``3510637111256283951``
 
     Example usage:
 
     .. code-block:: python
 
         >>> from torch.utils.data import IterDataPipe
-        >>> from gravitorch.data.datapipes.iter import TensorDictShuffler
+        >>> from gravitorch.datapipes.iter import TensorDictShuffler
         >>> class MyIterDataPipe(IterDataPipe[dict]):
         ...     def __iter__(self) -> Iterator[dict]:
         ...         for i in range(3):
         ...             yield {"key": torch.arange(4) + i}
         ...
         >>> list(TensorDictShuffler(MyIterDataPipe()))
         [{'key': tensor([2, 3, 0, 1])},
@@ -135,15 +135,15 @@
         ValueError if the tensors do not have the same shape for the
             common dimension.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter.shuffling import shuffle_tensors
+        >>> from gravitorch.datapipes.iter.shuffling import shuffle_tensors
         >>> shuffle_tensors([torch.arange(4), torch.arange(20).view(4, 5)])
         [
             torch.tensor([0, 2, 1, 3]),
             torch.tensor([[0, 1, 2, 3, 4],
                           [10, 11, 12, 13, 14],
                           [5, 6, 7, 8, 9],
                           [15, 16, 17, 18, 19]]),
@@ -206,15 +206,15 @@
         ValueError if the tensors do not have the same shape for the
             common dimension.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter.shuffling import shuffle_tensor_mapping
+        >>> from gravitorch.datapipes.iter.shuffling import shuffle_tensor_mapping
         # Shuffle all the tensors on dimension 0 (default)
         >>> shuffle_tensor_mapping({"key1": torch.arange(4), "key2": torch.arange(20).view(4, 5)})
         {
             "key1": tensor([0, 2, 1, 3]),
             "key2": tensor([[0, 1, 2, 3, 4],
                             [10, 11, 12, 13, 14],
                             [5, 6, 7, 8, 9],
@@ -302,15 +302,15 @@
     ------
         TypeError: if the input type is not supported.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.data.datapipes.iter.shuffling import get_first_dimension
+        >>> from gravitorch.datapipes.iter.shuffling import get_first_dimension
         # torch tensor
         >>> import torch
         >>> get_first_dimension(torch.ones(5, 4))
         5
         # NumPy ndarray
         >>> import numpy
         >>> get_first_dimension(numpy.ones((7, 4)))
```

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datapipes/iter/source.py` & `gravitorch-0.0.9/src/gravitorch/datapipes/iter/source.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/__init__.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/demo_map_style.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/demo_map_style.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/factory.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/image_folder.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/image_folder.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/in_memory.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/in_memory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/mnist.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/datasets/utils.py` & `gravitorch-0.0.9/src/gravitorch/data/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/__init__.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/base.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/distributed.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/distributed.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/even.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/even.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/fixed_size.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/fixed_size.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/sequential.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/sequential.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/shuffling.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/shuffling.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/data/partitioners/trivial.py` & `gravitorch-0.0.9/src/gravitorch/data/partitioners/trivial.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/__init__.py` & `gravitorch-0.0.9/src/gravitorch/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/base.py` & `gravitorch-0.0.9/src/gravitorch/datasources/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/datapipe.py` & `gravitorch-0.0.9/src/gravitorch/datasources/datapipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,53 +39,53 @@
     Example:
     -------
     .. code-block:: python
 
         >>> from gravitorch.datasources import IterDataPipeCreatorDataSource
         # Create by using a ``BaseIterDataPipeCreator`` object.
         >>> from gravitorch.creators.datapipe import SequentialIterDataPipeCreator
-        >>> from gravitorch.data.datapipes.iter import SourceWrapper
+        >>> from gravitorch.datapipes.iter import SourceWrapper
         >>> data_source = IterDataPipeCreatorDataSource(
         ...     datapipe_creators={
         ...         "train": SequentialIterDataPipeCreator(
         ...             config=[
         ...                 {
-        ...                     '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...                     '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...                     "data": [1, 2, 3, 4],
         ...                 },
         ...             ]
         ...         ),
         ...         "val": SequentialIterDataPipeCreator(
         ...             config=[
         ...                 {
-        ...                     '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...                     '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...                     "data": ["a", "b", "c"],
         ...                 },
         ...             ]
         ...         ),
         ...     }
         ... )
         # Create by using the configs
         >>> from objectory import OBJECT_TARGET
         >>> data_source = IterDataPipeCreatorDataSource(
         ...     datapipe_creators={
         ...         "train": {
         ...             '_target_': "gravitorch.creators.datapipe.SequentialIterDataPipeCreator",
         ...             "config": [
         ...                 {
-        ...                     OBJECT_TARGET: "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...                     OBJECT_TARGET: "gravitorch.datapipes.iter.SourceWrapper",
         ...                    "data": [1, 2, 3, 4],
         ...                },
         ...             ],
         ...         },
         ...         "val": {
         ...             '_target_': "gravitorch.creators.datapipe.SequentialIterDataPipeCreator",
         ...             "config": [
         ...                 {
-        ...                     '_target_': "gravitorch.data.datapipes.iter.SourceWrapper",
+        ...                     '_target_': "gravitorch.datapipes.iter.SourceWrapper",
         ...                     "data": ["a", "b", "c"],
         ...                 },
         ...             ],
         ...         },
         ...     }
         ... )
         # Note that both examples lead to the same result.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/dataset.py` & `gravitorch-0.0.9/src/gravitorch/datasources/dataset.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/imagenet.py` & `gravitorch-0.0.9/src/gravitorch/datasources/imagenet.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/mnist.py` & `gravitorch-0.0.9/src/gravitorch/datasources/mnist.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/datasources/utils.py` & `gravitorch-0.0.9/src/gravitorch/datasources/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/__init__.py` & `gravitorch-0.0.9/src/gravitorch/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/_constants.py` & `gravitorch-0.0.9/src/gravitorch/distributed/_constants.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/auto.py` & `gravitorch-0.0.9/src/gravitorch/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/comm.py` & `gravitorch-0.0.9/src/gravitorch/distributed/comm.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 get_rank = utils.get_rank
 get_world_size = utils.get_world_size
 hostname = utils.hostname
 initialize = utils.initialize
 model_name = utils.model_name
 set_local_rank = utils.set_local_rank
 show_config = utils.show_config
+spawn = utils.spawn
 
 
 class UnknownBackendError(Exception):
     r"""This exception is raised when you try to use an unknown backend."""
 
 
 def is_main_process() -> bool:
```

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/ddp.py` & `gravitorch-0.0.9/src/gravitorch/distributed/ddp.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/distributed/utils.py` & `gravitorch-0.0.9/src/gravitorch/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/engines/alpha.py` & `gravitorch-0.0.9/src/gravitorch/engines/alpha.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from torch.optim import Optimizer
 
 from gravitorch import constants as ct
 from gravitorch.creators.core.base import BaseCoreCreator, setup_core_creator
 from gravitorch.distributed import comm as dist
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import BaseEventHandler, EventManager
 from gravitorch.loops.evaluation import BaseEvaluationLoop, setup_evaluation_loop
 from gravitorch.loops.training import BaseTrainingLoop, setup_training_loop
 from gravitorch.lr_schedulers import LRSchedulerType
 from gravitorch.utils.artifacts import BaseArtifact
 from gravitorch.utils.engine_states import BaseEngineState, setup_engine_state
-from gravitorch.utils.events import BaseEventHandler, EventManager
 from gravitorch.utils.exp_trackers import BaseExpTracker, Step, setup_exp_tracker
 from gravitorch.utils.format import str_indent
 from gravitorch.utils.history import BaseHistory
 from gravitorch.utils.timing import timeblock
 
 if TYPE_CHECKING:
     from gravitorch.datasources import BaseDataSource
```

### Comparing `gravitorch-0.0.8/src/gravitorch/engines/base.py` & `gravitorch-0.0.9/src/gravitorch/engines/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any
 
 from objectory import AbstractFactory
 from torch.nn import Module
 from torch.optim import Optimizer
 
+from gravitorch.events import BaseEventHandler
 from gravitorch.lr_schedulers import LRSchedulerType
 from gravitorch.utils.artifacts import BaseArtifact
-from gravitorch.utils.events import BaseEventHandler
 from gravitorch.utils.exp_trackers.steps import Step
 from gravitorch.utils.history import BaseHistory
 
 if TYPE_CHECKING:
     from gravitorch.datasources import BaseDataSource
 
 
@@ -104,15 +104,15 @@
                 handler to attach to the event.
 
         Example usage:
 
         .. code-block:: python
 
             >>> from gravitorch.engines import BaseEngine
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> engine: BaseEngine = ...  # Create an engine
             >>> def hello_handler():
             ...     print('Hello!')
             >>> engine.add_event_handler('my_event', VanillaEventHandler(hello_handler))
         """
 
     @abstractmethod
@@ -214,15 +214,15 @@
             event (str): Specifies the event to fire.
 
         Example usage:
 
         .. code-block:: python
 
             >>> from gravitorch.engines import BaseEngine
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> engine: BaseEngine = ...  # Create an engine
             >>> engine.fire_event('my_event')  # should do nothing because there is no event handler
             >>> def hello_handler():
             ...     print("Hello!")
             >>> engine.add_event_handler('my_event', VanillaEventHandler(hello_handler))
             >>> engine.fire_event('my_event')
             Hello!
@@ -322,15 +322,15 @@
                 Default: ``None``
 
         Example usage:
 
         .. code-block:: python
 
             >>> from gravitorch.engines import BaseEngine
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> engine: BaseEngine = ...  # Create an engine
             # Define a handler
             >>> def hello_handler():
             ...     print("Hello!")
             >>> engine.has_event_handler(VanillaEventHandler(hello_handler))
             False
             >>> engine.has_event_handler(VanillaEventHandler(hello_handler), 'my_event')
@@ -605,15 +605,15 @@
                 is not attached to the event.
 
         Example usage:
 
         .. code-block:: python
 
             >>> from gravitorch.engines import BaseEngine
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> engine: BaseEngine = ...  # Create an engine
             >>> def hello_handler():
             ...     print('Hello!')
             >>> engine.add_event_handler('my_event', VanillaEventHandler(hello_handler))
             >>> engine.has_event_handler(VanillaEventHandler(hello_handler), 'my_event')
             True
             >>> engine.remove_event_handler('my_event', VanillaEventHandler(hello_handler))
```

### Comparing `gravitorch-0.0.8/src/gravitorch/engines/events.py` & `gravitorch-0.0.9/src/gravitorch/engines/events.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/experimental/object_ops.py` & `gravitorch-0.0.9/src/gravitorch/experimental/object_ops.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/__init__.py` & `gravitorch-0.0.9/src/gravitorch/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/base.py` & `gravitorch-0.0.9/src/gravitorch/handlers/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/cudamem.py` & `gravitorch-0.0.9/src/gravitorch/handlers/cudamem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __all__ = ["EpochCudaMemoryMonitor", "IterationCudaMemoryMonitor"]
 
 import torch
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
-from gravitorch.handlers.base import BaseHandler
-from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.cudamem import log_max_cuda_memory_allocated
-from gravitorch.utils.events import (
+from gravitorch.events import (
     ConditionalEventHandler,
     EpochPeriodicCondition,
     IterationPeriodicCondition,
 )
+from gravitorch.handlers.base import BaseHandler
+from gravitorch.handlers.utils import add_unique_event_handler
+from gravitorch.utils.cudamem import log_max_cuda_memory_allocated
 from gravitorch.utils.exp_trackers import EpochStep, IterationStep
 
 
 class EpochCudaMemoryMonitor(BaseHandler):
     r"""Implements a handler to monitor the CUDA memory usage every ``freq``
     epochs.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/early_stopping.py` & `gravitorch-0.0.9/src/gravitorch/handlers/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 import operator
 from collections.abc import Callable
 
 from gravitorch import constants as ct
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.history import BaseHistory, MaxScalarHistory, MinScalarHistory
 
 logger = logging.getLogger(__name__)
 
 
 class EarlyStopping(BaseHandler):
     r"""Implements an early stopping handler to stop the training if no
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/engine_loader.py` & `gravitorch-0.0.9/src/gravitorch/handlers/engine_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import logging
 from pathlib import Path
 from typing import Union
 
 import torch
 
 from gravitorch.engines.base import BaseEngine
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.path import sanitize_path
 
 logger = logging.getLogger(__name__)
 
 
 class EngineStateLoader(BaseHandler):
     r"""Implements a handler to load the engine state dict from a PyTorch file.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/engine_saver.py` & `gravitorch-0.0.9/src/gravitorch/handlers/engine_saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from abc import abstractmethod
 from pathlib import Path
 from typing import Union
 
 from gravitorch.distributed import comm as dist
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.history import get_best_values, get_last_values
 from gravitorch.utils.io import save_pytorch
 from gravitorch.utils.path import sanitize_path
 
 logger = logging.getLogger(__name__)
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/lr_monitor.py` & `gravitorch-0.0.9/src/gravitorch/handlers/lr_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __all__ = ["EpochLRMonitor", "IterationLRMonitor"]
 
 import logging
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
-from gravitorch.handlers.base import BaseHandler
-from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.optimizers.utils import get_learning_rate_per_group
-from gravitorch.utils.events import (
+from gravitorch.events import (
     ConditionalEventHandler,
     EpochPeriodicCondition,
     IterationPeriodicCondition,
 )
+from gravitorch.handlers.base import BaseHandler
+from gravitorch.handlers.utils import add_unique_event_handler
+from gravitorch.optimizers.utils import get_learning_rate_per_group
 from gravitorch.utils.exp_trackers import EpochStep, IterationStep
 
 logger = logging.getLogger(__name__)
 
 
 class EpochLRMonitor(BaseHandler):
     r"""Implements a handler to monitor the learning rate (LR) of an optimizer
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/lr_scheduler.py` & `gravitorch-0.0.9/src/gravitorch/handlers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/lr_scheduler_updater.py` & `gravitorch-0.0.9/src/gravitorch/handlers/lr_scheduler_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ]
 
 import logging
 
 from gravitorch import constants as ct
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import VanillaEventHandler
 
 logger = logging.getLogger(__name__)
 
 
 class LRSchedulerUpdater(BaseHandler):
     r"""Implements a handler to update the learning rate (LR) scheduler at a
     given event.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/model.py` & `gravitorch-0.0.9/src/gravitorch/handlers/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __all__ = ["ModelFreezer"]
 
 import logging
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
 from gravitorch.nn import freeze_module
-from gravitorch.utils.events import VanillaEventHandler
 
 logger = logging.getLogger(__name__)
 
 
 class ModelFreezer(BaseHandler):
     r"""Implements a handler to freeze the model or one of its submodules.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/model_architecture.py` & `gravitorch-0.0.9/src/gravitorch/handlers/model_architecture.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __all__ = ["ModelArchitectureAnalyzer", "NetworkArchitectureAnalyzer"]
 
 from typing import Union
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import to_events
 from gravitorch.models.utils import (
     analyze_model_architecture,
     analyze_network_architecture,
 )
-from gravitorch.utils.events import VanillaEventHandler
 
 
 class ModelArchitectureAnalyzer(BaseHandler):
     r"""Implements a handler to analyze a model architecture.
 
     Args:
     ----
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/model_initializer.py` & `gravitorch-0.0.9/src/gravitorch/handlers/model_initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 __all__ = ["ModelInitializer"]
 
 import logging
 from typing import Union
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
 from gravitorch.nn.init import BaseInitializer, setup_initializer
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.format import str_indent
 
 logger = logging.getLogger(__name__)
 
 
 class ModelInitializer(BaseHandler):
     r"""Implements a handler to initialize the model's parameters.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/model_parameter.py` & `gravitorch-0.0.9/src/gravitorch/handlers/model_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __all__ = ["ModelParameterAnalyzer"]
 
 from typing import Union
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import to_events
 from gravitorch.nn.utils.parameter import show_parameter_summary
-from gravitorch.utils.events import VanillaEventHandler
 
 
 class ModelParameterAnalyzer(BaseHandler):
     r"""Implements a handler to analyze the model parameter values.
 
     Args:
     ----
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/model_state_dict_loader.py` & `gravitorch-0.0.9/src/gravitorch/handlers/model_state_dict_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import logging
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Optional, Union
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
 from gravitorch.nn.utils.state_dict import (
     load_checkpoint_to_module,
     load_model_state_dict,
 )
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.path import sanitize_path
 
 logger = logging.getLogger(__name__)
 
 
 class ModelStateDictLoader(BaseHandler):
     r"""Implements a handler to load the model state dict.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/optimizer_monitor.py` & `gravitorch-0.0.9/src/gravitorch/handlers/optimizer_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 __all__ = ["EpochOptimizerMonitor", "IterationOptimizerMonitor"]
 
 import logging
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import (
+    ConditionalEventHandler,
+    EpochPeriodicCondition,
+    IterationPeriodicCondition,
+)
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
 from gravitorch.optimizers.utils import (
     log_optimizer_parameters_per_group,
     show_optimizer_parameters_per_group,
 )
-from gravitorch.utils.events import (
-    ConditionalEventHandler,
-    EpochPeriodicCondition,
-    IterationPeriodicCondition,
-)
 from gravitorch.utils.exp_trackers import EpochStep, IterationStep
 
 logger = logging.getLogger(__name__)
 
 
 class EpochOptimizerMonitor(BaseHandler):
     r"""Implements a handler to monitor the optimizer every ``freq`` epochs.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/optimizer_state.py` & `gravitorch-0.0.9/src/gravitorch/handlers/optimizer_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __all__ = ["ConsolidateOptimizerState"]
 
 import logging
 
 from gravitorch import distributed as dist
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import VanillaEventHandler
 
 logger = logging.getLogger(__name__)
 
 
 class ConsolidateOptimizerState(BaseHandler):
     r"""Implements a handler to consolidate the state dict of an optimizer.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/sysinfo.py` & `gravitorch-0.0.9/src/gravitorch/handlers/sysinfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["EpochSysInfoMonitor"]
 
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import ConditionalEventHandler, EpochPeriodicCondition
 from gravitorch.handlers.base import BaseHandler
 from gravitorch.handlers.utils import add_unique_event_handler
-from gravitorch.utils.events import ConditionalEventHandler, EpochPeriodicCondition
 from gravitorch.utils.sysinfo import log_system_info
 
 
 class EpochSysInfoMonitor(BaseHandler):
     r"""Implements a handler to monitor the system metrics every ``freq``
     epochs.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/handlers/utils.py` & `gravitorch-0.0.9/src/gravitorch/handlers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ["add_unique_event_handler", "setup_handler", "setup_and_attach_handlers", "to_events"]
 
 import logging
 from typing import Union
 
 from gravitorch.engines.base import BaseEngine
+from gravitorch.events import BaseEventHandler
 from gravitorch.handlers.base import BaseHandler
-from gravitorch.utils.events import BaseEventHandler
 from gravitorch.utils.format import str_target_object
 
 logger = logging.getLogger(__name__)
 
 
 def add_unique_event_handler(
     engine: BaseEngine, event: str, event_handler: BaseEventHandler
@@ -35,15 +35,15 @@
         # Create an engine
         >>> from gravitorch.engines import AlphaEngine
         >>> engine = AlphaEngine(...)
         # Create an event handler
         >>> def hello_handler():
         ...     print('Hello!')
         ...
-        >>> from gravitorch.utils.events import VanillaEventHandler
+        >>> from gravitorch.events import VanillaEventHandler
         >>> event_handler = VanillaEventHandler(hello_handler)
         # Add an event handler to the engine
         >>> from gravitorch.handlers import add_unique_event_handler
         >>> add_unique_event_handler(engine, 'my_event', event_handler)
     """
     if engine.has_event_handler(event_handler, event):
         logger.info(f"{event_handler} is already added to the engine for '{event}' event")
```

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/__init__.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/accelerate.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/accelerate.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/amp.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/amp.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/base.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/basic.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/basic.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/conditions.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/conditions.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/factory.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/noop.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/evaluation/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/loops/evaluation/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/observers/base.py` & `gravitorch-0.0.9/src/gravitorch/loops/observers/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/observers/batch_saving.py` & `gravitorch-0.0.9/src/gravitorch/loops/observers/batch_saving.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/observers/factory.py` & `gravitorch-0.0.9/src/gravitorch/loops/observers/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/observers/noop.py` & `gravitorch-0.0.9/src/gravitorch/loops/observers/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/observers/sequential.py` & `gravitorch-0.0.9/src/gravitorch/loops/observers/sequential.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/__init__.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/accelerate.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/accelerate.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             https://huggingface.co/docs/accelerate/accelerator.html.
             If ``None``, it will use the default parameters.
             Default: ``None``
         set_grad_to_none (bool, optional): If ``True``, set the
             gradients to ``None``, otherwise set the gradients to
             zero. Setting the gradients to ``None`` will in general
             have lower memory footprint, and can modestly improve
-            performance. Default: ``False``
+            performance. Default: ``True``
         tag (str, optional): Specifies the tag which is used to log
             metrics. Default: ``"train"``
         clip_grad (dict or None, optional): Specifies the
             configuration to clip the gradient. If ``None``, no
             gradient clipping is used during the training.
             Default: ``None``
         observer (``BaseLoopObserver`` or dict or None, optional):
@@ -63,15 +63,15 @@
             Specifies the profiler or its configuration. If ``None``,
             the ``NoOpProfiler`` is instantiated. Default: ``None``
     """
 
     def __init__(
         self,
         accelerator: Union[Accelerator, dict, None] = None,
-        set_grad_to_none: bool = False,
+        set_grad_to_none: bool = True,
         tag: str = "train",
         clip_grad: Optional[dict] = None,
         observer: Union[BaseLoopObserver, dict, None] = None,
         profiler: Union[BaseProfiler, dict, None] = None,
     ) -> None:
         check_accelerate()
         self._accelerator = self._setup_accelerator(accelerator or {})
```

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/amp.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/amp.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Args:
     ----
         set_grad_to_none (bool, optional): If ``True``, set the
             gradients to ``None``, otherwise set the gradients to
             zero. Setting the gradients to ``None`` will in general
             have lower memory footprint, and can modestly improve
-            performance. Default: ``False``
+            performance. Default: ``True``
         amp_enabled (bool, optional): If ``True``, automatic mixed
             precision (AMP) is enabled, otherwise it is disabled.
             Default: ``True``
         batch_device_placement (bool, optional): Specifies the batch
             device placement module. This module moves the batch on
             a target device. The target device should be compatible
             with the model. If ``None``, an ``AutoDevicePlacement``
@@ -55,15 +55,15 @@
             the profiler or its configuration. If ``None``, the
             ``NoOpProfiler`` is instantiated. Default: ``None``
     """
 
     def __init__(
         self,
         clip_grad: Optional[dict] = None,
-        set_grad_to_none: bool = False,
+        set_grad_to_none: bool = True,
         amp_enabled: bool = True,
         batch_device_placement: Union[BaseDevicePlacement, dict, None] = None,
         tag: str = "train",
         observer: Union[BaseLoopObserver, dict, None] = None,
         profiler: Union[BaseProfiler, dict, None] = None,
     ) -> None:
         super().__init__(
```

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/base.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/basic.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 
 from gravitorch import constants as ct
 from gravitorch.distributed import comm as dist
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
 from gravitorch.loops.observers import BaseLoopObserver, setup_loop_observer
 from gravitorch.loops.training.base import BaseTrainingLoop
-from gravitorch.optimizers.utils import (
-    log_optimizer_parameters_per_group,
-    show_optimizer_parameters_per_group,
-)
-from gravitorch.utils.exp_trackers import EpochStep
 from gravitorch.utils.history import MinScalarHistory
 from gravitorch.utils.metric_tracker import ScalarMetricTracker
 from gravitorch.utils.profilers import BaseProfiler, setup_profiler
 from gravitorch.utils.seed import get_random_seed, manual_seed
 from gravitorch.utils.timing import BatchLoadingTimer
 
 logger = logging.getLogger(__name__)
@@ -131,22 +126,14 @@
             )
         )
         engine.model.train()
 
         if not engine.has_history(f"{self._tag}/{ct.LOSS}"):
             engine.add_history(MinScalarHistory(f"{self._tag}/{ct.LOSS}"))
 
-        show_optimizer_parameters_per_group(engine.optimizer)  # TODO: move to handler
-        log_optimizer_parameters_per_group(
-            optimizer=engine.optimizer,
-            engine=engine,
-            step=EpochStep(engine.epoch),
-            prefix=f"{self._tag}/",
-        )
-
     @abstractmethod
     def _prepare_model_optimizer_data_loader(
         self, engine: BaseEngine
     ) -> tuple[Module, Optimizer, Iterable]:
         r"""Prepares the model, optimizer and data loader.
 
         Args:
```

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/factory.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/noop.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/loops/training/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/loops/training/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     Args:
     ----
         set_grad_to_none (bool, optional): If ``True``, set the
             gradients to ``None``, otherwise set the gradients to
             zero. Setting the gradients to ``None`` will in general
             have lower memory footprint, and can modestly improve
-            performance. Default: ``False``
+            performance. Default: ``True``
         batch_device_placement (``BaseDevicePlacement`` or dict or
             ``None``, optional): Specifies the batch device placement
             module. This module moves the batch on a target device.
             The target device should be compatible with the model.
             If ``None``, an ``AutoDevicePlacement`` object is
             instantiated. Default: ``None``
         tag (str, optional): Specifies the tag which is used to log
@@ -57,15 +57,15 @@
         profiler (``BaseProfiler`` or dict or None, optional): Specifies
             the profiler or its configuration. If ``None``, the
             ``NoOpProfiler`` is instantiated. Default: ``None``
     """
 
     def __init__(
         self,
-        set_grad_to_none: bool = False,
+        set_grad_to_none: bool = True,
         batch_device_placement: Union[BaseDevicePlacement, dict, None] = None,
         tag: str = ct.TRAIN,
         clip_grad: Optional[dict] = None,
         observer: Union[BaseLoopObserver, dict, None] = None,
         profiler: Union[BaseProfiler, dict, None] = None,
     ) -> None:
         super().__init__(tag=tag, clip_grad=clip_grad, observer=observer, profiler=profiler)
```

### Comparing `gravitorch-0.0.8/src/gravitorch/lr_schedulers/__init__.py` & `gravitorch-0.0.9/src/gravitorch/lr_schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/lr_schedulers/base.py` & `gravitorch-0.0.9/src/gravitorch/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/lr_schedulers/creation.py` & `gravitorch-0.0.9/src/gravitorch/lr_schedulers/creation.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/lr_schedulers/invsqrt.py` & `gravitorch-0.0.9/src/gravitorch/lr_schedulers/invsqrt.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/base.py` & `gravitorch-0.0.9/src/gravitorch/models/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/criteria/packed_seq.py` & `gravitorch-0.0.9/src/gravitorch/models/criteria/packed_seq.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/criteria/padded_seq.py` & `gravitorch-0.0.9/src/gravitorch/models/criteria/padded_seq.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/criteria/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/models/criteria/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/criteria/weighted_sum.py` & `gravitorch-0.0.9/src/gravitorch/models/criteria/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/__init__.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/base.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/base_epoch.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/base_epoch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import logging
 from typing import Optional, Union
 
 from gravitorch import constants as ct
 from gravitorch.engines.base import BaseEngine
 from gravitorch.engines.events import EngineEvents
+from gravitorch.events import VanillaEventHandler
 from gravitorch.models.metrics.base import BaseMetric
 from gravitorch.models.metrics.state import BaseState, setup_state
-from gravitorch.utils.events import VanillaEventHandler
 from gravitorch.utils.exp_trackers import EpochStep
 
 logger = logging.getLogger(__name__)
 
 
 class BaseEpochMetric(BaseMetric):
     r"""Implements the base class of an epoch-wise metric.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/classification/__init__.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/classification/accuracy.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/classification/confusion_matrix.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/classification/cross_entropy.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/classification/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/__init__.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/absolute_error.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/absolute_error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/absolute_relative_error.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/log_cosh_error.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/log_cosh_error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/nmse.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/nmse.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/squared_error.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/squared_error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/regression/squared_log_error.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/regression/squared_log_error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/sequential.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/sequential.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/state.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/state.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/transform.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/transform.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/metrics/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/models/metrics/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/networks/__init__.py` & `gravitorch-0.0.9/src/gravitorch/models/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/networks/image_classification.py` & `gravitorch-0.0.9/src/gravitorch/models/networks/image_classification.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/networks/lenet.py` & `gravitorch-0.0.9/src/gravitorch/models/networks/lenet.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/networks/mlp.py` & `gravitorch-0.0.9/src/gravitorch/models/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/networks/mnist.py` & `gravitorch-0.0.9/src/gravitorch/models/networks/mnist.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/utils/__init__.py` & `gravitorch-0.0.9/src/gravitorch/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/utils/architecture.py` & `gravitorch-0.0.9/src/gravitorch/models/utils/architecture.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/utils/setup_and_attach.py` & `gravitorch-0.0.9/src/gravitorch/models/utils/setup_and_attach.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/utils/summary.py` & `gravitorch-0.0.9/src/gravitorch/models/utils/summary.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/utils/testing.py` & `gravitorch-0.0.9/src/gravitorch/models/utils/testing.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/models/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/models/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/__init__.py` & `gravitorch-0.0.9/src/gravitorch/nn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "FusionFFN",
     "Gaussian",
     "Isymlog",
     "Laplacian",
     "Log1p",
     "MSLELoss",
     "ModuleSummary",
+    "Mul",
     "MultiQuadratic",
     "MulticlassFlattenModule",
     "MultiplicationFusion",
     "OnePolynomial",
     "ParameterSummary",
     "Quadratic",
     "ReLUn",
@@ -122,14 +123,15 @@
     ScalarEncoderFFN,
 )
 from gravitorch.nn.shift_scale import SequenceShiftScale, ShiftScale
 from gravitorch.nn.transforms import (
     Asinh,
     Isymlog,
     Log1p,
+    Mul,
     OnePolynomial,
     Safeexp,
     Safelog,
     SequenceToBatch,
     Sinh,
     Squeeze,
     Symlog,
```

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/activations.py` & `gravitorch-0.0.9/src/gravitorch/nn/activations.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/alpha_activations.py` & `gravitorch-0.0.9/src/gravitorch/nn/alpha_activations.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/barron_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/barron_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/clamp.py` & `gravitorch-0.0.9/src/gravitorch/nn/clamp.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/creators.py` & `gravitorch-0.0.9/src/gravitorch/nn/creators.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/experimental/exponential_nll.py` & `gravitorch-0.0.9/src/gravitorch/nn/experimental/exponential_nll.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/exu.py` & `gravitorch-0.0.9/src/gravitorch/nn/exu.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/flatten.py` & `gravitorch-0.0.9/src/gravitorch/nn/flatten.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/focal_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/focal_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/fourier_feature.py` & `gravitorch-0.0.9/src/gravitorch/nn/fourier_feature.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/__init__.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/barron_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/barron_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/error.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/error.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/experimental/exponential_nll.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/experimental/exponential_nll.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/loss_helpers.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/loss_helpers.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/functional/robust_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/functional/robust_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/fusion.py` & `gravitorch-0.0.9/src/gravitorch/nn/fusion.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/__init__.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/base.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/const.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/const.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/factory.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/kaiming.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/kaiming.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/noop.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/normal.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/normal.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/sequential.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/sequential.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/init/xavier.py` & `gravitorch-0.0.9/src/gravitorch/nn/init/xavier.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/residual.py` & `gravitorch-0.0.9/src/gravitorch/nn/residual.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/robust_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/robust_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/scalar_encoding.py` & `gravitorch-0.0.9/src/gravitorch/nn/scalar_encoding.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/shift_scale.py` & `gravitorch-0.0.9/src/gravitorch/nn/shift_scale.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/transforms.py` & `gravitorch-0.0.9/src/gravitorch/nn/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = [
     "Asinh",
     "Isymlog",
     "Log1p",
+    "Mul",
     "OnePolynomial",
     "Safeexp",
     "Safelog",
     "SequenceToBatch",
     "Sinh",
     "Squeeze",
     "Symlog",
@@ -44,14 +45,48 @@
     r"""Implements a ``torch.nn.Module`` to compute the natural logarithm of
     ``(1 + input)``."""
 
     def forward(self, tensor: Tensor) -> Tensor:
         return tensor.log1p()
 
 
+class Mul(Module):
+    r"""Implements a ``torch.nn.Module`` to multiply the input tensor with a
+    float scalar value.
+
+    Args:
+        value (float): Specifies the value.
+    """
+
+    def __init__(self, value: float) -> None:
+        super().__init__()
+        self.value = float(value)
+
+    def extra_repr(self) -> str:
+        return f"value={self.value}"
+
+    def forward(self, tensor: Tensor) -> Tensor:
+        r"""Multiplies the input tensor with a scalar value.
+
+        Note: the output is a float tensor.
+
+        Args:
+        ----
+            tensor (``torch.Tensor`` of shape
+                ``(d0, d1, ..., dn)``): Specifies the tensor of values
+                to transform.
+
+        Returns:
+        -------
+            ``torch.Tensor`` of type float and shape
+                ``(d0, d1, ..., dn)``: The transformed values.
+        """
+        return tensor.mul(self.value)
+
+
 class OnePolynomial(Module):
     r"""Implements a ``torch.nn.Module`` to compute a polynomial transformation
     with a single term.
 
     The equation is ``alpha * x^gamma + beta`` where ``x`` is the
     module input tensor.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/__init__.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/factory.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/module_helpers.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/module_helpers.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/parameter.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/state_dict.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/state_dict.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/summary.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/summary.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/utils/testing.py` & `gravitorch-0.0.9/src/gravitorch/nn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/nn/warmup_seq_loss.py` & `gravitorch-0.0.9/src/gravitorch/nn/warmup_seq_loss.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/optimizers/factory.py` & `gravitorch-0.0.9/src/gravitorch/optimizers/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/optimizers/noop.py` & `gravitorch-0.0.9/src/gravitorch/optimizers/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/optimizers/utils.py` & `gravitorch-0.0.9/src/gravitorch/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/rsrc/__init__.py` & `gravitorch-0.0.9/src/gravitorch/rsrc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 __all__ = [
     "BaseResource",
     "DistributedContext",
     "LogCudaMemory",
     "LogSysInfo",
     "Logging",
     "PyTorchConfig",
+    "PyTorchConfigState",
     "PyTorchCudaBackend",
     "PyTorchCudnnBackend",
+    "PyTorchMpsBackend",
+    "PyTorchMpsBackendState",
     "setup_resource",
 ]
 
 from gravitorch.rsrc.base import BaseResource, setup_resource
 from gravitorch.rsrc.distributed import DistributedContext
 from gravitorch.rsrc.logging import Logging
 from gravitorch.rsrc.pytorch import (
     PyTorchConfig,
+    PyTorchConfigState,
     PyTorchCudaBackend,
     PyTorchCudnnBackend,
+    PyTorchMpsBackend,
+    PyTorchMpsBackendState,
 )
 from gravitorch.rsrc.sysinfo import LogCudaMemory, LogSysInfo
```

### Comparing `gravitorch-0.0.8/src/gravitorch/rsrc/base.py` & `gravitorch-0.0.9/src/gravitorch/rsrc/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/rsrc/distributed.py` & `gravitorch-0.0.9/src/gravitorch/rsrc/distributed.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/rsrc/logging.py` & `gravitorch-0.0.9/src/gravitorch/rsrc/logging.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/rsrc/sysinfo.py` & `gravitorch-0.0.9/src/gravitorch/rsrc/sysinfo.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/__init__.py` & `gravitorch-0.0.9/src/gravitorch/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/evaluation.py` & `gravitorch-0.0.9/src/gravitorch/runners/evaluation.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/no_repeat.py` & `gravitorch-0.0.9/src/gravitorch/runners/no_repeat.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/resource.py` & `gravitorch-0.0.9/src/gravitorch/runners/resource.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/training.py` & `gravitorch-0.0.9/src/gravitorch/runners/training.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/runners/utils.py` & `gravitorch-0.0.9/src/gravitorch/runners/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/testing/__init__.py` & `gravitorch-0.0.9/src/gravitorch/testing/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,29 @@
     "cuda_available",
     "distributed_available",
     "gloo_available",
     "nccl_available",
     "pillow_available",
     "psutil_available",
     "tensorboard_available",
+    "torchdata_available",
     "torchvision_available",
     "two_gpus_available",
 ]
 
 from gravitorch.testing._pytest import (
     accelerate_available,
     cuda_available,
     distributed_available,
     gloo_available,
     nccl_available,
     pillow_available,
     psutil_available,
     tensorboard_available,
+    torchdata_available,
     torchvision_available,
     two_gpus_available,
 )
 from gravitorch.testing.dummy import (
     DummyClassificationModel,
     DummyDataset,
     DummyDataSource,
```

### Comparing `gravitorch-0.0.8/src/gravitorch/testing/_pytest.py` & `gravitorch-0.0.9/src/gravitorch/testing/_pytest.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from torch import distributed as tdist
 
 from gravitorch.distributed.comm import Backend, available_backends
 from gravitorch.utils.integrations import (
     is_accelerate_available,
     is_pillow_available,
     is_tensorboard_available,
+    is_torchdata_available,
     is_torchvision_available,
 )
 
 cuda_available = mark.skipif(not torch.cuda.is_available(), reason="Requires a device with CUDA")
 two_gpus_available = mark.skipif(torch.cuda.device_count() < 2, reason="Requires at least 2 GPUs")
 distributed_available = mark.skipif(not tdist.is_available(), reason="Requires PyTorch distributed")
 nccl_available = mark.skipif(Backend.NCCL not in available_backends(), reason="Requires NCCL")
@@ -33,14 +34,20 @@
 tensorboard_available = mark.skipif(
     not is_tensorboard_available(),
     reason=(
         "`tensorboard` is not available. Please install `tensorboard` if you want "
         "to run this test"
     ),
 )
+torchdata_available = mark.skipif(
+    not is_torchdata_available(),
+    reason=(
+        "`torchdata` is not available. Please install `torchdata` if you want " "to run this test"
+    ),
+)
 torchvision_available = mark.skipif(
     not is_torchvision_available(),
     reason=(
         "`torchvision` is not available. Please install `torchvision` if you want "
         "to run this test"
     ),
 )
```

### Comparing `gravitorch-0.0.8/src/gravitorch/testing/dummy.py` & `gravitorch-0.0.9/src/gravitorch/testing/dummy.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/artifacts/jsona.py` & `gravitorch-0.0.9/src/gravitorch/utils/artifacts/jsona.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/artifacts/picklea.py` & `gravitorch-0.0.9/src/gravitorch/utils/artifacts/picklea.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/artifacts/pytorcha.py` & `gravitorch-0.0.9/src/gravitorch/utils/artifacts/pytorcha.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/artifacts/text.py` & `gravitorch-0.0.9/src/gravitorch/utils/artifacts/text.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/asset.py` & `gravitorch-0.0.9/src/gravitorch/utils/asset.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/cudamem.py` & `gravitorch-0.0.9/src/gravitorch/utils/cudamem.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/continuous.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/continuous.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/discrete.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/discrete.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/float_tensor.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/float_tensor.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/float_value.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/float_value.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/integer.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/integer.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/long_tensor.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/long_tensor.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/noop.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/sequence.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/sequence.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/data_summary/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/data_summary/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/device_placement/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/device_placement/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/device_placement/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/device_placement/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/device_placement/manual.py` & `gravitorch-0.0.9/src/gravitorch/utils/device_placement/manual.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/device_placement/noop.py` & `gravitorch-0.0.9/src/gravitorch/utils/device_placement/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/device_placement/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/device_placement/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/engine_states/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/engine_states/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/engine_states/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/engine_states/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/engine_states/vanilla.py` & `gravitorch-0.0.9/src/gravitorch/utils/engine_states/vanilla.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/events/__init__.py` & `gravitorch-0.0.9/src/gravitorch/events/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     "EpochPeriodicCondition",
     "EventManager",
     "IterationPeriodicCondition",
     "PeriodicCondition",
     "VanillaEventHandler",
 ]
 
-from gravitorch.utils.events.conditions import (
+from gravitorch.events.conditions import (
     EpochPeriodicCondition,
     IterationPeriodicCondition,
     PeriodicCondition,
 )
-from gravitorch.utils.events.event_handlers import (
+from gravitorch.events.event_handlers import (
     BaseEventHandler,
     BaseEventHandlerWithArguments,
     ConditionalEventHandler,
     VanillaEventHandler,
 )
-from gravitorch.utils.events.manager import EventManager
+from gravitorch.events.manager import EventManager
```

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/events/conditions.py` & `gravitorch-0.0.9/src/gravitorch/events/conditions.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/events/event_handlers.py` & `gravitorch-0.0.9/src/gravitorch/events/event_handlers.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/events/manager.py` & `gravitorch-0.0.9/src/gravitorch/events/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __all__ = ["EventManager"]
 
 import logging
 from collections import defaultdict
 from typing import Optional
 
-from gravitorch.utils.events.event_handlers import BaseEventHandler
+from gravitorch.events.event_handlers import BaseEventHandler
 from gravitorch.utils.format import str_indent, to_torch_sequence_str
 
 logger = logging.getLogger(__name__)
 
 
 class EventManager:
     r"""Implements an event manager.
@@ -63,21 +63,21 @@
                 event handler to attach to the event.
 
         Example usage:
 
         .. code-block:: python
 
             # Create an event manager
-            >>> from gravitorch.utils.events import EventManager
+            >>> from gravitorch.events import EventManager
             >>> event_manager = EventManager()
             # Add an event handler to the event manager
             >>> def hello_handler():
             ...     print('Hello!')
             ...
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> event_manager.add_event_handler('my_event', VanillaEventHandler(hello_handler))
         """
         self._event_handlers[str(event)].append(event_handler)
         logger.debug(f"Added {event_handler} to event {event}")
 
     def fire_event(self, event: str) -> None:
         r"""Fires the handler(s) for the given event.
@@ -87,23 +87,23 @@
             event (str): Specifies the event to fire.
 
         Example usage:
 
         .. code-block:: python
 
             # Create an event manager
-            >>> from gravitorch.utils.events import EventManager
+            >>> from gravitorch.events import EventManager
             >>> event_manager = EventManager()
             # Fire the 'my_event' event
             >>> event_manager.fire_event('my_event')  # should do nothing because there is no event handler
             # Add an event handler
             >>> def hello_handler():
             ...     print("Hello!")
             ...
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> event_manager.add_event_handler('my_event', VanillaEventHandler(hello_handler))
             # Fire the 'my_event' event
             >>> event_manager.fire_event('my_event')
             Hello!
         """
         logger.debug(f"Firing {event} event")
         self._last_fired_event = event
@@ -127,22 +127,22 @@
                 Default: ``None``
 
         Example usage:
 
         .. code-block:: python
 
             # Create an event manager
-            >>> from gravitorch.utils.events import EventManager
+            >>> from gravitorch.events import EventManager
             >>> event_manager = EventManager()
             # Define a handler
             >>> def hello_handler():
             ...     print("Hello!")
             ...
             # Check if `hello_handler` is registered in the event manager
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> event_manager.has_event_handler(VanillaEventHandler(hello_handler))
             False
             # Check if `hello_handler` is registered in the event manager for 'my_event' event
             >>> event_manager.has_event_handler(VanillaEventHandler(hello_handler), 'my_event')
             False
             # Add an event handler
             >>> event_manager.add_event_handler('my_event', VanillaEventHandler(hello_handler))
@@ -183,21 +183,21 @@
                 is not attached to the event.
 
         Example usage:
 
         .. code-block:: python
 
             # Create an event manager
-            >>> from gravitorch.utils.events import EventManager
+            >>> from gravitorch.events import EventManager
             >>> event_manager = EventManager()
             # Add an event handler to the engine
             >>> def hello_handler():
             ...     print('Hello!')
             ...
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> event_manager.add_event_handler('my_event', VanillaEventHandler(hello_handler))
             # Check if `hello_handler` is registered in the event manager for 'my_event' event
             >>> event_manager.has_event_handler(VanillaEventHandler(hello_handler), 'my_event')
             True
             # Remove the event handler of the engine
             >>> event_manager.remove_event_handler('my_event', VanillaEventHandler(hello_handler))
             # Check if `hello_handler` is registered in the event manager for 'my_event' event
@@ -226,21 +226,21 @@
         This method removes all the event handlers from the event manager.
 
         Example usage:
 
         .. code-block:: python
 
             # Create an event manager
-            >>> from gravitorch.utils.events import EventManager
+            >>> from gravitorch.events import EventManager
             >>> event_manager = EventManager()
             # Add an event handler to the engine
             >>> def hello_handler():
             ...     print('Hello!')
             ...
-            >>> from gravitorch.utils.events import VanillaEventHandler
+            >>> from gravitorch.events import VanillaEventHandler
             >>> event_manager.add_event_handler('my_event', VanillaEventHandler(hello_handler))
             # Check if `hello_handler` is registered in the event manager for 'my_event' event
             >>> event_manager.has_event_handler(VanillaEventHandler(hello_handler), 'my_event')
             True
             >>> event_manager.fire_event('my_event')
             >>> event_manager.last_fired_event
             my_event
```

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/noop.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/steps.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/steps.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/tensorboard.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/exp_trackers/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/exp_trackers/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/factory.py` & `gravitorch-0.0.9/src/gravitorch/utils/factory.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/format.py` & `gravitorch-0.0.9/src/gravitorch/utils/format.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/comparable.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/comparable.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/comparator.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/comparator.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/generic.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/generic.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/manager.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/manager.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/history/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/history/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/info.py` & `gravitorch-0.0.9/src/gravitorch/utils/info.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/integrations.py` & `gravitorch-0.0.9/src/gravitorch/utils/integrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,14 +153,42 @@
 
 
 def is_tensorboard_available() -> bool:
     r"""Indicates if the ``tensorboard`` package is installed or not."""
     return find_spec("tensorboard") is not None
 
 
+#####################
+#     torchdata     #
+#####################
+
+
+def check_torchdata() -> None:
+    r"""Checks if the ``torchdata`` package is installed.
+
+    Raises
+    ------
+        RuntimeError if the ``torchdata`` package is not installed.
+    """
+    if not is_torchdata_available():
+        raise RuntimeError(
+            "`torchdata` package is required but not installed. "
+            "You can install `torchdata` package with the command:\n\n"
+            "pip install torchdata\n"
+        )
+
+
+def is_torchdata_available() -> bool:
+    r"""Indicates if the ``torchdata`` package is installed or not.
+
+    https://pytorch.org/vision/stable/index.html
+    """
+    return find_spec("torchdata") is not None
+
+
 #######################
 #     torchvision     #
 #######################
 
 
 def check_torchvision() -> None:
     r"""Checks if the ``torchvision`` package is installed.
```

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/io.py` & `gravitorch-0.0.9/src/gravitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/logging.py` & `gravitorch-0.0.9/src/gravitorch/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/mapping.py` & `gravitorch-0.0.9/src/gravitorch/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/average.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/average.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/confusion_matrix.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/moving_average.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/moving_average.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/scalar.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/scalar.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/meters/tensor.py` & `gravitorch-0.0.9/src/gravitorch/utils/meters/tensor.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/metric_tracker.py` & `gravitorch-0.0.9/src/gravitorch/utils/metric_tracker.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/module_manager.py` & `gravitorch-0.0.9/src/gravitorch/utils/module_manager.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/parameter.py` & `gravitorch-0.0.9/src/gravitorch/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/partitioning.py` & `gravitorch-0.0.9/src/gravitorch/utils/partitioning.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/path.py` & `gravitorch-0.0.9/src/gravitorch/utils/path.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/profilers/base.py` & `gravitorch-0.0.9/src/gravitorch/utils/profilers/base.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/profilers/noop.py` & `gravitorch-0.0.9/src/gravitorch/utils/profilers/noop.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/profilers/pytorch.py` & `gravitorch-0.0.9/src/gravitorch/utils/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/profilers/utils.py` & `gravitorch-0.0.9/src/gravitorch/utils/profilers/utils.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/seed.py` & `gravitorch-0.0.9/src/gravitorch/utils/seed.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/sequence.py` & `gravitorch-0.0.9/src/gravitorch/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/summary.py` & `gravitorch-0.0.9/src/gravitorch/utils/summary.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/sysinfo.py` & `gravitorch-0.0.9/src/gravitorch/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/tensor/__init__.py` & `gravitorch-0.0.9/src/gravitorch/utils/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/tensor/flatted.py` & `gravitorch-0.0.9/src/gravitorch/utils/tensor/flatted.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/tensor/math_ops.py` & `gravitorch-0.0.9/src/gravitorch/utils/tensor/math_ops.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/tensor/misc.py` & `gravitorch-0.0.9/src/gravitorch/utils/tensor/misc.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/tensor/recursive_ops.py` & `gravitorch-0.0.9/src/gravitorch/utils/tensor/recursive_ops.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/timing.py` & `gravitorch-0.0.9/src/gravitorch/utils/timing.py`

 * *Files identical despite different names*

### Comparing `gravitorch-0.0.8/src/gravitorch/utils/torch_device.py` & `gravitorch-0.0.9/src/gravitorch/utils/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     -------
         tuple: The available devices.
 
     Example usage:
 
     .. code-block:: python
 
-        >>> from gravitorch.utils.torch_device import get_available_devices
+        >>> from gravitorch.utils import get_available_devices
         >>> get_available_devices()
         ('cpu', 'cuda:0')
     """
     if torch.cuda.is_available():
         return ("cpu", "cuda:0")
     return ("cpu",)
 
@@ -62,15 +62,15 @@
             the object to the device, the input object is returned.
 
     Example usage:
 
     .. code-block:: python
 
         >>> import torch
-        >>> from gravitorch.utils.torch_device import move_to_device
+        >>> from gravitorch.utils import move_to_device
         >>> move_to_device(
         ...     {'tensor1': torch.ones(2, 3), 'tensor2': torch.zeros(4)},
         ...     device=torch.device('cuda:0'),
         ... )
         {'tensor1': tensor([[1., 1., 1.], [1., 1., 1.]], device='cuda:0'),
          'tensor2': tensor([0., 0., 0., 0.], device='cuda:0')}
     """
```

### Comparing `gravitorch-0.0.8/PKG-INFO` & `gravitorch-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Warning: API is not stable
 Keywords: gravitorch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,29 +17,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: all
 Provides-Extra: tb
 Provides-Extra: vision
-Requires-Dist: accelerate (>=0.17,<0.18) ; extra == "all"
+Requires-Dist: accelerate (>=0.18,<0.19) ; extra == "all"
 Requires-Dist: colorlog (>=6.7,<7.0) ; extra == "all"
 Requires-Dist: coola (>=0.0,<0.1)
 Requires-Dist: hya (>=0.0,<0.1)
 Requires-Dist: hydra-core (>=1.3,<2.0)
 Requires-Dist: matplotlib (>=3.7,<4.0) ; extra == "all"
 Requires-Dist: numpy (>=1.24,<2.0)
 Requires-Dist: objectory (>=0.0,<0.1)
 Requires-Dist: pillow (>=9.3,<10.0) ; extra == "all" or extra == "vision"
 Requires-Dist: psutil (>=5.9,<6.0)
 Requires-Dist: pytorch-ignite (>=0.4,<0.5)
 Requires-Dist: tabulate (>=0.9,<0.10)
 Requires-Dist: tensorboard (>=2.11,<3.0) ; extra == "all" or extra == "tb"
-Requires-Dist: torch (>=1.13,<2.0)
-Requires-Dist: torchvision (>=0.14,<0.15) ; extra == "all" or extra == "vision"
+Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: torchdata (>=0.6,<0.7) ; extra == "all"
+Requires-Dist: torchvision (>=0.15,<0.16) ; extra == "all" or extra == "vision"
 Requires-Dist: tqdm (>=4.64,<5.0)
 Description-Content-Type: text/markdown
 
 
 [//]: # (<p align="center">)
 
 [//]: # (   <a href="https://github.com/durandtibo/meteor/actions">)
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: gravitorch Version: 0.0.8 Summary: Warning: API is
+Metadata-Version: 2.1 Name: gravitorch Version: 0.0.9 Summary: Warning: API is
 not stable Keywords: gravitorch Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Provides-Extra: all
 Provides-Extra: tb Provides-Extra: vision Requires-Dist: accelerate
-(>=0.17,<0.18) ; extra == "all" Requires-Dist: colorlog (>=6.7,<7.0) ; extra ==
+(>=0.18,<0.19) ; extra == "all" Requires-Dist: colorlog (>=6.7,<7.0) ; extra ==
 "all" Requires-Dist: coola (>=0.0,<0.1) Requires-Dist: hya (>=0.0,<0.1)
 Requires-Dist: hydra-core (>=1.3,<2.0) Requires-Dist: matplotlib (>=3.7,<4.0) ;
 extra == "all" Requires-Dist: numpy (>=1.24,<2.0) Requires-Dist: objectory
 (>=0.0,<0.1) Requires-Dist: pillow (>=9.3,<10.0) ; extra == "all" or extra ==
 "vision" Requires-Dist: psutil (>=5.9,<6.0) Requires-Dist: pytorch-ignite
 (>=0.4,<0.5) Requires-Dist: tabulate (>=0.9,<0.10) Requires-Dist: tensorboard
 (>=2.11,<3.0) ; extra == "all" or extra == "tb" Requires-Dist: torch
-(>=1.13,<2.0) Requires-Dist: torchvision (>=0.14,<0.15) ; extra == "all" or
-extra == "vision" Requires-Dist: tqdm (>=4.64,<5.0) Description-Content-Type:
-text/markdown [//]: # (
+(>=2.0,<3.0) Requires-Dist: torchdata (>=0.6,<0.7) ; extra == "all" Requires-
+Dist: torchvision (>=0.15,<0.16) ; extra == "all" or extra == "vision"
+Requires-Dist: tqdm (>=4.64,<5.0) Description-Content-Type: text/markdown [//]:
+# (
 ) [//]: # ( )_[//]:_#_(_[CI])_[//]:_#_() [//]: # ( )_[//]:_#_(_[PYPI_version])_
  [//]:_#_() [//]: # ( )_[//]:_#_(_[Python])_[//]:_#_() [//]: # ( )_[//]:_#_(_
 [BSD-3-Clause])_[//]:_#_() [//]: # ( )_[//]:_#_(_[Codecov])_[//]:_#_() [//]: #
 ( )_[//]:_#_(_[Code_style:_black])_[//]:_#_() [//]: # ( )_[//]:_#_(_[Doc_style:
                         google])_[//]:_#_() [//]: # (
                                   ) [//]: # (
 )
```

