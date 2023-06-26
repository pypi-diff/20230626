# Comparing `tmp/funasr-0.6.2.tar.gz` & `tmp/funasr-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.6.2.tar", last modified: Mon Jun 19 11:14:29 2023, max compression
+gzip compressed data, was "funasr-0.6.3.tar", last modified: Mon Jun 26 06:19:59 2023, max compression
```

## Comparing `funasr-0.6.2.tar` & `funasr-0.6.3.tar`

### file list

```diff
@@ -1,424 +1,427 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.239728 funasr-0.6.2/
--rw-r--r--   0 zhifu      (502) staff       (20)     8149 2023-06-19 11:14:29.239490 funasr-0.6.2/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7149 2023-06-19 09:03:43.000000 funasr-0.6.2/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.562972 funasr-0.6.2/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.634647 funasr-0.6.2/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    69792 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73057 2023-06-19 11:11:09.000000 funasr-0.6.2/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.2/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.6.2/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.2/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17705 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.729439 funasr-0.6.2/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.2/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16062 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.774909 funasr-0.6.2/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.776569 funasr-0.6.2/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.803885 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.813982 funasr-0.6.2/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.2/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.814843 funasr-0.6.2/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.6.2/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.817185 funasr-0.6.2/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.818917 funasr-0.6.2/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.843602 funasr-0.6.2/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.2/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.860967 funasr-0.6.2/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.862253 funasr-0.6.2/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.890828 funasr-0.6.2/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.2/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.892775 funasr-0.6.2/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.895767 funasr-0.6.2/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.914662 funasr-0.6.2/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.918457 funasr-0.6.2/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.918801 funasr-0.6.2/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.921191 funasr-0.6.2/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.960179 funasr-0.6.2/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.2/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.963818 funasr-0.6.2/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18965 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31858 2023-06-13 03:13:40.000000 funasr-0.6.2/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.970556 funasr-0.6.2/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.973388 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.979316 funasr-0.6.2/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11467 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.980319 funasr-0.6.2/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.981100 funasr-0.6.2/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.986016 funasr-0.6.2/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.987214 funasr-0.6.2/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.988886 funasr-0.6.2/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.989583 funasr-0.6.2/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.000054 funasr-0.6.2/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.034597 funasr-0.6.2/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.036570 funasr-0.6.2/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.2/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.069542 funasr-0.6.2/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.2/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.076223 funasr-0.6.2/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.2/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.079243 funasr-0.6.2/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.081119 funasr-0.6.2/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.082875 funasr-0.6.2/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084210 funasr-0.6.2/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084564 funasr-0.6.2/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084891 funasr-0.6.2/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.086040 funasr-0.6.2/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.087466 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.090309 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.093303 funasr-0.6.2/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.096006 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.098650 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.101498 funasr-0.6.2/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.103063 funasr-0.6.2/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.108033 funasr-0.6.2/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.2/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    58550 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21358 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.111063 funasr-0.6.2/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.125732 funasr-0.6.2/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.129411 funasr-0.6.2/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.236653 funasr-0.6.2/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.2/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-19 11:13:21.000000 funasr-0.6.2/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.578277 funasr-0.6.2/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8149 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-19 11:14:29.239788 funasr-0.6.2/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-06 13:50:59.000000 funasr-0.6.2/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.238808 funasr-0.6.2/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.2/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.2/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.2/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.2/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1584 2023-06-19 09:03:43.000000 funasr-0.6.2/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.6.2/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.812091 funasr-0.6.3/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8306 2023-06-26 06:19:59.811848 funasr-0.6.3/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7306 2023-06-21 03:13:45.000000 funasr-0.6.3/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.565702 funasr-0.6.3/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.573589 funasr-0.6.3/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    69796 2023-06-26 06:18:54.000000 funasr-0.6.3/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    70608 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.3/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    11802 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17893 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14489 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8085 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     4991 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    10058 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.3/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3458 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9526 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6614 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12260 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.578359 funasr-0.6.3/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.3/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16711 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8714 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1907 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7941 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.581144 funasr-0.6.3/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.6.3/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.582497 funasr-0.6.3/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.583587 funasr-0.6.3/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.590478 funasr-0.6.3/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.3/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.3/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.590889 funasr-0.6.3/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10882 2023-06-20 02:01:53.000000 funasr-0.6.3/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.592382 funasr-0.6.3/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.3/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.593616 funasr-0.6.3/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.3/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.3/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.595077 funasr-0.6.3/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.3/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.3/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.597244 funasr-0.6.3/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.3/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.3/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.597715 funasr-0.6.3/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.3/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.600715 funasr-0.6.3/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.3/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.601473 funasr-0.6.3/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.3/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.606501 funasr-0.6.3/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.609626 funasr-0.6.3/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.614015 funasr-0.6.3/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.3/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.614405 funasr-0.6.3/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.3/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.617019 funasr-0.6.3/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.666113 funasr-0.6.3/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.3/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.669151 funasr-0.6.3/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.3/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.3/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15723 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11845 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18965 2023-06-19 09:03:43.000000 funasr-0.6.3/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51733 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.3/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.674876 funasr-0.6.3/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.3/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.3/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.3/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.676400 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.679816 funasr-0.6.3/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12621 2023-06-21 03:15:06.000000 funasr-0.6.3/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.680705 funasr-0.6.3/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.3/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.3/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.681085 funasr-0.6.3/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.3/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.681746 funasr-0.6.3/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.682160 funasr-0.6.3/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.683197 funasr-0.6.3/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.683675 funasr-0.6.3/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.690769 funasr-0.6.3/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.3/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.692407 funasr-0.6.3/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.3/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.694880 funasr-0.6.3/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.3/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.695546 funasr-0.6.3/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.3/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.3/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.697341 funasr-0.6.3/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.3/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.3/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.3/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.699469 funasr-0.6.3/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.700742 funasr-0.6.3/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.701862 funasr-0.6.3/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.6.3/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.702525 funasr-0.6.3/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.702764 funasr-0.6.3/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.3/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.702913 funasr-0.6.3/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.3/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.703726 funasr-0.6.3/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.3/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.704415 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.706052 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.709183 funasr-0.6.3/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.712622 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.715278 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1588 2023-06-19 11:16:01.000000 funasr-0.6.3/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.722177 funasr-0.6.3/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.726757 funasr-0.6.3/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.738623 funasr-0.6.3/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.3/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    58550 2023-06-19 09:03:43.000000 funasr-0.6.3/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21358 2023-06-19 09:03:43.000000 funasr-0.6.3/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.747990 funasr-0.6.3/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.758774 funasr-0.6.3/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.3/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.800211 funasr-0.6.3/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.3/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.3/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.808831 funasr-0.6.3/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.6.3/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.3/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.3/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.3/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.3/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-06-06 13:50:59.000000 funasr-0.6.3/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.3/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.3/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.6.3/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.3/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-26 06:19:23.000000 funasr-0.6.3/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.566669 funasr-0.6.3/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8306 2023-06-26 06:19:59.000000 funasr-0.6.3/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13491 2023-06-26 06:19:59.000000 funasr-0.6.3/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-26 06:19:59.000000 funasr-0.6.3/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-26 06:19:59.000000 funasr-0.6.3/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-26 06:19:59.000000 funasr-0.6.3/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-26 06:19:59.812157 funasr-0.6.3/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-26 06:18:54.000000 funasr-0.6.3/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-26 06:19:59.811437 funasr-0.6.3/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.3/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.3/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.3/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.3/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.3/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.3/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.6.2/PKG-INFO` & `funasr-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.2
+Version: 0.6.3
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -110,14 +110,19 @@
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
+
+## Stargazers over time
+
+[![Stargazers over time](https://starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-damo-academy/FunASR)
+
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
   year={2023},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.2 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.3 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -92,17 +92,19 @@
 (https://github.com/RapidAI) for contributing the Paraformer and
 CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
 www.aihealthx.com/) for contributing the websocket service and html5. ##
 License This project is licensed under the [The MIT License](https://
 opensource.org/licenses/MIT). FunASR also contains various third-party
 components and some code modified from other repos under other open source
 licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+MODEL_LICENSE) ## Stargazers over time [![Stargazers over time](https://
+starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-
+damo-academy/FunASR) ## Citations ``` bibtex @inproceedings{gao2023funasr,
+author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi
+and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao
+and Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
 Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
 {gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
 and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
 Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
 Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
 ```
```

### Comparing `funasr-0.6.2/README.md` & `funasr-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,19 @@
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
+
+## Stargazers over time
+
+[![Stargazers over time](https://starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-damo-academy/FunASR)
+
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
   year={2023},
```

#### html2text {}

```diff
@@ -79,17 +79,19 @@
 (https://github.com/RapidAI) for contributing the Paraformer and
 CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
 www.aihealthx.com/) for contributing the websocket service and html5. ##
 License This project is licensed under the [The MIT License](https://
 opensource.org/licenses/MIT). FunASR also contains various third-party
 components and some code modified from other repos under other open source
 licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+MODEL_LICENSE) ## Stargazers over time [![Stargazers over time](https://
+starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-
+damo-academy/FunASR) ## Citations ``` bibtex @inproceedings{gao2023funasr,
+author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi
+and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao
+and Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
 Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
 {gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
 and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
 Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
 Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
 ```
```

### Comparing `funasr-0.6.2/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.6.3/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/asr_infer.py` & `funasr-0.6.3/funasr/bin/asr_infer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,154 +1,133 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
-import logging
-import sys
-import time
+
+import codecs
 import copy
+import logging
 import os
 import re
-import codecs
 import tempfile
-import requests
 from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
-from typing import Any
-from typing import List
 
 import numpy as np
+import requests
 import torch
 from packaging.version import parse as V
 from typeguard import check_argument_types
 from typeguard import check_return_type
-from funasr.fileio.datadir_writer import DatadirWriter
+from  funasr.build_utils.build_model_from_file import build_model_from_file
+from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
+from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.modules.beam_search.beam_search import BeamSearch
-# from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
+from funasr.modules.beam_search.beam_search_sa_asr import Hypothesis as HypothesisSAASR
 from funasr.modules.beam_search.beam_search_transducer import BeamSearchTransducer
 from funasr.modules.beam_search.beam_search_transducer import Hypothesis as HypothesisTransducer
-from funasr.modules.beam_search.beam_search_sa_asr import Hypothesis as HypothesisSAASR
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTask
-from funasr.tasks.lm import LMTask
+from funasr.build_utils.build_asr_model import frontend_choices
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.token_id_converter import TokenIDConverter
 from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
-from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
-from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
-from funasr.bin.tp_infer import Speech2Timestamp
-from funasr.bin.vad_infer import Speech2VadSegment
-from funasr.bin.punc_infer import Text2Punc
-from funasr.utils.vad_utils import slice_padding_fbank
-from funasr.tasks.vad import VADTask
-from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
-from funasr.tasks.asr import frontend_choices
+
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
         >>> audio, rate = soundfile.read("speech.wav")
         >>> speech2text(audio)
         [(text, token, token_int, hypothesis object), ...]
 
     """
-    
+
     def __init__(
-        self,
-        asr_train_config: Union[Path, str] = None,
-        asr_model_file: Union[Path, str] = None,
-        cmvn_file: Union[Path, str] = None,
-        lm_train_config: Union[Path, str] = None,
-        lm_file: Union[Path, str] = None,
-        token_type: str = None,
-        bpemodel: str = None,
-        device: str = "cpu",
-        maxlenratio: float = 0.0,
-        minlenratio: float = 0.0,
-        batch_size: int = 1,
-        dtype: str = "float32",
-        beam_size: int = 20,
-        ctc_weight: float = 0.5,
-        lm_weight: float = 1.0,
-        ngram_weight: float = 0.9,
-        penalty: float = 0.0,
-        nbest: int = 1,
-        streaming: bool = False,
-        frontend_conf: dict = None,
-        **kwargs,
+            self,
+            asr_train_config: Union[Path, str] = None,
+            asr_model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            lm_train_config: Union[Path, str] = None,
+            lm_file: Union[Path, str] = None,
+            token_type: str = None,
+            bpemodel: str = None,
+            device: str = "cpu",
+            maxlenratio: float = 0.0,
+            minlenratio: float = 0.0,
+            batch_size: int = 1,
+            dtype: str = "float32",
+            beam_size: int = 20,
+            ctc_weight: float = 0.5,
+            lm_weight: float = 1.0,
+            ngram_weight: float = 0.9,
+            penalty: float = 0.0,
+            nbest: int = 1,
+            streaming: bool = False,
+            frontend_conf: dict = None,
+            **kwargs,
     ):
         assert check_argument_types()
-        
+
         # 1. Build ASR model
         scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
+        asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             if asr_train_args.frontend == 'wav_frontend':
                 frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
             else:
-                from funasr.tasks.asr import frontend_choices
                 frontend_class = frontend_choices.get_class(asr_train_args.frontend)
                 frontend = frontend_class(**asr_train_args.frontend_conf).eval()
-        
+
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
-        
+
         decoder = asr_model.decoder
-        
+
         ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
         token_list = asr_model.token_list
         scorers.update(
             decoder=decoder,
             ctc=ctc,
             length_bonus=LengthBonus(len(token_list)),
         )
-        
+
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
+            lm, lm_train_args = build_model_from_file(
                 lm_train_config, lm_file, None, device
             )
             scorers["lm"] = lm.lm
-        
+
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
-        
+
         # 4. Build BeamSearch object
         # transducer is not supported now
         beam_search_transducer = None
         from funasr.modules.beam_search.beam_search import BeamSearch
-        
+
         weights = dict(
             decoder=1.0 - ctc_weight,
             ctc=ctc_weight,
             lm=lm_weight,
             ngram=ngram_weight,
             length_bonus=penalty,
         )
@@ -158,49 +137,49 @@
             scorers=scorers,
             sos=asr_model.sos,
             eos=asr_model.eos,
             vocab_size=len(token_list),
             token_list=token_list,
             pre_beam_score_key=None if ctc_weight == 1.0 else "full",
         )
-        
+
         # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
-        
+
         if token_type is None:
             tokenizer = None
         elif token_type == "bpe":
             if bpemodel is not None:
                 tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
             else:
                 tokenizer = None
         else:
             tokenizer = build_tokenizer(token_type=token_type)
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
-        
+
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
         self.beam_search = beam_search
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
         self.frontend = frontend
-    
+
     @torch.no_grad()
     def __call__(
-        self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
     ) -> List[
         Tuple[
             Optional[str],
             List[str],
             List[int],
             Union[Hypothesis],
         ]
@@ -210,72 +189,73 @@
         Args:
             speech: Input speech data
         Returns:
             text, token, token_int, hyp
 
         """
         assert check_argument_types()
-        
+
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
-        
+
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             self.asr_model.frontend = None
         else:
             feats = speech
             feats_len = speech_lengths
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
         batch = {"speech": feats, "speech_lengths": feats_len}
-        
+
         # a. To device
         batch = to_device(batch, device=self.device)
-        
+
         # b. Forward Encoder
         enc, _ = self.asr_model.encode(**batch)
         if isinstance(enc, tuple):
             enc = enc[0]
         assert len(enc) == 1, len(enc)
-        
+
         # c. Passed the encoder result and the beam search
         nbest_hyps = self.beam_search(
             x=enc[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
         )
-        
+
         nbest_hyps = nbest_hyps[: self.nbest]
-        
+
         results = []
         for hyp in nbest_hyps:
             assert isinstance(hyp, (Hypothesis)), type(hyp)
-            
+
             # remove sos/eos and get results
             last_pos = -1
             if isinstance(hyp.yseq, list):
                 token_int = hyp.yseq[1:last_pos]
             else:
                 token_int = hyp.yseq[1:last_pos].tolist()
-            
+
             # remove blank symbol id, which is assumed to be 0
             token_int = list(filter(lambda x: x != 0, token_int))
-            
+
             # Change integer-ids to tokens
             token = self.converter.ids2tokens(token_int)
-            
+
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
-        
+
         assert check_return_type(results)
         return results
 
+
 class Speech2TextParaformer:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
             >>> speech2text = Speech2TextParaformer("asr_config.yml", "asr.pb")
             >>> audio, rate = soundfile.read("speech.wav")
@@ -308,17 +288,16 @@
             decoding_ind: int = 0,
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
-        from funasr.tasks.asr import ASRTaskParaformer as ASRTask
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        asr_model, asr_train_args = build_model_from_file(
+            asr_train_config, asr_model_file, cmvn_file, device, mode="paraformer"
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
@@ -332,16 +311,16 @@
         token_list = asr_model.token_list
         scorers.update(
             length_bonus=LengthBonus(len(token_list)),
         )
 
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, None, device, task_name="lm"
             )
             scorers["lm"] = lm.lm
 
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
@@ -394,14 +373,15 @@
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
 
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
+        self.cmvn_file = cmvn_file
 
         # 6. [Optional] Build hotword list from str, local file or url
         self.hotword_list = None
         self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
 
         is_use_lm = lm_weight != 0.0 and lm_file is not None
         if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
@@ -462,26 +442,29 @@
 
         predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
                                                                         predictor_outs[2], predictor_outs[3]
         pre_token_length = pre_token_length.round().long()
         if torch.max(pre_token_length) < 1:
             return []
-        if not isinstance(self.asr_model, ContextualParaformer) and not isinstance(self.asr_model, NeatContextualParaformer):
+        if not isinstance(self.asr_model, ContextualParaformer) and not isinstance(self.asr_model,
+                                                                                   NeatContextualParaformer):
             if self.hotword_list:
                 logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
+            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds,
+                                                                     pre_token_length)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
         else:
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
+            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds,
+                                                                     pre_token_length, hw_list=self.hotword_list)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
 
         if isinstance(self.asr_model, BiCifParaformer):
             _, _, us_alphas, us_peaks = self.asr_model.calc_predictor_timestamp(enc, enc_len,
-                                                                                   pre_token_length)  # test no bias cif2
+                                                                                pre_token_length)  # test no bias cif2
 
         results = []
         b, n, d = decoder_out.size()
         for i in range(b):
             x = enc[i, :enc_len[i], :]
             am_scores = decoder_out[i, :pre_token_length[i], :]
             if self.beam_search is not None:
@@ -523,38 +506,78 @@
 
                 if self.tokenizer is not None:
                     text = self.tokenizer.tokens2text(token)
                 else:
                     text = None
                 timestamp = []
                 if isinstance(self.asr_model, BiCifParaformer):
-                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i][:enc_len[i]*3], 
-                                                            us_peaks[i][:enc_len[i]*3], 
-                                                            copy.copy(token), 
-                                                            vad_offset=begin_time)
+                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i][:enc_len[i] * 3],
+                                                               us_peaks[i][:enc_len[i] * 3],
+                                                               copy.copy(token),
+                                                               vad_offset=begin_time)
                 results.append((text, token, token_int, hyp, timestamp, enc_len_batch_total, lfr_factor))
 
-
         # assert check_return_type(results)
         return results
 
     def generate_hotwords_list(self, hotword_list_or_file):
+        def load_seg_dict(seg_dict_file):
+            seg_dict = {}
+            assert isinstance(seg_dict_file, str)
+            with open(seg_dict_file, "r", encoding="utf8") as f:
+                lines = f.readlines()
+                for line in lines:
+                    s = line.strip().split()
+                    key = s[0]
+                    value = s[1:]
+                    seg_dict[key] = " ".join(value)
+            return seg_dict
+
+        def seg_tokenize(txt, seg_dict):
+            pattern = re.compile(r'^[\u4E00-\u9FA50-9]+$')
+            out_txt = ""
+            for word in txt:
+                word = word.lower()
+                if word in seg_dict:
+                    out_txt += seg_dict[word] + " "
+                else:
+                    if pattern.match(word):
+                        for char in word:
+                            if char in seg_dict:
+                                out_txt += seg_dict[char] + " "
+                            else:
+                                out_txt += "<unk>" + " "
+                    else:
+                        out_txt += "<unk>" + " "
+            return out_txt.strip().split()
+
+        seg_dict = None
+        if self.cmvn_file is not None:
+            model_dir = os.path.dirname(self.cmvn_file)
+            seg_dict_file = os.path.join(model_dir, 'seg_dict')
+            if os.path.exists(seg_dict_file):
+                seg_dict = load_seg_dict(seg_dict_file)
+            else:
+                seg_dict = None
         # for None
         if hotword_list_or_file is None:
             hotword_list = None
         # for local txt inputs
         elif os.path.exists(hotword_list_or_file) and hotword_list_or_file.endswith('.txt'):
             logging.info("Attempting to parse hotwords from local txt...")
             hotword_list = []
             hotword_str_list = []
             with codecs.open(hotword_list_or_file, 'r') as fin:
                 for line in fin.readlines():
                     hw = line.strip()
+                    hw_list = hw.split()
+                    if seg_dict is not None:
+                        hw_list = seg_tokenize(hw_list, seg_dict)
                     hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+                    hotword_list.append(self.converter.tokens2ids(hw_list))
                 hotword_list.append([self.asr_model.sos])
                 hotword_str_list.append('<s>')
             logging.info("Initialized hotword list from file: {}, hotword list: {}."
                          .format(hotword_list_or_file, hotword_str_list))
         # for url, download and generate txt
         elif hotword_list_or_file.startswith('http'):
             logging.info("Attempting to parse hotwords from url...")
@@ -566,35 +589,42 @@
             open(text_file_path, "wb").write(local_file.content)
             hotword_list_or_file = text_file_path
             hotword_list = []
             hotword_str_list = []
             with codecs.open(hotword_list_or_file, 'r') as fin:
                 for line in fin.readlines():
                     hw = line.strip()
+                    hw_list = hw.split()
+                    if seg_dict is not None:
+                        hw_list = seg_tokenize(hw_list, seg_dict)
                     hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+                    hotword_list.append(self.converter.tokens2ids(hw_list))
                 hotword_list.append([self.asr_model.sos])
                 hotword_str_list.append('<s>')
             logging.info("Initialized hotword list from file: {}, hotword list: {}."
                          .format(hotword_list_or_file, hotword_str_list))
         # for text str input
         elif not hotword_list_or_file.endswith('.txt'):
             logging.info("Attempting to parse hotwords as str...")
             hotword_list = []
             hotword_str_list = []
             for hw in hotword_list_or_file.strip().split():
                 hotword_str_list.append(hw)
-                hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+                hw_list = hw.strip().split()
+                if seg_dict is not None:
+                    hw_list = seg_tokenize(hw_list, seg_dict)
+                hotword_list.append(self.converter.tokens2ids(hw_list))
             hotword_list.append([self.asr_model.sos])
             hotword_str_list.append('<s>')
             logging.info("Hotword list: {}.".format(hotword_str_list))
         else:
             hotword_list = None
         return hotword_list
 
+
 class Speech2TextParaformerOnline:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
             >>> speech2text = Speech2TextParaformerOnline("asr_config.yml", "asr.pth")
             >>> audio, rate = soundfile.read("speech.wav")
@@ -626,17 +656,16 @@
             hotword_list_or_file: str = None,
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
-        from funasr.tasks.asr import ASRTaskParaformer as ASRTask
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        asr_model, asr_train_args = build_model_from_file(
+            asr_train_config, asr_model_file, cmvn_file, device, mode="paraformer"
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontendOnline(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
@@ -650,16 +679,16 @@
         token_list = asr_model.token_list
         scorers.update(
             length_bonus=LengthBonus(len(token_list)),
         )
 
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, None, device, task_name="lm"
             )
             scorers["lm"] = lm.lm
 
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
@@ -785,15 +814,15 @@
         enc, enc_len = self.asr_model.encode_chunk(feats, feats_len, cache=cache)
         if isinstance(enc, tuple):
             enc = enc[0]
         # assert len(enc) == 1, len(enc)
         enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
 
         predictor_outs = self.asr_model.calc_predictor_chunk(enc, cache)
-        pre_acoustic_embeds, pre_token_length= predictor_outs[0], predictor_outs[1]
+        pre_acoustic_embeds, pre_token_length = predictor_outs[0], predictor_outs[1]
         if torch.max(pre_token_length) < 1:
             return []
         decoder_outs = self.asr_model.cal_decoder_with_predictor_chunk(enc, pre_acoustic_embeds, cache)
         decoder_out = decoder_outs
 
         results = []
         b, n, d = decoder_out.size()
@@ -835,20 +864,21 @@
                 for item in token:
                     if item.endswith('@@'):
                         postprocessed_result += item[:-2]
                     elif re.match('^[a-zA-Z]+$', item):
                         postprocessed_result += item + " "
                     else:
                         postprocessed_result += item
-                        
+
                 results.append(postprocessed_result)
 
         # assert check_return_type(results)
         return results
 
+
 class Speech2TextUniASR:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2TextUniASR("asr_config.yml", "asr.pb")
         >>> audio, rate = soundfile.read("speech.wav")
@@ -882,17 +912,16 @@
             frontend_conf: dict = None,
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
-        from funasr.tasks.asr import ASRTaskUniASR as ASRTask
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+        asr_model, asr_train_args = build_model_from_file(
+            asr_train_config, asr_model_file, cmvn_file, device, mode="uniasr"
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
@@ -910,16 +939,16 @@
         scorers.update(
             decoder=decoder,
             length_bonus=LengthBonus(len(token_list)),
         )
 
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, device, "lm"
             )
             scorers["lm"] = lm.lm
 
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
@@ -1073,90 +1102,89 @@
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
 
         assert check_return_type(results)
         return results
-   
+
 
 class Speech2TextMFCCA:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2TextMFCCA("asr_config.yml", "asr.pb")
         >>> audio, rate = soundfile.read("speech.wav")
         >>> speech2text(audio)
         [(text, token, token_int, hypothesis object), ...]
 
     """
-    
+
     def __init__(
-        self,
-        asr_train_config: Union[Path, str] = None,
-        asr_model_file: Union[Path, str] = None,
-        cmvn_file: Union[Path, str] = None,
-        lm_train_config: Union[Path, str] = None,
-        lm_file: Union[Path, str] = None,
-        token_type: str = None,
-        bpemodel: str = None,
-        device: str = "cpu",
-        maxlenratio: float = 0.0,
-        minlenratio: float = 0.0,
-        batch_size: int = 1,
-        dtype: str = "float32",
-        beam_size: int = 20,
-        ctc_weight: float = 0.5,
-        lm_weight: float = 1.0,
-        ngram_weight: float = 0.9,
-        penalty: float = 0.0,
-        nbest: int = 1,
-        streaming: bool = False,
-        **kwargs,
+            self,
+            asr_train_config: Union[Path, str] = None,
+            asr_model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            lm_train_config: Union[Path, str] = None,
+            lm_file: Union[Path, str] = None,
+            token_type: str = None,
+            bpemodel: str = None,
+            device: str = "cpu",
+            maxlenratio: float = 0.0,
+            minlenratio: float = 0.0,
+            batch_size: int = 1,
+            dtype: str = "float32",
+            beam_size: int = 20,
+            ctc_weight: float = 0.5,
+            lm_weight: float = 1.0,
+            ngram_weight: float = 0.9,
+            penalty: float = 0.0,
+            nbest: int = 1,
+            streaming: bool = False,
+            **kwargs,
     ):
         assert check_argument_types()
-        
+
         # 1. Build ASR model
-        from funasr.tasks.asr import ASRTaskMFCCA as ASRTask
         scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
+        asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
-        
+
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
-        
+
         decoder = asr_model.decoder
-        
+
         ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
         token_list = asr_model.token_list
         scorers.update(
             decoder=decoder,
             ctc=ctc,
             length_bonus=LengthBonus(len(token_list)),
         )
-        
+
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, None, device, task_name="lm"
             )
             lm.to(device)
             scorers["lm"] = lm.lm
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
-        
+
         # 4. Build BeamSearch object
         # transducer is not supported now
         beam_search_transducer = None
-        
+
         weights = dict(
             decoder=1.0 - ctc_weight,
             ctc=ctc_weight,
             lm=lm_weight,
             ngram=ngram_weight,
             length_bonus=penalty,
         )
@@ -1172,42 +1200,42 @@
         )
         # beam_search.__class__ = BatchBeamSearch
         # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
-        
+
         if token_type is None:
             tokenizer = None
         elif token_type == "bpe":
             if bpemodel is not None:
                 tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
             else:
                 tokenizer = None
         else:
             tokenizer = build_tokenizer(token_type=token_type)
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
-        
+
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
         self.beam_search = beam_search
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
-    
+
     @torch.no_grad()
     def __call__(
-        self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
     ) -> List[
         Tuple[
             Optional[str],
             List[str],
             List[int],
             Union[Hypothesis],
         ]
@@ -1227,53 +1255,53 @@
         if (speech.dim() == 3):
             speech = torch.squeeze(speech, 2)
         # speech = speech.unsqueeze(0).to(getattr(torch, self.dtype))
         speech = speech.to(getattr(torch, self.dtype))
         # lenghts: (1,)
         lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
         batch = {"speech": speech, "speech_lengths": lengths}
-        
+
         # a. To device
         batch = to_device(batch, device=self.device)
-        
+
         # b. Forward Encoder
         enc, _ = self.asr_model.encode(**batch)
-        
+
         assert len(enc) == 1, len(enc)
-        
+
         # c. Passed the encoder result and the beam search
         nbest_hyps = self.beam_search(
             x=enc[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
         )
-        
+
         nbest_hyps = nbest_hyps[: self.nbest]
-        
+
         results = []
         for hyp in nbest_hyps:
             assert isinstance(hyp, (Hypothesis)), type(hyp)
-            
+
             # remove sos/eos and get results
             last_pos = -1
             if isinstance(hyp.yseq, list):
                 token_int = hyp.yseq[1:last_pos]
             else:
                 token_int = hyp.yseq[1:last_pos].tolist()
-            
+
             # remove blank symbol id, which is assumed to be 0
             token_int = list(filter(lambda x: x != 0, token_int))
-            
+
             # Change integer-ids to tokens
             token = self.converter.ids2tokens(token_int)
-            
+
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
-        
+
         assert check_return_type(results)
         return results
 
 
 class Speech2TextTransducer:
     """Speech2Text class for Transducer models.
     Args:
@@ -1294,172 +1322,171 @@
         nbest: Number of final hypothesis.
         streaming: Whether to perform chunk-by-chunk inference.
         chunk_size: Number of frames in chunk AFTER subsampling.
         left_context: Number of frames in left context AFTER subsampling.
         right_context: Number of frames in right context AFTER subsampling.
         display_partial_hypotheses: Whether to display partial hypotheses.
     """
-    
+
     def __init__(
-        self,
-        asr_train_config: Union[Path, str] = None,
-        asr_model_file: Union[Path, str] = None,
-        cmvn_file: Union[Path, str] = None,
-        beam_search_config: Dict[str, Any] = None,
-        lm_train_config: Union[Path, str] = None,
-        lm_file: Union[Path, str] = None,
-        token_type: str = None,
-        bpemodel: str = None,
-        device: str = "cpu",
-        beam_size: int = 5,
-        dtype: str = "float32",
-        lm_weight: float = 1.0,
-        quantize_asr_model: bool = False,
-        quantize_modules: List[str] = None,
-        quantize_dtype: str = "qint8",
-        nbest: int = 1,
-        streaming: bool = False,
-        simu_streaming: bool = False,
-        chunk_size: int = 16,
-        left_context: int = 32,
-        right_context: int = 0,
-        display_partial_hypotheses: bool = False,
+            self,
+            asr_train_config: Union[Path, str] = None,
+            asr_model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            beam_search_config: Dict[str, Any] = None,
+            lm_train_config: Union[Path, str] = None,
+            lm_file: Union[Path, str] = None,
+            token_type: str = None,
+            bpemodel: str = None,
+            device: str = "cpu",
+            beam_size: int = 5,
+            dtype: str = "float32",
+            lm_weight: float = 1.0,
+            quantize_asr_model: bool = False,
+            quantize_modules: List[str] = None,
+            quantize_dtype: str = "qint8",
+            nbest: int = 1,
+            streaming: bool = False,
+            simu_streaming: bool = False,
+            chunk_size: int = 16,
+            left_context: int = 32,
+            right_context: int = 0,
+            display_partial_hypotheses: bool = False,
     ) -> None:
         """Construct a Speech2Text object."""
         super().__init__()
-        
+
         assert check_argument_types()
-        from funasr.tasks.asr import ASRTransducerTask
-        asr_model, asr_train_args = ASRTransducerTask.build_model_from_file(
+        asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
-        
+
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-        
+
         if quantize_asr_model:
             if quantize_modules is not None:
                 if not all([q in ["LSTM", "Linear"] for q in quantize_modules]):
                     raise ValueError(
                         "Only 'Linear' and 'LSTM' modules are currently supported"
                         " by PyTorch and in --quantize_modules"
                     )
-                
+
                 q_config = set([getattr(torch.nn, q) for q in quantize_modules])
             else:
                 q_config = {torch.nn.Linear}
-            
+
             if quantize_dtype == "float16" and (V(torch.__version__) < V("1.5.0")):
                 raise ValueError(
                     "float16 dtype for dynamic quantization is not supported with torch"
                     " version < 1.5.0. Switching to qint8 dtype instead."
                 )
             q_dtype = getattr(torch, quantize_dtype)
-            
+
             asr_model = torch.quantization.quantize_dynamic(
                 asr_model, q_config, dtype=q_dtype
             ).eval()
         else:
             asr_model.to(dtype=getattr(torch, dtype)).eval()
-        
+
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, None, device, task_name="lm"
             )
             lm_scorer = lm.lm
         else:
             lm_scorer = None
-        
+
         # 4. Build BeamSearch object
         if beam_search_config is None:
             beam_search_config = {}
-        
+
         beam_search = BeamSearchTransducer(
             asr_model.decoder,
             asr_model.joint_network,
             beam_size,
             lm=lm_scorer,
             lm_weight=lm_weight,
             nbest=nbest,
             **beam_search_config,
         )
-        
+
         token_list = asr_model.token_list
-        
+
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
-        
+
         if token_type is None:
             tokenizer = None
         elif token_type == "bpe":
             if bpemodel is not None:
                 tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
             else:
                 tokenizer = None
         else:
             tokenizer = build_tokenizer(token_type=token_type)
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
-        
+
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
-        
+
         self.converter = converter
         self.tokenizer = tokenizer
-        
+
         self.beam_search = beam_search
         self.streaming = streaming
         self.simu_streaming = simu_streaming
         self.chunk_size = max(chunk_size, 0)
         self.left_context = left_context
         self.right_context = max(right_context, 0)
-        
+
         if not streaming or chunk_size == 0:
             self.streaming = False
             self.asr_model.encoder.dynamic_chunk_training = False
-        
+
         if not simu_streaming or chunk_size == 0:
             self.simu_streaming = False
             self.asr_model.encoder.dynamic_chunk_training = False
-        
+
         self.frontend = frontend
         self.window_size = self.chunk_size + self.right_context
-        
+
         if self.streaming:
             self._ctx = self.asr_model.encoder.get_encoder_input_size(
                 self.window_size
             )
-            
+
             self.last_chunk_length = (
-                self.asr_model.encoder.embed.min_frame_length + self.right_context + 1
+                    self.asr_model.encoder.embed.min_frame_length + self.right_context + 1
             )
             self.reset_inference_cache()
-    
+
     def reset_inference_cache(self) -> None:
         """Reset Speech2Text parameters."""
         self.frontend_cache = None
-        
+
         self.asr_model.encoder.reset_streaming_cache(
             self.left_context, device=self.device
         )
         self.beam_search.reset_inference_cache()
-        
+
         self.num_processed_frames = torch.tensor([[0]], device=self.device)
-    
+
     @torch.no_grad()
     def streaming_decode(
-        self,
-        speech: Union[torch.Tensor, np.ndarray],
-        is_final: bool = True,
+            self,
+            speech: Union[torch.Tensor, np.ndarray],
+            is_final: bool = True,
     ) -> List[HypothesisTransducer]:
         """Speech2Text streaming call.
         Args:
             speech: Chunk of speech data. (S)
             is_final: Whether speech corresponds to the final chunk of data.
         Returns:
             nbest_hypothesis: N-best hypothesis.
@@ -1469,238 +1496,237 @@
         if is_final:
             if self.streaming and speech.size(0) < self.last_chunk_length:
                 pad = torch.zeros(
                     self.last_chunk_length - speech.size(0), speech.size(1), dtype=speech.dtype
                 )
                 speech = torch.cat([speech, pad],
                                    dim=0)  # feats, feats_length = self.apply_frontend(speech, is_final=is_final)
-        
+
         feats = speech.unsqueeze(0).to(getattr(torch, self.dtype))
         feats_lengths = feats.new_full([1], dtype=torch.long, fill_value=feats.size(1))
-        
+
         if self.asr_model.normalize is not None:
             feats, feats_lengths = self.asr_model.normalize(feats, feats_lengths)
-        
+
         feats = to_device(feats, device=self.device)
         feats_lengths = to_device(feats_lengths, device=self.device)
         enc_out = self.asr_model.encoder.chunk_forward(
             feats,
             feats_lengths,
             self.num_processed_frames,
             chunk_size=self.chunk_size,
             left_context=self.left_context,
             right_context=self.right_context,
         )
         nbest_hyps = self.beam_search(enc_out[0], is_final=is_final)
-        
+
         self.num_processed_frames += self.chunk_size
-        
+
         if is_final:
             self.reset_inference_cache()
-        
+
         return nbest_hyps
-    
+
     @torch.no_grad()
     def simu_streaming_decode(self, speech: Union[torch.Tensor, np.ndarray]) -> List[HypothesisTransducer]:
         """Speech2Text call.
         Args:
             speech: Speech data. (S)
         Returns:
             nbest_hypothesis: N-best hypothesis.
         """
         assert check_argument_types()
-        
+
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
-        
+
         if self.frontend is not None:
             speech = torch.unsqueeze(speech, axis=0)
             speech_lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
             feats, feats_lengths = self.frontend(speech, speech_lengths)
-        else:                
+        else:
             feats = speech.unsqueeze(0).to(getattr(torch, self.dtype))
             feats_lengths = feats.new_full([1], dtype=torch.long, fill_value=feats.size(1))
-        
+
         if self.asr_model.normalize is not None:
             feats, feats_lengths = self.asr_model.normalize(feats, feats_lengths)
-        
+
         feats = to_device(feats, device=self.device)
         feats_lengths = to_device(feats_lengths, device=self.device)
         enc_out = self.asr_model.encoder.simu_chunk_forward(feats, feats_lengths, self.chunk_size, self.left_context,
                                                             self.right_context)
         nbest_hyps = self.beam_search(enc_out[0])
-        
+
         return nbest_hyps
-    
+
     @torch.no_grad()
     def __call__(self, speech: Union[torch.Tensor, np.ndarray]) -> List[HypothesisTransducer]:
         """Speech2Text call.
         Args:
             speech: Speech data. (S)
         Returns:
             nbest_hypothesis: N-best hypothesis.
         """
         assert check_argument_types()
-        
+
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
 
         if self.frontend is not None:
             speech = torch.unsqueeze(speech, axis=0)
             speech_lengths = speech.new_full([1], dtype=torch.long, fill_value=speech.size(1))
             feats, feats_lengths = self.frontend(speech, speech_lengths)
-        else:                
+        else:
             feats = speech.unsqueeze(0).to(getattr(torch, self.dtype))
             feats_lengths = feats.new_full([1], dtype=torch.long, fill_value=feats.size(1))
-        
+
         feats = to_device(feats, device=self.device)
         feats_lengths = to_device(feats_lengths, device=self.device)
-        
+
         enc_out, _, _ = self.asr_model.encoder(feats, feats_lengths)
-        
+
         nbest_hyps = self.beam_search(enc_out[0])
-        
+
         return nbest_hyps
-    
+
     def hypotheses_to_results(self, nbest_hyps: List[HypothesisTransducer]) -> List[Any]:
         """Build partial or final results from the hypotheses.
         Args:
             nbest_hyps: N-best hypothesis.
         Returns:
             results: Results containing different representation for the hypothesis.
         """
         results = []
-        
+
         for hyp in nbest_hyps:
             token_int = list(filter(lambda x: x != 0, hyp.yseq))
-            
+
             token = self.converter.ids2tokens(token_int)
-            
+
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
             results.append((text, token, token_int, hyp))
-            
+
             assert check_return_type(results)
-        
+
         return results
-    
+
     @staticmethod
     def from_pretrained(
-        model_tag: Optional[str] = None,
-        **kwargs: Optional[Any],
+            model_tag: Optional[str] = None,
+            **kwargs: Optional[Any],
     ) -> Speech2Text:
         """Build Speech2Text instance from the pretrained model.
         Args:
             model_tag: Model tag of the pretrained models.
         Return:
             : Speech2Text instance.
         """
         if model_tag is not None:
             try:
                 from espnet_model_zoo.downloader import ModelDownloader
-            
+
             except ImportError:
                 logging.error(
                     "`espnet_model_zoo` is not installed. "
                     "Please install via `pip install -U espnet_model_zoo`."
                 )
                 raise
             d = ModelDownloader()
             kwargs.update(**d.download_and_unpack(model_tag))
-        
+
         return Speech2TextTransducer(**kwargs)
 
 
 class Speech2TextSAASR:
     """Speech2Text class
 
     Examples:
         >>> import soundfile
         >>> speech2text = Speech2TextSAASR("asr_config.yml", "asr.pb")
         >>> audio, rate = soundfile.read("speech.wav")
         >>> speech2text(audio)
         [(text, token, token_int, hypothesis object), ...]
 
     """
-    
+
     def __init__(
-        self,
-        asr_train_config: Union[Path, str] = None,
-        asr_model_file: Union[Path, str] = None,
-        cmvn_file: Union[Path, str] = None,
-        lm_train_config: Union[Path, str] = None,
-        lm_file: Union[Path, str] = None,
-        token_type: str = None,
-        bpemodel: str = None,
-        device: str = "cpu",
-        maxlenratio: float = 0.0,
-        minlenratio: float = 0.0,
-        batch_size: int = 1,
-        dtype: str = "float32",
-        beam_size: int = 20,
-        ctc_weight: float = 0.5,
-        lm_weight: float = 1.0,
-        ngram_weight: float = 0.9,
-        penalty: float = 0.0,
-        nbest: int = 1,
-        streaming: bool = False,
-        frontend_conf: dict = None,
-        **kwargs,
+            self,
+            asr_train_config: Union[Path, str] = None,
+            asr_model_file: Union[Path, str] = None,
+            cmvn_file: Union[Path, str] = None,
+            lm_train_config: Union[Path, str] = None,
+            lm_file: Union[Path, str] = None,
+            token_type: str = None,
+            bpemodel: str = None,
+            device: str = "cpu",
+            maxlenratio: float = 0.0,
+            minlenratio: float = 0.0,
+            batch_size: int = 1,
+            dtype: str = "float32",
+            beam_size: int = 20,
+            ctc_weight: float = 0.5,
+            lm_weight: float = 1.0,
+            ngram_weight: float = 0.9,
+            penalty: float = 0.0,
+            nbest: int = 1,
+            streaming: bool = False,
+            frontend_conf: dict = None,
+            **kwargs,
     ):
         assert check_argument_types()
-        
+
         # 1. Build ASR model
-        from funasr.tasks.asr import ASRTaskSAASR
         scorers = {}
-        asr_model, asr_train_args = ASRTaskSAASR.build_model_from_file(
+        asr_model, asr_train_args = build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
             from funasr.tasks.sa_asr import frontend_choices
             if asr_train_args.frontend == 'wav_frontend' or asr_train_args.frontend == "multichannelfrontend":
                 frontend_class = frontend_choices.get_class(asr_train_args.frontend)
                 frontend = frontend_class(cmvn_file=cmvn_file, **asr_train_args.frontend_conf).eval()
             else:
                 frontend_class = frontend_choices.get_class(asr_train_args.frontend)
                 frontend = frontend_class(**asr_train_args.frontend_conf).eval()
-        
+
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
-        
+
         decoder = asr_model.decoder
-        
+
         ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
         token_list = asr_model.token_list
         scorers.update(
             decoder=decoder,
             ctc=ctc,
             length_bonus=LengthBonus(len(token_list)),
         )
-        
+
         # 2. Build Language model
         if lm_train_config is not None:
-            lm, lm_train_args = LMTask.build_model_from_file(
-                lm_train_config, lm_file, None, device
+            lm, lm_train_args = build_model_from_file(
+                lm_train_config, lm_file, None, device, task_name="lm"
             )
             scorers["lm"] = lm.lm
-        
+
         # 3. Build ngram model
         # ngram is not supported now
         ngram = None
         scorers["ngram"] = ngram
-        
+
         # 4. Build BeamSearch object
         # transducer is not supported now
         beam_search_transducer = None
         from funasr.modules.beam_search.beam_search_sa_asr import BeamSearch
-        
+
         weights = dict(
             decoder=1.0 - ctc_weight,
             ctc=ctc_weight,
             lm=lm_weight,
             ngram=ngram_weight,
             length_bonus=penalty,
         )
@@ -1710,50 +1736,50 @@
             scorers=scorers,
             sos=asr_model.sos,
             eos=asr_model.eos,
             vocab_size=len(token_list),
             token_list=token_list,
             pre_beam_score_key=None if ctc_weight == 1.0 else "full",
         )
-        
+
         # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
         if token_type is None:
             token_type = asr_train_args.token_type
         if bpemodel is None:
             bpemodel = asr_train_args.bpemodel
-        
+
         if token_type is None:
             tokenizer = None
         elif token_type == "bpe":
             if bpemodel is not None:
                 tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
             else:
                 tokenizer = None
         else:
             tokenizer = build_tokenizer(token_type=token_type)
         converter = TokenIDConverter(token_list=token_list)
         logging.info(f"Text tokenizer: {tokenizer}")
-        
+
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
         self.beam_search = beam_search
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
         self.frontend = frontend
-    
+
     @torch.no_grad()
     def __call__(
-        self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray],
-        profile: Union[torch.Tensor, np.ndarray], profile_lengths: Union[torch.Tensor, np.ndarray]
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray],
+            profile: Union[torch.Tensor, np.ndarray], profile_lengths: Union[torch.Tensor, np.ndarray]
     ) -> List[
         Tuple[
             Optional[str],
             Optional[str],
             List[str],
             List[int],
             Union[HypothesisSAASR],
@@ -1764,101 +1790,101 @@
         Args:
             speech: Input speech data
         Returns:
             text, text_id, token, token_int, hyp
 
         """
         assert check_argument_types()
-        
+
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
-        
+
         if isinstance(profile, np.ndarray):
             profile = torch.tensor(profile)
-        
+
         if self.frontend is not None:
             feats, feats_len = self.frontend.forward(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             self.asr_model.frontend = None
         else:
             feats = speech
             feats_len = speech_lengths
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
         batch = {"speech": feats, "speech_lengths": feats_len}
-        
+
         # a. To device
         batch = to_device(batch, device=self.device)
-        
+
         # b. Forward Encoder
         asr_enc, _, spk_enc = self.asr_model.encode(**batch)
         if isinstance(asr_enc, tuple):
             asr_enc = asr_enc[0]
         if isinstance(spk_enc, tuple):
             spk_enc = spk_enc[0]
         assert len(asr_enc) == 1, len(asr_enc)
         assert len(spk_enc) == 1, len(spk_enc)
-        
+
         # c. Passed the encoder result and the beam search
         nbest_hyps = self.beam_search(
             asr_enc[0], spk_enc[0], profile[0], maxlenratio=self.maxlenratio, minlenratio=self.minlenratio
         )
-        
+
         nbest_hyps = nbest_hyps[: self.nbest]
-        
+
         results = []
         for hyp in nbest_hyps:
             assert isinstance(hyp, (HypothesisSAASR)), type(hyp)
-            
+
             # remove sos/eos and get results
             last_pos = -1
             if isinstance(hyp.yseq, list):
                 token_int = hyp.yseq[1: last_pos]
             else:
                 token_int = hyp.yseq[1: last_pos].tolist()
-            
+
             spk_weigths = torch.stack(hyp.spk_weigths, dim=0)
-            
+
             token_ori = self.converter.ids2tokens(token_int)
             text_ori = self.tokenizer.tokens2text(token_ori)
-            
+
             text_ori_spklist = text_ori.split('$')
             cur_index = 0
             spk_choose = []
             for i in range(len(text_ori_spklist)):
                 text_ori_split = text_ori_spklist[i]
                 n = len(text_ori_split)
                 spk_weights_local = spk_weigths[cur_index: cur_index + n]
                 cur_index = cur_index + n + 1
                 spk_weights_local = spk_weights_local.mean(dim=0)
                 spk_choose_local = spk_weights_local.argmax(-1)
                 spk_choose.append(spk_choose_local.item() + 1)
-            
+
             # remove blank symbol id, which is assumed to be 0
             token_int = list(filter(lambda x: x != 0, token_int))
-            
+
             # Change integer-ids to tokens
             token = self.converter.ids2tokens(token_int)
-            
+
             if self.tokenizer is not None:
                 text = self.tokenizer.tokens2text(token)
             else:
                 text = None
-            
+
             text_spklist = text.split('$')
             assert len(spk_choose) == len(text_spklist)
-            
+
             spk_list = []
             for i in range(len(text_spklist)):
                 text_split = text_spklist[i]
                 n = len(text_split)
                 spk_list.append(str(spk_choose[i]) * n)
-            
+
             text_id = '$'.join(spk_list)
-            
+
             assert len(text) == len(text_id)
-            
+
             results.append((text, text_id, token, token_int, hyp))
-        
+
         assert check_return_type(results)
         return results
```

### Comparing `funasr-0.6.2/funasr/bin/asr_inference_launch.py` & `funasr-0.6.3/funasr/bin/asr_inference_launch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,146 +1,114 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-
-#!/usr/bin/env python3
-import argparse
-import logging
-import sys
 import time
-import copy
-import os
-import codecs
-import tempfile
-import requests
 from pathlib import Path
+from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
-from typing import Any
-from typing import List
-import yaml
+
 import numpy as np
 import torch
 import torchaudio
+import yaml
 from typeguard import check_argument_types
-from typeguard import check_return_type
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.beam_search.beam_search import BeamSearch
-# from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 
+from funasr.bin.asr_infer import Speech2Text
+from funasr.bin.asr_infer import Speech2TextMFCCA
+from funasr.bin.asr_infer import Speech2TextParaformer, Speech2TextParaformerOnline
+from funasr.bin.asr_infer import Speech2TextSAASR
+from funasr.bin.asr_infer import Speech2TextTransducer
+from funasr.bin.asr_infer import Speech2TextUniASR
+from funasr.bin.punc_infer import Text2Punc
+from funasr.bin.tp_infer import Speech2Timestamp
+from funasr.bin.vad_infer import Speech2VadSegment
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
+from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.modules.beam_search.beam_search import Hypothesis
-from funasr.modules.scorers.ctc import CTCPrefixScorer
-from funasr.modules.scorers.length_bonus import LengthBonus
 from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.asr import ASRTask
-from funasr.tasks.lm import LMTask
-from funasr.text.build_tokenizer import build_tokenizer
-from funasr.text.token_id_converter import TokenIDConverter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
+from funasr.utils import asr_utils, postprocess_utils
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
-from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
-from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
-from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
-
-
 from funasr.utils.vad_utils import slice_padding_fbank
-from funasr.tasks.vad import VADTask
-from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
-from funasr.bin.asr_infer import Speech2Text
-from funasr.bin.asr_infer import Speech2TextParaformer, Speech2TextParaformerOnline
-from funasr.bin.asr_infer import Speech2TextUniASR
-from funasr.bin.asr_infer import Speech2TextMFCCA
-from funasr.bin.vad_infer import Speech2VadSegment
-from funasr.bin.punc_infer import Text2Punc
-from funasr.bin.tp_infer import Speech2Timestamp
-from funasr.bin.asr_infer import Speech2TextTransducer
-from funasr.bin.asr_infer import Speech2TextSAASR
+
 
 def inference_asr(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    mc: bool = False,
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        streaming: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        mc: bool = False,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     for handler in logging.root.handlers[:]:
         logging.root.removeHandler(handler)
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -156,159 +124,157 @@
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         streaming=streaming,
     )
     logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
     speech2text = Speech2Text(**speech2text_kwargs)
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
             mc=mc,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            
+
             # N-best list of (text, token, token_int, hyp_object)
             try:
                 results = speech2text(**batch)
             except TooShortUttError as e:
                 logging.warning(f"Utterance {keys} {e}")
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
                 results = [[" ", ["sil"], [2], hyp]] * nbest
-            
+
             # Only supporting batch_size==1
             key = keys[0]
             for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                 # Create a directory: outdir/{n}best_recog
                 if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
-                    
+
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
-                
+
                 if text is not None:
                     text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
                         ibest_writer["text"][key] = text
-                
+
                 logging.info("uttid: {}".format(key))
                 logging.info("text predictions: {}\n".format(text))
         return asr_result_list
-    
+
     return _forward
 
 
 def inference_paraformer(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    output_dir: Optional[str] = None,
-    timestamp_infer_config: Union[Path, str] = None,
-    timestamp_model_file: Union[Path, str] = None,
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        output_dir: Optional[str] = None,
+        timestamp_infer_config: Union[Path, str] = None,
+        timestamp_model_file: Union[Path, str] = None,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    
+
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     export_mode = False
     if param_dict is not None:
         hotword_list_or_file = param_dict.get('hotword')
         export_mode = param_dict.get("export_mode", False)
     else:
         hotword_list_or_file = None
-    
+
     if kwargs.get("device", None) == "cpu":
         ngpu = 0
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
         batch_size = 1
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -322,89 +288,87 @@
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         hotword_list_or_file=hotword_list_or_file,
     )
-    
+
     speech2text = Speech2TextParaformer(**speech2text_kwargs)
-    
+
     if timestamp_model_file is not None:
         speechtext2timestamp = Speech2Timestamp(
             timestamp_cmvn_file=cmvn_file,
             timestamp_model_file=timestamp_model_file,
             timestamp_infer_config=timestamp_infer_config,
         )
     else:
         speechtext2timestamp = None
-    
+
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        output_dir_v2: Optional[str] = None,
-        fs: dict = None,
-        param_dict: dict = None,
-        **kwargs,
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None,
+            **kwargs,
     ):
-        
+
         hotword_list_or_file = None
         if param_dict is not None:
             hotword_list_or_file = param_dict.get('hotword')
         if 'hotword' in kwargs and kwargs['hotword'] is not None:
             hotword_list_or_file = kwargs['hotword']
         if hotword_list_or_file is not None or 'hotword' in kwargs:
             speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
-        
+
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         if param_dict is not None:
             use_timestamp = param_dict.get('use_timestamp', True)
         else:
             use_timestamp = True
-        
+
         forward_time_total = 0.0
         length_total = 0.0
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v for k, v in batch.items() if not k.endswith("_lengths")}
-            
+
             logging.info("decoding, utt_id: {}".format(keys))
             # N-best list of (text, token, token_int, hyp_object)
-            
+
             time_beg = time.time()
             results = speech2text(**batch)
             if len(results) < 1:
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
                 results = [[" ", ["sil"], [2], hyp, 10, 6]] * nbest
             time_end = time.time()
             forward_time = time_end - time_beg
@@ -412,18 +376,18 @@
             length = results[0][-2]
             forward_time_total += forward_time
             length_total += length
             rtf_cur = "decoding, feature length: {}, forward_time: {:.4f}, rtf: {:.4f}".format(length, forward_time,
                                                                                                100 * forward_time / (
                                                                                                        length * lfr_factor))
             logging.info(rtf_cur)
-            
+
             for batch_id in range(_bs):
                 result = [results[batch_id][:-2]]
-                
+
                 key = keys[batch_id]
                 for n, result in zip(range(1, nbest + 1), result):
                     text, token, token_int, hyp = result[0], result[1], result[2], result[3]
                     timestamp = result[4] if len(result[4]) > 0 else None
                     # conduct timestamp prediction here
                     # timestamp inference requires token length
                     # thus following inference cannot be conducted in batch
@@ -434,21 +398,21 @@
                         ts_batch['text_lengths'] = torch.tensor([len(token)])
                         us_alphas, us_peaks = speechtext2timestamp(**ts_batch)
                         ts_str, timestamp = ts_prediction_lfr6_standard(us_alphas[0], us_peaks[0], token,
                                                                         force_time_shift=-3.0)
                     # Create a directory: outdir/{n}best_recog
                     if writer is not None:
                         ibest_writer = writer[f"{n}best_recog"]
-                        
+
                         # Write the result to each file
                         ibest_writer["token"][key] = " ".join(token)
                         # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                         ibest_writer["score"][key] = str(hyp.score)
                         ibest_writer["rtf"][key] = rtf_cur
-                    
+
                     if text is not None:
                         if use_timestamp and timestamp is not None:
                             postprocessed_result = postprocess_utils.sentence_postprocess(token, timestamp)
                         else:
                             postprocessed_result = postprocess_utils.sentence_postprocess(token)
                         timestamp_postprocessed = ""
                         if len(postprocessed_result) == 3:
@@ -461,103 +425,103 @@
                         if timestamp_postprocessed != "":
                             item['timestamp'] = timestamp_postprocessed
                         asr_result_list.append(item)
                         finish_count += 1
                         # asr_utils.print_progress(finish_count / file_count)
                         if writer is not None:
                             ibest_writer["text"][key] = " ".join(word_lists)
-                    
+
                     logging.info("decoding, utt: {}, predictions: {}".format(key, text))
         rtf_avg = "decoding, feature length total: {}, forward_time total: {:.4f}, rtf avg: {:.4f}".format(length_total,
                                                                                                            forward_time_total,
                                                                                                            100 * forward_time_total / (
                                                                                                                    length_total * lfr_factor))
         logging.info(rtf_avg)
         if writer is not None:
             ibest_writer["rtf"]["rtf_avf"] = rtf_avg
         return asr_result_list
-    
+
     return _forward
 
 
 def inference_paraformer_vad_punc(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    vad_infer_config: Optional[str] = None,
-    vad_model_file: Optional[str] = None,
-    vad_cmvn_file: Optional[str] = None,
-    time_stamp_writer: bool = True,
-    punc_infer_config: Optional[str] = None,
-    punc_model_file: Optional[str] = None,
-    outputs_dict: Optional[bool] = True,
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        vad_infer_config: Optional[str] = None,
+        vad_model_file: Optional[str] = None,
+        vad_cmvn_file: Optional[str] = None,
+        time_stamp_writer: bool = True,
+        punc_infer_config: Optional[str] = None,
+        punc_model_file: Optional[str] = None,
+        outputs_dict: Optional[bool] = True,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    
+
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if param_dict is not None:
         hotword_list_or_file = param_dict.get('hotword')
     else:
         hotword_list_or_file = None
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2vadsegment
     speech2vadsegment_kwargs = dict(
         vad_infer_config=vad_infer_config,
         vad_model_file=vad_model_file,
         vad_cmvn_file=vad_cmvn_file,
         device=device,
         dtype=dtype,
     )
     # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
     speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
-    
+
     # 3. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -575,119 +539,119 @@
         nbest=nbest,
         hotword_list_or_file=hotword_list_or_file,
     )
     speech2text = Speech2TextParaformer(**speech2text_kwargs)
     text2punc = None
     if punc_model_file is not None:
         text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
-    
+
     if output_dir is not None:
         writer = DatadirWriter(output_dir)
         ibest_writer = writer[f"1best_recog"]
         ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
-        
+
         hotword_list_or_file = None
         if param_dict is not None:
             hotword_list_or_file = param_dict.get('hotword')
-        
+
         if 'hotword' in kwargs:
             hotword_list_or_file = kwargs['hotword']
-        
+
         batch_size_token = kwargs.get("batch_size_token", 6000)
         print("batch_size_token: ", batch_size_token)
-        
+
         if speech2text.hotword_list is None:
             speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
-        
+
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=None,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
             batch_size=1,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         if param_dict is not None:
             use_timestamp = param_dict.get('use_timestamp', True)
         else:
             use_timestamp = True
-        
+
         finish_count = 0
         file_count = 1
         lfr_factor = 6
         # 7 .Start for-loop
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         writer = None
         if output_path is not None:
             writer = DatadirWriter(output_path)
             ibest_writer = writer[f"1best_recog"]
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             beg_vad = time.time()
             vad_results = speech2vadsegment(**batch)
             end_vad = time.time()
-            print("time cost vad: ", end_vad-beg_vad)
+            print("time cost vad: ", end_vad - beg_vad)
             _, vadsegments = vad_results[0], vad_results[1][0]
-            
+
             speech, speech_lengths = batch["speech"], batch["speech_lengths"]
-            
+
             n = len(vadsegments)
             data_with_index = [(vadsegments[i], i) for i in range(n)]
             sorted_data = sorted(data_with_index, key=lambda x: x[0][1] - x[0][0])
             results_sorted = []
+            
             batch_size_token_ms = batch_size_token*60
             if speech2text.device == "cpu":
                 batch_size_token_ms = 0
             batch_size_token_ms = max(batch_size_token_ms, sorted_data[0][0][1] - sorted_data[0][0][0])
             
             batch_size_token_ms_cum = 0
             beg_idx = 0
             for j, _ in enumerate(range(0, n)):
                 batch_size_token_ms_cum += (sorted_data[j][0][1] - sorted_data[j][0][0])
-                if j < n-1 and (batch_size_token_ms_cum + sorted_data[j+1][0][1] - sorted_data[j+1][0][0])<batch_size_token_ms:
+                if j < n - 1 and (batch_size_token_ms_cum + sorted_data[j + 1][0][1] - sorted_data[j + 1][0][
+                    0]) < batch_size_token_ms:
                     continue
                 batch_size_token_ms_cum = 0
                 end_idx = j + 1
                 speech_j, speech_lengths_j = slice_padding_fbank(speech, speech_lengths, sorted_data[beg_idx:end_idx])
                 beg_idx = end_idx
                 batch = {"speech": speech_j, "speech_lengths": speech_lengths_j}
                 batch = to_device(batch, device=device)
                 print("batch: ", speech_j.shape[0])
                 beg_asr = time.time()
                 results = speech2text(**batch)
                 end_asr = time.time()
                 print("time cost asr: ", end_asr - beg_asr)
-                
+
                 if len(results) < 1:
                     results = [["", [], [], [], [], [], []]]
                 results_sorted.extend(results)
-            
+
             restored_data = [0] * n
             for j in range(n):
                 index = sorted_data[j][1]
                 restored_data[index] = results_sorted[j]
             result = ["", [], [], [], [], [], []]
             for j in range(n):
                 result[0] += restored_data[j][0]
@@ -695,68 +659,69 @@
                 result[2] += restored_data[j][2]
                 if len(restored_data[j][4]) > 0:
                     for t in restored_data[j][4]:
                         t[0] += vadsegments[j][0]
                         t[1] += vadsegments[j][0]
                     result[4] += restored_data[j][4]
                 # result = [result[k]+restored_data[j][k] for k in range(len(result[:-2]))]
-            
+
             key = keys[0]
             # result = result_segments[0]
             text, token, token_int = result[0], result[1], result[2]
             time_stamp = result[4] if len(result[4]) > 0 else None
-            
+
             if use_timestamp and time_stamp is not None:
                 postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
             else:
                 postprocessed_result = postprocess_utils.sentence_postprocess(token)
             text_postprocessed = ""
             time_stamp_postprocessed = ""
             text_postprocessed_punc = postprocessed_result
             if len(postprocessed_result) == 3:
                 text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
                                                                            postprocessed_result[1], \
                                                                            postprocessed_result[2]
             else:
                 text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
-            
+
             text_postprocessed_punc = text_postprocessed
             punc_id_list = []
             if len(word_lists) > 0 and text2punc is not None:
                 beg_punc = time.time()
                 text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
                 end_punc = time.time()
-                print("time cost punc: ", end_punc-beg_punc)
-            
+                print("time cost punc: ", end_punc - beg_punc)
+
             item = {'key': key, 'value': text_postprocessed_punc}
             if text_postprocessed != "":
                 item['text_postprocessed'] = text_postprocessed
             if time_stamp_postprocessed != "":
                 item['time_stamp'] = time_stamp_postprocessed
-            
+
             item['sentences'] = time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed)
-            
+
             asr_result_list.append(item)
             finish_count += 1
             # asr_utils.print_progress(finish_count / file_count)
             if writer is not None:
                 # Write the result to each file
                 ibest_writer["token"][key] = " ".join(token)
                 ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                 ibest_writer["vad"][key] = "{}".format(vadsegments)
                 ibest_writer["text"][key] = " ".join(word_lists)
                 ibest_writer["text_with_punc"][key] = text_postprocessed_punc
                 if time_stamp_postprocessed is not None:
                     ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
-            
+
             logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
         return asr_result_list
-    
+
     return _forward
 
+
 def inference_paraformer_online(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
         beam_size: int,
         ngpu: int,
         ctc_weight: float,
@@ -848,15 +813,15 @@
         if not Path(yaml_path).exists():
             raise FileExistsError(f'The {yaml_path} does not exist.')
 
         with open(str(yaml_path), 'rb') as f:
             data = yaml.load(f, Loader=yaml.Loader)
         return data
 
-    def _prepare_cache(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
+    def _prepare_cache(cache: dict = {}, chunk_size=[5, 10, 5], batch_size=1):
         if len(cache) > 0:
             return cache
         config = _read_yaml(asr_train_config)
         enc_output_size = config["encoder_conf"]["output_size"]
         feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
         cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
                     "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
@@ -864,22 +829,23 @@
         cache["encoder"] = cache_en
 
         cache_de = {"decode_fsmn": None}
         cache["decoder"] = cache_de
 
         return cache
 
-    def _cache_reset(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
+    def _cache_reset(cache: dict = {}, chunk_size=[5, 10, 5], batch_size=1):
         if len(cache) > 0:
             config = _read_yaml(asr_train_config)
             enc_output_size = config["encoder_conf"]["output_size"]
             feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
             cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
                         "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
-                        "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)), "tail_chunk": False}
+                        "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)),
+                        "tail_chunk": False}
             cache["encoder"] = cache_en
 
             cache_de = {"decode_fsmn": None}
             cache["decoder"] = cache_de
 
         return cache
 
@@ -916,15 +882,15 @@
         raw_inputs = torch.unsqueeze(raw_inputs, axis=0)
         asr_result_list = []
         cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
         item = {}
         if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
             sample_offset = 0
             speech_length = raw_inputs.shape[1]
-            stride_size =  chunk_size[1] * 960
+            stride_size = chunk_size[1] * 960
             cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
             final_result = ""
             for sample_offset in range(0, speech_length, min(stride_size, speech_length - sample_offset)):
                 if sample_offset + stride_size >= speech_length - 1:
                     stride_size = speech_length - sample_offset
                     cache["encoder"]["is_final"] = True
                 else:
@@ -945,85 +911,85 @@
             cache = _cache_reset(cache, chunk_size=chunk_size, batch_size=1)
         return asr_result_list
 
     return _forward
 
 
 def inference_uniasr(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    ngram_file: Optional[str] = None,
-    cmvn_file: Optional[str] = None,
-    # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    token_num_relax: int = 1,
-    decoding_ind: int = 0,
-    decoding_mode: str = "model1",
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        ngram_file: Optional[str] = None,
+        cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        streaming: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        token_num_relax: int = 1,
+        decoding_ind: int = 0,
+        decoding_mode: str = "model1",
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     if param_dict is not None and "decoding_model" in param_dict:
         if param_dict["decoding_model"] == "fast":
             decoding_ind = 0
             decoding_mode = "model1"
         elif param_dict["decoding_model"] == "normal":
             decoding_ind = 0
             decoding_mode = "model2"
         elif param_dict["decoding_model"] == "offline":
             decoding_ind = 1
             decoding_mode = "model2"
         else:
             raise NotImplementedError("unsupported decoding model {}".format(param_dict["decoding_model"]))
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -1042,146 +1008,144 @@
         nbest=nbest,
         streaming=streaming,
         token_num_relax=token_num_relax,
         decoding_ind=decoding_ind,
         decoding_mode=decoding_mode,
     )
     speech2text = Speech2TextUniASR(**speech2text_kwargs)
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            
+
             # N-best list of (text, token, token_int, hyp_object)
             try:
                 results = speech2text(**batch)
             except TooShortUttError as e:
                 logging.warning(f"Utterance {keys} {e}")
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
                 results = [[" ", ["sil"], [2], hyp]] * nbest
-            
+
             # Only supporting batch_size==1
             key = keys[0]
             logging.info(f"Utterance: {key}")
             for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                 # Create a directory: outdir/{n}best_recog
                 if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
-                    
+
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
-                
+
                 if text is not None:
                     text_postprocessed, word_lists = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
                         ibest_writer["text"][key] = " ".join(word_lists)
         return asr_result_list
-    
+
     return _forward
 
 
 def inference_mfcca(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        streaming: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -1197,124 +1161,123 @@
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         streaming=streaming,
     )
     logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
     speech2text = Speech2TextMFCCA(**speech2text_kwargs)
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             fs=fs,
             mc=True,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            
+
             # N-best list of (text, token, token_int, hyp_object)
             try:
                 results = speech2text(**batch)
             except TooShortUttError as e:
                 logging.warning(f"Utterance {keys} {e}")
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
                 results = [[" ", ["<space>"], [2], hyp]] * nbest
-            
+
             # Only supporting batch_size==1
             key = keys[0]
             for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                 # Create a directory: outdir/{n}best_recog
                 if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
-                    
+
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     # ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
-                
+
                 if text is not None:
                     text_postprocessed = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
                         ibest_writer["text"][key] = text
         return asr_result_list
-    
+
     return _forward
 
+
 def inference_transducer(
-    output_dir: str,
-    batch_size: int,
-    dtype: str,
-    beam_size: int,
-    ngpu: int,
-    seed: int,
-    lm_weight: float,
-    nbest: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str],
-    beam_search_config: Optional[dict],
-    lm_train_config: Optional[str],
-    lm_file: Optional[str],
-    model_tag: Optional[str],
-    token_type: Optional[str],
-    bpemodel: Optional[str],
-    key_file: Optional[str],
-    allow_variable_data_keys: bool,
-    quantize_asr_model: Optional[bool],
-    quantize_modules: Optional[List[str]],
-    quantize_dtype: Optional[str],
-    streaming: Optional[bool],
-    simu_streaming: Optional[bool],
-    chunk_size: Optional[int],
-    left_context: Optional[int],
-    right_context: Optional[int],
-    display_partial_hypotheses: bool,
-    **kwargs,
+        output_dir: str,
+        batch_size: int,
+        dtype: str,
+        beam_size: int,
+        ngpu: int,
+        seed: int,
+        lm_weight: float,
+        nbest: int,
+        num_workers: int,
+        log_level: Union[int, str],
+        data_path_and_name_and_type: Sequence[Tuple[str, str, str]],
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str],
+        beam_search_config: Optional[dict],
+        lm_train_config: Optional[str],
+        lm_file: Optional[str],
+        model_tag: Optional[str],
+        token_type: Optional[str],
+        bpemodel: Optional[str],
+        key_file: Optional[str],
+        allow_variable_data_keys: bool,
+        quantize_asr_model: Optional[bool],
+        quantize_modules: Optional[List[str]],
+        quantize_dtype: Optional[str],
+        streaming: Optional[bool],
+        simu_streaming: Optional[bool],
+        chunk_size: Optional[int],
+        left_context: Optional[int],
+        right_context: Optional[int],
+        display_partial_hypotheses: bool,
+        **kwargs,
 ) -> None:
     """Transducer model inference.
     Args:
         output_dir: Output directory path.
         batch_size: Batch decoding size.
         dtype: Data type.
         beam_size: Beam size.
@@ -1387,148 +1350,141 @@
         left_context=left_context,
         right_context=right_context,
     )
     speech2text = Speech2TextTransducer.from_pretrained(
         model_tag=model_tag,
         **speech2text_kwargs,
     )
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
         # 3. Build data-iterator
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(
-                speech2text.asr_train_args, False
-            ),
-            collate_fn=ASRTask.build_collate_fn(
-                speech2text.asr_train_args, False
-            ),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-    
+
         # 4 .Start for-loop
         with DatadirWriter(output_dir) as writer:
             for keys, batch in loader:
                 assert isinstance(batch, dict), type(batch)
                 assert all(isinstance(s, str) for s in keys), keys
-    
+
                 _bs = len(next(iter(batch.values())))
                 assert len(keys) == _bs, f"{len(keys)} != {_bs}"
                 batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
                 assert len(batch.keys()) == 1
-    
+
                 try:
                     if speech2text.streaming:
                         speech = batch["speech"]
-    
+
                         _steps = len(speech) // speech2text._ctx
                         _end = 0
                         for i in range(_steps):
                             _end = (i + 1) * speech2text._ctx
-    
+
                             speech2text.streaming_decode(
-                                speech[i * speech2text._ctx : _end], is_final=False
+                                speech[i * speech2text._ctx: _end], is_final=False
                             )
-    
+
                         final_hyps = speech2text.streaming_decode(
-                            speech[_end : len(speech)], is_final=True
+                            speech[_end: len(speech)], is_final=True
                         )
                     elif speech2text.simu_streaming:
                         final_hyps = speech2text.simu_streaming_decode(**batch)
                     else:
                         final_hyps = speech2text(**batch)
-    
+
                     results = speech2text.hypotheses_to_results(final_hyps)
                 except TooShortUttError as e:
                     logging.warning(f"Utterance {keys} {e}")
                     hyp = Hypothesis(score=0.0, yseq=[], dec_state=None)
                     results = [[" ", ["<space>"], [2], hyp]] * nbest
-    
+
                 key = keys[0]
                 for n, (text, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                     ibest_writer = writer[f"{n}best_recog"]
-    
+
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
-    
+
                     if text is not None:
                         ibest_writer["text"][key] = text
 
-
     return _forward
 
 
 def inference_sa_asr(
-    maxlenratio: float,
-    minlenratio: float,
-    batch_size: int,
-    beam_size: int,
-    ngpu: int,
-    ctc_weight: float,
-    lm_weight: float,
-    penalty: float,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    asr_train_config: Optional[str],
-    asr_model_file: Optional[str],
-    cmvn_file: Optional[str] = None,
-    lm_train_config: Optional[str] = None,
-    lm_file: Optional[str] = None,
-    token_type: Optional[str] = None,
-    key_file: Optional[str] = None,
-    word_lm_train_config: Optional[str] = None,
-    bpemodel: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    streaming: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    ngram_weight: float = 0.9,
-    nbest: int = 1,
-    num_workers: int = 1,
-    mc: bool = False,
-    param_dict: dict = None,
-    **kwargs,
+        maxlenratio: float,
+        minlenratio: float,
+        batch_size: int,
+        beam_size: int,
+        ngpu: int,
+        ctc_weight: float,
+        lm_weight: float,
+        penalty: float,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        asr_train_config: Optional[str],
+        asr_model_file: Optional[str],
+        cmvn_file: Optional[str] = None,
+        lm_train_config: Optional[str] = None,
+        lm_file: Optional[str] = None,
+        token_type: Optional[str] = None,
+        key_file: Optional[str] = None,
+        word_lm_train_config: Optional[str] = None,
+        bpemodel: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        streaming: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        ngram_weight: float = 0.9,
+        nbest: int = 1,
+        num_workers: int = 1,
+        mc: bool = False,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     for handler in logging.root.handlers[:]:
         logging.root.removeHandler(handler)
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
@@ -1544,93 +1500,91 @@
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         streaming=streaming,
     )
     logging.info("speech2text_kwargs: {}".format(speech2text_kwargs))
     speech2text = Speech2TextSAASR(**speech2text_kwargs)
-    
+
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
                  ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speech2text.asr_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             fs=fs,
             mc=mc,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=ASRTask.build_preprocess_fn(speech2text.asr_train_args, False),
-            collate_fn=ASRTask.build_collate_fn(speech2text.asr_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             # batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
             # N-best list of (text, token, token_int, hyp_object)
             try:
                 results = speech2text(**batch)
             except TooShortUttError as e:
                 logging.warning(f"Utterance {keys} {e}")
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
                 results = [[" ", ["sil"], [2], hyp]] * nbest
-            
+
             # Only supporting batch_size==1
             key = keys[0]
             for n, (text, text_id, token, token_int, hyp) in zip(range(1, nbest + 1), results):
                 # Create a directory: outdir/{n}best_recog
                 if writer is not None:
                     ibest_writer = writer[f"{n}best_recog"]
-                    
+
                     # Write the result to each file
                     ibest_writer["token"][key] = " ".join(token)
                     ibest_writer["token_int"][key] = " ".join(map(str, token_int))
                     ibest_writer["score"][key] = str(hyp.score)
                     ibest_writer["text_id"][key] = text_id
-                
+
                 if text is not None:
                     text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
                     item = {'key': key, 'value': text_postprocessed}
                     asr_result_list.append(item)
                     finish_count += 1
                     asr_utils.print_progress(finish_count / file_count)
                     if writer is not None:
                         ibest_writer["text"][key] = text
-                
+
                 logging.info("uttid: {}".format(key))
                 logging.info("text predictions: {}".format(text))
                 logging.info("text_id predictions: {}\n".format(text_id))
         return asr_result_list
-    
+
     return _forward
 
 
 def inference_launch(**kwargs):
     if 'mode' in kwargs:
         mode = kwargs['mode']
     else:
@@ -1660,25 +1614,25 @@
 
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="ASR Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    
+
     # Note(kamo): Use '_' instead of '-' as separator.
     # '-' is confusing if written in yaml.
     parser.add_argument(
         "--log_level",
         type=lambda x: x.upper(),
         default="INFO",
         choices=("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"),
         help="The verbose level of logging",
     )
-    
+
     parser.add_argument("--output_dir", type=str, required=True)
     parser.add_argument(
         "--ngpu",
         type=int,
         default=0,
         help="The number of gpus. 0 indicates CPU mode",
     )
@@ -1703,15 +1657,15 @@
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
-    
+
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=True,
         action="append",
     )
@@ -1725,15 +1679,15 @@
     group.add_argument("--allow_variable_data_keys", type=str2bool, default=False)
     group.add_argument(
         "--mc",
         type=bool,
         default=False,
         help="MultiChannel input",
     )
-    
+
     group = parser.add_argument_group("The model configuration related")
     group.add_argument(
         "--vad_infer_config",
         type=str,
         help="VAD infer configuration",
     )
     group.add_argument(
@@ -1788,15 +1742,15 @@
              "*_file will be overwritten",
     )
     group.add_argument(
         "--beam_search_config",
         default={},
         help="The keyword arguments for transducer beam search.",
     )
-    
+
     group = parser.add_argument_group("Beam-search related")
     group.add_argument(
         "--batch_size",
         type=int,
         default=1,
         help="The batch size for inference",
     )
@@ -1835,15 +1789,15 @@
     group.add_argument("--right_context", type=int, default=0)
     group.add_argument(
         "--display_partial_hypotheses",
         type=bool,
         default=False,
         help="Whether to display partial hypotheses during chunk-by-chunk inference.",
     )
-    
+
     group = parser.add_argument_group("Dynamic quantization related")
     group.add_argument(
         "--quantize_asr_model",
         type=bool,
         default=False,
         help="Apply dynamic quantization to ASR model.",
     )
@@ -1860,15 +1814,15 @@
     group.add_argument(
         "--quantize_dtype",
         type=str,
         default="qint8",
         choices=["float16", "qint8"],
         help="Dtype for dynamic quantization.",
     )
-    
+
     group = parser.add_argument_group("Text converter related")
     group.add_argument(
         "--token_type",
         type=str_or_none,
         default=None,
         choices=["char", "bpe", None],
         help="The token type for ASR model. "
@@ -1920,10 +1874,9 @@
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
 
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"], hotword=kwargs.get("hotword", None))
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.6.2/funasr/bin/asr_train.py` & `funasr-0.6.3/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/build_trainer.py` & `funasr-0.6.3/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/data2vec_train.py` & `funasr-0.6.3/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/diar_infer.py` & `funasr-0.6.3/funasr/bin/diar_infer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,32 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
 import logging
 import os
-import sys
+from collections import OrderedDict
 from pathlib import Path
 from typing import Any
-from typing import List
 from typing import Optional
-from typing import Sequence
-from typing import Tuple
 from typing import Union
 
-from collections import OrderedDict
 import numpy as np
-import soundfile
 import torch
+from scipy.ndimage import median_filter
 from torch.nn import functional as F
 from typeguard import check_argument_types
-from typeguard import check_return_type
 
-from funasr.utils.cli_utils import get_commandline_args
+from funasr.models.frontend.wav_frontend import WavFrontendMel23
 from funasr.tasks.diar import DiarTask
-from funasr.tasks.diar import EENDOLADiarTask
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from scipy.ndimage import median_filter
 from funasr.utils.misc import statistic_model_parameters
-from funasr.datasets.iterable_dataset import load_bytes
-from funasr.models.frontend.wav_frontend import WavFrontendMel23
+
 
 class Speech2DiarizationEEND:
     """Speech2Diarlization class
 
     Examples:
         >>> import soundfile
         >>> import numpy as np
@@ -57,18 +44,20 @@
             diar_model_file: Union[Path, str] = None,
             device: str = "cpu",
             dtype: str = "float32",
     ):
         assert check_argument_types()
 
         # 1. Build Diarization model
-        diar_model, diar_train_args = EENDOLADiarTask.build_model_from_file(
+        diar_model, diar_train_args = build_model_from_file(
             config_file=diar_train_config,
             model_file=diar_model_file,
-            device=device
+            device=device,
+            task_name="diar",
+            mode="eend-ola",
         )
         frontend = None
         if diar_train_args.frontend is not None and diar_train_args.frontend_conf is not None:
             frontend = WavFrontendMel23(**diar_train_args.frontend_conf)
 
         # set up seed for eda
         np.random.seed(diar_train_args.seed)
@@ -173,18 +162,20 @@
             streaming: bool = False,
             smooth_size: int = 83,
             dur_threshold: float = 10,
     ):
         assert check_argument_types()
 
         # TODO: 1. Build Diarization model
-        diar_model, diar_train_args = DiarTask.build_model_from_file(
+        diar_model, diar_train_args = build_model_from_file(
             config_file=diar_train_config,
             model_file=diar_model_file,
-            device=device
+            device=device,
+            task_name="diar",
+            mode="sond",
         )
         logging.info("diar_model: {}".format(diar_model))
         logging.info("model parameter number: {}".format(statistic_model_parameters(diar_model)))
         logging.info("diar_train_args: {}".format(diar_train_args))
         diar_model.to(dtype=getattr(torch, dtype)).eval()
 
         self.diar_model = diar_model
@@ -244,15 +235,15 @@
 
     def post_processing(self, raw_logits: torch.Tensor, spk_num: int, output_format: str = "speaker_turn"):
         logits_idx = raw_logits.argmax(-1)  # B, T, vocab_size -> B, T
         # upsampling outputs to match inputs
         ut = logits_idx.shape[1] * self.diar_model.encoder.time_ds_ratio
         logits_idx = F.upsample(
             logits_idx.unsqueeze(1).float(),
-            size=(ut, ),
+            size=(ut,),
             mode="nearest",
         ).squeeze(1).long()
         logits_idx = logits_idx[0].tolist()
         pse_labels = [self.token_list[x] for x in logits_idx]
         if output_format == "pse_labels":
             return pse_labels, None
 
@@ -264,15 +255,15 @@
         spk_list = ["spk{}".format(i + 1) for i in range(spk_num)]
         spk_turns = self.calc_spk_turns(multi_labels, spk_list)
         results = OrderedDict()
         for spk, st, dur in spk_turns:
             if spk not in results:
                 results[spk] = []
             if dur > self.dur_threshold:
-                results[spk].append((st, st+dur))
+                results[spk].append((st, st + dur))
 
         # sort segments in start time ascending
         for spk in results:
             results[spk] = sorted(results[spk], key=lambda x: x[0])
 
         return results, pse_labels
 
@@ -340,11 +331,7 @@
                     "Please install via `pip install -U espnet_model_zoo`."
                 )
                 raise
             d = ModelDownloader()
             kwargs.update(**d.download_and_unpack(model_tag))
 
         return Speech2DiarizationSOND(**kwargs)
-
-
-
-
```

### Comparing `funasr-0.6.2/funasr/bin/diar_inference_launch.py` & `funasr-0.6.3/funasr/bin/diar_inference_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,39 @@
+# !/usr/bin/env python3
 # -*- encoding: utf-8 -*-
-#!/usr/bin/env python3
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-
-import argparse
-import logging
-import os
-import sys
-from pathlib import Path
-from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
-from collections import OrderedDict
 import numpy as np
 import soundfile
 import torch
-from torch.nn import functional as F
-from typeguard import check_argument_types
-from typeguard import check_return_type
 from scipy.signal import medfilt
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.diar import DiarTask
-from funasr.tasks.diar import EENDOLADiarTask
-from funasr.torch_utils.device_funcs import to_device
+from typeguard import check_argument_types
+
+from funasr.bin.diar_infer import Speech2DiarizationSOND, Speech2DiarizationEEND
+from funasr.datasets.iterable_dataset import load_bytes
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from scipy.ndimage import median_filter
-from funasr.utils.misc import statistic_model_parameters
-from funasr.datasets.iterable_dataset import load_bytes
-from funasr.bin.diar_infer import Speech2DiarizationSOND, Speech2DiarizationEEND
+
 
 def inference_sond(
         diar_train_config: str,
         diar_model_file: str,
         output_dir: Optional[str] = None,
         batch_size: int = 1,
         dtype: str = "float32",
@@ -90,15 +71,16 @@
     else:
         device = "cpu"
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
     # 2a. Build speech2xvec [Optional]
-    if mode == "sond_demo" and param_dict is not None and "extract_profile" in param_dict and param_dict["extract_profile"]:
+    if mode == "sond_demo" and param_dict is not None and "extract_profile" in param_dict and param_dict[
+        "extract_profile"]:
         assert "sv_train_config" in param_dict, "sv_train_config must be provided param_dict."
         assert "sv_model_file" in param_dict, "sv_model_file must be provided in param_dict."
         sv_train_config = param_dict["sv_train_config"]
         sv_model_file = param_dict["sv_model_file"]
         if "model_dir" in param_dict:
             sv_train_config = os.path.join(param_dict["model_dir"], sv_train_config)
             sv_model_file = os.path.join(param_dict["model_dir"], sv_model_file)
@@ -135,15 +117,15 @@
     )
     speech2diar.diar_model.eval()
 
     def output_results_str(results: dict, uttid: str):
         rst = []
         mid = uttid.rsplit("-", 1)[0]
         for key in results:
-            results[key] = [(x[0]/100, x[1]/100) for x in results[key]]
+            results[key] = [(x[0] / 100, x[1] / 100) for x in results[key]]
         if out_format == "vad":
             for spk, segs in results.items():
                 rst.append("{} {}".format(spk, segs))
         else:
             template = "SPEAKER {} 0 {:.2f} {:.2f} <NA> <NA> {} <NA> <NA>"
             for spk, segs in results.items():
                 rst.extend([template.format(mid, st, ed, spk) for st, ed in segs])
@@ -172,34 +154,33 @@
                                    for x in example]
                         example = [soundfile.read(x)[0] if isinstance(x, str) else x
                                    for x in example]
                         # convert torch tensor to numpy array
                         example = [x.numpy() if isinstance(example[0], torch.Tensor) else x
                                    for x in example]
                         speech = example[0]
-                        logging.info("Extracting profiles for {} waveforms".format(len(example)-1))
+                        logging.info("Extracting profiles for {} waveforms".format(len(example) - 1))
                         profile = [speech2xvector.calculate_embedding(x) for x in example[1:]]
                         profile = torch.cat(profile, dim=0)
                         yield ["test{}".format(idx)], {"speech": [speech], "profile": [profile]}
 
                 loader = prepare_dataset()
             else:
                 raise TypeError("raw_inputs must be a list or tuple in [speech, profile1, profile2, ...] ")
         else:
             # 3. Build data-iterator
-            loader = DiarTask.build_streaming_iterator(
-                data_path_and_name_and_type,
+            loader = build_streaming_iterator(
+                task_name="diar",
+                preprocess_args=None,
+                data_path_and_name_and_type=data_path_and_name_and_type,
                 dtype=dtype,
                 batch_size=batch_size,
                 key_file=key_file,
                 num_workers=num_workers,
-                preprocess_fn=None,
-                collate_fn=None,
-                allow_variable_data_keys=allow_variable_data_keys,
-                inference=True,
+                use_collate_fn=False,
             )
 
         # 7. Start for-loop
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             os.makedirs(output_path, exist_ok=True)
             output_writer = open("{}/result.txt".format(output_path), "w")
@@ -231,14 +212,15 @@
             output_writer.close()
             pse_label_writer.close()
 
         return result_list
 
     return _forward
 
+
 def inference_eend(
         diar_train_config: str,
         diar_model_file: str,
         output_dir: Optional[str] = None,
         batch_size: int = 1,
         dtype: str = "float32",
         ngpu: int = 1,
@@ -302,24 +284,22 @@
             param_dict: Optional[dict] = None,
     ):
         # 2. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs[0], "speech", "sound"]
-        loader = EENDOLADiarTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="diar",
+            preprocess_args=None,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=EENDOLADiarTask.build_preprocess_fn(speech2diar.diar_train_args, False),
-            collate_fn=EENDOLADiarTask.build_collate_fn(speech2diar.diar_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
 
         # 3. Start for-loop
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             os.makedirs(output_path, exist_ok=True)
             output_writer = open("{}/result.txt".format(output_path), "w")
@@ -358,16 +338,14 @@
             output_writer.close()
 
         return result_list
 
     return _forward
 
 
-
-
 def inference_launch(mode, **kwargs):
     if mode == "sond":
         return inference_sond(mode=mode, **kwargs)
     elif mode == "sond_demo":
         param_dict = {
             "extract_profile": True,
             "sv_train_config": "sv.yaml",
@@ -382,14 +360,15 @@
         return inference_sond(mode=mode, **kwargs)
     elif mode == "eend-ola":
         return inference_eend(mode=mode, **kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Speaker Verification",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
```

### Comparing `funasr-0.6.2/funasr/bin/diar_train.py` & `funasr-0.6.3/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/lm_inference_launch.py` & `funasr-0.6.3/funasr/bin/lm_inference_launch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,116 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils.types import float_or_none
-import argparse
-import logging
-from pathlib import Path
-import sys
-import os
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
-from typing import Dict
 from typing import Any
 from typing import List
+from typing import Optional
+from typing import Union
 
 import numpy as np
 import torch
 from torch.nn.parallel import data_parallel
 from typeguard import check_argument_types
 
-from funasr.tasks.lm import LMTask
+from funasr.build_utils.build_model_from_file import build_model_from_file
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.datasets.preprocessor import LMPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import float_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 
 
 def inference_lm(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    log_base: Optional[float] = 10,
-    allow_variable_data_keys: bool = False,
-    split_with_space: Optional[bool] = False,
-    seg_dict_file: Optional[str] = None,
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
+        batch_size: int,
+        dtype: str,
+        ngpu: int,
+        seed: int,
+        num_workers: int,
+        log_level: Union[int, str],
+        key_file: Optional[str],
+        train_config: Optional[str],
+        model_file: Optional[str],
+        log_base: Optional[float] = 10,
+        allow_variable_data_keys: bool = False,
+        split_with_space: Optional[bool] = False,
+        seg_dict_file: Optional[str] = None,
+        output_dir: Optional[str] = None,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build Model
-    model, train_args = LMTask.build_model_from_file(
-        train_config, model_file, device)
+    model, train_args = build_model_from_file(
+        train_config, model_file, None, device, "lm")
     wrapped_model = ForwardAdaptor(model, "nll")
     wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
     logging.info(f"Model:\n{model}")
-    
+
     preprocessor = LMPreprocessor(
         train=False,
         token_type=train_args.token_type,
         token_list=train_args.token_list,
         bpemodel=train_args.bpemodel,
         text_cleaner=train_args.cleaner,
         g2p_type=train_args.g2p,
         text_name="text",
         non_linguistic_symbols=train_args.non_linguistic_symbols,
         split_with_space=split_with_space,
         seg_dict_file=seg_dict_file
     )
-    
+
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        param_dict: dict = None,
+            data_path_and_name_and_type,
+            raw_inputs: Union[List[Any], bytes, str] = None,
+            output_dir_v2: Optional[str] = None,
+            param_dict: dict = None,
     ):
         results = []
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         if output_path is not None:
             writer = DatadirWriter(output_path)
         else:
             writer = None
-        
+
         if raw_inputs != None:
             line = raw_inputs.strip()
             key = "lm demo"
             if line == "":
                 item = {'key': key, 'value': ""}
                 results.append(item)
                 return results
             batch = {}
             batch['text'] = line
             if preprocessor != None:
                 batch = preprocessor(key, batch)
-            
+
             #  Force data-precision
             for name in batch:
                 value = batch[name]
                 if not isinstance(value, np.ndarray):
                     raise RuntimeError(
                         f"All values must be converted to np.ndarray object "
                         f'by preprocessing, but "{name}" is still {type(value)}.'
@@ -134,19 +119,19 @@
                 if value.dtype.kind == "f":
                     value = value.astype("float32")
                 elif value.dtype.kind == "i":
                     value = value.astype("long")
                 else:
                     raise NotImplementedError(f"Not supported dtype: {value.dtype}")
                 batch[name] = value
-            
+
             batch["text_lengths"] = torch.from_numpy(
                 np.array([len(batch["text"])], dtype='int32'))
             batch["text"] = np.expand_dims(batch["text"], axis=0)
-            
+
             with torch.no_grad():
                 batch = to_device(batch, device)
                 if ngpu <= 1:
                     nll, lengths = wrapped_model(**batch)
                 else:
                     nll, lengths = data_parallel(
                         wrapped_model, (), range(ngpu), module_kwargs=batch
@@ -169,15 +154,15 @@
                         ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
                             cur=cur_word,
                             pre=pre_word,
                             prob=round(word_prob.item(), 8),
                             word_nll=round(word_nll.item(), 8)
                         )
                         pre_word = cur_word
-                    
+
                     sent_nll_mean = sent_nll.mean().cpu().numpy()
                     sent_nll_sum = sent_nll.sum().cpu().numpy()
                     if log_base is None:
                         sent_ppl = np.exp(sent_nll_mean)
                     else:
                         sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
                     ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
@@ -185,40 +170,38 @@
                         sent_ppl=round(sent_ppl.item(), 4)
                     )
                     ppl_out_batch += ppl_out
                     item = {'key': key, 'value': ppl_out}
                     if writer is not None:
                         writer["ppl"][key + ":\n"] = ppl_out
                     results.append(item)
-            
+
             return results
-        
+
         # 3. Build data-iterator
-        loader = LMTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="lm",
+            preprocess_args=train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=preprocessor,
-            collate_fn=LMTask.build_collate_fn(train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         # 4. Start for-loop
         total_nll = 0.0
         total_ntokens = 0
         ppl_out_all = ""
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            
+
             ppl_out_batch = ""
             with torch.no_grad():
                 batch = to_device(batch, device)
                 if ngpu <= 1:
                     # NOTE(kamo): data_parallel also should work with ngpu=1,
                     # but for debuggability it's better to keep this block.
                     nll, lengths = wrapped_model(**batch)
@@ -243,15 +226,15 @@
                         ppl_out += '    p( {cur} | {pre} ) = {prob} [ {word_nll} ]\n'.format(
                             cur=cur_word,
                             pre=pre_word,
                             prob=round(word_prob.item(), 8),
                             word_nll=round(word_nll.item(), 8)
                         )
                         pre_word = cur_word
-                    
+
                     sent_nll_mean = sent_nll.mean().cpu().numpy()
                     sent_nll_sum = sent_nll.sum().cpu().numpy()
                     if log_base is None:
                         sent_ppl = np.exp(sent_nll_mean)
                     else:
                         sent_ppl = log_base ** (sent_nll_mean / np.log(log_base))
                     ppl_out += 'logprob= {sent_nll} ppl= {sent_ppl}\n\n'.format(
@@ -261,52 +244,53 @@
                     ppl_out_batch += ppl_out
                     utt2nll = round(-sent_nll_sum.item(), 5)
                     item = {'key': key, 'value': ppl_out}
                     if writer is not None:
                         writer["ppl"][key + ":\n"] = ppl_out
                         writer["utt2nll"][key] = str(utt2nll)
                     results.append(item)
-            
+
             ppl_out_all += ppl_out_batch
-            
+
             assert _bs == len(nll) == len(lengths), (_bs, len(nll), len(lengths))
             # nll: (B, L) -> (B,)
             nll = nll.detach().cpu().numpy().sum(1)
             # lengths: (B,)
             lengths = lengths.detach().cpu().numpy()
             total_nll += nll.sum()
             total_ntokens += lengths.sum()
-        
+
         if log_base is None:
             ppl = np.exp(total_nll / total_ntokens)
         else:
             ppl = log_base ** (total_nll / total_ntokens / np.log(log_base))
-        
+
         avg_ppl = 'logprob= {total_nll} ppl= {total_ppl}\n'.format(
             total_nll=round(-total_nll.item(), 4),
             total_ppl=round(ppl.item(), 4)
         )
         item = {'key': 'AVG PPL', 'value': avg_ppl}
         ppl_out_all += avg_ppl
         if writer is not None:
             writer["ppl"]["AVG PPL : "] = avg_ppl
         results.append(item)
-        
+
         return results
-    
+
     return _forward
 
 
 def inference_launch(mode, **kwargs):
     if mode == "transformer":
         return inference_lm(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
-    
+
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Calc perplexity",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
@@ -403,8 +387,7 @@
     kwargs.pop("njob", None)
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `funasr-0.6.2/funasr/bin/lm_train.py` & `funasr-0.6.3/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/punc_infer.py` & `funasr-0.6.3/funasr/bin/punc_infer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,36 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
-import logging
-from pathlib import Path
-import sys
 from typing import Optional
-from typing import Sequence
-from typing import Tuple
 from typing import Union
-from typing import Any
-from typing import List
 
 import numpy as np
 import torch
-from typeguard import check_argument_types
 
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.punctuation import PunctuationTask
+from funasr.datasets.preprocessor import split_to_mini_sentence
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.datasets.preprocessor import split_to_mini_sentence
 
 
 class Text2Punc:
 
     def __init__(
-        self,
-        train_config: Optional[str],
-        model_file: Optional[str],
-        device: str = "cpu",
-        dtype: str = "float32",
+            self,
+            train_config: Optional[str],
+            model_file: Optional[str],
+            device: str = "cpu",
+            dtype: str = "float32",
     ):
         #  Build Model
-        model, train_args = PunctuationTask.build_model_from_file(train_config, model_file, device)
+        model, train_args = build_model_from_file(train_config, model_file, None, device, task_name="punc")
         self.device = device
         # Wrape model to make model.nll() data-parallel
         self.wrapped_model = ForwardAdaptor(model, "inference")
         self.wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
         # logging.info(f"Model:\n{model}")
         self.punc_list = train_args.punc_list
         self.period = 0
@@ -140,24 +126,24 @@
                 elif new_mini_sentence[-1] != "。" and new_mini_sentence[-1] != "？":
                     new_mini_sentence_out = new_mini_sentence + "。"
                     new_mini_sentence_punc_out = new_mini_sentence_punc[:-1] + [self.period]
         return new_mini_sentence_out, new_mini_sentence_punc_out
 
 
 class Text2PuncVADRealtime:
-    
+
     def __init__(
-        self,
-        train_config: Optional[str],
-        model_file: Optional[str],
-        device: str = "cpu",
-        dtype: str = "float32",
+            self,
+            train_config: Optional[str],
+            model_file: Optional[str],
+            device: str = "cpu",
+            dtype: str = "float32",
     ):
         #  Build Model
-        model, train_args = PunctuationTask.build_model_from_file(train_config, model_file, device)
+        model, train_args = build_model_from_file(train_config, model_file, None, device, task_name="punc")
         self.device = device
         # Wrape model to make model.nll() data-parallel
         self.wrapped_model = ForwardAdaptor(model, "inference")
         self.wrapped_model.to(dtype=getattr(torch, dtype)).to(device=device).eval()
         # logging.info(f"Model:\n{model}")
         self.punc_list = train_args.punc_list
         self.period = 0
@@ -174,15 +160,15 @@
             token_list=train_args.token_list,
             bpemodel=train_args.bpemodel,
             text_cleaner=train_args.cleaner,
             g2p_type=train_args.g2p,
             text_name="text",
             non_linguistic_symbols=train_args.non_linguistic_symbols,
         )
-    
+
     @torch.no_grad()
     def __call__(self, text: Union[list, str], cache: list, split_size=20):
         if cache is not None and len(cache) > 0:
             precache = "".join(cache)
         else:
             precache = ""
             cache = []
@@ -211,39 +197,39 @@
             data = to_device(data, self.device)
             y, _ = self.wrapped_model(**data)
             _, indices = y.view(-1, y.shape[-1]).topk(1, dim=1)
             punctuations = indices
             if indices.size()[0] != 1:
                 punctuations = torch.squeeze(indices)
             assert punctuations.size()[0] == len(mini_sentence)
-            
+
             # Search for the last Period/QuestionMark as cache
             if mini_sentence_i < len(mini_sentences) - 1:
                 sentenceEnd = -1
                 last_comma_index = -1
                 for i in range(len(punctuations) - 2, 1, -1):
                     if self.punc_list[punctuations[i]] == "。" or self.punc_list[punctuations[i]] == "？":
                         sentenceEnd = i
                         break
                     if last_comma_index < 0 and self.punc_list[punctuations[i]] == "，":
                         last_comma_index = i
-                
+
                 if sentenceEnd < 0 and len(mini_sentence) > cache_pop_trigger_limit and last_comma_index >= 0:
                     # The sentence it too long, cut off at a comma.
                     sentenceEnd = last_comma_index
                     punctuations[sentenceEnd] = self.period
                 cache_sent = mini_sentence[sentenceEnd + 1:]
                 cache_sent_id = mini_sentence_id[sentenceEnd + 1:]
                 mini_sentence = mini_sentence[0:sentenceEnd + 1]
                 punctuations = punctuations[0:sentenceEnd + 1]
-            
+
             punctuations_np = punctuations.cpu().numpy()
             sentence_punc_list += [self.punc_list[int(x)] for x in punctuations_np]
             sentence_words_list += mini_sentence
-        
+
         assert len(sentence_punc_list) == len(sentence_words_list)
         words_with_punc = []
         sentence_punc_list_out = []
         for i in range(0, len(sentence_words_list)):
             if i > 0:
                 if len(sentence_words_list[i][0].encode()) == 1 and len(sentence_words_list[i - 1][-1].encode()) == 1:
                     sentence_words_list[i] = " " + sentence_words_list[i]
@@ -252,20 +238,18 @@
             else:
                 words_with_punc.append(sentence_words_list[i])
             if skip_num >= len(cache):
                 sentence_punc_list_out.append(sentence_punc_list[i])
                 if sentence_punc_list[i] != "_":
                     words_with_punc.append(sentence_punc_list[i])
         sentence_out = "".join(words_with_punc)
-        
+
         sentenceEnd = -1
         for i in range(len(sentence_punc_list) - 2, 1, -1):
             if sentence_punc_list[i] == "。" or sentence_punc_list[i] == "？":
                 sentenceEnd = i
                 break
         cache_out = sentence_words_list[sentenceEnd + 1:]
         if sentence_out[-1] in self.punc_list:
             sentence_out = sentence_out[:-1]
             sentence_punc_list_out[-1] = "_"
         return sentence_out, sentence_punc_list_out, cache_out
-
-
```

### Comparing `funasr-0.6.2/funasr/bin/punc_inference_launch.py` & `funasr-0.6.3/funasr/bin/punc_inference_launch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,46 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils.types import float_or_none
-
-import argparse
-import logging
 from pathlib import Path
-import sys
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
 from typing import Any
 from typing import List
+from typing import Optional
+from typing import Union
 
-import numpy as np
 import torch
 from typeguard import check_argument_types
 
-from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.punctuation import PunctuationTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.forward_adaptor import ForwardAdaptor
+from funasr.bin.punc_infer import Text2Punc, Text2PuncVADRealtime
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.datasets.preprocessor import split_to_mini_sentence
-from funasr.bin.punc_infer import Text2Punc, Text2PuncVADRealtime
+
 
 def inference_punc(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
+        batch_size: int,
+        dtype: str,
+        ngpu: int,
+        seed: int,
+        num_workers: int,
+        log_level: Union[int, str],
+        key_file: Optional[str],
+        train_config: Optional[str],
+        model_file: Optional[str],
+        output_dir: Optional[str] = None,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
@@ -69,19 +50,19 @@
         device = "cpu"
 
     # 1. Set random-seed
     set_all_random_seed(seed)
     text2punc = Text2Punc(train_config, model_file, device)
 
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        cache: List[Any] = None,
-        param_dict: dict = None,
+            data_path_and_name_and_type,
+            raw_inputs: Union[List[Any], bytes, str] = None,
+            output_dir_v2: Optional[str] = None,
+            cache: List[Any] = None,
+            param_dict: dict = None,
     ):
         results = []
         split_size = 20
 
         if raw_inputs != None:
             line = raw_inputs.strip()
             key = "demo"
@@ -117,28 +98,29 @@
                     key_out = item_i["key"]
                     value_out = item_i["value"]
                     fout.write(f"{key_out}\t{value_out}\n")
         return results
 
     return _forward
 
+
 def inference_punc_vad_realtime(
-    batch_size: int,
-    dtype: str,
-    ngpu: int,
-    seed: int,
-    num_workers: int,
-    log_level: Union[int, str],
-    #cache: list,
-    key_file: Optional[str],
-    train_config: Optional[str],
-    model_file: Optional[str],
-    output_dir: Optional[str] = None,
-    param_dict: dict = None,
-    **kwargs,
+        batch_size: int,
+        dtype: str,
+        ngpu: int,
+        seed: int,
+        num_workers: int,
+        log_level: Union[int, str],
+        # cache: list,
+        key_file: Optional[str],
+        train_config: Optional[str],
+        model_file: Optional[str],
+        output_dir: Optional[str] = None,
+        param_dict: dict = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
@@ -146,19 +128,19 @@
         device = "cpu"
 
     # 1. Set random-seed
     set_all_random_seed(seed)
     text2punc = Text2PuncVADRealtime(train_config, model_file, device)
 
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[List[Any], bytes, str] = None,
-        output_dir_v2: Optional[str] = None,
-        cache: List[Any] = None,
-        param_dict: dict = None,
+            data_path_and_name_and_type,
+            raw_inputs: Union[List[Any], bytes, str] = None,
+            output_dir_v2: Optional[str] = None,
+            cache: List[Any] = None,
+            param_dict: dict = None,
     ):
         results = []
         split_size = 10
         cache_in = param_dict["cache"]
         if raw_inputs != None:
             line = raw_inputs.strip()
             key = "demo"
@@ -173,24 +155,24 @@
             return results
 
         return results
 
     return _forward
 
 
-
 def inference_launch(mode, **kwargs):
     if mode == "punc":
         return inference_punc(**kwargs)
     if mode == "punc_VadRealtime":
         return inference_punc_vad_realtime(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Punctuation inference",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
@@ -265,10 +247,9 @@
 
     kwargs.pop("gpuid_list", None)
     kwargs.pop("njob", None)
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.6.2/funasr/bin/punc_train.py` & `funasr-0.6.3/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/sa_asr_train.py` & `funasr-0.6.3/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/sv_infer.py` & `funasr-0.6.3/funasr/bin/sv_infer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
 import logging
-import os
-import sys
 from pathlib import Path
 from typing import Any
-from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
-from kaldiio import WriteHelper
 from typeguard import check_argument_types
 from typeguard import check_return_type
 
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.sv import SVTask
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
 from funasr.utils.misc import statistic_model_parameters
 
+
 class Speech2Xvector:
     """Speech2Xvector class
 
     Examples:
         >>> import soundfile
         >>> speech2xvector = Speech2Xvector("sv_config.yml", "sv.pb")
         >>> audio, rate = soundfile.read("speech.wav")
@@ -52,18 +41,21 @@
             dtype: str = "float32",
             streaming: bool = False,
             embedding_node: str = "resnet1_dense",
     ):
         assert check_argument_types()
 
         # TODO: 1. Build SV model
-        sv_model, sv_train_args = SVTask.build_model_from_file(
+        sv_model, sv_train_args = build_model_from_file(
             config_file=sv_train_config,
             model_file=sv_model_file,
-            device=device
+            cmvn_file=None,
+            device=device,
+            task_name="sv",
+            mode="sv",
         )
         logging.info("sv_model: {}".format(sv_model))
         logging.info("model parameter number: {}".format(statistic_model_parameters(sv_model)))
         logging.info("sv_train_args: {}".format(sv_train_args))
         sv_model.to(dtype=getattr(torch, dtype)).eval()
 
         self.sv_model = sv_model
@@ -153,11 +145,7 @@
                     "Please install via `pip install -U espnet_model_zoo`."
                 )
                 raise
             d = ModelDownloader()
             kwargs.update(**d.download_and_unpack(model_tag))
 
         return Speech2Xvector(**kwargs)
-
-
-
-
```

### Comparing `funasr-0.6.2/funasr/bin/sv_inference_launch.py` & `funasr-0.6.3/funasr/bin/sv_inference_launch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,94 +1,78 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-import argparse
-import logging
-import os
-import sys
-from pathlib import Path
-from typing import Any
-from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import torch
 from kaldiio import WriteHelper
 from typeguard import check_argument_types
-from typeguard import check_return_type
 
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.tasks.sv import SVTask
-from funasr.torch_utils.device_funcs import to_device
+from funasr.bin.sv_infer import Speech2Xvector
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
+from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils.misc import statistic_model_parameters
-from funasr.bin.sv_infer import Speech2Xvector
+
 
 def inference_sv(
-    output_dir: Optional[str] = None,
-    batch_size: int = 1,
-    dtype: str = "float32",
-    ngpu: int = 1,
-    seed: int = 0,
-    num_workers: int = 0,
-    log_level: Union[int, str] = "INFO",
-    key_file: Optional[str] = None,
-    sv_train_config: Optional[str] = "sv.yaml",
-    sv_model_file: Optional[str] = "sv.pb",
-    model_tag: Optional[str] = None,
-    allow_variable_data_keys: bool = True,
-    streaming: bool = False,
-    embedding_node: str = "resnet1_dense",
-    sv_threshold: float = 0.9465,
-    param_dict: Optional[dict] = None,
-    **kwargs,
+        output_dir: Optional[str] = None,
+        batch_size: int = 1,
+        dtype: str = "float32",
+        ngpu: int = 1,
+        seed: int = 0,
+        num_workers: int = 0,
+        log_level: Union[int, str] = "INFO",
+        key_file: Optional[str] = None,
+        sv_train_config: Optional[str] = "sv.yaml",
+        sv_model_file: Optional[str] = "sv.pb",
+        model_tag: Optional[str] = None,
+        allow_variable_data_keys: bool = True,
+        streaming: bool = False,
+        embedding_node: str = "resnet1_dense",
+        sv_threshold: float = 0.9465,
+        param_dict: Optional[dict] = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    
+
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
     logging.info("param_dict: {}".format(param_dict))
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-    
+
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2xvector
     speech2xvector_kwargs = dict(
         sv_train_config=sv_train_config,
         sv_model_file=sv_model_file,
         device=device,
         dtype=dtype,
         streaming=streaming,
@@ -96,54 +80,53 @@
     )
     logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
     speech2xvector = Speech2Xvector.from_pretrained(
         model_tag=model_tag,
         **speech2xvector_kwargs,
     )
     speech2xvector.sv_model.eval()
-    
+
     def _forward(
-        data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        output_dir_v2: Optional[str] = None,
-        param_dict: Optional[dict] = None,
+            data_path_and_name_and_type: Sequence[Tuple[str, str, str]] = None,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            param_dict: Optional[dict] = None,
     ):
         logging.info("param_dict: {}".format(param_dict))
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        
+
         # 3. Build data-iterator
-        loader = SVTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="sv",
+            preprocess_args=None,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=None,
-            collate_fn=None,
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
+            use_collate_fn=False,
         )
-        
+
         # 7 .Start for-loop
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         embd_writer, ref_embd_writer, score_writer = None, None, None
         if output_path is not None:
             os.makedirs(output_path, exist_ok=True)
             embd_writer = WriteHelper("ark,scp:{}/xvector.ark,{}/xvector.scp".format(output_path, output_path))
         sv_result_list = []
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
             batch = {k: v[0] for k, v in batch.items() if not k.endswith("_lengths")}
-            
+
             embedding, ref_embedding, score = speech2xvector(**batch)
             # Only supporting batch_size==1
             key = keys[0]
             normalized_score = 0.0
             if score is not None:
                 score = score.item()
                 normalized_score = max(score - sv_threshold, 0.0) / (1.0 - sv_threshold) * 100.0
@@ -157,35 +140,34 @@
                     if ref_embd_writer is None:
                         ref_embd_writer = WriteHelper(
                             "ark,scp:{}/ref_xvector.ark,{}/ref_xvector.scp".format(output_path, output_path)
                         )
                         score_writer = open(os.path.join(output_path, "score.txt"), "w")
                     ref_embd_writer(key, ref_embedding[0].cpu().numpy())
                     score_writer.write("{} {:.6f}\n".format(key, normalized_score))
-        
+
         if output_path is not None:
             embd_writer.close()
             if ref_embd_writer is not None:
                 ref_embd_writer.close()
                 score_writer.close()
-        
-        return sv_result_list
-    
-    return _forward
 
+        return sv_result_list
 
+    return _forward
 
 
 def inference_launch(mode, **kwargs):
     if mode == "sv":
         return inference_sv(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Speaker Verification",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
```

### Comparing `funasr-0.6.2/funasr/bin/tokenize_text.py` & `funasr-0.6.3/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/bin/tp_infer.py` & `funasr-0.6.3/funasr/bin/tp_infer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,72 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
 import logging
-from optparse import Option
-import sys
-import json
 from pathlib import Path
-from typing import Any
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
 from typing import Union
-from typing import Dict
 
 import numpy as np
 import torch
 from typeguard import check_argument_types
-
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.datasets.preprocessor import LMPreprocessor
-from funasr.tasks.asr import ASRTaskAligner as ASRTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.text.token_id_converter import TokenIDConverter
-from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
-
-
+from funasr.torch_utils.device_funcs import to_device
 
 
 class Speech2Timestamp:
     def __init__(
-        self,
-        timestamp_infer_config: Union[Path, str] = None,
-        timestamp_model_file: Union[Path, str] = None,
-        timestamp_cmvn_file: Union[Path, str] = None,
-        device: str = "cpu",
-        dtype: str = "float32",
-        **kwargs,
+            self,
+            timestamp_infer_config: Union[Path, str] = None,
+            timestamp_model_file: Union[Path, str] = None,
+            timestamp_cmvn_file: Union[Path, str] = None,
+            device: str = "cpu",
+            dtype: str = "float32",
+            **kwargs,
     ):
         assert check_argument_types()
         # 1. Build ASR model
-        tp_model, tp_train_args = ASRTask.build_model_from_file(
-            timestamp_infer_config, timestamp_model_file, device=device
+        tp_model, tp_train_args = build_model_from_file(
+            timestamp_infer_config, timestamp_model_file, cmvn_file=None, device=device, task_name="asr", mode="tp"
         )
         if 'cuda' in device:
             tp_model = tp_model.cuda()  # force model to cuda
 
         frontend = None
         if tp_train_args.frontend is not None:
             frontend = WavFrontend(cmvn_file=timestamp_cmvn_file, **tp_train_args.frontend_conf)
-        
+
         logging.info("tp_model: {}".format(tp_model))
         logging.info("tp_train_args: {}".format(tp_train_args))
         tp_model.to(dtype=getattr(torch, dtype)).eval()
 
         logging.info(f"Decoding device={device}, dtype={dtype}")
 
-
         self.tp_model = tp_model
         self.tp_train_args = tp_train_args
 
         token_list = self.tp_model.token_list
         self.converter = TokenIDConverter(token_list=token_list)
 
         self.device = device
         self.dtype = dtype
         self.frontend = frontend
         self.encoder_downsampling_factor = 1
         if tp_train_args.encoder_conf["input_layer"] == "conv2d":
             self.encoder_downsampling_factor = 4
-    
+
     @torch.no_grad()
     def __call__(
-        self, 
-        speech: Union[torch.Tensor, np.ndarray], 
-        speech_lengths: Union[torch.Tensor, np.ndarray] = None, 
-        text_lengths: Union[torch.Tensor, np.ndarray] = None
+            self,
+            speech: Union[torch.Tensor, np.ndarray],
+            speech_lengths: Union[torch.Tensor, np.ndarray] = None,
+            text_lengths: Union[torch.Tensor, np.ndarray] = None
     ):
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
         if self.frontend is not None:
@@ -109,12 +86,10 @@
 
         # b. Forward Encoder
         enc, enc_len = self.tp_model.encode(**batch)
         if isinstance(enc, tuple):
             enc = enc[0]
 
         # c. Forward Predictor
-        _, _, us_alphas, us_peaks = self.tp_model.calc_predictor_timestamp(enc, enc_len, text_lengths.to(self.device)+1)
+        _, _, us_alphas, us_peaks = self.tp_model.calc_predictor_timestamp(enc, enc_len,
+                                                                           text_lengths.to(self.device) + 1)
         return us_alphas, us_peaks
-
-
-
```

### Comparing `funasr-0.6.2/funasr/bin/tp_inference_launch.py` & `funasr-0.6.3/funasr/bin/tp_inference_launch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,200 +1,177 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 
 import argparse
 import logging
 import os
 import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-
-import argparse
-import logging
-from optparse import Option
-import sys
-import json
-from pathlib import Path
-from typing import Any
-from typing import List
 from typing import Optional
-from typing import Sequence
-from typing import Tuple
 from typing import Union
-from typing import Dict
 
 import numpy as np
 import torch
 from typeguard import check_argument_types
 
-from funasr.fileio.datadir_writer import DatadirWriter
+from funasr.bin.tp_infer import Speech2Timestamp
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.datasets.preprocessor import LMPreprocessor
-from funasr.tasks.asr import ASRTaskAligner as ASRTask
-from funasr.torch_utils.device_funcs import to_device
+from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
+from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.text.token_id_converter import TokenIDConverter
-from funasr.utils.timestamp_tools import ts_prediction_lfr6_standard
-from funasr.bin.tp_infer import Speech2Timestamp
+
 
 def inference_tp(
-    batch_size: int,
-    ngpu: int,
-    log_level: Union[int, str],
-    # data_path_and_name_and_type,
-    timestamp_infer_config: Optional[str],
-    timestamp_model_file: Optional[str],
-    timestamp_cmvn_file: Optional[str] = None,
-    # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-    key_file: Optional[str] = None,
-    allow_variable_data_keys: bool = False,
-    output_dir: Optional[str] = None,
-    dtype: str = "float32",
-    seed: int = 0,
-    num_workers: int = 1,
-    split_with_space: bool = True,
-    seg_dict_file: Optional[str] = None,
-    **kwargs,
+        batch_size: int,
+        ngpu: int,
+        log_level: Union[int, str],
+        # data_path_and_name_and_type,
+        timestamp_infer_config: Optional[str],
+        timestamp_model_file: Optional[str],
+        timestamp_cmvn_file: Optional[str] = None,
+        # raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+        key_file: Optional[str] = None,
+        allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
+        dtype: str = "float32",
+        seed: int = 0,
+        num_workers: int = 1,
+        split_with_space: bool = True,
+        seg_dict_file: Optional[str] = None,
+        **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
-    
+
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
-    
+
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
-    
+
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
     # 1. Set random-seed
     set_all_random_seed(seed)
-    
+
     # 2. Build speech2vadsegment
     speechtext2timestamp_kwargs = dict(
         timestamp_infer_config=timestamp_infer_config,
         timestamp_model_file=timestamp_model_file,
         timestamp_cmvn_file=timestamp_cmvn_file,
         device=device,
         dtype=dtype,
     )
     logging.info("speechtext2timestamp_kwargs: {}".format(speechtext2timestamp_kwargs))
     speechtext2timestamp = Speech2Timestamp(**speechtext2timestamp_kwargs)
-    
+
     preprocessor = LMPreprocessor(
         train=False,
         token_type=speechtext2timestamp.tp_train_args.token_type,
         token_list=speechtext2timestamp.tp_train_args.token_list,
         bpemodel=None,
         text_cleaner=None,
         g2p_type=None,
         text_name="text",
         non_linguistic_symbols=speechtext2timestamp.tp_train_args.non_linguistic_symbols,
         split_with_space=split_with_space,
         seg_dict_file=seg_dict_file,
     )
-    
+
     if output_dir is not None:
         writer = DatadirWriter(output_dir)
         tp_writer = writer[f"timestamp_prediction"]
         # ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
     else:
         tp_writer = None
-    
+
     def _forward(
-        data_path_and_name_and_type,
-        raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-        output_dir_v2: Optional[str] = None,
-        fs: dict = None,
-        param_dict: dict = None,
-        **kwargs
+            data_path_and_name_and_type,
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None,
+            **kwargs
     ):
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
         writer = None
         if output_path is not None:
             writer = DatadirWriter(output_path)
             tp_writer = writer[f"timestamp_prediction"]
         else:
             tp_writer = None
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        
-        loader = ASRTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+
+        loader = build_streaming_iterator(
+            task_name="asr",
+            preprocess_args=speechtext2timestamp.tp_train_args,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
             preprocess_fn=preprocessor,
-            collate_fn=ASRTask.build_collate_fn(speechtext2timestamp.tp_train_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
-        
+
         tp_result_list = []
         for keys, batch in loader:
             assert isinstance(batch, dict), type(batch)
             assert all(isinstance(s, str) for s in keys), keys
             _bs = len(next(iter(batch.values())))
             assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-            
+
             logging.info("timestamp predicting, utt_id: {}".format(keys))
             _batch = {'speech': batch['speech'],
                       'speech_lengths': batch['speech_lengths'],
                       'text_lengths': batch['text_lengths']}
             us_alphas, us_cif_peak = speechtext2timestamp(**_batch)
-            
+
             for batch_id in range(_bs):
                 key = keys[batch_id]
                 token = speechtext2timestamp.converter.ids2tokens(batch['text'][batch_id])
                 ts_str, ts_list = ts_prediction_lfr6_standard(us_alphas[batch_id], us_cif_peak[batch_id], token,
                                                               force_time_shift=-3.0)
                 logging.warning(ts_str)
                 item = {'key': key, 'value': ts_str, 'timestamp': ts_list}
                 if tp_writer is not None:
                     tp_writer["tp_sync"][key + '#'] = ts_str
                     tp_writer["tp_time"][key + '#'] = str(ts_list)
                 tp_result_list.append(item)
         return tp_result_list
-    
-    return _forward
-
 
+    return _forward
 
 
 def inference_launch(mode, **kwargs):
     if mode == "tp_norm":
         return inference_tp(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="Timestamp Prediction Inference",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -304,10 +281,9 @@
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
 
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.6.2/funasr/bin/train.py` & `funasr-0.6.3/funasr/bin/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import argparse
 import logging
 import os
 import sys
 from io import BytesIO
```

### Comparing `funasr-0.6.2/funasr/bin/vad_infer.py` & `funasr-0.6.3/funasr/bin/vad_infer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,27 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
-import argparse
 import logging
-import os
-import sys
-import json
+import math
 from pathlib import Path
-from typing import Any
+from typing import Dict
 from typing import List
-from typing import Optional
-from typing import Sequence
 from typing import Tuple
 from typing import Union
-from typing import Dict
 
-import math
 import numpy as np
 import torch
 from typeguard import check_argument_types
-from typeguard import check_return_type
 
-from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.vad import VADTask
-from funasr.torch_utils.device_funcs import to_device
-from funasr.torch_utils.set_all_random_seed import set_all_random_seed
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
+from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
-
+from funasr.torch_utils.device_funcs import to_device
 
 
 class Speech2VadSegment:
     """Speech2VadSegment class
 
     Examples:
         >>> import soundfile
@@ -60,16 +41,16 @@
             batch_size: int = 1,
             dtype: str = "float32",
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build vad model
-        vad_model, vad_infer_args = VADTask.build_model_from_file(
-            vad_infer_config, vad_model_file, device
+        vad_model, vad_infer_args = build_model_from_file(
+            vad_infer_config, vad_model_file, None, device, task_name="vad"
         )
         frontend = None
         if vad_infer_args.frontend is not None:
             frontend = WavFrontend(cmvn_file=vad_cmvn_file, **vad_infer_args.frontend_conf)
 
         logging.info("vad_model: {}".format(vad_model))
         logging.info("vad_infer_args: {}".format(vad_infer_args))
@@ -124,40 +105,41 @@
             batch = {
                 "feats": feats[:, t_offset:t_offset + step, :],
                 "waveform": speech[:, t_offset * 160:min(speech.shape[-1], (t_offset + step - 1) * 160 + 400)],
                 "is_final": is_final,
                 "in_cache": in_cache
             }
             # a. To device
-            #batch = to_device(batch, device=self.device)
+            # batch = to_device(batch, device=self.device)
             segments_part, in_cache = self.vad_model(**batch)
             if segments_part:
                 for batch_num in range(0, self.batch_size):
                     segments[batch_num] += segments_part[batch_num]
         return fbanks, segments
 
+
 class Speech2VadSegmentOnline(Speech2VadSegment):
     """Speech2VadSegmentOnline class
 
     Examples:
         >>> import soundfile
         >>> speech2segment = Speech2VadSegmentOnline("vad_config.yml", "vad.pt")
         >>> audio, rate = soundfile.read("speech.wav")
         >>> speech2segment(audio)
         [[10, 230], [245, 450], ...]
 
     """
+
     def __init__(self, **kwargs):
         super(Speech2VadSegmentOnline, self).__init__(**kwargs)
         vad_cmvn_file = kwargs.get('vad_cmvn_file', None)
         self.frontend = None
         if self.vad_infer_args.frontend is not None:
             self.frontend = WavFrontendOnline(cmvn_file=vad_cmvn_file, **self.vad_infer_args.frontend_conf)
 
-
     @torch.no_grad()
     def __call__(
             self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
             in_cache: Dict[str, torch.Tensor] = dict(), is_final: bool = False, max_end_sil: int = 800
     ) -> Tuple[torch.Tensor, List[List[int]], torch.Tensor]:
         """Inference
 
@@ -194,9 +176,7 @@
             }
             # a. To device
             batch = to_device(batch, device=self.device)
             segments, in_cache = self.vad_model.forward_online(**batch)
             # in_cache.update(batch['in_cache'])
             # in_cache = {key: value for key, value in batch['in_cache'].items()}
         return fbanks, segments, in_cache
-
-
```

### Comparing `funasr-0.6.2/funasr/bin/vad_inference_launch.py` & `funasr-0.6.3/funasr/bin/vad_inference_launch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,39 @@
-# -*- encoding: utf-8 -*-
 #!/usr/bin/env python3
+# -*- encoding: utf-8 -*-
 # Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 
 import torch
-torch.set_num_threads(1)
 
-import argparse
-import logging
-import os
-import sys
-from typing import Union, Dict, Any
-
-from funasr.utils import config_argparse
-from funasr.utils.cli_utils import get_commandline_args
-from funasr.utils.types import str2bool
-from funasr.utils.types import str2triple_str
-from funasr.utils.types import str_or_none
+torch.set_num_threads(1)
 
 import argparse
 import logging
 import os
 import sys
 import json
-from pathlib import Path
-from typing import Any
-from typing import List
 from typing import Optional
-from typing import Sequence
-from typing import Tuple
 from typing import Union
-from typing import Dict
 
-import math
 import numpy as np
 import torch
 from typeguard import check_argument_types
-from typeguard import check_return_type
-
+from funasr.build_utils.build_streaming_iterator import build_streaming_iterator
 from funasr.fileio.datadir_writer import DatadirWriter
-from funasr.modules.scorers.scorer_interface import BatchScorerInterface
-from funasr.modules.subsampling import TooShortUttError
-from funasr.tasks.vad import VADTask
-from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
-from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
 from funasr.bin.vad_infer import Speech2VadSegment, Speech2VadSegmentOnline
 
+
 def inference_vad(
         batch_size: int,
         ngpu: int,
         log_level: Union[int, str],
         # data_path_and_name_and_type,
         vad_infer_config: Optional[str],
         vad_model_file: Optional[str],
@@ -71,15 +47,14 @@
         num_workers: int = 1,
         **kwargs,
 ):
     assert check_argument_types()
     if batch_size > 1:
         raise NotImplementedError("batch decoding is not implemented")
 
-
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
@@ -108,24 +83,22 @@
             param_dict: dict = None
     ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="vad",
+            preprocess_args=None,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
 
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
@@ -153,14 +126,15 @@
                 if writer is not None:
                     ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
+
 def inference_vad_online(
         batch_size: int,
         ngpu: int,
         log_level: Union[int, str],
         # data_path_and_name_and_type,
         vad_infer_config: Optional[str],
         vad_model_file: Optional[str],
@@ -172,15 +146,14 @@
         dtype: str = "float32",
         seed: int = 0,
         num_workers: int = 1,
         **kwargs,
 ):
     assert check_argument_types()
 
-
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
@@ -210,24 +183,22 @@
             param_dict: dict = None,
     ):
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = VADTask.build_streaming_iterator(
-            data_path_and_name_and_type,
+        loader = build_streaming_iterator(
+            task_name="vad",
+            preprocess_args=None,
+            data_path_and_name_and_type=data_path_and_name_and_type,
             dtype=dtype,
             batch_size=batch_size,
             key_file=key_file,
             num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
         )
 
         finish_count = 0
         file_count = 1
         # 7 .Start for-loop
         # FIXME(kamo): The output format should be discussed about
         output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
@@ -269,25 +240,24 @@
                             ibest_writer["text"][keys[i]] = "{}".format(results[i])
 
         return vad_results
 
     return _forward
 
 
-
-
 def inference_launch(mode, **kwargs):
     if mode == "offline":
         return inference_vad(**kwargs)
     elif mode == "online":
         return inference_vad_online(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
 
+
 def get_parser():
     parser = config_argparse.ArgumentParser(
         description="VAD Decoding",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Note(kamo): Use '_' instead of '-' as separator.
@@ -401,9 +371,10 @@
         gpuid = args.gpuid_list.split(",")[(jobid - 1) // args.njob]
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpuid
 
     inference_pipeline = inference_launch(**kwargs)
     return inference_pipeline(kwargs["data_path_and_name_and_type"])
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_args.py` & `funasr-0.6.3/funasr/build_utils/build_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             default=get_default_kwargs(CTC),
             help="The keyword arguments for CTC class.",
         )
         task_parser.add_argument(
             "--cmvn_file",
             type=str_or_none,
             default=None,
-            help="The file path of noise scp file.",
+            help="The path of cmvn file.",
         )
 
     elif args.task_name == "pretrain":
         from funasr.build_utils.build_pretrain_model import class_choices_list
         for class_choices in class_choices_list:
             class_choices.add_arguments(task_parser)
         task_parser.add_argument(
@@ -71,20 +71,37 @@
             class_choices.add_arguments(task_parser)
         task_parser.add_argument(
             "--input_size",
             type=int_or_none,
             default=None,
             help="The number of input dimension of the feature",
         )
+        task_parser.add_argument(
+            "--cmvn_file",
+            type=str_or_none,
+            default=None,
+            help="The path of cmvn file.",
+        )
 
     elif args.task_name == "diar":
         from funasr.build_utils.build_diar_model import class_choices_list
         for class_choices in class_choices_list:
             class_choices.add_arguments(task_parser)
 
+    elif args.task_name == "sv":
+        from funasr.build_utils.build_sv_model import class_choices_list
+        for class_choices in class_choices_list:
+            class_choices.add_arguments(task_parser)
+        task_parser.add_argument(
+            "--input_size",
+            type=int_or_none,
+            default=None,
+            help="The number of input dimension of the feature",
+        )
+
     else:
         raise NotImplementedError("Not supported task: {}".format(args.task_name))
 
     for action in parser._actions:
         if not any(action.dest == a.dest for a in task_parser._actions):
             task_parser._add_action(action)
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_asr_model.py` & `funasr-0.6.3/funasr/build_utils/build_asr_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,40 @@
 )
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
-from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.decoder.transformer_decoder import SAAsrTransformerDecoder
 from funasr.models.e2e_asr import ASRModel
+from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_asr_mfcca import MFCCA
+
+from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
+
 from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
+
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_uni_asr import UniASR
-from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
 from funasr.models.encoder.resnet34_encoder import ResNet34Diar
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.default import MultiChannelFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.windowing import SlidingWindow
+from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.modules.subsampling import Conv1dSubsampling
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 
@@ -85,14 +89,15 @@
         asr=ASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
         paraformer_online=ParaformerOnline,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
+        neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
         sa_asr=SAASRModel,
 
     ),
@@ -254,48 +259,56 @@
     # --spk_encoder and --spk_encoder_conf
     spk_encoder_choices,
 ]
 
 
 def build_asr_model(args):
     # token_list
-    if args.token_list is not None:
-        with open(args.token_list) as f:
+    if isinstance(args.token_list, str):
+        with open(args.token_list, encoding="utf-8") as f:
             token_list = [line.rstrip() for line in f]
         args.token_list = list(token_list)
         vocab_size = len(token_list)
         logging.info(f"Vocabulary size: {vocab_size}")
+    elif isinstance(args.token_list, (tuple, list)):
+        token_list = list(args.token_list)
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
     else:
+        token_list = None
         vocab_size = None
 
     # frontend
-    if args.input_size is None:
+    if hasattr(args, "input_size") and args.input_size is None:
         frontend_class = frontend_choices.get_class(args.frontend)
         if args.frontend == 'wav_frontend' or args.frontend == 'multichannelfrontend':
             frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
         else:
             frontend = frontend_class(**args.frontend_conf)
         input_size = frontend.output_size()
     else:
         args.frontend = None
         args.frontend_conf = {}
         frontend = None
-        input_size = args.input_size
+        input_size = args.input_size if hasattr(args, "input_size") else None
 
     # data augmentation for spectrogram
     if args.specaug is not None:
         specaug_class = specaug_choices.get_class(args.specaug)
         specaug = specaug_class(**args.specaug_conf)
     else:
         specaug = None
 
     # normalization layer
     if args.normalize is not None:
         normalize_class = normalize_choices.get_class(args.normalize)
-        normalize = normalize_class(**args.normalize_conf)
+        if args.model == "mfcca":
+            normalize = normalize_class(stats_file=args.cmvn_file, **args.normalize_conf)
+        else:
+            normalize = normalize_class(**args.normalize_conf)
     else:
         normalize = None
 
     # encoder
     encoder_class = encoder_choices.get_class(args.encoder)
     encoder = encoder_class(input_size=input_size, **args.encoder_conf)
 
@@ -321,15 +334,16 @@
             normalize=normalize,
             encoder=encoder,
             decoder=decoder,
             ctc=ctc,
             token_list=token_list,
             **args.model_conf,
         )
-    elif args.model in ["paraformer", "paraformer_online", "paraformer_bert", "bicif_paraformer", "contextual_paraformer"]:
+    elif args.model in ["paraformer", "paraformer_online", "paraformer_bert", "bicif_paraformer",
+                        "contextual_paraformer", "neatcontextual_paraformer"]:
         # predictor
         predictor_class = predictor_choices.get_class(args.predictor)
         predictor = predictor_class(**args.predictor_conf)
 
         model_class = model_choices.get_class(args.model)
         model = model_class(
             vocab_size=vocab_size,
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_dataloader.py` & `funasr-0.6.3/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_diar_model.py` & `funasr-0.6.3/funasr/build_utils/build_diar_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,22 +174,26 @@
     # --eda and --eda_conf
     encoder_decoder_attractor_choices,
 ]
 
 
 def build_diar_model(args):
     # token_list
-    if args.token_list is not None:
-        with open(args.token_list) as f:
+    if isinstance(args.token_list, str):
+        with open(args.token_list, encoding="utf-8") as f:
             token_list = [line.rstrip() for line in f]
+
+        # Overwriting token_list to keep it as "portable".
         args.token_list = list(token_list)
-        vocab_size = len(token_list)
-        logging.info(f"Vocabulary size: {vocab_size}")
+    elif isinstance(args.token_list, (tuple, list)):
+        token_list = list(args.token_list)
     else:
-        vocab_size = None
+        raise RuntimeError("token_list must be str or list")
+    vocab_size = len(token_list)
+    logging.info(f"Vocabulary size: {vocab_size}")
 
     # frontend
     if args.input_size is None:
         frontend_class = frontend_choices.get_class(args.frontend)
         if args.frontend == 'wav_frontend':
             frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
         else:
@@ -201,15 +205,15 @@
         frontend = None
         input_size = args.input_size
 
     # encoder
     encoder_class = encoder_choices.get_class(args.encoder)
     encoder = encoder_class(input_size=input_size, **args.encoder_conf)
 
-    if args.model_name == "sond":
+    if args.model == "sond":
         # data augmentation for spectrogram
         if args.specaug is not None:
             specaug_class = specaug_choices.get_class(args.specaug)
             specaug = specaug_class(**args.specaug_conf)
         else:
             specaug = None
 
@@ -239,19 +243,15 @@
             cd_scorer_class = cd_scorer_choices.get_class(args.cd_scorer)
             cd_scorer = cd_scorer_class(**args.cd_scorer_conf)
         else:
             cd_scorer = None
 
         # decoder
         decoder_class = decoder_choices.get_class(args.decoder)
-        decoder = decoder_class(
-            vocab_size=vocab_size,
-            encoder_output_size=encoder.output_size(),
-            **args.decoder_conf,
-        )
+        decoder = decoder_class(**args.decoder_conf)
 
         # logger aggregator
         if getattr(args, "label_aggregator", None) is not None:
             label_aggregator_class = label_aggregator_choices.get_class(args.label_aggregator)
             label_aggregator = label_aggregator_class(**args.label_aggregator_conf)
         else:
             label_aggregator = None
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_distributed.py` & `funasr-0.6.3/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_lm_model.py` & `funasr-0.6.3/funasr/build_utils/build_lm_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,27 +30,32 @@
     # --model and --model_conf
     model_choices
 ]
 
 
 def build_lm_model(args):
     # token_list
-    if args.token_list is not None:
-        with open(args.token_list) as f:
+    if isinstance(args.token_list, str):
+        with open(args.token_list, encoding="utf-8") as f:
             token_list = [line.rstrip() for line in f]
         args.token_list = list(token_list)
         vocab_size = len(token_list)
         logging.info(f"Vocabulary size: {vocab_size}")
+    elif isinstance(args.token_list, (tuple, list)):
+        token_list = list(args.token_list)
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
     else:
         vocab_size = None
 
     # lm
     lm_class = lm_choices.get_class(args.lm)
     lm = lm_class(vocab_size=vocab_size, **args.lm_conf)
 
+    args.model = args.model if hasattr(args, "model") else "lm"
     model_class = model_choices.get_class(args.model)
     model = model_class(lm=lm, vocab_size=vocab_size, **args.model_conf)
 
     # initialize
     if args.init is not None:
         initialize(model, args.init)
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_model.py` & `funasr-0.6.3/funasr/build_utils/build_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from funasr.build_utils.build_asr_model import build_asr_model
+from funasr.build_utils.build_diar_model import build_diar_model
 from funasr.build_utils.build_lm_model import build_lm_model
 from funasr.build_utils.build_pretrain_model import build_pretrain_model
 from funasr.build_utils.build_punc_model import build_punc_model
+from funasr.build_utils.build_sv_model import build_sv_model
 from funasr.build_utils.build_vad_model import build_vad_model
-from funasr.build_utils.build_diar_model import build_diar_model
 
 
 def build_model(args):
     if args.task_name == "asr":
         model = build_asr_model(args)
     elif args.task_name == "pretrain":
         model = build_pretrain_model(args)
@@ -15,11 +16,13 @@
         model = build_lm_model(args)
     elif args.task_name == "punc":
         model = build_punc_model(args)
     elif args.task_name == "vad":
         model = build_vad_model(args)
     elif args.task_name == "diar":
         model = build_diar_model(args)
+    elif args.task_name == "sv":
+        model = build_sv_model(args)
     else:
         raise NotImplementedError("Not supported task: {}".format(args.task_name))
 
     return model
```

### Comparing `funasr-0.6.2/funasr/build_utils/build_optimizer.py` & `funasr-0.6.3/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_pretrain_model.py` & `funasr-0.6.3/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_punc_model.py` & `funasr-0.6.3/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_scheduler.py` & `funasr-0.6.3/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_trainer.py` & `funasr-0.6.3/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/build_utils/build_vad_model.py` & `funasr-0.6.3/funasr/build_utils/build_vad_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     # --model and --model_conf
     model_choices,
 ]
 
 
 def build_vad_model(args):
     # frontend
+    if not hasattr(args, "cmvn_file"):
+        args.cmvn_file = None
+    if not hasattr(args, "init"):
+        args.init = None
     if args.input_size is None:
         frontend_class = frontend_choices.get_class(args.frontend)
         if args.frontend == 'wav_frontend':
             frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
         else:
             frontend = frontend_class(**args.frontend_conf)
         input_size = frontend.output_size()
```

### Comparing `funasr-0.6.2/funasr/datasets/collate_fn.py` & `funasr-0.6.3/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/dataset.py` & `funasr-0.6.3/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/iterable_dataset.py` & `funasr-0.6.3/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.6.3/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.6.3/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.6.3/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/dataset.py` & `funasr-0.6.3/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.6.3/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/ms_dataset.py` & `funasr-0.6.3/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/datasets/preprocessor.py` & `funasr-0.6.3/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/export_model.py` & `funasr-0.6.3/funasr/export/export_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,42 +225,43 @@
             dummy_input = model.get_dummy_inputs(enc_size)
         else:
             dummy_input = model.get_dummy_inputs()
 
         # model_script = torch.jit.script(model)
         model_script = model #torch.jit.trace(model)
         model_path = os.path.join(path, f'{model.model_name}.onnx')
-
-        torch.onnx.export(
-            model_script,
-            dummy_input,
-            model_path,
-            verbose=verbose,
-            opset_version=14,
-            input_names=model.get_input_names(),
-            output_names=model.get_output_names(),
-            dynamic_axes=model.get_dynamic_axes()
-        )
+        if not os.path.exists(model_path):
+            torch.onnx.export(
+                model_script,
+                dummy_input,
+                model_path,
+                verbose=verbose,
+                opset_version=14,
+                input_names=model.get_input_names(),
+                output_names=model.get_output_names(),
+                dynamic_axes=model.get_dynamic_axes()
+            )
 
         if self.quant:
             from onnxruntime.quantization import QuantType, quantize_dynamic
             import onnx
             quant_model_path = os.path.join(path, f'{model.model_name}_quant.onnx')
-            onnx_model = onnx.load(model_path)
-            nodes = [n.name for n in onnx_model.graph.node]
-            nodes_to_exclude = [m for m in nodes if 'output' in m]
-            quantize_dynamic(
-                model_input=model_path,
-                model_output=quant_model_path,
-                op_types_to_quantize=['MatMul'],
-                per_channel=True,
-                reduce_range=False,
-                weight_type=QuantType.QUInt8,
-                nodes_to_exclude=nodes_to_exclude,
-            )
+            if not os.path.exists(quant_model_path):
+                onnx_model = onnx.load(model_path)
+                nodes = [n.name for n in onnx_model.graph.node]
+                nodes_to_exclude = [m for m in nodes if 'output' in m]
+                quantize_dynamic(
+                    model_input=model_path,
+                    model_output=quant_model_path,
+                    op_types_to_quantize=['MatMul'],
+                    per_channel=True,
+                    reduce_range=False,
+                    weight_type=QuantType.QUInt8,
+                    nodes_to_exclude=nodes_to_exclude,
+                )
 
 
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument('--model-name', type=str, required=True)
     parser.add_argument('--export-dir', type=str, required=True)
```

### Comparing `funasr-0.6.2/funasr/export/models/CT_Transformer.py` & `funasr-0.6.3/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/__init__.py` & `funasr-0.6.3/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.6.3/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.6.3/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.6.3/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/e2e_vad.py` & `funasr-0.6.3/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.6.3/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.6.3/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.6.3/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/modules/decoder_layer.py` & `funasr-0.6.3/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/modules/encoder_layer.py` & `funasr-0.6.3/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/modules/feedforward.py` & `funasr-0.6.3/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/modules/multihead_att.py` & `funasr-0.6.3/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/models/predictor/cif.py` & `funasr-0.6.3/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/test/test_onnx.py` & `funasr-0.6.3/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/test/test_onnx_punc.py` & `funasr-0.6.3/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.6.3/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/test/test_onnx_vad.py` & `funasr-0.6.3/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/export/utils/torch_function.py` & `funasr-0.6.3/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/fileio/datadir_writer.py` & `funasr-0.6.3/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/fileio/npy_scp.py` & `funasr-0.6.3/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/fileio/rand_gen_dataset.py` & `funasr-0.6.3/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/fileio/read_text.py` & `funasr-0.6.3/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/fileio/sound_scp.py` & `funasr-0.6.3/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/iterators/chunk_iter_factory.py` & `funasr-0.6.3/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/iterators/multiple_iter_factory.py` & `funasr-0.6.3/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/iterators/sequence_iter_factory.py` & `funasr-0.6.3/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/complex_utils.py` & `funasr-0.6.3/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/global_mvn.py` & `funasr-0.6.3/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/label_aggregation.py` & `funasr-0.6.3/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/log_mel.py` & `funasr-0.6.3/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/mask_along_axis.py` & `funasr-0.6.3/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/sinc_conv.py` & `funasr-0.6.3/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/stft.py` & `funasr-0.6.3/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/time_warp.py` & `funasr-0.6.3/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/layers/utterance_mvn.py` & `funasr-0.6.3/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/losses/label_smoothing_loss.py` & `funasr-0.6.3/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/main_funcs/average_nbest_models.py` & `funasr-0.6.3/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.6.3/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/main_funcs/collect_stats.py` & `funasr-0.6.3/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/main_funcs/pack_funcs.py` & `funasr-0.6.3/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/ctc.py` & `funasr-0.6.3/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/data2vec.py` & `funasr-0.6.3/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/contextual_decoder.py` & `funasr-0.6.3/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/rnn_decoder.py` & `funasr-0.6.3/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.6.3/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/sanm_decoder.py` & `funasr-0.6.3/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/sv_decoder.py` & `funasr-0.6.3/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/decoder/transformer_decoder.py` & `funasr-0.6.3/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_asr.py` & `funasr-0.6.3/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_asr_common.py` & `funasr-0.6.3/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.6.3/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
         normalize: Optional[AbsNormalize],
-        preencoder: Optional[AbsPreEncoder],
         encoder: AbsEncoder,
-        postencoder: Optional[AbsPostEncoder],
         decoder: AbsDecoder,
         ctc: CTC,
         ctc_weight: float = 0.5,
         interctc_weight: float = 0.0,
         ignore_id: int = -1,
         blank_id: int = 0,
         sos: int = 1,
@@ -68,14 +66,16 @@
         target_buffer_length: int = -1,
         inner_dim: int = 256, 
         bias_encoder_type: str = 'lstm',
         use_decoder_embedding: bool = False,
         crit_attn_weight: float = 0.0,
         crit_attn_smooth: float = 0.0,
         bias_encoder_dropout_rate: float = 0.0,
+        preencoder: Optional[AbsPreEncoder] = None,
+        postencoder: Optional[AbsPostEncoder] = None,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__(
         vocab_size=vocab_size,
```

### Comparing `funasr-0.6.2/funasr/models/e2e_asr_mfcca.py` & `funasr-0.6.3/funasr/models/e2e_asr_mfcca.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
             encoder: AbsEncoder,
             decoder: AbsDecoder,
             ctc: CTC,
-            rnnt_decoder: None,
+            rnnt_decoder: None = None,
             ctc_weight: float = 0.5,
             ignore_id: int = -1,
             lsm_weight: float = 0.0,
             mask_ratio: float = 0.0,
             length_normalized_loss: bool = False,
             report_cer: bool = True,
             report_wer: bool = True,
```

### Comparing `funasr-0.6.2/funasr/models/e2e_asr_paraformer.py` & `funasr-0.6.3/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_asr_transducer.py` & `funasr-0.6.3/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.6.3/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_diar_sond.py` & `funasr-0.6.3/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_sa_asr.py` & `funasr-0.6.3/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_sv.py` & `funasr-0.6.3/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_tp.py` & `funasr-0.6.3/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/e2e_uni_asr.py` & `funasr-0.6.3/funasr/models/e2e_uni_asr.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,15 @@
     def __init__(
         self,
         vocab_size: int,
         token_list: Union[Tuple[str, ...], List[str]],
         frontend: Optional[AbsFrontend],
         specaug: Optional[AbsSpecAug],
         normalize: Optional[AbsNormalize],
-        preencoder: Optional[AbsPreEncoder],
         encoder: AbsEncoder,
-        postencoder: Optional[AbsPostEncoder],
         decoder: AbsDecoder,
         ctc: CTC,
         ctc_weight: float = 0.5,
         interctc_weight: float = 0.0,
         ignore_id: int = -1,
         lsm_weight: float = 0.0,
         length_normalized_loss: bool = False,
@@ -76,14 +74,16 @@
         predictor2=None,
         predictor_weight2: float = 0.0,
         decoder_attention_chunk_type2: str = 'chunk',
         stride_conv=None,
         loss_weight_model1: float = 0.5,
         enable_maas_finetune: bool = False,
         freeze_encoder2: bool = False,
+        preencoder: Optional[AbsPreEncoder] = None,
+        postencoder: Optional[AbsPostEncoder] = None,
         encoder1_encoder2_joint_training: bool = True,
     ):
         assert check_argument_types()
         assert 0.0 <= ctc_weight <= 1.0, ctc_weight
         assert 0.0 <= interctc_weight < 1.0, interctc_weight
 
         super().__init__()
```

### Comparing `funasr-0.6.2/funasr/models/e2e_vad.py` & `funasr-0.6.3/funasr/models/e2e_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import List, Tuple, Dict, Any
 
 import torch
 from torch import nn
 import math
 from funasr.models.encoder.fsmn_encoder import FSMN
+from funasr.models.base_model import FunASRModel
 
 
 class VadStateMachine(Enum):
     kVadInStateStartPointNotDetected = 1
     kVadInStateInSpeechSegment = 2
     kVadInStateEndPointDetected = 3
 
@@ -207,15 +208,15 @@
             return AudioChangeState.kChangeStateSpeech2Speech
         return AudioChangeState.kChangeStateInvalid
 
     def FrameSizeMs(self) -> int:
         return int(self.frame_size_ms)
 
 
-class E2EVadModel(nn.Module):
+class E2EVadModel(FunASRModel):
     """
     Author: Speech Lab of DAMO Academy, Alibaba Group
     Deep-FSMN for Large Vocabulary Continuous Speech Recognition
     https://arxiv.org/abs/1803.05030
     """
     def __init__(self, encoder: FSMN, vad_post_args: Dict[str, Any], frontend=None):
         super(E2EVadModel, self).__init__()
```

### Comparing `funasr-0.6.2/funasr/models/encoder/conformer_encoder.py` & `funasr-0.6.3/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.6.3/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.6.3/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.6.3/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.6.3/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.6.3/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.6.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.6.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.6.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.6.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.6.3/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/rnn_encoder.py` & `funasr-0.6.3/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/sanm_encoder.py` & `funasr-0.6.3/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/encoder/transformer_encoder.py` & `funasr-0.6.3/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/default.py` & `funasr-0.6.3/funasr/models/frontend/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             n_fft=n_fft,
             n_mels=n_mels,
             fmin=fmin,
             fmax=fmax,
             htk=htk,
         )
         self.n_mels = n_mels
-        self.frontend_type = "default"
         self.use_channel = use_channel
+        self.frontend_type = "default"
 
     def output_size(self) -> int:
         return self.n_mels
 
     def forward(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
@@ -142,41 +142,54 @@
     """Conventional frontend structure for ASR.
     Stft -> WPE -> MVDR-Beamformer -> Power-spec -> Mel-Fbank -> CMVN
     """
 
     def __init__(
             self,
             fs: Union[int, str] = 16000,
-            n_fft: int = 400,
-            frame_length: int = 25,
-            frame_shift: int = 10,
+            n_fft: int = 512,
+            win_length: int = None,
+            hop_length: int = None,
+            frame_length: int = None,
+            frame_shift: int = None,
             window: Optional[str] = "hann",
             center: bool = True,
             normalized: bool = False,
             onesided: bool = True,
             n_mels: int = 80,
             fmin: int = None,
             fmax: int = None,
             htk: bool = False,
             frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
             apply_stft: bool = True,
             use_channel: int = None,
             lfr_m: int = 1,
             lfr_n: int = 1,
-            cmvn_file: str = None
+            cmvn_file: str = None,
+            mc: bool = True
     ):
         assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         # Deepcopy (In general, dict shouldn't be used as default arg)
         frontend_conf = copy.deepcopy(frontend_conf)
-        self.win_length = frame_length * 16
-        self.hop_length = frame_shift * 16
+        if win_length is None and hop_length is None:
+            self.win_length = frame_length * 16
+            self.hop_length = frame_shift * 16
+        elif frame_length is None and frame_shift is None:
+            self.win_length = self.win_length
+            self.hop_length = self.hop_length
+        else:
+            logging.error(
+                "Only one of (win_length, hop_length) and (frame_length, frame_shift)"
+                "can be set."
+            )
+            exit(1)
 
         if apply_stft:
             self.stft = Stft(
                 n_fft=n_fft,
                 win_length=self.win_length,
                 hop_length=self.hop_length,
                 center=center,
@@ -198,25 +211,27 @@
             n_fft=n_fft,
             n_mels=n_mels,
             fmin=fmin,
             fmax=fmax,
             htk=htk,
         )
         self.n_mels = n_mels
-        self.frontend_type = "default"
         self.use_channel = use_channel
-        if self.use_channel is not None:
-            logging.info("use the channel %d" % (self.use_channel))
-        else:
-            logging.info("random select channel")
-        self.cmvn_file = cmvn_file
-        if self.cmvn_file is not None:
-            mean, std = self._load_cmvn(self.cmvn_file)
-            self.register_buffer("mean", torch.from_numpy(mean))
-            self.register_buffer("std", torch.from_numpy(std))
+        self.mc = mc
+        if not self.mc:
+            if self.use_channel is not None:
+                logging.info("use the channel %d" % (self.use_channel))
+            else:
+                logging.info("random select channel")
+            self.cmvn_file = cmvn_file
+            if self.cmvn_file is not None:
+                mean, std = self._load_cmvn(self.cmvn_file)
+                self.register_buffer("mean", torch.from_numpy(mean))
+                self.register_buffer("std", torch.from_numpy(std))
+        self.frontend_type = "multichannelfrontend"
 
     def output_size(self) -> int:
         return self.n_mels
 
     def forward(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
@@ -229,16 +244,16 @@
             feats_lens = input_lengths
         # 2. [Option] Speech enhancement
         if self.frontend is not None:
             assert isinstance(input_stft, ComplexTensor), type(input_stft)
             # input_stft: (Batch, Length, [Channel], Freq)
             input_stft, _, mask = self.frontend(input_stft, feats_lens)
 
-        # 3. [Multi channel case]: Select a channel
-        if input_stft.dim() == 4:
+        # 3. [Multi channel case]: Select a channel(sa_asr)
+        if input_stft.dim() == 4 and not self.mc:
             # h: (B, T, C, F) -> h: (B, T, F)
             if self.training:
                 if self.use_channel is not None:
                     input_stft = input_stft[:, :, self.use_channel, :]
                     
                 else:
                     # Select 1ch randomly
@@ -252,35 +267,45 @@
         # h: ComplexTensor(B, T, F) -> torch.Tensor(B, T, F)
         input_power = input_stft.real ** 2 + input_stft.imag ** 2
 
         # 5. Feature transform e.g. Stft -> Log-Mel-Fbank
         # input_power: (Batch, [Channel,] Length, Freq)
         #       -> input_feats: (Batch, Length, Dim)
         input_feats, _ = self.logmel(input_power, feats_lens)
-        
-        # 6. Apply CMVN
-        if self.cmvn_file is not None:
-            if feats_lens is None:
-                feats_lens = input_feats.new_full([input_feats.size(0)], input_feats.size(1))
-            self.mean = self.mean.to(input_feats.device, input_feats.dtype)
-            self.std = self.std.to(input_feats.device, input_feats.dtype)
-            mask = make_pad_mask(feats_lens, input_feats, 1)
-
-            if input_feats.requires_grad:
-                input_feats = input_feats + self.mean
+        if self.mc:
+            # MFCCA
+            if input_feats.dim() ==4:
+                bt = input_feats.size(0)
+                channel_size = input_feats.size(2)
+                input_feats = input_feats.transpose(1,2).reshape(bt*channel_size,-1,80).contiguous()
+                feats_lens = feats_lens.repeat(1,channel_size).squeeze()
             else:
-                input_feats += self.mean
-            if input_feats.requires_grad:
-                input_feats = input_feats.masked_fill(mask, 0.0)
-            else:
-                input_feats.masked_fill_(mask, 0.0)
+                channel_size = 1
+            return input_feats, feats_lens, channel_size
+        else:
+            # 6. Apply CMVN
+            if self.cmvn_file is not None:
+                if feats_lens is None:
+                    feats_lens = input_feats.new_full([input_feats.size(0)], input_feats.size(1))
+                self.mean = self.mean.to(input_feats.device, input_feats.dtype)
+                self.std = self.std.to(input_feats.device, input_feats.dtype)
+                mask = make_pad_mask(feats_lens, input_feats, 1)
 
-            input_feats *= self.std
+                if input_feats.requires_grad:
+                    input_feats = input_feats + self.mean
+                else:
+                    input_feats += self.mean
+                if input_feats.requires_grad:
+                    input_feats = input_feats.masked_fill(mask, 0.0)
+                else:
+                    input_feats.masked_fill_(mask, 0.0)
 
-        return input_feats, feats_lens
+                input_feats *= self.std
+
+            return input_feats, feats_lens
 
     def _compute_stft(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> torch.Tensor:
         input_stft, feats_lens = self.stft(input, input_lengths)
 
         assert input_stft.dim() >= 4, input_stft.shape
@@ -309,8 +334,8 @@
                 line_item = lines[i + 1].split()
                 if line_item[0] == '<LearnRateCoef>':
                     rescale_line = line_item[3:(len(line_item) - 1)]
                     vars_list = list(rescale_line)
                     continue
         means = np.array(means_list).astype(np.float)
         vars = np.array(vars_list).astype(np.float)
-        return means, vars
+        return means, vars
```

### Comparing `funasr-0.6.2/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.6.3/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/fused.py` & `funasr-0.6.3/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/s3prl.py` & `funasr-0.6.3/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/wav_frontend.py` & `funasr-0.6.3/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.6.3/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/frontend/windowing.py` & `funasr-0.6.3/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/joint_net/joint_network.py` & `funasr-0.6.3/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/pooling/statistic_pooling.py` & `funasr-0.6.3/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.6.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/predictor/cif.py` & `funasr-0.6.3/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/preencoder/linear.py` & `funasr-0.6.3/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/preencoder/sinc.py` & `funasr-0.6.3/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/seq_rnn_lm.py` & `funasr-0.6.3/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/specaug/specaug.py` & `funasr-0.6.3/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/target_delay_transformer.py` & `funasr-0.6.3/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/transformer_lm.py` & `funasr-0.6.3/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/models/vad_realtime_transformer.py` & `funasr-0.6.3/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/add_sos_eos.py` & `funasr-0.6.3/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/attention.py` & `funasr-0.6.3/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.6.3/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.6.3/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/beam_search/beam_search.py` & `funasr-0.6.3/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.6.3/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.6.3/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/data_utils.py` & `funasr-0.6.3/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/ema_module.py` & `funasr-0.6.3/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.6.3/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/quant_noise.py` & `funasr-0.6.3/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/utils.py` & `funasr-0.6.3/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.6.3/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/dynamic_conv.py` & `funasr-0.6.3/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/dynamic_conv2d.py` & `funasr-0.6.3/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/e2e_asr_common.py` & `funasr-0.6.3/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/eend_ola/encoder.py` & `funasr-0.6.3/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.6.3/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/embedding.py` & `funasr-0.6.3/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/beamformer.py` & `funasr-0.6.3/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.6.3/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.6.3/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/feature_transform.py` & `funasr-0.6.3/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/frontend.py` & `funasr-0.6.3/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/frontends/mask_estimator.py` & `funasr-0.6.3/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/layer_norm.py` & `funasr-0.6.3/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/lightconv.py` & `funasr-0.6.3/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/lightconv2d.py` & `funasr-0.6.3/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/mask.py` & `funasr-0.6.3/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/multi_layer_conv.py` & `funasr-0.6.3/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/nets_utils.py` & `funasr-0.6.3/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/positionwise_feed_forward.py` & `funasr-0.6.3/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/repeat.py` & `funasr-0.6.3/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/rnn/argument.py` & `funasr-0.6.3/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/rnn/attentions.py` & `funasr-0.6.3/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/rnn/decoders.py` & `funasr-0.6.3/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/rnn/encoders.py` & `funasr-0.6.3/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/scorers/ctc.py` & `funasr-0.6.3/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.6.3/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/scorers/length_bonus.py` & `funasr-0.6.3/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/scorers/scorer_interface.py` & `funasr-0.6.3/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.6.3/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.6.3/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/streaming_utils/utils.py` & `funasr-0.6.3/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/subsampling.py` & `funasr-0.6.3/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/modules/subsampling_without_posenc.py` & `funasr-0.6.3/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/optimizers/fairseq_adam.py` & `funasr-0.6.3/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/optimizers/sgd.py` & `funasr-0.6.3/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/demo.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/libtorch/setup.py` & `funasr-0.6.3/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.6.3/funasr/runtime/python/onnxruntime/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.1.0'
+VERSION_NUM = '0.1.1'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
@@ -27,15 +27,15 @@
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa",
                       "onnxruntime>=1.7.0",
                       "scipy",
                       "numpy>=1.19.3",
-                      "typeguard",
+                      "typeguard==2.13.3",
                       "kaldi-native-fbank",
                       "PyYAML>=5.1.2",
                       "funasr",
                       "modelscope",
                       "onnx"
                       ],
     packages=[MODULE_NAME, f'{MODULE_NAME}.utils'],
```

### Comparing `funasr-0.6.2/funasr/samplers/build_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/samplers/folded_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/samplers/length_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.6.3/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/schedulers/abs_scheduler.py` & `funasr-0.6.3/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/schedulers/noam_lr.py` & `funasr-0.6.3/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.6.3/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/schedulers/warmup_lr.py` & `funasr-0.6.3/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/abs_task.py` & `funasr-0.6.3/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/asr.py` & `funasr-0.6.3/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/data2vec.py` & `funasr-0.6.3/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/diar.py` & `funasr-0.6.3/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/lm.py` & `funasr-0.6.3/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/punctuation.py` & `funasr-0.6.3/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/sa_asr.py` & `funasr-0.6.3/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/sv.py` & `funasr-0.6.3/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/tasks/vad.py` & `funasr-0.6.3/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/build_tokenizer.py` & `funasr-0.6.3/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/char_tokenizer.py` & `funasr-0.6.3/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/cleaner.py` & `funasr-0.6.3/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/korean_cleaner.py` & `funasr-0.6.3/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/phoneme_tokenizer.py` & `funasr-0.6.3/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.6.3/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/token_id_converter.py` & `funasr-0.6.3/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/text/word_tokenizer.py` & `funasr-0.6.3/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.6.3/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/device_funcs.py` & `funasr-0.6.3/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/forward_adaptor.py` & `funasr-0.6.3/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/initialize.py` & `funasr-0.6.3/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.6.3/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/model_summary.py` & `funasr-0.6.3/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/torch_utils/recursive_op.py` & `funasr-0.6.3/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/train/abs_model.py` & `funasr-0.6.3/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/train/class_choices.py` & `funasr-0.6.3/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/train/distributed_utils.py` & `funasr-0.6.3/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/train/reporter.py` & `funasr-0.6.3/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/train/trainer.py` & `funasr-0.6.3/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/asr_env_checking.py` & `funasr-0.6.3/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/asr_utils.py` & `funasr-0.6.3/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/build_dataclass.py` & `funasr-0.6.3/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/cli_utils.py` & `funasr-0.6.3/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/compute_eer.py` & `funasr-0.6.3/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/compute_min_dcf.py` & `funasr-0.6.3/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/compute_wer.py` & `funasr-0.6.3/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/config_argparse.py` & `funasr-0.6.3/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/get_default_kwargs.py` & `funasr-0.6.3/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/griffin_lim.py` & `funasr-0.6.3/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/job_runner.py` & `funasr-0.6.3/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/misc.py` & `funasr-0.6.3/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/modelscope_param.py` & `funasr-0.6.3/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/modelscope_utils.py` & `funasr-0.6.3/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/nested_dict_action.py` & `funasr-0.6.3/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/postprocess_utils.py` & `funasr-0.6.3/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/prepare_data.py` & `funasr-0.6.3/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/sized_dict.py` & `funasr-0.6.3/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/timestamp_tools.py` & `funasr-0.6.3/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/types.py` & `funasr-0.6.3/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/vad_utils.py` & `funasr-0.6.3/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr/utils/wav_utils.py` & `funasr-0.6.3/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/funasr.egg-info/PKG-INFO` & `funasr-0.6.3/funasr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.2
+Version: 0.6.3
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -110,14 +110,19 @@
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
+
+## Stargazers over time
+
+[![Stargazers over time](https://starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-damo-academy/FunASR)
+
 ## Citations
 
 ``` bibtex
 @inproceedings{gao2023funasr,
   author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and Shiliang Zhang},
   title={FunASR: A Fundamental End-to-End Speech Recognition Toolkit},
   year={2023},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.2 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.3 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -92,17 +92,19 @@
 (https://github.com/RapidAI) for contributing the Paraformer and
 CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
 www.aihealthx.com/) for contributing the websocket service and html5. ##
 License This project is licensed under the [The MIT License](https://
 opensource.org/licenses/MIT). FunASR also contains various third-party
 components and some code modified from other repos under other open source
 licenses. The use of pretraining model is subject to [model licencs](./
-MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
-{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
-Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
-Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+MODEL_LICENSE) ## Stargazers over time [![Stargazers over time](https://
+starchart.cc/alibaba-damo-academy/FunASR.svg)](https://starchart.cc/alibaba-
+damo-academy/FunASR) ## Citations ``` bibtex @inproceedings{gao2023funasr,
+author={Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi
+and Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao
+and Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
 Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
 {gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
 and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
 Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
 Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
 ```
```

### Comparing `funasr-0.6.2/funasr.egg-info/SOURCES.txt` & `funasr-0.6.3/funasr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,21 @@
 funasr/build_utils/build_args.py
 funasr/build_utils/build_asr_model.py
 funasr/build_utils/build_dataloader.py
 funasr/build_utils/build_diar_model.py
 funasr/build_utils/build_distributed.py
 funasr/build_utils/build_lm_model.py
 funasr/build_utils/build_model.py
+funasr/build_utils/build_model_from_file.py
 funasr/build_utils/build_optimizer.py
 funasr/build_utils/build_pretrain_model.py
 funasr/build_utils/build_punc_model.py
 funasr/build_utils/build_scheduler.py
+funasr/build_utils/build_streaming_iterator.py
+funasr/build_utils/build_sv_model.py
 funasr/build_utils/build_trainer.py
 funasr/build_utils/build_vad_model.py
 funasr/datasets/__init__.py
 funasr/datasets/collate_fn.py
 funasr/datasets/dataset.py
 funasr/datasets/iterable_dataset.py
 funasr/datasets/ms_dataset.py
```

### Comparing `funasr-0.6.2/funasr.egg-info/requires.txt` & `funasr-0.6.3/funasr.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 kaldiio>=2.17.0
 torch_complex
 nltk>=3.4.5
 sentencepiece
 pypinyin<=0.44.0
 espnet_tts_frontend
 pytorch_wpe
-editdistance==0.5.2
+editdistance>=0.5.2
 tensorboard==1.15
 g2p
 oss2
 edit-distance
 textgrid
 protobuf==3.20.0
```

### Comparing `funasr-0.6.2/setup.py` & `funasr-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         # TTS
         # "pyworld>=0.2.10",
         "pypinyin<=0.44.0",
         "espnet_tts_frontend",
         # ENH
         # "ci_sdr",
         "pytorch_wpe",
-        "editdistance==0.5.2",
+        "editdistance>=0.5.2",
         "tensorboard==1.15",
         "g2p",
         # PAI
         "oss2",
         # "kaldi-native-fbank",
         # timestamp
         "edit-distance",
```

### Comparing `funasr-0.6.2/tests/test_asr_inference_pipeline.py` & `funasr-0.6.3/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.6.3/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/tests/test_lm_pipeline.py` & `funasr-0.6.3/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/tests/test_punctuation_pipeline.py` & `funasr-0.6.3/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.2/tests/test_sv_inference_pipeline.py` & `funasr-0.6.3/tests/test_sv_inference_pipeline.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         rec_result = inference_sv_pipline(audio_in=(
             'https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/sv_example_enroll.wav',
             'https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/sv_example_different.wav'))
         assert abs(rec_result["scores"][0]-0.0) < 0.1 and abs(rec_result["scores"][1]-1.0) < 0.1
         logger.info(f"Similarity {rec_result['scores']}")
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `funasr-0.6.2/tests/test_vad_inference_pipeline.py` & `funasr-0.6.3/tests/test_vad_inference_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         inference_pipeline = pipeline(
             task=Tasks.voice_activity_detection,
             model="damo/speech_fsmn_vad_zh-cn-16k-common-pytorch",
         )
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/vad_example.wav')
         logger.info("vad inference result: {0}".format(rec_result))
-        assert rec_result["text"] == [[80, 2340], [2620, 6200], [6480, 23670], [23950, 26250], [26780, 28990],
+        assert rec_result["text"] == [[70, 2340], [2620, 6200], [6480, 23670], [23950, 26250], [26780, 28990],
                                       [29950, 31430], [31750, 37600], [38210, 46900], [47310, 49630], [49910, 56460],
                                       [56740, 59540], [59820, 70450]]
 
 
 if __name__ == '__main__':
     unittest.main()
```

