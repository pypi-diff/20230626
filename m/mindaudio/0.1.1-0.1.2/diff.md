# Comparing `tmp/mindaudio-0.1.1.tar.gz` & `tmp/mindaudio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindaudio-0.1.1.tar", last modified: Fri Jun 23 14:04:48 2023, max compression
+gzip compressed data, was "mindaudio-0.1.2.tar", last modified: Mon Jun 26 03:23:26 2023, max compression
```

## Comparing `mindaudio-0.1.1.tar` & `mindaudio-0.1.2.tar`

### file list

```diff
@@ -1,98 +1,105 @@
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.368666 mindaudio-0.1.1/
--rw-r--r--   0 weizheng   (501) staff       (20)    11357 2023-06-23 13:51:55.000000 mindaudio-0.1.1/LICENSE
--rw-r--r--   0 weizheng   (501) staff       (20)      857 2023-06-23 14:04:48.368512 mindaudio-0.1.1/PKG-INFO
--rw-r--r--   0 weizheng   (501) staff       (20)     6232 2023-06-23 13:51:55.000000 mindaudio-0.1.1/README.md
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.356345 mindaudio-0.1.1/mindaudio/
--rw-r--r--   0 weizheng   (501) staff       (20)      163 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/__init__.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.359084 mindaudio-0.1.1/mindaudio/data/
--rw-r--r--   0 weizheng   (501) staff       (20)      418 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3715 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/aishell.py
--rw-r--r--   0 weizheng   (501) staff       (20)    32116 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/augment.py
--rw-r--r--   0 weizheng   (501) staff       (20)    18036 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/features.py
--rw-r--r--   0 weizheng   (501) staff       (20)    15717 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/filters.py
--rw-r--r--   0 weizheng   (501) staff       (20)    34040 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/io.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3925 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/librispeech.py
--rw-r--r--   0 weizheng   (501) staff       (20)    20826 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/processing.py
--rw-r--r--   0 weizheng   (501) staff       (20)    30025 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/spectrum.py
--rw-r--r--   0 weizheng   (501) staff       (20)    13957 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/data/voxceleb.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.359964 mindaudio-0.1.1/mindaudio/loss/
--rw-r--r--   0 weizheng   (501) staff       (20)     1214 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/loss/AdditiveAngularMargin.py
--rw-r--r--   0 weizheng   (501) staff       (20)       60 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/loss/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3879 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/loss/ctc_loss.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3652 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/loss/label_smoothing_loss.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3678 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/loss/loss_scale.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.360705 mindaudio-0.1.1/mindaudio/metric/
--rw-r--r--   0 weizheng   (501) staff       (20)       57 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/metric/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)    21447 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/metric/cer.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1144 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/metric/eer.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1963 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/metric/wer.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.361411 mindaudio-0.1.1/mindaudio/models/
--rw-r--r--   0 weizheng   (501) staff       (20)      326 2023-06-23 13:53:07.000000 mindaudio-0.1.1/mindaudio/models/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)    23376 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/conformer.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.361853 mindaudio-0.1.1/mindaudio/models/decoders/
--rw-r--r--   0 weizheng   (501) staff       (20)       68 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/decoders/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)    16012 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/decoders/decoder_factory.py
--rw-r--r--   0 weizheng   (501) staff       (20)     4457 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/decoders/greedydecoder.py
--rw-r--r--   0 weizheng   (501) staff       (20)     9488 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/deepspeech2.py
--rw-r--r--   0 weizheng   (501) staff       (20)    14036 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/ecapatdnn.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.362619 mindaudio-0.1.1/mindaudio/models/fastspeech2/
--rw-r--r--   0 weizheng   (501) staff       (20)      104 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/fastspeech2/__init__.py
--rwxr-xr-x   0 weizheng   (501) staff       (20)     3993 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/fastspeech2/fastspeech2_v190.py
--rw-r--r--   0 weizheng   (501) staff       (20)     2494 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/fastspeech2/loss.py
--rw-r--r--   0 weizheng   (501) staff       (20)      971 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/fastspeech2/utils.py
--rw-r--r--   0 weizheng   (501) staff       (20)     7702 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/fastspeech2/variance_adapter.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.364571 mindaudio-0.1.1/mindaudio/models/layers/
--rw-r--r--   0 weizheng   (501) staff       (20)       55 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     9654 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/attention.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1003 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/cmvn.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3933 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/conv1d.py
--rw-r--r--   0 weizheng   (501) staff       (20)     2187 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/conv2d.py
--rw-r--r--   0 weizheng   (501) staff       (20)     4039 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/convolution.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1905 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/dense.py
--rw-r--r--   0 weizheng   (501) staff       (20)     5734 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/embedding.py
--rw-r--r--   0 weizheng   (501) staff       (20)      771 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/glu.py
--rw-r--r--   0 weizheng   (501) staff       (20)     2135 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/layernorm.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1470 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/positionwise_feed_forward.py
--rw-r--r--   0 weizheng   (501) staff       (20)      864 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/softmax_cross_entropy.py
--rw-r--r--   0 weizheng   (501) staff       (20)     2551 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/subsampling.py
--rw-r--r--   0 weizheng   (501) staff       (20)      425 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/layers/swish.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.365501 mindaudio-0.1.1/mindaudio/models/transformer/
--rw-r--r--   0 weizheng   (501) staff       (20)       89 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)      136 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/constants.py
--rw-r--r--   0 weizheng   (501) staff       (20)      858 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/layers.py
--rw-r--r--   0 weizheng   (501) staff       (20)     5111 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/models.py
--rw-r--r--   0 weizheng   (501) staff       (20)      659 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/positional_encoding.py
--rw-r--r--   0 weizheng   (501) staff       (20)      896 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/score_function.py
--rw-r--r--   0 weizheng   (501) staff       (20)     3953 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/transformer/sublayers.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.365763 mindaudio-0.1.1/mindaudio/models/wavegrad/
--rw-r--r--   0 weizheng   (501) staff       (20)       79 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/wavegrad/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     8156 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/models/wavegrad/wavegrad_v190.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.366034 mindaudio-0.1.1/mindaudio/scheduler/
--rw-r--r--   0 weizheng   (501) staff       (20)       33 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/scheduler/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     4871 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/scheduler/scheduler_factory.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.368243 mindaudio-0.1.1/mindaudio/utils/
--rw-r--r--   0 weizheng   (501) staff       (20)       45 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/__init__.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1927 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/average_model.py
--rw-r--r--   0 weizheng   (501) staff       (20)    16786 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/callback.py
--rw-r--r--   0 weizheng   (501) staff       (20)     4810 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/common.py
--rw-r--r--   0 weizheng   (501) staff       (20)     7909 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/config.py
--rw-r--r--   0 weizheng   (501) staff       (20)      746 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/distributed.py
--rw-r--r--   0 weizheng   (501) staff       (20)     1697 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/hparams.py
--rw-r--r--   0 weizheng   (501) staff       (20)     2768 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/initializer.py
--rw-r--r--   0 weizheng   (501) staff       (20)      933 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/load_files.py
--rw-r--r--   0 weizheng   (501) staff       (20)     9277 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/log.py
--rw-r--r--   0 weizheng   (501) staff       (20)     8835 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/mask.py
--rw-r--r--   0 weizheng   (501) staff       (20)      320 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/parallel_info.py
--rw-r--r--   0 weizheng   (501) staff       (20)    15060 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/recognize.py
--rwxr-xr-x   0 weizheng   (501) staff       (20)     5091 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/text2token.py
--rw-r--r--   0 weizheng   (501) staff       (20)    30220 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/utils/train_one_step.py
--rw-r--r--   0 weizheng   (501) staff       (20)       41 2023-06-23 13:51:55.000000 mindaudio-0.1.1/mindaudio/version.py
-drwxr-xr-x   0 weizheng   (501) staff       (20)        0 2023-06-23 14:04:48.357156 mindaudio-0.1.1/mindaudio.egg-info/
--rw-r--r--   0 weizheng   (501) staff       (20)      857 2023-06-23 14:04:48.000000 mindaudio-0.1.1/mindaudio.egg-info/PKG-INFO
--rw-r--r--   0 weizheng   (501) staff       (20)     2668 2023-06-23 14:04:48.000000 mindaudio-0.1.1/mindaudio.egg-info/SOURCES.txt
--rw-r--r--   0 weizheng   (501) staff       (20)        1 2023-06-23 14:04:48.000000 mindaudio-0.1.1/mindaudio.egg-info/dependency_links.txt
--rw-r--r--   0 weizheng   (501) staff       (20)        1 2023-06-23 14:04:30.000000 mindaudio-0.1.1/mindaudio.egg-info/not-zip-safe
--rw-r--r--   0 weizheng   (501) staff       (20)       31 2023-06-23 14:04:48.000000 mindaudio-0.1.1/mindaudio.egg-info/requires.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       10 2023-06-23 14:04:48.000000 mindaudio-0.1.1/mindaudio.egg-info/top_level.txt
--rw-r--r--   0 weizheng   (501) staff       (20)       38 2023-06-23 14:04:48.368711 mindaudio-0.1.1/setup.cfg
--rw-r--r--   0 weizheng   (501) staff       (20)     1458 2023-06-23 13:51:55.000000 mindaudio-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.022515 mindaudio-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 03:21:51.000000 mindaudio-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-26 03:23:26.018515 mindaudio-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-26 03:21:51.000000 mindaudio-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:25.994515 mindaudio-0.1.2/mindaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.002515 mindaudio-0.1.2/mindaudio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/aishell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34040 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30025 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/data/voxceleb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.002515 mindaudio-0.1.2/mindaudio/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/loss/AdditiveAngularMargin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/loss/ctc_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/loss/label_smoothing_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/loss/loss_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.006515 mindaudio-0.1.2/mindaudio/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/metric/cer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/metric/eer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/metric/wer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.006515 mindaudio-0.1.2/mindaudio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/conformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.006515 mindaudio-0.1.2/mindaudio/models/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/decoders/decoder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/decoders/greedydecoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/deepspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/ecapatdnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.006515 mindaudio-0.1.2/mindaudio/models/fastspeech2/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/fastspeech2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3993 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/fastspeech2/fastspeech2_v190.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/fastspeech2/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/fastspeech2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/fastspeech2/variance_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.014515 mindaudio-0.1.2/mindaudio/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/cmvn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/glu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/positionwise_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/softmax_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/layers/swish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.014515 mindaudio-0.1.2/mindaudio/models/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/score_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/transformer/sublayers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.014515 mindaudio-0.1.2/mindaudio/models/wavegrad/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/wavegrad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/models/wavegrad/wavegrad_v190.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.014515 mindaudio-0.1.2/mindaudio/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/scheduler/scheduler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.018515 mindaudio-0.1.2/mindaudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/average_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/load_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/parallel_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/recognize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5091 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/text2token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/utils/train_one_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 03:21:51.000000 mindaudio-0.1.2/mindaudio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:25.998515 mindaudio-0.1.2/mindaudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 03:23:25.000000 mindaudio-0.1.2/mindaudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:23:26.022515 mindaudio-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 03:21:51.000000 mindaudio-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:23:26.018515 mindaudio-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_dataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-26 03:21:51.000000 mindaudio-0.1.2/tests/test_spectrum.py
```

### Comparing `mindaudio-0.1.1/LICENSE` & `mindaudio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/aishell.py` & `mindaudio-0.1.2/mindaudio/data/aishell.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import wget
 
 import mindaudio
 
 logger = logging.getLogger(__name__)
 
+__all__ = ["prepare_aishell"]
+
 
 def download_aishell(data_folder):
     """
     This function prepares the AISHELL-1 dataset.
     If the folder does not exist, the zip file will be extracted. If the zip file does not exist, it will be downloaded.
     data_folder : path to AISHELL-1 dataset.
 
@@ -95,26 +97,26 @@
 
         msg = "\t%s successfully created!" % (new_filename)
         logger.info(msg)
 
         ID_start += len(all_wavs)
 
 
-def prepare_aishell(data_path, download):
+def prepare_aishell(data_path, download=False):
     if download:
         download_aishell(data_path)
     save_aishell_info(data_path, data_path)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="prepare aishell")
     parser.add_argument(
         "--data_path", type=str, default="", help="The path to store data"
     )
     parser.add_argument(
         "--download",
         type=bool,
         default=False,
-        help="Whether need to download aishell",
+        help="set true to download aishell datasets",
     )
     arg = parser.parse_args()
     prepare_aishell(arg.data_path, arg.download)
```

### Comparing `mindaudio-0.1.1/mindaudio/data/augment.py` & `mindaudio-0.1.2/mindaudio/data/augment.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/features.py` & `mindaudio-0.1.2/mindaudio/data/features.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/filters.py` & `mindaudio-0.1.2/mindaudio/data/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Optional, Union
+from typing import Literal, Optional, Union
 
 import mindspore.dataset.audio as msaudio
 import numpy as np
-from typing_extensions import Literal
 
 __all__ = [
     "notch_filter",
     "low_pass_filter",
     "peaking_equalizer",
     "contrast",
     "riaa_biquad",
```

### Comparing `mindaudio-0.1.1/mindaudio/data/io.py` & `mindaudio-0.1.2/mindaudio/data/io.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/processing.py` & `mindaudio-0.1.2/mindaudio/data/processing.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/spectrum.py` & `mindaudio-0.1.2/mindaudio/data/spectrum.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/data/voxceleb.py` & `mindaudio-0.1.2/mindaudio/data/voxceleb.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 import numpy as np
 from tqdm.contrib import tqdm
 
 from .io import read
 from .processing import stereo_to_mono
 
+__all__ = ["prepare_voxceleb"]
+
 logger = logging.getLogger(__name__)
 VOX_OPT_FILE = "opt_voxceleb_prepare.pkl"
 VOX_TRAIN_CSV = "train.csv"
 VOX_DEV_CSV = "dev.csv"
 VOX_TEST_CSV = "test.csv"
 VOX_ENROL_CSV = "enrol.csv"
 SAMPLERATE = 16000
```

### Comparing `mindaudio-0.1.1/mindaudio/loss/AdditiveAngularMargin.py` & `mindaudio-0.1.2/mindaudio/loss/AdditiveAngularMargin.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/loss/ctc_loss.py` & `mindaudio-0.1.2/mindaudio/loss/ctc_loss.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/loss/label_smoothing_loss.py` & `mindaudio-0.1.2/mindaudio/loss/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/loss/loss_scale.py` & `mindaudio-0.1.2/mindaudio/loss/loss_scale.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/metric/cer.py` & `mindaudio-0.1.2/mindaudio/metric/cer.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/metric/eer.py` & `mindaudio-0.1.2/mindaudio/metric/eer.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/metric/wer.py` & `mindaudio-0.1.2/mindaudio/metric/wer.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/conformer.py` & `mindaudio-0.1.2/mindaudio/models/conformer.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/decoders/decoder_factory.py` & `mindaudio-0.1.2/mindaudio/models/decoders/decoder_factory.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/decoders/greedydecoder.py` & `mindaudio-0.1.2/mindaudio/models/decoders/greedydecoder.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/deepspeech2.py` & `mindaudio-0.1.2/mindaudio/models/deepspeech2.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/ecapatdnn.py` & `mindaudio-0.1.2/mindaudio/models/ecapatdnn.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/fastspeech2/fastspeech2_v190.py` & `mindaudio-0.1.2/mindaudio/models/fastspeech2/fastspeech2_v190.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/fastspeech2/loss.py` & `mindaudio-0.1.2/mindaudio/models/fastspeech2/loss.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/fastspeech2/utils.py` & `mindaudio-0.1.2/mindaudio/models/fastspeech2/utils.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/fastspeech2/variance_adapter.py` & `mindaudio-0.1.2/mindaudio/models/fastspeech2/variance_adapter.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/attention.py` & `mindaudio-0.1.2/mindaudio/models/layers/attention.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/cmvn.py` & `mindaudio-0.1.2/mindaudio/models/layers/cmvn.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/conv1d.py` & `mindaudio-0.1.2/mindaudio/models/layers/conv1d.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/conv2d.py` & `mindaudio-0.1.2/mindaudio/models/layers/conv2d.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/convolution.py` & `mindaudio-0.1.2/mindaudio/models/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/dense.py` & `mindaudio-0.1.2/mindaudio/models/layers/dense.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/embedding.py` & `mindaudio-0.1.2/mindaudio/models/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/glu.py` & `mindaudio-0.1.2/mindaudio/models/layers/glu.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/layernorm.py` & `mindaudio-0.1.2/mindaudio/models/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/positionwise_feed_forward.py` & `mindaudio-0.1.2/mindaudio/models/layers/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/softmax_cross_entropy.py` & `mindaudio-0.1.2/mindaudio/models/layers/softmax_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/layers/subsampling.py` & `mindaudio-0.1.2/mindaudio/models/layers/subsampling.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/transformer/layers.py` & `mindaudio-0.1.2/mindaudio/models/transformer/layers.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/transformer/models.py` & `mindaudio-0.1.2/mindaudio/models/transformer/models.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/transformer/positional_encoding.py` & `mindaudio-0.1.2/mindaudio/models/transformer/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/transformer/score_function.py` & `mindaudio-0.1.2/mindaudio/models/transformer/score_function.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/transformer/sublayers.py` & `mindaudio-0.1.2/mindaudio/models/transformer/sublayers.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/models/wavegrad/wavegrad_v190.py` & `mindaudio-0.1.2/mindaudio/models/wavegrad/wavegrad_v190.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/scheduler/scheduler_factory.py` & `mindaudio-0.1.2/mindaudio/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/average_model.py` & `mindaudio-0.1.2/mindaudio/utils/average_model.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/callback.py` & `mindaudio-0.1.2/mindaudio/utils/callback.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/common.py` & `mindaudio-0.1.2/mindaudio/utils/common.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/config.py` & `mindaudio-0.1.2/mindaudio/utils/config.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/distributed.py` & `mindaudio-0.1.2/mindaudio/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/hparams.py` & `mindaudio-0.1.2/mindaudio/utils/hparams.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/initializer.py` & `mindaudio-0.1.2/mindaudio/utils/initializer.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/load_files.py` & `mindaudio-0.1.2/mindaudio/utils/load_files.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/log.py` & `mindaudio-0.1.2/mindaudio/utils/log.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/mask.py` & `mindaudio-0.1.2/mindaudio/utils/mask.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/recognize.py` & `mindaudio-0.1.2/mindaudio/utils/recognize.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/text2token.py` & `mindaudio-0.1.2/mindaudio/utils/text2token.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio/utils/train_one_step.py` & `mindaudio-0.1.2/mindaudio/utils/train_one_step.py`

 * *Files identical despite different names*

### Comparing `mindaudio-0.1.1/mindaudio.egg-info/SOURCES.txt` & `mindaudio-0.1.2/mindaudio.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -75,8 +75,14 @@
 mindaudio/utils/initializer.py
 mindaudio/utils/load_files.py
 mindaudio/utils/log.py
 mindaudio/utils/mask.py
 mindaudio/utils/parallel_info.py
 mindaudio/utils/recognize.py
 mindaudio/utils/text2token.py
-mindaudio/utils/train_one_step.py
+mindaudio/utils/train_one_step.py
+tests/test_augment.py
+tests/test_dataio.py
+tests/test_features.py
+tests/test_filters.py
+tests/test_processing.py
+tests/test_spectrum.py
```

