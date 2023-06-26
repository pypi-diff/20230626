# Comparing `tmp/xformers-0.0.8.tar.gz` & `tmp/xformers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xformers-0.0.8.tar", last modified: Fri Jan  7 21:00:22 2022, max compression
+gzip compressed data, was "xformers-0.0.9.tar", last modified: Wed Feb  9 20:53:29 2022, max compression
```

## Comparing `xformers-0.0.8.tar` & `xformers-0.0.9.tar`

### file list

```diff
@@ -1,116 +1,131 @@
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:22.059042 xformers-0.0.8/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1588 2021-10-20 21:28:13.000000 xformers-0.0.8/LICENSE
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       41 2021-10-20 21:28:13.000000 xformers-0.0.8/MANIFEST.in
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      886 2022-01-07 21:00:22.060691 xformers-0.0.8/PKG-INFO
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11101 2022-01-06 22:50:20.000000 xformers-0.0.8/README.md
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      187 2021-11-11 19:38:19.000000 xformers-0.0.8/requirements.txt
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       97 2022-01-07 21:00:22.066031 xformers-0.0.8/setup.cfg
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5173 2022-01-07 20:19:08.000000 xformers-0.0.8/setup.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.625853 xformers-0.0.8/xformers/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2435 2022-01-07 19:11:31.000000 xformers-0.0.8/xformers/__init__.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.720011 xformers-0.0.8/xformers/benchmarks/
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.748090 xformers-0.0.8/xformers/benchmarks/LRA/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/benchmarks/LRA/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4238 2021-10-26 21:52:43.000000 xformers-0.0.8/xformers/benchmarks/LRA/batch_fetch_results.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1986 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/LRA/batch_submit.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.762457 xformers-0.0.8/xformers/benchmarks/LRA/code/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/benchmarks/LRA/code/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1403 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/LRA/code/dataset.py
--rwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)     7133 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/benchmarks/LRA/code/model_wrapper.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5350 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/benchmarks/LRA/run_grid_search.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    17918 2021-11-03 16:11:34.000000 xformers-0.0.8/xformers/benchmarks/LRA/run_tasks.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4636 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/benchmarks/LRA/run_with_submitit.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/benchmarks/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8527 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/benchmarks/benchmark_core.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11166 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/benchmarks/benchmark_encoder.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3176 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/benchmark_nystrom_utils.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7630 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/benchmarks/benchmark_pytorch_transformer.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2673 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/benchmarks/benchmark_revnet.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3658 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/benchmarks/benchmark_sddmm.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4941 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_blocksparse.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3477 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_dropout.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5492 2021-11-11 19:38:19.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_fused_linear.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2659 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_layernorm.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2180 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_softmax.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1823 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/benchmarks/benchmark_triton_stride_sum.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11843 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/benchmarks/benchmark_vit_timm.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3691 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/benchmarks/utils.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.793127 xformers-0.0.8/xformers/components/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2660 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/components/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1162 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/activations.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.890529 xformers-0.0.8/xformers/components/attention/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3943 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/attention/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3167 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/components/attention/_sputnik_sparse.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4575 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/attention/attention_mask.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8718 2021-10-21 22:08:14.000000 xformers-0.0.8/xformers/components/attention/attention_patterns.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2682 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/base.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7822 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/blocksparse.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7283 2021-11-30 19:17:15.000000 xformers-0.0.8/xformers/components/attention/core.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5955 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/attention/favor.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.903832 xformers-0.0.8/xformers/components/attention/feature_maps/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      592 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/attention/feature_maps/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1672 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/attention/feature_maps/base.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    10633 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/attention/feature_maps/softmax.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      926 2021-11-30 19:17:15.000000 xformers-0.0.8/xformers/components/attention/fourier_mix.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3841 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/global_tokens.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2663 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/lambda_layer.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2312 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/linformer.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3420 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/local.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    10793 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/attention/nystrom.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11872 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/components/attention/ortho.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3936 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/attention/random.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4320 2021-11-30 19:17:15.000000 xformers-0.0.8/xformers/components/attention/scaled_dot_product.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3803 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/attention/utils.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.924562 xformers-0.0.8/xformers/components/feedforward/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2556 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/components/feedforward/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1300 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/feedforward/base.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2257 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/feedforward/fused_mlp.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1196 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/feedforward/mlp.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7053 2021-10-26 21:52:44.000000 xformers-0.0.8/xformers/components/in_proj_container.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7738 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/multi_head_dispatch.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.946605 xformers-0.0.8/xformers/components/positional_embedding/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2755 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/components/positional_embedding/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      972 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/components/positional_embedding/base.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3155 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/components/positional_embedding/rotary.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1871 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/components/positional_embedding/sine.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1679 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/components/positional_embedding/vocab.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2654 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/components/residual.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4487 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/components/reversible.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.965253 xformers-0.0.8/xformers/factory/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      566 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/factory/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    13309 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/factory/block_factory.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1304 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/factory/hydra_helper.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     9520 2022-01-07 19:11:31.000000 xformers-0.0.8/xformers/factory/model_factory.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.973949 xformers-0.0.8/xformers/helpers/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      263 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/helpers/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1528 2021-10-20 21:28:14.000000 xformers-0.0.8/xformers/helpers/timm_sparse_attention.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      768 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/ops.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.992023 xformers-0.0.8/xformers/sparse/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      254 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/sparse/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4846 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/sparse/_csr_ops.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    14255 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/sparse/csr_tensor.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4604 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/sparse/utils.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.8/xformers/test.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:22.054856 xformers-0.0.8/xformers/triton/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      803 2021-11-24 16:12:15.000000 xformers-0.0.8/xformers/triton/__init__.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7431 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/dropout.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4065 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/triton/fused_linear_layer.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3254 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/k_activations.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7519 2022-01-07 17:32:01.000000 xformers-0.0.8/xformers/triton/k_dropout.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4787 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/k_fused_matmul_bw.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7139 2021-11-11 19:38:19.000000 xformers-0.0.8/xformers/triton/k_fused_matmul_fw.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11443 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/triton/k_layer_norm.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5326 2021-11-03 16:36:53.000000 xformers-0.0.8/xformers/triton/k_softmax.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1570 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/k_sum.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2715 2021-11-12 19:41:24.000000 xformers-0.0.8/xformers/triton/layer_norm.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     6568 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/softmax.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1457 2022-01-06 22:50:20.000000 xformers-0.0.8/xformers/triton/sum_strided.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1456 2021-12-02 16:31:26.000000 xformers-0.0.8/xformers/triton/utils.py
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3265 2021-10-25 21:28:22.000000 xformers-0.0.8/xformers/utils.py
-drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-01-07 21:00:21.649348 xformers-0.0.8/xformers.egg-info/
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      886 2022-01-07 21:00:21.000000 xformers-0.0.8/xformers.egg-info/PKG-INFO
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4601 2022-01-07 21:00:21.000000 xformers-0.0.8/xformers.egg-info/SOURCES.txt
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)        1 2022-01-07 21:00:21.000000 xformers-0.0.8/xformers.egg-info/dependency_links.txt
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)        1 2022-01-06 22:34:50.000000 xformers-0.0.8/xformers.egg-info/not-zip-safe
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       43 2022-01-07 21:00:21.000000 xformers-0.0.8/xformers.egg-info/requires.txt
--rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)        9 2022-01-07 21:00:21.000000 xformers-0.0.8/xformers.egg-info/top_level.txt
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.652305 xformers-0.0.9/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1588 2021-10-20 21:28:13.000000 xformers-0.0.9/LICENSE
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       41 2021-10-20 21:28:13.000000 xformers-0.0.9/MANIFEST.in
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      886 2022-02-09 20:53:29.653429 xformers-0.0.9/PKG-INFO
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11772 2022-01-27 19:44:26.000000 xformers-0.0.9/README.md
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.268582 xformers-0.0.9/experimental/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/__init__.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.298216 xformers-0.0.9/experimental/ragged_inference/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/ragged_inference/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     6277 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/ragged_inference/garbage_pad_ragged_acts.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4700 2022-02-09 19:49:58.000000 xformers-0.0.9/experimental/ragged_inference/seq_kv_cache.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3890 2022-02-09 19:49:58.000000 xformers-0.0.9/experimental/ragged_inference/test_utils.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5556 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/ragged_inference/triton_v2_matmul.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     6450 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/ragged_inference/triton_v2_qk_dotprod.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    12918 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/ragged_inference/triton_v2_ragged_qk_dotprod.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      429 2022-01-27 19:44:26.000000 xformers-0.0.9/experimental/setup.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      187 2021-11-11 19:38:19.000000 xformers-0.0.9/requirements.txt
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       97 2022-02-09 20:53:29.655931 xformers-0.0.9/setup.cfg
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5173 2022-02-09 20:47:35.000000 xformers-0.0.9/setup.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.311054 xformers-0.0.9/xformers/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2435 2022-02-09 20:35:30.000000 xformers-0.0.9/xformers/__init__.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.385436 xformers-0.0.9/xformers/benchmarks/
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.405455 xformers-0.0.9/xformers/benchmarks/LRA/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/benchmarks/LRA/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4238 2021-10-26 21:52:43.000000 xformers-0.0.9/xformers/benchmarks/LRA/batch_fetch_results.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1986 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/benchmarks/LRA/batch_submit.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.415532 xformers-0.0.9/xformers/benchmarks/LRA/code/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/benchmarks/LRA/code/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1403 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/benchmarks/LRA/code/dataset.py
+-rwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)     7133 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/benchmarks/LRA/code/model_wrapper.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5350 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/benchmarks/LRA/run_grid_search.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    17918 2021-11-03 16:11:34.000000 xformers-0.0.9/xformers/benchmarks/LRA/run_tasks.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4636 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/benchmarks/LRA/run_with_submitit.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/benchmarks/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8527 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/benchmarks/benchmark_core.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11166 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/benchmarks/benchmark_encoder.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3176 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/benchmarks/benchmark_nystrom_utils.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7630 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/benchmarks/benchmark_pytorch_transformer.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2673 2021-11-03 16:36:53.000000 xformers-0.0.9/xformers/benchmarks/benchmark_revnet.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3658 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/benchmarks/benchmark_sddmm.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5099 2022-02-09 19:49:58.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_blocksparse.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3477 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_dropout.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5492 2021-11-11 19:38:19.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_fused_linear.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2659 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_layernorm.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2180 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_softmax.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1823 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/benchmarks/benchmark_triton_stride_sum.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11843 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/benchmarks/benchmark_vit_timm.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3724 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/benchmarks/utils.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.436208 xformers-0.0.9/xformers/components/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2858 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1162 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/activations.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.507658 xformers-0.0.9/xformers/components/attention/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3943 2021-11-24 16:12:15.000000 xformers-0.0.9/xformers/components/attention/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3164 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/components/attention/_sputnik_sparse.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4630 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/attention/attention_mask.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8718 2021-10-21 22:08:14.000000 xformers-0.0.9/xformers/components/attention/attention_patterns.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2909 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/attention/base.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8157 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/components/attention/blocksparse.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    12775 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/attention/compositional.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7283 2021-11-30 19:17:15.000000 xformers-0.0.9/xformers/components/attention/core.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     6001 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/attention/favor.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.518590 xformers-0.0.9/xformers/components/attention/feature_maps/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      592 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/attention/feature_maps/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1672 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/attention/feature_maps/base.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    10633 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/attention/feature_maps/softmax.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      926 2021-11-30 19:17:15.000000 xformers-0.0.9/xformers/components/attention/fourier_mix.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3841 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/attention/global_tokens.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2663 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/attention/lambda_layer.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2312 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/attention/linformer.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3420 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/attention/local.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    10793 2021-11-24 16:12:15.000000 xformers-0.0.9/xformers/components/attention/nystrom.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11872 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/components/attention/ortho.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3936 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/attention/random.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4320 2021-11-30 19:17:15.000000 xformers-0.0.9/xformers/components/attention/scaled_dot_product.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3803 2021-11-24 16:12:15.000000 xformers-0.0.9/xformers/components/attention/utils.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.534878 xformers-0.0.9/xformers/components/feedforward/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2556 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/components/feedforward/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1300 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/feedforward/base.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2158 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/feedforward/fused_mlp.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5305 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/components/feedforward/mixture_of_experts.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1196 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/feedforward/mlp.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7421 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/components/in_proj_container.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     8229 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/multi_head_dispatch.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.552326 xformers-0.0.9/xformers/components/positional_embedding/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2755 2021-11-03 16:36:53.000000 xformers-0.0.9/xformers/components/positional_embedding/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      972 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/components/positional_embedding/base.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3155 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/components/positional_embedding/rotary.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1365 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/positional_embedding/sine.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1679 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/components/positional_embedding/vocab.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2654 2021-11-24 16:12:15.000000 xformers-0.0.9/xformers/components/residual.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4676 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/components/reversible.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.569617 xformers-0.0.9/xformers/factory/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      566 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/factory/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    13309 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/factory/block_factory.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1304 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/factory/hydra_helper.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     9520 2022-01-07 19:11:31.000000 xformers-0.0.9/xformers/factory/model_factory.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.582159 xformers-0.0.9/xformers/helpers/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      263 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/helpers/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      659 2022-01-27 19:44:26.000000 xformers-0.0.9/xformers/helpers/test_utils.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1528 2021-10-20 21:28:14.000000 xformers-0.0.9/xformers/helpers/timm_sparse_attention.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      768 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/ops.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.601135 xformers-0.0.9/xformers/sparse/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      317 2022-02-09 19:49:58.000000 xformers-0.0.9/xformers/sparse/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4846 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/sparse/_csr_ops.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11228 2022-02-09 19:49:58.000000 xformers-0.0.9/xformers/sparse/blocksparse_tensor.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    14236 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/sparse/csr_tensor.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4274 2022-02-08 17:19:26.000000 xformers-0.0.9/xformers/sparse/utils.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      198 2021-12-08 18:30:59.000000 xformers-0.0.9/xformers/test.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.649353 xformers-0.0.9/xformers/triton/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      803 2021-11-24 16:12:15.000000 xformers-0.0.9/xformers/triton/__init__.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7431 2022-01-27 20:51:30.000000 xformers-0.0.9/xformers/triton/dropout.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4065 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/triton/fused_linear_layer.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3254 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/triton/k_activations.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7519 2022-01-07 17:32:01.000000 xformers-0.0.9/xformers/triton/k_dropout.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     4787 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/triton/k_fused_matmul_bw.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     7139 2021-11-11 19:38:19.000000 xformers-0.0.9/xformers/triton/k_fused_matmul_fw.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)    11443 2021-11-03 16:36:53.000000 xformers-0.0.9/xformers/triton/k_layer_norm.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5326 2021-11-03 16:36:53.000000 xformers-0.0.9/xformers/triton/k_softmax.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1570 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/triton/k_sum.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     2715 2021-11-12 19:41:24.000000 xformers-0.0.9/xformers/triton/layer_norm.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     6372 2022-02-09 19:49:58.000000 xformers-0.0.9/xformers/triton/softmax.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1457 2022-01-06 22:50:20.000000 xformers-0.0.9/xformers/triton/sum_strided.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     1456 2021-12-02 16:31:26.000000 xformers-0.0.9/xformers/triton/utils.py
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     3265 2021-10-25 21:28:22.000000 xformers-0.0.9/xformers/utils.py
+drwxrwxr-x   0 dianaml  (1185200879) dianaml  (1185200879)        0 2022-02-09 20:53:29.332583 xformers-0.0.9/xformers.egg-info/
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)      886 2022-02-09 20:53:29.000000 xformers-0.0.9/xformers.egg-info/PKG-INFO
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)     5172 2022-02-09 20:53:29.000000 xformers-0.0.9/xformers.egg-info/SOURCES.txt
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)        1 2022-02-09 20:53:29.000000 xformers-0.0.9/xformers.egg-info/dependency_links.txt
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)        1 2022-01-06 22:34:50.000000 xformers-0.0.9/xformers.egg-info/not-zip-safe
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       43 2022-02-09 20:53:29.000000 xformers-0.0.9/xformers.egg-info/requires.txt
+-rw-rw-r--   0 dianaml  (1185200879) dianaml  (1185200879)       22 2022-02-09 20:53:29.000000 xformers-0.0.9/xformers.egg-info/top_level.txt
```

### Comparing `xformers-0.0.8/LICENSE` & `xformers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/PKG-INFO` & `xformers-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xformers
-Version: 0.0.8
+Version: 0.0.9
 Summary: XFormers: A collection of composable Transformer building blocks.
 Home-page: UNKNOWN
 Author: Facebook AI Research
 Author-email: lefaudeux@fb.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `xformers-0.0.8/README.md` & `xformers-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![PyPI - License](https://img.shields.io/pypi/l/xformers)
 [![Documentation Status](https://github.com/facebookresearch/xformers/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/facebookresearch/xformers/actions/workflows/gh-pages.yml/badge.svg)
 [![CircleCI](https://circleci.com/gh/facebookresearch/xformers.svg?style=shield)](https://app.circleci.com/pipelines/github/facebookresearch/xformers/)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
 [![codecov](https://codecov.io/gh/facebookresearch/xformers/branch/main/graph/badge.svg?token=PKGKDR4JQM)](https://codecov.io/gh/facebookresearch/xformers)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/facebookresearch/xformers/blob/main/docs/source/xformers_mingpt.ipynb)
-
+[![Downloads](https://pepy.tech/badge/xformers)](https://pepy.tech/project/xformers)
 --------------------------------------------------------------------------------
 
 ## Description
 
 xFormers is a modular and field agnostic library to flexibly generate transformer architectures by interoperable and optimized building blocks.
 
 ## Getting started
@@ -100,19 +100,23 @@
 │   │    └ ...                  # all the supported attentions
 │   ├── feedforward             #
 │   │    └ ...                  # all the supported feedforwards
 │   ├── positional_embedding    #
 │   │    └ ...                  # all the supported positional embeddings
 │   ├── activations.py          #
 │   └── multi_head_dispatch.py  # (optional) multihead wrap
-├── factory
+│
+├── factory                     # Build model programatically
 │   ├── block_factory.py        # (optional) helper to programatically generate layers
 │   └── model_factory.py        # (optional) helper to programatically generate models
-├── models
-...                             # Full models, ready to be used
+│
+├── benchmarks
+│     └ ...                     # A lot of benchmarks that you can use to test some parts
+└── triton
+      └ ...                     # (optional) all the triton parts, requires triton + CUDA gpu
 ```
 
 <details><summary> Attention mechanisms</summary><p>
 
 - [Scaled dot product](xformers/components/attention/scaled_dot_product.py)
   - *[Attention is all you need, Vaswani et al., 2017](https://arxiv.org/abs/1706.03762)*
 - [Sparse](xformers/components/attention/scaled_dot_product.py)
@@ -135,22 +139,26 @@
 Patrick et al., 2021](https://arxiv.org/abs/2106.05392)*
 - [Random](xformers/components/attention/random.py)
   - See BigBird, Longformers,..
 - [Global](xformers/components/attention/random.py)
   - See BigBird, Longformers,..
 - [FourierMix](xformers/components/attention/fourier_mix.py)
   - *[FNet: Mixing Tokens with Fourier Transforms, Lee-Thorp et al.](https://arxiv.org/abs/2105.03824v1)*
+- [CompositionalAttention](xformers/components/attention/compositional.py)
+  - *[Compositional Attention: Disentangling search and retrieval, S. Mittal et al.](https://arxiv.org/pdf/2110.09419v1.pdf)*
+
 - ... add a new one [see Contribution.md](CONTRIBUTING.md)
 
 </p></details>
 
 <details><summary>Feed forward mechanisms </summary><p>
 
 - [MLP](xformers/components/feedforward/mlp.py)
 - [Fused](xformers/components/feedforward/fused_mlp.py)
+- [Mixture of Experts](xformers/components/feedforward/mixture_of_experts.py)
 
 </p></details>
 
 <details><summary>Positional embedding </summary><p>
 
 - [Sine](xformers/components/positional_embedding/sine.py)
 - [Vocabulary](xformers/components/positional_embedding/vocab.py)
@@ -163,14 +171,15 @@
 1. Many attention mechanisms, interchangeables
 2. Optimized building blocks, beyond PyTorch primitives
    1. sparse attention
    2. block-sparse attention
    3. fused softmax
    4. fused linear layer
    5. fused layer norm
+   6. fused dropout(activation(x+bias))
 3. Benchmarking and testing tools
    1. [micro benchnmarks](BENCHMARKS.md)
    2. transformer block benchmark
    3. [LRA](xformers/benchmarks/LRA/README.md), with SLURM suppot
 4. Programatic and sweep friendly layer and model construction
 5. Hackable
    1. Not using monolithic CUDA kernels, composable building blocks
@@ -204,7 +213,8 @@
 
 * [Sputnik](https://github.com/google-research/sputnik)
 * [GE-SpMM](https://github.com/hgyhungry/ge-spmm)
 * [Triton](https://github.com/openai/triton)
 * [LucidRain Reformer](https://github.com/lucidrains/reformer-pytorch)
 * [RevTorch](https://github.com/RobinBruegger/RevTorch)
 * [Nystromformer](https://github.com/mlpen/Nystromformer)
+* [FairScale](https://github.com/facebookresearch/fairscale/)
```

### Comparing `xformers-0.0.8/setup.py` & `xformers-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/__init__.py` & `xformers-0.0.9/xformers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 
 import torch
 
 # Please update the doc version in docs/source/conf.py as well.
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 _is_sparse_available = True
 _is_triton_available = torch.cuda.is_available()
 
 
 def _register_extensions():
     import importlib
```

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/batch_fetch_results.py` & `xformers-0.0.9/xformers/benchmarks/LRA/batch_fetch_results.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/batch_submit.py` & `xformers-0.0.9/xformers/benchmarks/LRA/batch_submit.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/code/dataset.py` & `xformers-0.0.9/xformers/benchmarks/LRA/code/dataset.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/code/model_wrapper.py` & `xformers-0.0.9/xformers/benchmarks/LRA/code/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/run_grid_search.py` & `xformers-0.0.9/xformers/benchmarks/LRA/run_grid_search.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/run_tasks.py` & `xformers-0.0.9/xformers/benchmarks/LRA/run_tasks.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/LRA/run_with_submitit.py` & `xformers-0.0.9/xformers/benchmarks/LRA/run_with_submitit.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_core.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_core.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_encoder.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_encoder.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_nystrom_utils.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_nystrom_utils.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_pytorch_transformer.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_pytorch_transformer.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_revnet.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_revnet.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_sddmm.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_sddmm.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_blocksparse.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_blocksparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,22 @@
             layout = _layout.unsqueeze(0).expand(H, -1, -1)
             a_triton = (
                 triton.testing.sparsify_tensor(a, layout, block) if mode == "dsd" else a
             )
             b_triton = (
                 triton.testing.sparsify_tensor(b, layout, block) if mode == "dds" else b
             )
-            bsmm = blocksparse_matmul(layout, block, mode, trans_a=False, trans_b=False)
+            bsmm = blocksparse_matmul(
+                layout=layout,
+                block=block,
+                mode=mode,
+                device=torch.device("cuda"),
+                trans_a=False,
+                trans_b=False,
+            )
 
             # - dense
             ta = triton.testing.mask_tensor(a, layout, block) if mode == "dsd" else a
             tb = triton.testing.mask_tensor(b, layout, block) if mode == "dds" else b
 
             # - sparse / sputnik
             mask = torch.ones_like(a, dtype=torch.float, device="cuda")
```

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_dropout.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_dropout.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_fused_linear.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_fused_linear.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_layernorm.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_layernorm.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_softmax.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_softmax.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_triton_stride_sum.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_triton_stride_sum.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/benchmark_vit_timm.py` & `xformers-0.0.9/xformers/benchmarks/benchmark_vit_timm.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/benchmarks/utils.py` & `xformers-0.0.9/xformers/benchmarks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
     """Graph out the contents of a dict.
     Dash key means that if the result label has this key, then it will be displayed with a dash"""
 
     if not filename:
         filename = title + ".png"
 
     # Sanitize the filename
-    filename = filename.replace(" ", "_").replace("/", "_").replace("-", "_")
+    filename = (
+        filename.replace(" ", "_").replace("/", "_").replace("-", "_").replace(":", "")
+    )
 
     # Gather all the results in "collumns"
     workloads: Dict[str, Any] = {k: [] for v in results.values() for k in v.keys()}
     for v in results.values():
         for k in v.keys():
             workloads[k].append(float(v[k]))
```

### Comparing `xformers-0.0.8/xformers/components/__init__.py` & `xformers-0.0.9/xformers/components/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,19 @@
         if not isinstance(multi_head_config["attention"], Attention):
             # Convenience: fill in possible missing fields
             if "num_heads" not in multi_head_config["attention"]:
                 multi_head_config["attention"]["num_heads"] = multi_head_config[
                     "num_heads"
                 ]
 
+            if "dim_model" not in multi_head_config["attention"]:
+                multi_head_config["attention"]["dim_model"] = multi_head_config[
+                    "dim_model"
+                ]
+
             if (
                 "dim_features" not in multi_head_config["attention"]
                 or multi_head_config["attention"]["dim_features"] is None
             ):
                 multi_head_config["attention"]["dim_features"] = (
                     multi_head_config["dim_model"] // multi_head_config["num_heads"]
                 )
```

### Comparing `xformers-0.0.8/xformers/components/activations.py` & `xformers-0.0.9/xformers/components/activations.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/__init__.py` & `xformers-0.0.9/xformers/components/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/_sputnik_sparse.py` & `xformers-0.0.9/xformers/components/attention/_sputnik_sparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     @property
     def shape(self):
         return self._mat.shape[1:]
 
     @property
     def values(self):
-        return self._mat._csr_values
+        return self._mat.values()
 
     @property
     def row_indices(self):
         return self._mat._csr_row_indices
 
     @property
     def column_indices(self):
```

### Comparing `xformers-0.0.8/xformers/components/attention/attention_mask.py` & `xformers-0.0.9/xformers/components/attention/attention_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         is to bias the attention computation for instance
 
     .. note: the attention mask dimensions are expected to be `[batch, to_sequence, from_sequence]`,
         `[to_sequence, from_sequence]`, or anything broadcastable in between
     """
 
     def __init__(self, additive_mask: torch.Tensor, is_causal: bool = False):
-        assert additive_mask.is_floating_point()
+        assert additive_mask.is_floating_point(), additive_mask.dtype
         assert not additive_mask.requires_grad
 
         if additive_mask.ndim == 2:
             additive_mask = additive_mask.unsqueeze(0)
 
         self.values = additive_mask
         self.is_causal = is_causal
@@ -45,28 +45,28 @@
     def from_bool(cls: Type[Self], x: torch.Tensor) -> Self:
         """
         Create an AttentionMask given a boolean pattern.
         .. warning: we assume here that True implies that the value should be computed
         """
         assert x.dtype == torch.bool
 
-        additive_mask = torch.empty_like(x, dtype=torch.float)
+        additive_mask = torch.empty_like(x, dtype=torch.float, device=x.device)
         additive_mask.masked_fill_(x, 0.0)
         additive_mask.masked_fill_(~x, float("-inf"))
 
         return cls(additive_mask)
 
     @classmethod
     def from_multiplicative(cls: Type[Self], x: torch.Tensor) -> Self:
         """
         Create an AttentionMask given a multiplicative attention mask.
         """
         assert not x.dtype == torch.bool
 
-        additive_mask = torch.empty_like(x, dtype=torch.float)
+        additive_mask = torch.empty_like(x, dtype=torch.float, device=x.device)
         x = x.bool()
 
         additive_mask.masked_fill_(x, 0.0)
         additive_mask.masked_fill_(~x, float("-inf"))
 
         return cls(additive_mask)
```

### Comparing `xformers-0.0.8/xformers/components/attention/attention_patterns.py` & `xformers-0.0.9/xformers/components/attention/attention_patterns.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/base.py` & `xformers-0.0.9/xformers/components/attention/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import asdict, dataclass
 from typing import Optional, Type, TypeVar
 
 import torch
 import torch.nn as nn
 
+from xformers.components.attention import AttentionMask
+
 
 @dataclass
 class AttentionConfig:
     """Parameters required for all Attentions.
     Can accept and store extra parameters.
     """
 
@@ -25,15 +27,15 @@
 Self = TypeVar("Self", bound="Attention")
 
 
 # Define the common interface, every attention block needs to derive from it
 class Attention(nn.Module, metaclass=ABCMeta):
     r"""The base Attention mechanism, which is typically a sub-part of the multi-head attention"""
 
-    _causal_mask: Optional[torch.Tensor] = None
+    _causal_mask: Optional[AttentionMask] = None
 
     @abstractmethod
     def __init__(self, dropout: Optional[float] = None, *args, **kwargs):
         super().__init__()
 
         # Requires the inputs to be projected
         self.requires_input_projection = True
@@ -43,14 +45,18 @@
 
         # key padding mask and attention mask must be passed in as separate arguments instead of a merged attention mask
         self.requires_separate_masks = False
 
         # Requires that K and Q have the same sequence length
         self.requires_same_k_q_dimensions = False
 
+        # Whether the attention owns the single head/multihead mechanism
+        # so that the MHA wrapper should skip it
+        self.requires_skip_multi_head = False
+
     @classmethod
     def from_config(cls: Type[Self], config: AttentionConfig) -> Self:
         # Generate the class inputs from the config
         fields = asdict(config)
 
         # Skip all Nones so that default values are used
         fields = {k: v for k, v in fields.items() if v is not None}
```

### Comparing `xformers-0.0.8/xformers/components/attention/blocksparse.py` & `xformers-0.0.9/xformers/components/attention/blocksparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from xformers import _is_triton_available
 from xformers.components.attention import Attention, AttentionConfig, register_attention
 from xformers.components.attention.utils import bool_mask_to_additive
 
 _mask_type_warning = True
 
 if _is_triton_available:
-    from triton.ops.blocksparse import matmul as blocksparse_matmul
-    from triton.ops.blocksparse import softmax as blocksparse_softmax
+    from triton.ops.blocksparse import matmul as blocksparse_matmul  # type: ignore
+    from triton.ops.blocksparse import softmax as blocksparse_softmax  # type: ignore
 
     from xformers.triton.softmax import MaskType
     from xformers.triton.utils import gpu_capabilities_older_than_70
 
     # Blocksparse requires Tensor cores
     if gpu_capabilities_older_than_70():
         logging.warning(
@@ -48,14 +48,17 @@
 
         .. warning: the layout is assumed to have the dimensions [heads, seq, seq].
             If some dimensions are missing, we assume that the same layout is to be used across heads.
 
         .. warning: for now, the sequence (context) length has to be a power of two. This constraint could
             be relaxed in the future.
 
+        .. warning: the block size has to be picked from [16, 32, 64]. Some speed is gained from bigger blocks.
+            It is of course possible to reproduce coarser patterns given these primitives, as the user sees fit.
+
         .. note: it is possible to pass a specific per batch mask in the forward call,
             but this will not lead to any speed up.
             Any constant sparsity pattern is better passed through the layout parameter.
         """
 
         def __init__(
             self,
@@ -72,15 +75,19 @@
                 )
                 logging.warning(
                     "Now assuming that the same layout is to be used across all heads"
                 )
                 layout = layout.unsqueeze(0).expand(num_heads, -1, -1)
                 logging.warning(f"New layout dimensions: {layout.shape}")
 
-            assert block_size >= 16, "Minimum block size is 16, for now at least"
+            assert block_size in (
+                16,
+                32,
+                64,
+            ), "Only block sizes in [16, 32, 64] are supported"
 
             super().__init__()
             self.attn_drop = torch.nn.Dropout(dropout, inplace=False)
 
             # Pure blocksparse data
             self.layout = layout
             self.block_size = block_size
```

### Comparing `xformers-0.0.8/xformers/components/attention/core.py` & `xformers-0.0.9/xformers/components/attention/core.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/favor.py` & `xformers-0.0.9/xformers/components/attention/favor.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,32 +46,36 @@
         iter_before_redraw: Optional[int] = None,
         feature_map_type: FeatureMapType = FeatureMapType.SMReg,
         normalize_inputs: bool = False,
         *_,
         **__,
     ):
         r"""
-        Kernelized attention, as proposed in Performers_.
+        Kernelized attention, as proposed in Performers_
+        ("Rethinking attention with performers." K. Choromanski et al. (2020).).
 
         FAVOR stands for "Fast Attention Via positive Orthogonal Random features"
 
         Args:
             dropout (float): the probability of an output to be randomly dropped at training time
             dim_features (int): the dimension of the random features space
-            iter_before_redraw (int): the number of iterations before a redraw of the features
+            iter_before_redraw (int): the number of steps (forward calls) before a redraw of the features
             feature_map_type (FeatureMapType): the type of feature map being used,
             for instance orthogonal random features.
 
-        .. _Performers: "Rethinking attention with performers." K. Choromanski et al. (2020).
-            https://arxiv.org/pdf/2009.14794v1.pdf
+        .. _Performers: https://arxiv.org/pdf/2009.14794v1.pdf
         """
         super().__init__()
 
         self.causal = causal
-        self.iter_before_redraw = iter_before_redraw
+        self.iter_before_redraw = (
+            (2 * iter_before_redraw)
+            if iter_before_redraw is not None
+            else iter_before_redraw
+        )  # This will be used for both key and query
         self.normalize_inputs = normalize_inputs
         self.feature_map_type = feature_map_type
         self.attn_drop = nn.Dropout(dropout, inplace=True)
 
         # Setup dimension-dependent variables
         # Reasonable dimension default
         if dim_features is None:
@@ -94,16 +98,15 @@
 
         feature_settings = {
             "dim_features": self.dim_features,
             "iter_before_redraw": self.iter_before_redraw,
             "normalize_inputs": self.normalize_inputs,
         }
 
-        self.feature_map_query: FeatureMap = feature_map_constructor(**feature_settings)  # type: ignore
-        self.feature_map_key: FeatureMap = feature_map_constructor(**feature_settings)  # type: ignore
+        self.feature_map: FeatureMap = feature_map_constructor(**feature_settings)  # type: ignore
 
     @staticmethod
     def _maybe_promote(x: torch.Tensor) -> torch.Tensor:
         # Only promote fp16 buffers, bfloat16 would be fine for instance
         return x.float() if x.dtype == torch.float16 else x
 
     @staticmethod
@@ -131,16 +134,16 @@
         k: torch.Tensor,
         v: torch.Tensor,
         *_,
         **__,
     ):
 
         # Project key and queries onto the feature map space
-        k_prime = self.feature_map_key(k)
-        q_prime = self.feature_map_query(q)
+        k_prime = self.feature_map(k)
+        q_prime = self.feature_map(q)
 
         with autocast(enabled=False):
             # The softmax kernel approximation for Favor will easily overflow
             # Force the computations here to stay in fp32 for numerical stability
             # Note that the dimensions are vastly reduced when compared to scaled_dot_product
             k_prime = self._maybe_promote(k_prime)
             q_prime = self._maybe_promote(q_prime)
```

### Comparing `xformers-0.0.8/xformers/components/attention/feature_maps/__init__.py` & `xformers-0.0.9/xformers/components/attention/feature_maps/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/feature_maps/base.py` & `xformers-0.0.9/xformers/components/attention/feature_maps/base.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/feature_maps/softmax.py` & `xformers-0.0.9/xformers/components/attention/feature_maps/softmax.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/fourier_mix.py` & `xformers-0.0.9/xformers/components/attention/fourier_mix.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/global_tokens.py` & `xformers-0.0.9/xformers/components/attention/global_tokens.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/lambda_layer.py` & `xformers-0.0.9/xformers/components/attention/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/linformer.py` & `xformers-0.0.9/xformers/components/attention/linformer.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/local.py` & `xformers-0.0.9/xformers/components/attention/local.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/nystrom.py` & `xformers-0.0.9/xformers/components/attention/nystrom.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/ortho.py` & `xformers-0.0.9/xformers/components/attention/ortho.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/random.py` & `xformers-0.0.9/xformers/components/attention/random.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/scaled_dot_product.py` & `xformers-0.0.9/xformers/components/attention/scaled_dot_product.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/attention/utils.py` & `xformers-0.0.9/xformers/components/attention/utils.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/feedforward/__init__.py` & `xformers-0.0.9/xformers/components/feedforward/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/feedforward/base.py` & `xformers-0.0.9/xformers/components/feedforward/base.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/feedforward/fused_mlp.py` & `xformers-0.0.9/xformers/components/feedforward/fused_mlp.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         class FusedMlpConfig(FeedforwardConfig):
             hidden_layer_multiplier: int
 
         @register_feedforward("FusedMLP", FusedMlpConfig)
         class FusedMLP(Feedforward):
             """
             A MLP using fused linear layers.
-
-            .. warning: This is not currently competitive with PyTorch in terms of training speed
             """
 
             def __init__(
                 self,
                 dim_model: int,
                 dropout: float,
                 activation: Activation,
```

### Comparing `xformers-0.0.8/xformers/components/feedforward/mlp.py` & `xformers-0.0.9/xformers/components/feedforward/mlp.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/in_proj_container.py` & `xformers-0.0.9/xformers/components/in_proj_container.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,18 +48,14 @@
 class InProjParams:
     in_features: int
     out_features: int
     bias: bool
     small_init: bool = False
 
 
-def _init_from_params(params: InProjParams):
-    return small_init_ if params.small_init else xavier_uniform_
-
-
 class InProjContainer(nn.Module):
     """
     Handle all the input projections in one go, opportunistically fuse some operations.
 
     CREDITS: Inspired by https://github.com/pytorch/text/blob/master/torchtext/nn/modules/multiheadattention.py
     and the MultiHeadAttention implementation from PyTorch
     """
@@ -87,67 +83,78 @@
         # Catch a beneficial case, if Q,K,V dimensions are the same
         self.same_dimensions = (
             query_proj_params.in_features == key_proj_params.in_features
             and value_proj_params.in_features == key_proj_params.in_features
         )
 
         self.out_features = query_proj_params.out_features
+        self.q_p_params = query_proj_params
+        self.k_p_params = key_proj_params
+        self.v_p_params = value_proj_params
 
         # - handle all the weights
         # save the requested init method
         if self.same_dimensions:
             # We can use a single weight and bias buffer, which will speed up self attention
             self.in_proj_weight = nn.Parameter(
                 torch.empty((3 * self.out_features, self.out_features))
             )
             self.register_parameter("q_proj_weight", None)
             self.register_parameter("k_proj_weight", None)
             self.register_parameter("v_proj_weight", None)
-            self.weight_init = _init_from_params(query_proj_params)
         else:
             # The dimensions are different, use seperate buffers
             self.q_proj_weight = nn.Parameter(
                 torch.empty((self.out_features, query_proj_params.in_features))
             )
             self.k_proj_weight = nn.Parameter(
                 torch.empty((self.out_features, key_proj_params.in_features))
             )
             self.v_proj_weight = nn.Parameter(
                 torch.empty((self.out_features, value_proj_params.in_features))
             )
             self.register_parameter("in_proj_weight", None)
 
-            self.weight_init = list(
-                map(
-                    _init_from_params,
-                    [query_proj_params, key_proj_params, value_proj_params],
-                )
-            )
-
         # - handle all the inputs
         if query_proj_params.bias:
             self.in_proj_bias = nn.Parameter(torch.empty(3 * self.out_features))
         else:
             self.register_parameter("in_proj_bias", None)
 
         # - multi-head attention specific init for the weights and biases
         self._reset_parameters()
 
     def _reset_parameters(self):
         if self.in_proj_weight is not None:
-            self.weight_init(self.in_proj_weight)
-        else:
-            weights = [self.q_proj_weight, self.k_proj_weight, self.v_proj_weight]
+            # 1/sqrt(2) init is empirically beneficial in that case
+            self.in_proj_weight = self._init_weights(
+                self.q_p_params, self.in_proj_weight, gain=1.0 / math.sqrt(2)
+            )
 
-            for init, weight in zip(self.weight_init, weights):
-                init(weight)
+        else:
+            self.q_proj_weight = self._init_weights(
+                self.q_p_params, self.q_proj_weight, gain=1.0
+            )
+            self.k_proj_weight = self._init_weights(
+                self.k_p_params, self.k_proj_weight, gain=1.0
+            )
+            self.v_proj_weight = self._init_weights(
+                self.v_p_params, self.v_proj_weight, gain=1.0
+            )
 
         if self.in_proj_bias is not None:
             constant_(self.in_proj_bias, 0.0)
 
+    @staticmethod
+    def _init_weights(params: InProjParams, weights: torch.Tensor, gain: float):
+        if params.small_init:
+            return small_init_(weights, gain=gain)
+        else:
+            return xavier_uniform_(weights, gain=gain)
+
     def forward(
         self,
         query: torch.Tensor,
         key: torch.Tensor,
         value: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         if self.in_proj_weight is not None:
```

### Comparing `xformers-0.0.8/xformers/components/multi_head_dispatch.py` & `xformers-0.0.9/xformers/components/multi_head_dispatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 
     def forward(
         self,
         query: torch.Tensor,
         key: Optional[torch.Tensor] = None,
         value: Optional[torch.Tensor] = None,
         att_mask: Optional[torch.Tensor] = None,
+        key_padding_mask: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """
         Expected input dimensions are [batch size, sequence length, embed dim]
         Output dimensions are [batch size, sequence length, embed dim]
         """
 
         if key is None:
@@ -139,14 +140,19 @@
             value = query
 
         # Check the dimensions properly
         self._check(query, "query")
         self._check(value, "value")
         self._check(key, "key")
 
+        max_batch = max((query.shape[0], key.shape[0], value.shape[0]))
+        query, key, value = map(
+            lambda x: x.expand(max_batch, -1, -1), [query, key, value]
+        )
+
         B, S_Q, _ = query.size()  # Batch x Sequence x Embedding (latent)
         _, S_K, _ = key.size()  # K, Q's sequence length could differ
 
         # Catch different query and key length but a causal attention
         if S_Q != S_K:
             assert (
                 not self.attention.requires_same_k_q_dimensions
@@ -154,14 +160,19 @@
 
             if hasattr(self.attention, "causal"):
                 assert not self.attention.causal, (
                     "Causal attention is not supported when key and query have different sequence lengths.\n"
                     + "In that case causality is ill-determined. Please pad your sequences accordingly"
                 )
 
+        if self.attention.requires_skip_multi_head:
+            return self.attention(
+                query, key, value, att_mask=att_mask, key_padding_mask=key_padding_mask
+            )
+
         # Calculate query, key, values for all heads in batch
         if self.attention.requires_input_projection:
             q, k, v = self.in_proj_container(query=query, key=key, value=value)
         else:
             k, q, v = key, query, value
 
         # Optional: rotary embedding, add relative positioning information
@@ -183,15 +194,17 @@
             )
 
             q = reshape_fn(q, B, S_Q, self.num_heads, self.dim_k)
             k = reshape_fn(k, B, S_K, self.num_heads, self.dim_k)
             v = reshape_fn(v, B, S_K, self.num_heads, self.dim_k)
 
         # Self-attend
-        y = self.attention(q=q, k=k, v=v, att_mask=att_mask)
+        y = self.attention(
+            q=q, k=k, v=v, att_mask=att_mask, key_padding_mask=key_padding_mask
+        )
 
         # Re-assemble all head outputs side by side
         y = (
             y.view(B, self.num_heads, S_Q, self.dim_k)
             .transpose(1, 2)
             .flatten(start_dim=2, end_dim=3)
         )
```

### Comparing `xformers-0.0.8/xformers/components/positional_embedding/__init__.py` & `xformers-0.0.9/xformers/components/positional_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/positional_embedding/base.py` & `xformers-0.0.9/xformers/components/positional_embedding/base.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/positional_embedding/rotary.py` & `xformers-0.0.9/xformers/components/positional_embedding/rotary.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/positional_embedding/vocab.py` & `xformers-0.0.9/xformers/components/positional_embedding/vocab.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/residual.py` & `xformers-0.0.9/xformers/components/residual.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/components/reversible.py` & `xformers-0.0.9/xformers/components/reversible.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 # pyre-fixme[13]: `cpu_state` is not initialized in the constructor.
 class Deterministic(nn.Module):
     def __init__(self, net: nn.Module):
         super().__init__()
         self.net = net
-        self.cpu_state: torch.Tensor
+        self.cpu_state: torch.Tensor = torch.get_rng_state()
         self.cuda_in_fwd: bool = False
         self.gpu_devices: List[int] = []
         self.gpu_states: List[torch.Tensor] = []
 
     def record_rng(self, *args):
         self.cpu_state = torch.get_rng_state()
         if torch.cuda._initialized:
@@ -64,15 +64,17 @@
 
         with torch.no_grad():
             y1 = x1 + self.f(x2, record_rng=self.training, **f_args)
             y2 = x2 + self.g(y1, record_rng=self.training, **g_args)
 
         return torch.cat([y1, y2], dim=self.split_dim)
 
-    def backward_pass(self, y: torch.Tensor, dy: torch.Tensor, f_args={}, g_args={}):
+    def backward_pass(
+        self, y: torch.Tensor, dy: torch.Tensor, f_args={}, g_args={}
+    ):  # pragma: no cover  # this is covered, but called directly from C++
         y1, y2 = torch.chunk(y, 2, dim=self.split_dim)
         del y
 
         dy1, dy2 = torch.chunk(dy, 2, dim=self.split_dim)
         del dy
 
         with torch.enable_grad():
@@ -114,15 +116,17 @@
         for block in blocks:
             x = block(x, **kwargs)
         ctx.y = x.detach()
         ctx.blocks = blocks
         return x
 
     @staticmethod
-    def backward(ctx, dy):
+    def backward(
+        ctx, dy
+    ):  # pragma: no cover # this is covered, but called directly from C++
         y = ctx.y
         kwargs = ctx.kwargs
         for block in ctx.blocks[::-1]:
             y, dy = block.backward_pass(y, dy, **kwargs)
         return dy, None, None
```

### Comparing `xformers-0.0.8/xformers/factory/__init__.py` & `xformers-0.0.9/xformers/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/factory/block_factory.py` & `xformers-0.0.9/xformers/factory/block_factory.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/factory/hydra_helper.py` & `xformers-0.0.9/xformers/factory/hydra_helper.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/factory/model_factory.py` & `xformers-0.0.9/xformers/factory/model_factory.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/helpers/timm_sparse_attention.py` & `xformers-0.0.9/xformers/helpers/timm_sparse_attention.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/ops.py` & `xformers-0.0.9/xformers/ops.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/sparse/_csr_ops.py` & `xformers-0.0.9/xformers/sparse/_csr_ops.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/sparse/csr_tensor.py` & `xformers-0.0.9/xformers/sparse/csr_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,16 +76,15 @@
         matrix.__values = values
         matrix.__row_indices = row_indices
         matrix.__row_offsets = row_offsets
         matrix.__column_indices = column_indices
         matrix.__transp_info = _transp_info
         return matrix
 
-    @property
-    def _csr_values(self):
+    def values(self):
         return self.__values
 
     @property
     def _csr_row_indices(self):
         return self.__row_indices
 
     @property
```

### Comparing `xformers-0.0.8/xformers/sparse/utils.py` & `xformers-0.0.9/xformers/sparse/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,16 @@
     # - get permutation for stable sort of the columns to get the rows for the transposed matrix
     # - compress the new rows and return the permutation to be applied on the values
 
     # convert from compressed rows to uncompressed
     row_coo, _ = _csr_to_coo(m, n, row_offsets, column_indices)
 
     # get the permutation for the stable sort
-    # unfortunately PyTorch sort is not stable, so we need to
-    # do it in two steps
-    row_offsets_t, perm1 = column_indices.sort(0)
-    new_columns = row_coo[perm1]
-
-    # workaround the lack of stable sorting in PyTorch
-    perm2 = torch.argsort(new_columns + row_offsets_t * m)
-    column_indices_t = new_columns[perm2]
-
-    # find the final permutation corresponding to the indices of the stable sort
-    perm = perm1[perm2]
+    row_offsets_t, perm = column_indices.sort(dim=0, stable=True)
+    column_indices_t = row_coo[perm]
 
     row_offsets_t, _ = _coo_to_csr(m, n, row_offsets_t, column_indices)
     row_indices_t = _diffsort(row_offsets_t).int()
 
     return row_indices_t, row_offsets_t, column_indices_t, perm
```

### Comparing `xformers-0.0.8/xformers/triton/__init__.py` & `xformers-0.0.9/xformers/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/dropout.py` & `xformers-0.0.9/xformers/triton/dropout.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/fused_linear_layer.py` & `xformers-0.0.9/xformers/triton/fused_linear_layer.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_activations.py` & `xformers-0.0.9/xformers/triton/k_activations.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_dropout.py` & `xformers-0.0.9/xformers/triton/k_dropout.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_fused_matmul_bw.py` & `xformers-0.0.9/xformers/triton/k_fused_matmul_bw.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_fused_matmul_fw.py` & `xformers-0.0.9/xformers/triton/k_fused_matmul_fw.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_layer_norm.py` & `xformers-0.0.9/xformers/triton/k_layer_norm.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_softmax.py` & `xformers-0.0.9/xformers/triton/k_softmax.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/k_sum.py` & `xformers-0.0.9/xformers/triton/k_sum.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/layer_norm.py` & `xformers-0.0.9/xformers/triton/layer_norm.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/softmax.py` & `xformers-0.0.9/xformers/triton/softmax.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from xformers.triton.k_softmax import _softmax, _softmax_backward
 
 # CREDITS: This is adapted from the vanilla Triton example. See https://openai.com/blog/triton/
 # and https://triton-lang.org/getting-started/tutorials/02-fused-softmax.html
 
 
 _triton_registered_overflow = False
-_triton_registered_warnings = False
 _triton_softmax_fp16_enabled = False  # NOTE: PyTorch keeps softmax as fp32
 
 
 class MaskType(str, Enum):
     ADD = "add"
     MUL = "mul"
 
@@ -36,14 +35,15 @@
         """
         Fused softmax implementation, using the Triton programming model.
         This only supports a reduction over the last dimension for now
         """
 
         # Handle 2D/3D tensors
         x_ = x.unsqueeze(0) if x.ndim == 2 else x
+        x_ = x_.flatten(0, -3)
 
         if not x_.is_contiguous():
             x_ = x_.contiguous()
 
         y = torch.empty_like(x_)
         assert (
             y.stride(2) == 1 and x_.stride(2) == 1
@@ -88,14 +88,15 @@
     @staticmethod
     @custom_bwd
     def backward(ctx, grad_out):
         (out,) = ctx.saved_tensors
 
         # Handle 2D/3D tensors
         grad_out_ = grad_out.unsqueeze(0) if grad_out.ndim == 2 else grad_out
+        grad_out_ = grad_out_.flatten(0, -3)
 
         # SPMD launch grid
         grid_2d = (
             grad_out_.shape[0],
             grad_out_.shape[1],
         )
 
@@ -173,36 +174,31 @@
 ) -> torch.Tensor:
     # Triton is used if
     # - CUDA
     # - there's enough data to make it faster than pytorch. This could change over time, Triton is improving
     # - there was no previous failure
 
     global _triton_registered_overflow
-    global _triton_registered_warnings
 
     try:
         if torch.cuda.is_available() and x.is_cuda and not _triton_registered_overflow:
             return _softmax_triton.apply(x, mask, log, causal)
     except (triton.code_gen.OutOfResources, RuntimeError) as e:
         # Catch cases where the current GPU does not have enough registers to hold a full tensor line
         # fallback to PyTorch's implementation, which streams the tensor in and out
         _triton_registered_overflow = True
         logging.warning(
             "Triton softmax kernel register spillover or invalid image caught."
             "Deactivating this kernel, please file an issue int the xFormers repository"
         )
         logging.warning(e)
 
-    if causal and not _triton_registered_warnings:
-        logging.warning(
-            "Triton softmax could not be used. \
-                The causal flags is being passed but it does not provide any benefit with PyTorch softmax."
-        )
-        _triton_registered_warnings = True
-
     if mask is not None:
         x = x + mask
 
+    if causal:
+        x = x + torch.triu(torch.full_like(x, float("-inf")), diagonal=1)
+
     if log:
         return torch.log_softmax(x, dim=-1)
     else:
         return torch.softmax(x, dim=-1)
```

### Comparing `xformers-0.0.8/xformers/triton/sum_strided.py` & `xformers-0.0.9/xformers/triton/sum_strided.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/triton/utils.py` & `xformers-0.0.9/xformers/triton/utils.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers/utils.py` & `xformers-0.0.9/xformers/utils.py`

 * *Files identical despite different names*

### Comparing `xformers-0.0.8/xformers.egg-info/PKG-INFO` & `xformers-0.0.9/xformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xformers
-Version: 0.0.8
+Version: 0.0.9
 Summary: XFormers: A collection of composable Transformer building blocks.
 Home-page: UNKNOWN
 Author: Facebook AI Research
 Author-email: lefaudeux@fb.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `xformers-0.0.8/xformers.egg-info/SOURCES.txt` & `xformers-0.0.9/xformers.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/sparse_softmax.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/spmm.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/autograd/matmul.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/cpu/matmul.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/cpu/sddmm.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/cpu/sparse_softmax.cpp
 /private/home/dianaml/src/facebookresearch/xformers/xformers/components/attention/csrc/cpu/spmm.cpp
+experimental/__init__.py
+experimental/setup.py
+experimental/ragged_inference/__init__.py
+experimental/ragged_inference/garbage_pad_ragged_acts.py
+experimental/ragged_inference/seq_kv_cache.py
+experimental/ragged_inference/test_utils.py
+experimental/ragged_inference/triton_v2_matmul.py
+experimental/ragged_inference/triton_v2_qk_dotprod.py
+experimental/ragged_inference/triton_v2_ragged_qk_dotprod.py
 xformers/__init__.py
 xformers/ops.py
 xformers/test.py
 xformers/utils.py
 xformers.egg-info/PKG-INFO
 xformers.egg-info/SOURCES.txt
 xformers.egg-info/dependency_links.txt
@@ -55,14 +64,15 @@
 xformers/components/reversible.py
 xformers/components/attention/__init__.py
 xformers/components/attention/_sputnik_sparse.py
 xformers/components/attention/attention_mask.py
 xformers/components/attention/attention_patterns.py
 xformers/components/attention/base.py
 xformers/components/attention/blocksparse.py
+xformers/components/attention/compositional.py
 xformers/components/attention/core.py
 xformers/components/attention/favor.py
 xformers/components/attention/fourier_mix.py
 xformers/components/attention/global_tokens.py
 xformers/components/attention/lambda_layer.py
 xformers/components/attention/linformer.py
 xformers/components/attention/local.py
@@ -73,28 +83,31 @@
 xformers/components/attention/utils.py
 xformers/components/attention/feature_maps/__init__.py
 xformers/components/attention/feature_maps/base.py
 xformers/components/attention/feature_maps/softmax.py
 xformers/components/feedforward/__init__.py
 xformers/components/feedforward/base.py
 xformers/components/feedforward/fused_mlp.py
+xformers/components/feedforward/mixture_of_experts.py
 xformers/components/feedforward/mlp.py
 xformers/components/positional_embedding/__init__.py
 xformers/components/positional_embedding/base.py
 xformers/components/positional_embedding/rotary.py
 xformers/components/positional_embedding/sine.py
 xformers/components/positional_embedding/vocab.py
 xformers/factory/__init__.py
 xformers/factory/block_factory.py
 xformers/factory/hydra_helper.py
 xformers/factory/model_factory.py
 xformers/helpers/__init__.py
+xformers/helpers/test_utils.py
 xformers/helpers/timm_sparse_attention.py
 xformers/sparse/__init__.py
 xformers/sparse/_csr_ops.py
+xformers/sparse/blocksparse_tensor.py
 xformers/sparse/csr_tensor.py
 xformers/sparse/utils.py
 xformers/triton/__init__.py
 xformers/triton/dropout.py
 xformers/triton/fused_linear_layer.py
 xformers/triton/k_activations.py
 xformers/triton/k_dropout.py
```

