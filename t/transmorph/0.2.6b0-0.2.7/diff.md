# Comparing `tmp/transmorph-0.2.6b0.tar.gz` & `tmp/transmorph-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmorph-0.2.6b0.tar", last modified: Fri Nov 25 15:28:13 2022, max compression
+gzip compressed data, was "transmorph-0.2.7.tar", last modified: Mon Jun 26 09:02:02 2023, max compression
```

## Comparing `transmorph-0.2.6b0.tar` & `transmorph-0.2.7.tar`

### file list

```diff
@@ -1,134 +1,130 @@
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      312 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/.gitignore
--rw-r--r--   0 risitop   (1000) risitop   (1000)       71 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/.projectile
--rw-r--r--   0 risitop   (1000) risitop   (1000)      574 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/.readthedocs.yaml
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1074 2021-09-01 08:37:37.000000 transmorph-0.2.6b0/LICENSE
--rw-r--r--   0 risitop   (1000) risitop   (1000)       89 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/MANIFEST.in
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4768 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/PKG-INFO
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4267 2022-11-25 14:42:36.000000 transmorph-0.2.6b0/README.md
--rw-r--r--   0 risitop   (1000) risitop   (1000)       95 2021-09-01 08:37:37.000000 transmorph-0.2.6b0/build.sh
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.456233 transmorph-0.2.6b0/img/
--rw-r--r--   0 risitop   (1000) risitop   (1000)   616077 2022-04-11 08:40:28.000000 transmorph-0.2.6b0/img/logo.png
--rw-r--r--   0 risitop   (1000) risitop   (1000)      100 2021-09-01 08:37:37.000000 transmorph-0.2.6b0/pyproject.toml
--rw-r--r--   0 risitop   (1000) risitop   (1000)       69 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/setup.cfg
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1178 2022-11-25 15:28:07.000000 transmorph-0.2.6b0/setup.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.456233 transmorph-0.2.6b0/src/
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      814 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1482 2022-10-05 08:49:42.000000 transmorph-0.2.6b0/src/transmorph/_logging.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2747 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/_profiling.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     6346 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/_settings.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/datasets/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      713 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/datasets/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/datasets/data/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2021-09-01 08:37:37.000000 transmorph-0.2.6b0/src/transmorph/datasets/data/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/
--rw-r--r--   0 risitop   (1000) risitop   (1000)    33176 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralA.csv
--rw-r--r--   0 risitop   (1000) risitop   (1000)    10825 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralA_labels.csv
--rw-r--r--   0 risitop   (1000) risitop   (1000)    50577 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralB.csv
--rw-r--r--   0 risitop   (1000) risitop   (1000)    16575 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralB_labels.csv
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5711 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/datasets/databank_api.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2863 2022-11-25 14:50:08.000000 transmorph-0.2.6b0/src/transmorph/datasets/datasets.json
--rw-r--r--   0 risitop   (1000) risitop   (1000)    17627 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/datasets/datasets.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       70 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/checking/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      196 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/checking/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1611 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/lisi.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2252 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/neighborentropy.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1651 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/checking/checking.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/evaluators/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      290 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/evaluators/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1783 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/evaluators/matching_evaluators.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/layers/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      449 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4346 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layer.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     7722 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layerchecking.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1945 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layerinput.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5671 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layermatching.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2682 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layermerging.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1479 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layeroutput.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1988 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/layers/layertransformation.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph/engine/matching/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      483 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3789 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/bknn.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1875 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/combinematching.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4958 2022-10-05 08:43:26.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/fusedgw.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5497 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/gw.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1407 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/labels.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5664 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/mnn.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     9920 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/ot.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2332 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/matching/matching.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/merging/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      305 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1780 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/barycenter.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     8499 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/graphembedding.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5155 2022-11-25 11:17:27.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/linearcorrection.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2622 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/merging/merging.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)    10758 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/engine/model.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/subsampling/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      217 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/subsampling/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)      673 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/keepall.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1902 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/vertexcover.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1843 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/subsampling/subsampling.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/traits/
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1185 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1987 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/cancatchchecking.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1984 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/canlog.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3709 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/containstransformations.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3883 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/hasmetadata.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1287 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/isprofilable.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3528 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/isrepresentable.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     9490 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/issubsamplable.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4835 2022-08-17 08:34:23.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/usescommonfeatures.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1728 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/usesmatching.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3909 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/usesmetric.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1722 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/usesreference.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2152 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/usessamplelabels.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1426 2022-10-05 08:43:26.000000 transmorph-0.2.6b0/src/transmorph/engine/traits/utils.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.462900 transmorph-0.2.6b0/src/transmorph/engine/transforming/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      388 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/__init__.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1678 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/commonfeatures.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1885 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/ica.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3096 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/pca.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3062 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/pooling.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1110 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/standardize.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3931 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/engine/transforming/transformation.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/src/transmorph/models/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      213 2022-08-10 09:48:38.000000 transmorph-0.2.6b0/src/transmorph/models/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     6229 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/models/embedmnn.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     6377 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/models/mnncorrection.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     7558 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/models/transportcorrection.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/src/transmorph/stats/
--rw-r--r--   0 risitop   (1000) risitop   (1000)      358 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/stats/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1969 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/stats/entropy.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3994 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/stats/integration.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3725 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/stats/lisi.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     7426 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/stats/matching.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.466233 transmorph-0.2.6b0/src/transmorph/utils/
--rw-r--r--   0 risitop   (1000) risitop   (1000)       23 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/utils/__init__.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)    14522 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/utils/anndata_manager.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     3705 2022-11-15 11:06:40.000000 transmorph-0.2.6b0/src/transmorph/utils/dimred.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)      210 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/utils/file.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     2277 2022-08-05 10:06:10.000000 transmorph-0.2.6b0/src/transmorph/utils/geometry.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)    22810 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/utils/graph.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     5292 2022-11-16 16:12:31.000000 transmorph-0.2.6b0/src/transmorph/utils/infer.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4636 2022-10-05 08:43:26.000000 transmorph-0.2.6b0/src/transmorph/utils/matrix.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)     1705 2022-10-19 12:23:41.000000 transmorph-0.2.6b0/src/transmorph/utils/misc.py
--rw-r--r--   0 risitop   (1000) risitop   (1000)    18878 2022-11-16 13:45:58.000000 transmorph-0.2.6b0/src/transmorph/utils/plotting.py
-drwxr-xr-x   0 risitop   (1000) risitop   (1000)        0 2022-11-25 15:28:13.459567 transmorph-0.2.6b0/src/transmorph.egg-info/
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4768 2022-11-25 15:28:13.000000 transmorph-0.2.6b0/src/transmorph.egg-info/PKG-INFO
--rw-r--r--   0 risitop   (1000) risitop   (1000)     4400 2022-11-25 15:28:13.000000 transmorph-0.2.6b0/src/transmorph.egg-info/SOURCES.txt
--rw-r--r--   0 risitop   (1000) risitop   (1000)        1 2022-11-25 15:28:13.000000 transmorph-0.2.6b0/src/transmorph.egg-info/dependency_links.txt
--rw-r--r--   0 risitop   (1000) risitop   (1000)      155 2022-11-25 15:28:13.000000 transmorph-0.2.6b0/src/transmorph.egg-info/requires.txt
--rw-r--r--   0 risitop   (1000) risitop   (1000)       11 2022-11-25 15:28:13.000000 transmorph-0.2.6b0/src/transmorph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.381046 transmorph-0.2.7/
+-rw-rw-rw-   0        0        0     1093 2022-10-10 09:12:24.000000 transmorph-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       90 2022-10-19 13:47:49.000000 transmorph-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4858 2023-06-26 09:02:02.381046 transmorph-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4344 2022-11-18 09:22:14.000000 transmorph-0.2.7/README.md
+-rw-rw-rw-   0        0        0      102 2022-10-10 09:12:24.000000 transmorph-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2023-06-26 09:02:02.382046 transmorph-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-06-26 08:44:08.000000 transmorph-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.255350 transmorph-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.278304 transmorph-0.2.7/src/transmorph/
+-rw-rw-rw-   0        0        0      841 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/__init__.py
+-rw-rw-rw-   0        0        0     1543 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_logging.py
+-rw-rw-rw-   0        0        0     2845 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_profiling.py
+-rw-rw-rw-   0        0        0     6536 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.307603 transmorph-0.2.7/src/transmorph/datasets/
+-rw-rw-rw-   0        0        0      741 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.308603 transmorph-0.2.7/src/transmorph/datasets/data/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.330608 transmorph-0.2.7/src/transmorph/datasets/data/spirals/
+-rw-rw-rw-   0        0        0    33609 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA.csv
+-rw-rw-rw-   0        0        0    11258 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA_labels.csv
+-rw-rw-rw-   0        0        0    51240 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB.csv
+-rw-rw-rw-   0        0        0    17238 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB_labels.csv
+-rw-rw-rw-   0        0        0     5866 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/databank_api.py
+-rw-rw-rw-   0        0        0     2957 2022-11-28 15:56:35.000000 transmorph-0.2.7/src/transmorph/datasets/datasets.json
+-rw-rw-rw-   0        0        0    18148 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/datasets/datasets.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.331608 transmorph-0.2.7/src/transmorph/engine/
+-rw-rw-rw-   0        0        0       75 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.332600 transmorph-0.2.7/src/transmorph/engine/checking/
+-rw-rw-rw-   0        0        0      203 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/checking/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.334609 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1660 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/lisi.py
+-rw-rw-rw-   0        0        0     2321 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/algorithms/neighborentropy.py
+-rw-rw-rw-   0        0        0     1704 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/checking/checking.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.335609 transmorph-0.2.7/src/transmorph/engine/evaluators/
+-rw-rw-rw-   0        0        0      303 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/evaluators/__init__.py
+-rw-rw-rw-   0        0        0     1846 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/evaluators/matching_evaluators.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.340297 transmorph-0.2.7/src/transmorph/engine/layers/
+-rw-rw-rw-   0        0        0      468 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/__init__.py
+-rw-rw-rw-   0        0        0     4468 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layer.py
+-rw-rw-rw-   0        0        0     7936 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/layers/layerchecking.py
+-rw-rw-rw-   0        0        0     2002 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layerinput.py
+-rw-rw-rw-   0        0        0     5835 2022-10-20 15:53:39.000000 transmorph-0.2.7/src/transmorph/engine/layers/layermatching.py
+-rw-rw-rw-   0        0        0     2760 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/layers/layermerging.py
+-rw-rw-rw-   0        0        0     1527 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/engine/layers/layeroutput.py
+-rw-rw-rw-   0        0        0     2054 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/layers/layertransformation.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.341308 transmorph-0.2.7/src/transmorph/engine/matching/
+-rw-rw-rw-   0        0        0      505 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.346309 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3897 2022-11-10 14:04:53.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/bknn.py
+-rw-rw-rw-   0        0        0     1923 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/combinematching.py
+-rw-rw-rw-   0        0        0     5095 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/fusedgw.py
+-rw-rw-rw-   0        0        0     5640 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/gw.py
+-rw-rw-rw-   0        0        0     1455 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/labels.py
+-rw-rw-rw-   0        0        0     5816 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/mnn.py
+-rw-rw-rw-   0        0        0    10156 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/matching/algorithms/ot.py
+-rw-rw-rw-   0        0        0     2398 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/matching/matching.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.348320 transmorph-0.2.7/src/transmorph/engine/merging/
+-rw-rw-rw-   0        0        0      318 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.350320 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/barycenter.py
+-rw-rw-rw-   0        0        0     8716 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/graphembedding.py
+-rw-rw-rw-   0        0        0     5301 2022-11-26 11:46:46.000000 transmorph-0.2.7/src/transmorph/engine/merging/algorithms/linearcorrection.py
+-rw-rw-rw-   0        0        0     2690 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/merging/merging.py
+-rw-rw-rw-   0        0        0    11038 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/engine/model.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.351321 transmorph-0.2.7/src/transmorph/engine/subsampling/
+-rw-rw-rw-   0        0        0      228 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.353321 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      699 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/keepall.py
+-rw-rw-rw-   0        0        0     1957 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/vertexcover.py
+-rw-rw-rw-   0        0        0     1905 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/subsampling/subsampling.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.362031 transmorph-0.2.7/src/transmorph/engine/traits/
+-rw-rw-rw-   0        0        0     1223 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/traits/__init__.py
+-rw-rw-rw-   0        0        0     2050 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/cancatchchecking.py
+-rw-rw-rw-   0        0        0     2060 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/canlog.py
+-rw-rw-rw-   0        0        0     3809 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/traits/containstransformations.py
+-rw-rw-rw-   0        0        0     3988 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/hasmetadata.py
+-rw-rw-rw-   0        0        0     1336 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/isprofilable.py
+-rw-rw-rw-   0        0        0     3642 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/isrepresentable.py
+-rw-rw-rw-   0        0        0     9772 2022-10-20 15:49:57.000000 transmorph-0.2.7/src/transmorph/engine/traits/issubsamplable.py
+-rw-rw-rw-   0        0        0     4956 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usescommonfeatures.py
+-rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesmatching.py
+-rw-rw-rw-   0        0        0     4034 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesmetric.py
+-rw-rw-rw-   0        0        0     1779 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usesreference.py
+-rw-rw-rw-   0        0        0     2219 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/usessamplelabels.py
+-rw-rw-rw-   0        0        0     1474 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/traits/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.363042 transmorph-0.2.7/src/transmorph/engine/transforming/
+-rw-rw-rw-   0        0        0      516 2022-12-09 09:35:34.000000 transmorph-0.2.7/src/transmorph/engine/transforming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.367043 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1729 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/commonfeatures.py
+-rw-rw-rw-   0        0        0     1948 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/ica.py
+-rw-rw-rw-   0        0        0     3184 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pca.py
+-rw-rw-rw-   0        0        0     3150 2022-11-10 09:45:55.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pooling.py
+-rw-rw-rw-   0        0        0     1155 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/standardize.py
+-rw-rw-rw-   0        0        0     4046 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/engine/transforming/transformation.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.370043 transmorph-0.2.7/src/transmorph/models/
+-rw-rw-rw-   0        0        0      297 2022-12-09 09:39:17.000000 transmorph-0.2.7/src/transmorph/models/__init__.py
+-rw-rw-rw-   0        0        0     6411 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/embedmnn.py
+-rw-rw-rw-   0        0        0     2687 2022-12-09 09:31:47.000000 transmorph-0.2.7/src/transmorph/models/harmony.py
+-rw-rw-rw-   0        0        0     6564 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/mnncorrection.py
+-rw-rw-rw-   0        0        0     3075 2022-12-09 09:31:40.000000 transmorph-0.2.7/src/transmorph/models/scvi_vae.py
+-rw-rw-rw-   0        0        0     7768 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/models/transportcorrection.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.373044 transmorph-0.2.7/src/transmorph/stats/
+-rw-rw-rw-   0        0        0      376 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/__init__.py
+-rw-rw-rw-   0        0        0     2035 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/entropy.py
+-rw-rw-rw-   0        0        0     4118 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/stats/integration.py
+-rw-rw-rw-   0        0        0     3854 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/stats/lisi.py
+-rw-rw-rw-   0        0        0     7658 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/stats/matching.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.381046 transmorph-0.2.7/src/transmorph/utils/
+-rw-rw-rw-   0        0        0       24 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/__init__.py
+-rw-rw-rw-   0        0        0    14929 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/anndata_manager.py
+-rw-rw-rw-   0        0        0     3842 2022-11-02 15:25:44.000000 transmorph-0.2.7/src/transmorph/utils/dimred.py
+-rw-rw-rw-   0        0        0      220 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/utils/file.py
+-rw-rw-rw-   0        0        0     2353 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/geometry.py
+-rw-rw-rw-   0        0        0    23531 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/graph.py
+-rw-rw-rw-   0        0        0     5464 2022-11-18 09:21:05.000000 transmorph-0.2.7/src/transmorph/utils/infer.py
+-rw-rw-rw-   0        0        0     4791 2022-10-10 09:12:24.000000 transmorph-0.2.7/src/transmorph/utils/matrix.py
+-rw-rw-rw-   0        0        0     1766 2022-10-19 13:47:50.000000 transmorph-0.2.7/src/transmorph/utils/misc.py
+-rw-rw-rw-   0        0        0    19910 2022-11-30 09:32:06.000000 transmorph-0.2.7/src/transmorph/utils/plotting.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:02:02.292307 transmorph-0.2.7/src/transmorph.egg-info/
+-rw-rw-rw-   0        0        0     4858 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 09:02:02.000000 transmorph-0.2.7/src/transmorph.egg-info/top_level.txt
```

### Comparing `transmorph-0.2.6b0/LICENSE` & `transmorph-0.2.7/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `transmorph-0.2.6b0/PKG-INFO` & `transmorph-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1
-Name: transmorph
-Version: 0.2.6b0
-Summary: A unifying data integration framework.
-Home-page: https://github.com/Risitop/transmorph
-Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
-Author-email: aziz.fouche@curie.fr
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
-
-[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
-[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
-[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
-[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
-[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
-
-**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
-
-<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
-
-Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
-
-## Documentation
-
-https://transmorph.readthedocs.io/en/latest/
-
-## Installation
-
-**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
-
-See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
-
-### Quick starting with a pre-built model
-
-All **transmorph** models take a list or a dictionary containing AnnData objects as input
-for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
-
-```python
-from transmorph.datasets import load_chen_10x
-chen_10x = load_chen_10x()
-```
-
-One can then either create a custom integration model, or load 
-a pre-built transmorph model. We will choose the *EmbedMNN* model with
-default parameters for this example, which embeds all datasets into 
-a common abstract 2D space. 
-
-```python
-from transmorph.models import EmbedMNN
-model = EmbedMNN()
-model.transform(chen_10x)
-```
-
-Integration embedding coordinates can be gathered in each AnnData object,
-in AnnData.obsm['X_transmorph'].
-
-```python
-chen_10x['P01'].obsm['X_transmorph']
-```
-
-One can for instance use a plotting function from transmorph to display integration results.
-
-```python
-from transmorph.utils.plotting import scatter_plot
-
-scatter_plot(chen_10x, use_rep="X_transmorph")
-scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
-```
-
-## Citing transmorph
-
-If you find transmorph useful for your research, please consider citing our pre-print
-which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
-
-```bibtex
-@article{fouche2022transmorph,
-  title={transmorph: a unifying computational framework for single-cell data integration},
-  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
-  journal={bioRxiv},
-  year={2022}
-}
-```
-
-# References
-
-[Chen 2020] [Chen, Y. P., Yin, J. H., Li, W. F., Li, H. J., Chen, D. P., Zhang, C. J., ... & Ma, J. (2020). Single-cell transcriptomics reveals regulators underlying immune cell diversity and immune subtypes associated with prognosis in nasopharyngeal carcinoma. Cell research, 30(11), 1024-1042.](https://www.nature.com/articles/s41422-020-0374-x)
+Metadata-Version: 2.1
+Name: transmorph
+Version: 0.2.7
+Summary: A unifying data integration framework.
+Home-page: https://github.com/Risitop/transmorph
+Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
+Author-email: aziz.fouche@curie.fr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
+
+[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
+[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
+[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+
+**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
+
+<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
+
+Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
+
+## Documentation
+
+https://transmorph.readthedocs.io/en/latest/
+
+## Installation
+
+**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
+
+See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
+
+### Quick starting with a pre-built model
+
+All **transmorph** models take a list or a dictionary containing AnnData objects as input
+for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
+
+```python
+from transmorph.datasets import load_chen_10x
+chen_10x = load_chen_10x()
+```
+
+One can then either create a custom integration model, or load 
+a pre-built transmorph model. We will choose the *EmbedMNN* model with
+default parameters for this example, which embeds all datasets into 
+a common abstract 2D space. 
+
+```python
+from transmorph.models import EmbedMNN
+model = EmbedMNN()
+model.transform(chen_10x)
+```
+
+Integration embedding coordinates can be gathered in each AnnData object,
+in AnnData.obsm['X_transmorph'].
+
+```python
+chen_10x['P01'].obsm['X_transmorph']
+```
+
+One can for instance use a plotting function from transmorph to display integration results.
+
+```python
+from transmorph.utils.plotting import scatter_plot
+
+scatter_plot(chen_10x, use_rep="X_transmorph")
+scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
+```
+
+## Citing transmorph
+
+If you find transmorph useful for your research, please consider citing our pre-print
+which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
+
+```bibtex
+@article{fouche2022transmorph,
+  title={transmorph: a unifying computational framework for single-cell data integration},
+  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
+  journal={bioRxiv},
+  year={2022}
+}
+```
+
+# References
+
+[Chen 2020] [Chen, Y. P., Yin, J. H., Li, W. F., Li, H. J., Chen, D. P., Zhang, C. J., ... & Ma, J. (2020). Single-cell transcriptomics reveals regulators underlying immune cell diversity and immune subtypes associated with prognosis in nasopharyngeal carcinoma. Cell research, 30(11), 1024-1042.](https://www.nature.com/articles/s41422-020-0374-x)
```

### Comparing `transmorph-0.2.6b0/README.md` & `transmorph-0.2.7/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
-
-[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
-[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
-[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
-[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
-[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
-
-**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
-
-<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
-
-Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
-
-## Documentation
-
-https://transmorph.readthedocs.io/en/latest/
-
-## Installation
-
-**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
-
-See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
-
-### Quick starting with a pre-built model
-
-All **transmorph** models take a list or a dictionary containing AnnData objects as input
-for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
-
-```python
-from transmorph.datasets import load_chen_10x
-chen_10x = load_chen_10x()
-```
-
-One can then either create a custom integration model, or load 
-a pre-built transmorph model. We will choose the *EmbedMNN* model with
-default parameters for this example, which embeds all datasets into 
-a common abstract 2D space. 
-
-```python
-from transmorph.models import EmbedMNN
-model = EmbedMNN()
-model.transform(chen_10x)
-```
-
-Integration embedding coordinates can be gathered in each AnnData object,
-in AnnData.obsm['X_transmorph'].
-
-```python
-chen_10x['P01'].obsm['X_transmorph']
-```
-
-One can for instance use a plotting function from transmorph to display integration results.
-
-```python
-from transmorph.utils.plotting import scatter_plot
-
-scatter_plot(chen_10x, use_rep="X_transmorph")
-scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
-```
-
-## Citing transmorph
-
-If you find transmorph useful for your research, please consider citing our pre-print
-which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
-
-```bibtex
-@article{fouche2022transmorph,
-  title={transmorph: a unifying computational framework for single-cell data integration},
-  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
-  journal={bioRxiv},
-  year={2022}
-}
-```
-
-# References
-
+# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
+
+[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
+[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
+[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+
+**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
+
+<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
+
+Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
+
+## Documentation
+
+https://transmorph.readthedocs.io/en/latest/
+
+## Installation
+
+**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
+
+See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
+
+### Quick starting with a pre-built model
+
+All **transmorph** models take a list or a dictionary containing AnnData objects as input
+for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
+
+```python
+from transmorph.datasets import load_chen_10x
+chen_10x = load_chen_10x()
+```
+
+One can then either create a custom integration model, or load 
+a pre-built transmorph model. We will choose the *EmbedMNN* model with
+default parameters for this example, which embeds all datasets into 
+a common abstract 2D space. 
+
+```python
+from transmorph.models import EmbedMNN
+model = EmbedMNN()
+model.transform(chen_10x)
+```
+
+Integration embedding coordinates can be gathered in each AnnData object,
+in AnnData.obsm['X_transmorph'].
+
+```python
+chen_10x['P01'].obsm['X_transmorph']
+```
+
+One can for instance use a plotting function from transmorph to display integration results.
+
+```python
+from transmorph.utils.plotting import scatter_plot
+
+scatter_plot(chen_10x, use_rep="X_transmorph")
+scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
+```
+
+## Citing transmorph
+
+If you find transmorph useful for your research, please consider citing our pre-print
+which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
+
+```bibtex
+@article{fouche2022transmorph,
+  title={transmorph: a unifying computational framework for single-cell data integration},
+  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
+  journal={bioRxiv},
+  year={2022}
+}
+```
+
+# References
+
 [Chen 2020] [Chen, Y. P., Yin, J. H., Li, W. F., Li, H. J., Chen, D. P., Zhang, C. J., ... & Ma, J. (2020). Single-cell transcriptomics reveals regulators underlying immune cell diversity and immune subtypes associated with prognosis in nasopharyngeal carcinoma. Cell research, 30(11), 1024-1042.](https://www.nature.com/articles/s41422-020-0374-x)
```

### Comparing `transmorph-0.2.6b0/setup.py` & `transmorph-0.2.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#!/usr/bin/env python3
-
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="transmorph",
-    version="0.2.6b",
-    author="Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)",
-    author_email="aziz.fouche@curie.fr",
-    description="A unifying data integration framework.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Risitop/transmorph",
-    packages=setuptools.find_packages(where="src"),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "src"},
-    include_package_data=True,
-    install_requires=[
-        "anndata>=0.8.0",
-        "cython",
-        "igraph",
-        "leidenalg",
-        "numpy>=1.22,<1.24",
-        "pre-commit",
-        "pot",
-        "pymde",
-        "pynndescent",
-        "scanpy",
-        "sccover",
-        "scikit-learn",
-        "scipy",
-        "stabilized-ica>=2.0",
-        "umap-learn",
-    ],
-    python_requires=">=3.9",
-)
+#!/usr/bin/env python3
+
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="transmorph",
+    version="0.2.7",
+    author="Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)",
+    author_email="aziz.fouche@curie.fr",
+    description="A unifying data integration framework.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Risitop/transmorph",
+    packages=setuptools.find_packages(where="src"),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"": "src"},
+    include_package_data=True,
+    install_requires=[
+        "anndata>=0.8.0",
+        "cython",
+        "igraph",
+        "leidenalg",
+        "numpy>=1.22,<1.24",
+        "pre-commit",
+        "pot",
+        "pymde",
+        "pynndescent",
+        "scanpy",
+        "sccover",
+        "scikit-learn",
+        "scipy",
+        "stabilized-ica>=2.0",
+        "umap-learn",
+    ],
+    python_requires=">=3.9",
+)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/__init__.py` & `transmorph-0.2.7/src/transmorph/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#!/usr/bin/env python3
-
-from typing import Dict, List, Union
-
-import anndata as ad
-
-from ._logging import logger
-from ._profiling import profiler
-from ._settings import settings, use_setting
-
-__all__ = ["logger", "profiler", "settings", "use_setting"]
-
-InputType = Union[List[ad.AnnData], Dict[str, ad.AnnData]]
-
-
-def check_input_transmorph(datasets: InputType) -> None:
-    # Simple input type checker for now
-    # May be enhanced in the future
-    if isinstance(datasets, List):
-        assert all(isinstance(item, ad.AnnData) for item in datasets)
-    elif isinstance(datasets, Dict):
-        assert all(
-            isinstance(key, str) and isinstance(value, ad.AnnData)
-            for (key, value) in datasets.items()
-        )
-    else:
-        raise TypeError(f"Unknown input type: {datasets.__type__}.")
+#!/usr/bin/env python3
+
+from typing import Dict, List, Union
+
+import anndata as ad
+
+from ._logging import logger
+from ._profiling import profiler
+from ._settings import settings, use_setting
+
+__all__ = ["logger", "profiler", "settings", "use_setting"]
+
+InputType = Union[List[ad.AnnData], Dict[str, ad.AnnData]]
+
+
+def check_input_transmorph(datasets: InputType) -> None:
+    # Simple input type checker for now
+    # May be enhanced in the future
+    if isinstance(datasets, List):
+        assert all(isinstance(item, ad.AnnData) for item in datasets)
+    elif isinstance(datasets, Dict):
+        assert all(
+            isinstance(key, str) and isinstance(value, ad.AnnData)
+            for (key, value) in datasets.items()
+        )
+    else:
+        raise TypeError(f"Unknown input type: {datasets.__type__}.")
```

### Comparing `transmorph-0.2.6b0/src/transmorph/_logging.py` & `transmorph-0.2.7/src/transmorph/_logging.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#!/usr/bin/env python3
-
-from datetime import datetime
-
-import os
-import logging
-import random
-import string
-import sys
-
-FORBIDDEN_FILE_CHARS = '{}[]()/<>:"/\\|?*.'
-
-# Simple function that creates module global logger.
-
-
-def create_logger():
-
-    DEFAULT_LEVEL = logging.DEBUG
-
-    # create logger
-    logger = logging.getLogger(__name__)
-    logger.setLevel(DEFAULT_LEVEL)
-
-    # create formatter
-    console_formatter = logging.Formatter(
-        "%(message)s",
-    )
-    file_formatter = logging.Formatter(
-        "[%(asctime)s] %(levelname)s - %(message)s",
-    )
-
-    # create console handler, file handler and set level to debug
-    ch = logging.StreamHandler(sys.stdout)
-    ch.setLevel(logging.INFO)
-    ch.setFormatter(console_formatter)
-
-    # add ch to logger
-    logger.addHandler(ch)
-
-    log_dir_path = f"{os.path.dirname(__file__)}/logs/"
-    if not os.path.exists(log_dir_path):
-        os.mkdir(log_dir_path)
-    randstr = "".join(random.choices(string.ascii_letters, k=10))
-    file_name = f"{datetime.now()}_{randstr}"
-    for c in FORBIDDEN_FILE_CHARS:
-        file_name = file_name.replace(c, "_")
-    file_name = f"{file_name}.log"
-    file_path = f"{log_dir_path}{file_name}"
-    if os.path.exists(file_path):
-        os.remove(file_path)
-    fh = logging.FileHandler(file_path)
-    fh.setLevel(DEFAULT_LEVEL)
-    fh.setFormatter(file_formatter)
-    logger.addHandler(fh)
-
-    logger.debug("Logger initialized.")
-
-    return logger
-
-
-logger = create_logger()
+#!/usr/bin/env python3
+
+from datetime import datetime
+
+import os
+import logging
+import random
+import string
+import sys
+
+FORBIDDEN_FILE_CHARS = '{}[]()/<>:"/\\|?*.'
+
+# Simple function that creates module global logger.
+
+
+def create_logger():
+
+    DEFAULT_LEVEL = logging.DEBUG
+
+    # create logger
+    logger = logging.getLogger(__name__)
+    logger.setLevel(DEFAULT_LEVEL)
+
+    # create formatter
+    console_formatter = logging.Formatter(
+        "%(message)s",
+    )
+    file_formatter = logging.Formatter(
+        "[%(asctime)s] %(levelname)s - %(message)s",
+    )
+
+    # create console handler, file handler and set level to debug
+    ch = logging.StreamHandler(sys.stdout)
+    ch.setLevel(logging.INFO)
+    ch.setFormatter(console_formatter)
+
+    # add ch to logger
+    logger.addHandler(ch)
+
+    log_dir_path = f"{os.path.dirname(__file__)}/logs/"
+    if not os.path.exists(log_dir_path):
+        os.mkdir(log_dir_path)
+    randstr = "".join(random.choices(string.ascii_letters, k=10))
+    file_name = f"{datetime.now()}_{randstr}"
+    for c in FORBIDDEN_FILE_CHARS:
+        file_name = file_name.replace(c, "_")
+    file_name = f"{file_name}.log"
+    file_path = f"{log_dir_path}{file_name}"
+    if os.path.exists(file_path):
+        os.remove(file_path)
+    fh = logging.FileHandler(file_path)
+    fh.setLevel(DEFAULT_LEVEL)
+    fh.setFormatter(file_formatter)
+    logger.addHandler(fh)
+
+    logger.debug("Logger initialized.")
+
+    return logger
+
+
+logger = create_logger()
```

### Comparing `transmorph-0.2.6b0/src/transmorph/_settings.py` & `transmorph-0.2.7/src/transmorph/_settings.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-#!/usr/bin/env python3
-
-import logging
-
-from numpy.random.mtrand import RandomState
-from sklearn.utils import check_random_state
-from typing import Any, Dict, Literal, Optional, TypeVar
-
-from ._logging import logger
-from .utils.misc import assert_type
-
-T = TypeVar("T")
-
-
-def use_setting(value: Optional[T], setting: T) -> T:
-    """
-    If value is None, returns setting, otherwise returns value.
-    """
-    if value is None:
-        return setting
-    return value
-
-
-class TransmorphSettings:
-    """
-    Settings manager.
-    TODO check all settings that are at risk
-    TODO update random generation numpy
-    """
-
-    def __init__(self):
-
-        # Logging
-        self._logging_level_console: int = logging.INFO
-        self._logging_level_file: int = logging.DEBUG
-        self.logging_level_console = self._logging_level_console
-        self.logging_level_file = self._logging_level_file
-
-        # General
-        self.global_random_seed: int = 42
-
-        # Neighbors
-        self._n_neighbors_max_init: int = 50
-        self._n_neighbors_max: int = self._n_neighbors_max_init
-        self._neighbors_algorithm: Literal["auto", "sklearn", "nndescent"] = "auto"
-        self.neighbors_metric: str = "sqeuclidean"
-        self._neighbors_metric_kwargs: Dict[str, Any] = {}
-        self._neighbors_n_pcs: int = 15
-        self.neighbors_random_seed: int = 42
-
-        # UMAP
-        self.umap_metric: str = "euclidean"
-        self.umap_metric_kwargs: Dict[str, Any] = {}
-        self.umap_min_dist: float = 0.5
-        self.umap_spread: float = 1.0
-        self.umap_maxiter: Optional[int] = None  # Automatic chhoice
-        self.umap_alpha: float = 1.0
-        self.umap_gamma: float = 1.0
-        self.umap_negative_sample_rate: int = 5
-        self.umap_a: Optional[float] = None
-        self.umap_b: Optional[float] = None
-        self.umap_random_state: RandomState = check_random_state(
-            self.global_random_seed
-        )
-        self.umap_n_neighbors: int = 15
-
-        # MDE
-        self.mde_initialization: str = "quadratic"
-        self.mde_repulsive_fraction: float = 1.0
-        self.mde_device: Literal["cpu", "cuda"] = "cpu"
-
-        # Scale
-        self.small_dataset_threshold: int = 100
-        self.large_dataset_threshold: int = 4096
-        self.low_dimensional_threshold: int = 5
-        self.high_dimensional_threshold: int = 60
-        self.large_number_edges: int = 10_000_000
-        self.low_features_ratio_threshold: float = 0.005
-        self.is_discrete_unique_thr: int = 50
-        self.vertexcover_n_neighbors: int = 5
-
-        # End
-        logger.debug("Transmorph settings initialized.")
-
-    @property
-    def logging_level_file(self) -> int:
-        return self._logging_level_file
-
-    @logging_level_file.setter
-    def logging_level_file(self, value: int) -> None:
-        logger.debug(f"Changing console logging level to {value}.")
-        assert_type(value, int)
-        if value < min(self._logging_level_file, self._logging_level_console):
-            logger.setLevel(value)
-        self._logging_level_file = value
-        for handler in logger.handlers:
-            if type(handler) is logging.StreamHandler:
-                handler.setLevel(self._logging_level_console)
-            if type(handler) is logging.FileHandler:
-                handler.setLevel(self._logging_level_file)
-
-    @property
-    def logging_level_console(self) -> int:
-        return self._logging_level_console
-
-    @logging_level_console.setter
-    def logging_level_console(self, value: int) -> None:
-        logger.debug(f"Changing console logging level to {value}.")
-        assert_type(value, int)
-        if value < min(self._logging_level_file, self._logging_level_console):
-            logger.setLevel(value)
-        self._logging_level_console = value
-        for handler in logger.handlers:
-            if type(handler) is logging.StreamHandler:
-                handler.setLevel(self._logging_level_console)
-            if type(handler) is logging.FileHandler:
-                handler.setLevel(self._logging_level_file)
-
-    @property
-    def verbose(self) -> str:
-        if self.logging_level_console <= logging.DEBUG:
-            return "DEBUG"
-        if self.logging_level_console <= logging.INFO:
-            return "INFO"
-        if self.logging_level_console <= logging.WARNING:
-            return "WARNING"
-        return "ERROR"
-
-    @verbose.setter
-    def verbose(self, level: Literal["DEBUG", "INFO", "WARNING", "ERROR"]) -> None:
-        if level == "DEBUG":
-            int_level = logging.DEBUG
-        elif level == "INFO":
-            int_level = logging.INFO
-        elif level == "WARNING":
-            int_level = logging.WARNING
-        elif level == "ERROR":
-            int_level = logging.ERROR
-        else:
-            raise ValueError(
-                level,
-                f"Unknown verbose level {level}. Available options are "
-                "'DEBUG', 'INFO', 'WARNING' or 'ERROR'.",
-            )
-        self.logging_level_console = int_level
-
-    @property
-    def n_neighbors_max(self) -> int:
-        return self._n_neighbors_max
-
-    @n_neighbors_max.setter
-    def n_neighbors_max(self, n: int) -> None:
-        n = int(n)
-        assert n > 0, f"Invalid number of neighbors {n}"
-        self._n_neighbors_max = n
-
-    @property
-    def neighbors_algorithm(self) -> Literal["auto", "sklearn", "nndescent"]:
-        return self._neighbors_algorithm
-
-    @neighbors_algorithm.setter
-    def neighbors_algorithm(
-        self, algorithm: Literal["auto", "sklearn", "nndescent"]
-    ) -> None:
-        assert algorithm in ("auto", "sklearn", "nndescent")
-        self._neighbors_algorithm = algorithm
-
-    @property
-    def neighbors_metric_kwargs(self) -> Dict:
-        return self._neighbors_metric_kwargs
-
-    @neighbors_metric_kwargs.setter
-    def neighbors_metric_kwargs(self, kwargs: Optional[Dict]) -> None:
-        if kwargs is None:
-            kwargs = {}
-        assert isinstance(kwargs, Dict)
-        self._neighbors_metric_kwargs = kwargs
-
-    @property
-    def neighbors_n_pcs(self) -> int:
-        return self._neighbors_n_pcs
-
-    @neighbors_n_pcs.setter
-    def neighbors_n_pcs(self, n: int) -> None:
-        n = int(n)
-        assert n > 0, f"Invalid number of pcs {n}."
-        self._neighbors_n_pcs = n
-
-
-settings = TransmorphSettings()
+#!/usr/bin/env python3
+
+import logging
+
+from numpy.random.mtrand import RandomState
+from sklearn.utils import check_random_state
+from typing import Any, Dict, Literal, Optional, TypeVar
+
+from ._logging import logger
+from .utils.misc import assert_type
+
+T = TypeVar("T")
+
+
+def use_setting(value: Optional[T], setting: T) -> T:
+    """
+    If value is None, returns setting, otherwise returns value.
+    """
+    if value is None:
+        return setting
+    return value
+
+
+class TransmorphSettings:
+    """
+    Settings manager.
+    TODO check all settings that are at risk
+    TODO update random generation numpy
+    """
+
+    def __init__(self):
+
+        # Logging
+        self._logging_level_console: int = logging.INFO
+        self._logging_level_file: int = logging.DEBUG
+        self.logging_level_console = self._logging_level_console
+        self.logging_level_file = self._logging_level_file
+
+        # General
+        self.global_random_seed: int = 42
+
+        # Neighbors
+        self._n_neighbors_max_init: int = 50
+        self._n_neighbors_max: int = self._n_neighbors_max_init
+        self._neighbors_algorithm: Literal["auto", "sklearn", "nndescent"] = "auto"
+        self.neighbors_metric: str = "sqeuclidean"
+        self._neighbors_metric_kwargs: Dict[str, Any] = {}
+        self._neighbors_n_pcs: int = 15
+        self.neighbors_random_seed: int = 42
+
+        # UMAP
+        self.umap_metric: str = "euclidean"
+        self.umap_metric_kwargs: Dict[str, Any] = {}
+        self.umap_min_dist: float = 0.5
+        self.umap_spread: float = 1.0
+        self.umap_maxiter: Optional[int] = None  # Automatic chhoice
+        self.umap_alpha: float = 1.0
+        self.umap_gamma: float = 1.0
+        self.umap_negative_sample_rate: int = 5
+        self.umap_a: Optional[float] = None
+        self.umap_b: Optional[float] = None
+        self.umap_random_state: RandomState = check_random_state(
+            self.global_random_seed
+        )
+        self.umap_n_neighbors: int = 15
+
+        # MDE
+        self.mde_initialization: str = "quadratic"
+        self.mde_repulsive_fraction: float = 1.0
+        self.mde_device: Literal["cpu", "cuda"] = "cpu"
+
+        # Scale
+        self.small_dataset_threshold: int = 100
+        self.large_dataset_threshold: int = 4096
+        self.low_dimensional_threshold: int = 5
+        self.high_dimensional_threshold: int = 60
+        self.large_number_edges: int = 10_000_000
+        self.low_features_ratio_threshold: float = 0.005
+        self.is_discrete_unique_thr: int = 50
+        self.vertexcover_n_neighbors: int = 5
+
+        # End
+        logger.debug("Transmorph settings initialized.")
+
+    @property
+    def logging_level_file(self) -> int:
+        return self._logging_level_file
+
+    @logging_level_file.setter
+    def logging_level_file(self, value: int) -> None:
+        logger.debug(f"Changing console logging level to {value}.")
+        assert_type(value, int)
+        if value < min(self._logging_level_file, self._logging_level_console):
+            logger.setLevel(value)
+        self._logging_level_file = value
+        for handler in logger.handlers:
+            if type(handler) is logging.StreamHandler:
+                handler.setLevel(self._logging_level_console)
+            if type(handler) is logging.FileHandler:
+                handler.setLevel(self._logging_level_file)
+
+    @property
+    def logging_level_console(self) -> int:
+        return self._logging_level_console
+
+    @logging_level_console.setter
+    def logging_level_console(self, value: int) -> None:
+        logger.debug(f"Changing console logging level to {value}.")
+        assert_type(value, int)
+        if value < min(self._logging_level_file, self._logging_level_console):
+            logger.setLevel(value)
+        self._logging_level_console = value
+        for handler in logger.handlers:
+            if type(handler) is logging.StreamHandler:
+                handler.setLevel(self._logging_level_console)
+            if type(handler) is logging.FileHandler:
+                handler.setLevel(self._logging_level_file)
+
+    @property
+    def verbose(self) -> str:
+        if self.logging_level_console <= logging.DEBUG:
+            return "DEBUG"
+        if self.logging_level_console <= logging.INFO:
+            return "INFO"
+        if self.logging_level_console <= logging.WARNING:
+            return "WARNING"
+        return "ERROR"
+
+    @verbose.setter
+    def verbose(self, level: Literal["DEBUG", "INFO", "WARNING", "ERROR"]) -> None:
+        if level == "DEBUG":
+            int_level = logging.DEBUG
+        elif level == "INFO":
+            int_level = logging.INFO
+        elif level == "WARNING":
+            int_level = logging.WARNING
+        elif level == "ERROR":
+            int_level = logging.ERROR
+        else:
+            raise ValueError(
+                level,
+                f"Unknown verbose level {level}. Available options are "
+                "'DEBUG', 'INFO', 'WARNING' or 'ERROR'.",
+            )
+        self.logging_level_console = int_level
+
+    @property
+    def n_neighbors_max(self) -> int:
+        return self._n_neighbors_max
+
+    @n_neighbors_max.setter
+    def n_neighbors_max(self, n: int) -> None:
+        n = int(n)
+        assert n > 0, f"Invalid number of neighbors {n}"
+        self._n_neighbors_max = n
+
+    @property
+    def neighbors_algorithm(self) -> Literal["auto", "sklearn", "nndescent"]:
+        return self._neighbors_algorithm
+
+    @neighbors_algorithm.setter
+    def neighbors_algorithm(
+        self, algorithm: Literal["auto", "sklearn", "nndescent"]
+    ) -> None:
+        assert algorithm in ("auto", "sklearn", "nndescent")
+        self._neighbors_algorithm = algorithm
+
+    @property
+    def neighbors_metric_kwargs(self) -> Dict:
+        return self._neighbors_metric_kwargs
+
+    @neighbors_metric_kwargs.setter
+    def neighbors_metric_kwargs(self, kwargs: Optional[Dict]) -> None:
+        if kwargs is None:
+            kwargs = {}
+        assert isinstance(kwargs, Dict)
+        self._neighbors_metric_kwargs = kwargs
+
+    @property
+    def neighbors_n_pcs(self) -> int:
+        return self._neighbors_n_pcs
+
+    @neighbors_n_pcs.setter
+    def neighbors_n_pcs(self, n: int) -> None:
+        n = int(n)
+        assert n > 0, f"Invalid number of pcs {n}."
+        self._neighbors_n_pcs = n
+
+
+settings = TransmorphSettings()
```

### Comparing `transmorph-0.2.6b0/src/transmorph/datasets/__init__.py` & `transmorph-0.2.7/src/transmorph/datasets/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#!/usr/bin/env python3
-
-from .databank_api import check_files
-from .datasets import load_bank
-from .datasets import remove_bank
-
-from .datasets import load_chen_10x
-from .datasets import load_cell_cycle
-from .datasets import load_pal_10x
-from .datasets import load_spirals
-from .datasets import load_test_datasets_random
-from .datasets import load_test_datasets_small
-from .datasets import load_travaglini_10x
-from .datasets import load_zhou_10x
-
-__all__ = [
-    "check_files",
-    "load_bank",
-    "remove_bank",
-    "load_spirals",
-    "load_test_datasets_random",
-    "load_test_datasets_small",
-    "load_cell_cycle",
-    "load_chen_10x",
-    "load_pal_10x",
-    "load_travaglini_10x",
-    "load_zhou_10x",
-]
+#!/usr/bin/env python3
+
+from .databank_api import check_files
+from .datasets import load_bank
+from .datasets import remove_bank
+
+from .datasets import load_chen_10x
+from .datasets import load_cell_cycle
+from .datasets import load_pal_10x
+from .datasets import load_spirals
+from .datasets import load_test_datasets_random
+from .datasets import load_test_datasets_small
+from .datasets import load_travaglini_10x
+from .datasets import load_zhou_10x
+
+__all__ = [
+    "check_files",
+    "load_bank",
+    "remove_bank",
+    "load_spirals",
+    "load_test_datasets_random",
+    "load_test_datasets_small",
+    "load_cell_cycle",
+    "load_chen_10x",
+    "load_pal_10x",
+    "load_travaglini_10x",
+    "load_zhou_10x",
+]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralA.csv` & `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralA.csv`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,433 +1,433 @@
-4.395250595036668706e+00,-4.322663868386681152e+00,-4.971164226449628742e+00
-5.464502063414679256e+00,-4.440635391753692041e+00,-5.655311415943845788e+00
-4.816082401592716167e+00,-3.760850775547923242e+00,-6.244057362492451801e+00
-4.745651181664434226e+00,-3.520985471737261285e+00,-6.425287235864297841e+00
-5.143417018105640892e+00,-3.769231601723258329e+00,-6.667001493987497085e+00
-4.682671393843319763e+00,-4.214836713990881556e+00,-7.263347824176770828e+00
-4.632631213160046002e+00,-3.244833835867647842e+00,-7.118236051895419969e+00
-4.031937727141903238e+00,-3.680862188183487760e+00,-6.577724542069433689e+00
-3.773553551336611633e+00,-4.709611143852578508e+00,-7.092710208142162465e+00
-6.035645899548843119e+00,-4.157390994574154952e+00,-4.537637138422331518e+00
-4.441820081212016547e+00,-3.757077437121850938e+00,-5.377318270987054838e+00
-4.019996924716306097e+00,-3.595435894698909784e+00,-7.472054943412725692e+00
-4.546973880381376176e+00,-4.705362330457607989e+00,-7.168970149921851664e+00
-4.218853456840061078e+00,-4.004649112098787711e+00,-5.689728936182667951e+00
-5.094352674240221646e+00,-3.312716352726931213e+00,-6.448881632377177375e+00
-4.976689714674379594e+00,-3.460792155550518334e+00,-5.736484596831427751e+00
-5.593090830375377465e+00,-3.677049303093503418e+00,-6.478883997405122663e+00
-3.743942389505838353e+00,-4.978315239030565387e+00,-6.382412467092967390e+00
-4.719851067643378251e+00,-3.564997910544921211e+00,-6.930491281523351255e+00
-3.509042320998985609e+00,-4.075031457567797055e+00,-7.529789903700861764e+00
-4.422154513908088447e+00,-4.073047695107685051e+00,-5.770936423537373017e+00
-5.903061369353857835e+00,-3.333470887820057182e+00,-5.149531069211041867e+00
-5.320061273013488190e+00,-4.900966278643878127e+00,-6.011214688346447232e+00
-4.386030844677042850e+00,-4.362466414500863365e+00,-5.867253157156456567e+00
-4.185189254387175595e+00,-4.439924987741166618e+00,-7.572141142042074335e+00
-4.942030220319173495e+00,-3.463824980279692323e+00,-5.902864229833759246e+00
-3.668413359819459707e+00,-4.546183564105624519e+00,-6.910565031961458438e+00
-5.311832290371190979e+00,-3.477423392958457704e+00,-6.355732706688390188e+00
-1.001623244718298089e+01,-1.248338026820153601e+01,-6.975115843194810594e+00
-9.746047524311890697e+00,-1.234602955463430973e+01,-5.789917664650237050e+00
-1.226313539578390355e+01,-1.221788971161849702e+01,-1.049925018831972245e+01
-1.074858711255845733e+01,-1.319460832729752298e+01,-7.044217943157934592e+00
-9.510610972292333543e+00,-1.053218118160822669e+01,-3.191987672990745928e+00
-1.075556831488009557e+01,-1.380605656435415085e+01,-9.681023588688230319e+00
-1.239984239604647520e+01,-1.130425900231670333e+01,-1.490606197102359332e+01
-9.886284250200747081e+00,-1.346505253961593240e+01,-7.480705471248404237e+00
-9.343375845911809918e+00,-1.118841666220255959e+01,-3.363274088290253427e+00
-9.173719526831138893e+00,-1.080471664309665947e+01,-4.572699446149313118e+00
-9.410657408812545199e+00,-1.245168042356199578e+01,-5.759540231959079826e+00
-1.036319024552942025e+01,-1.317108591702204201e+01,-7.002380547205122596e+00
-1.082365444353933093e+01,-1.282800038362785955e+01,-6.366720032462955814e+00
-9.812859452446542008e+00,-1.290800079730089500e+01,-7.656748215638626398e+00
-7.499149414234647537e+00,-7.769221077547984855e+00,-2.504820919063063478e+00
-1.141153828109480806e+01,-1.314418961705730915e+01,-1.032553736258267740e+01
-1.095853923999918678e+01,-1.298491757987332917e+01,-6.768323379190671396e+00
-8.672724450648097161e+00,-1.013328436035949665e+01,-3.128271773883745333e+00
-1.032622464401251605e+01,-1.310220476518617438e+01,-9.081164192728834905e+00
-9.889109234781914282e+00,-1.270394120633862656e+01,-4.065018695329629672e+00
-9.815268076722158952e+00,-1.295616014137147864e+01,-6.239129368279058951e+00
-8.892292357825327898e+00,-9.288905949172741927e+00,-3.551138605407810900e+00
-8.975744294190628025e+00,-9.295787711290845579e+00,-3.513719809478732969e+00
-8.379909104901010153e+00,-8.635166578746488852e+00,-1.879361369055306596e+00
-9.762884571397854927e+00,-1.023836563220016060e+01,-3.398738455820169868e+00
-8.731284177973209992e+00,-9.293783176422163450e+00,-2.766092812813486290e+00
-7.899911251126299661e+00,-9.506823880050692566e+00,-2.604402749314255416e+00
-9.731959157140854799e+00,-1.034000968358193795e+01,-3.435779939702835684e+00
-1.035719926870322105e+01,-1.308235357102338092e+01,-9.341539860265154260e+00
-7.654682114372681312e+00,-4.330253356305346912e+00,-2.987674829030328105e+00
-9.306203420390966485e+00,-1.406702220181735541e+01,-9.150251498175723697e+00
-1.014911150048022215e+01,-1.265435780392008169e+01,-6.247722507453955743e+00
-1.003190093143867401e+01,-1.299324923292024891e+01,-7.279288219316636166e+00
-9.011463401155614505e+00,-1.234406573494549875e+01,-4.987416593295200151e+00
-9.747876515955013588e+00,-1.356929033495655901e+01,-6.281615324604515216e+00
-1.095873265490255299e+01,-1.341215311515254527e+01,-8.072667583212597364e+00
-1.023313390484863561e+01,-1.285195814961189242e+01,-5.003435992934814891e+00
-9.560415276819307806e+00,-1.176390953557082852e+01,-4.840284594763478054e+00
-8.726491126080192728e+00,-1.064016230571775878e+01,-4.204087355889096322e+00
-8.746381188116510330e+00,-9.181624294424377553e+00,-3.095571632160803333e+00
-9.073694019185431614e+00,-1.041293984221182711e+01,-2.761047322707135265e+00
-9.080828775841769840e+00,-1.157967794373984205e+01,-4.875282134119531818e+00
-9.705168846735871213e+00,-1.395160253636398906e+01,-6.953602487585388126e+00
-1.060893835564072596e+01,-1.358143196579211320e+01,-7.331515016952955044e+00
-8.890633788856165509e+00,-8.549841352690226159e+00,-3.102810717366640603e+00
-7.689708342648051698e+00,-8.317816779351453249e+00,-3.673782492687565071e+00
-1.036648116944628306e+01,-1.273110720850786315e+01,-6.776974019740150013e+00
-1.036250513551251196e+01,-1.348174618267534264e+01,-7.813690311801156696e+00
-8.608686267366518763e+00,-8.401086558886060374e+00,-1.751645182339836460e+00
-1.021449314462090463e+01,-1.176300229511189599e+01,-7.094474648682265183e+00
-7.286065623640102018e+00,-6.371821818146274907e+00,-1.963986481598901435e+00
-9.650406516947663604e+00,-1.358609338205300787e+01,-8.632143621637300868e+00
-1.050290508583148430e+01,-1.292288438371390846e+01,-6.801667227988794195e+00
-1.017972627467378111e+01,-1.184768388328544653e+01,-4.764489523859370301e+00
-7.696346386977783283e+00,-5.832091720334171114e+00,-3.305916269236620408e+00
-8.972799883575337532e+00,-1.086033415740480201e+01,-3.077954171257880844e+00
-8.292488182000942842e+00,-8.704818157236919873e+00,-2.845082799917594940e+00
-1.107841080136359579e+01,-1.316655456044676242e+01,-9.302312517386928548e+00
-9.745359465449064729e+00,-1.231529300361775725e+01,-5.028936417917496904e+00
-8.478809339834770142e+00,-1.221600989547063065e+01,-4.459622869527334998e+00
-8.852500263772505207e+00,-9.007977612217839436e+00,-2.457086525620048256e+00
-7.551587982240722141e+00,-7.390924712159323562e+00,-2.465509969589359862e+00
-8.404382709847265431e+00,-8.736907374221489775e+00,-2.929705380523430769e+00
-1.005639414966485390e+01,-1.177873343078086066e+01,-5.837812672238696265e+00
-8.925463857406237267e+00,-9.788086679139645696e+00,-2.830254610270173110e+00
-1.032757821120249986e+01,-1.329956219406319207e+01,-7.851523401458935680e+00
-1.081958776732908412e+01,-1.320603629163440473e+01,-7.784668722969446897e+00
-7.584698305368953619e+00,-6.144443995298825456e+00,-1.964060351459080422e+00
-1.422440566345288104e+01,6.664656239356148149e-01,-1.748458449632873624e+01
-1.209211895314341945e+01,-1.395198990754988166e+01,-1.294512112936691572e+01
-1.204484132896206461e+01,-1.162847258283540697e+01,-1.349147052379273504e+01
-1.363309817471195196e+01,-4.690118982502275990e+00,-1.812698810422864426e+01
-1.321794691948816691e+01,-4.725842437851797584e+00,-1.682453206547122448e+01
-1.330138311704246235e+01,-1.028332373266535171e+01,-1.554599597718006798e+01
-1.299794660769330967e+01,-7.629650725764824060e+00,-1.740075707863643473e+01
-1.273508492167364636e+01,-9.940554485766080361e+00,-1.687214661600456367e+01
-1.211301819494347676e+01,-9.803996791212910011e+00,-1.601748581960441697e+01
-1.411067780523191573e+01,-6.565823475510969232e+00,-1.747617407053593297e+01
-1.251930561918896245e+01,-1.037615327945981392e+01,-1.695316723643325929e+01
-1.337049379021845574e+01,-4.944629667103464854e+00,-1.830385006109548485e+01
-1.591512523181550698e+01,5.230776523220260543e+00,-1.395055095972282544e+01
-1.343853436334039309e+01,-6.169476090609759211e+00,-1.829381003312731835e+01
-1.144814910437605704e+01,-1.352699163364047052e+01,-1.254816379143971261e+01
-1.452156408138628230e+01,3.224544127597482657e+00,-1.594468183501004610e+01
-1.443563928508468130e+01,-5.256380644623710019e+00,-1.760902093339744567e+01
-1.332207393146289043e+01,-2.036763707876132479e+00,-1.813326373217121557e+01
-1.382034832759745413e+01,-9.523074623212330891e+00,-1.564110570520793786e+01
-1.697481318573218800e+01,7.377017130819920609e+00,-9.281558563274238338e+00
-1.450597355019188939e+01,-3.837366278349945148e-01,-1.773154640754879807e+01
-1.314741597332643330e+01,-9.921472000309114136e+00,-1.463081694245978603e+01
-1.327433790167815353e+01,-2.337707503980743784e+00,-1.764863409683201922e+01
-1.515566226815671769e+01,3.235122009065914739e+00,-1.481951957903419625e+01
-1.283737809678832242e+01,-2.311194451897040647e+00,-1.803706541334578972e+01
-1.234507040648451692e+01,-1.148583282998043842e+01,-1.533048188863032735e+01
-1.403451864582015851e+01,-1.267330320629449503e+00,-1.723929668751237188e+01
-1.474395624404557736e+01,-3.509430616015811744e+00,-1.728353234207030908e+01
-1.312169581312165079e+01,-9.411084323360272563e+00,-1.660377278613343321e+01
-1.359355967399659981e+01,-1.791061369903209410e+00,-1.777786262748419688e+01
-1.298412052647757164e+01,-2.763773284403350239e+00,-1.864495588837796092e+01
-1.317564493368682577e+01,-1.099327049626182351e+01,-1.464418637422346592e+01
-1.331745860998589848e+01,-8.064170655338038785e+00,-1.815350606072040307e+01
-1.355490971140668144e+01,-3.668129628788647345e+00,-1.832575302085016489e+01
-1.341095543126219347e+01,-4.961370215759112412e+00,-1.727950749131285590e+01
-1.264544633259677830e+01,-6.238205236825889344e+00,-1.817043066121454586e+01
-1.304202522351826588e+01,-6.879516322041464349e+00,-1.763172217221836036e+01
-1.575372210259419070e+01,4.080489382037058022e+00,-1.550889800616303305e+01
-1.537214912549692158e+01,-4.023603523606151811e-01,-1.746618064396603387e+01
-1.468408596455508075e+01,-2.625262897804098383e+00,-1.699519195835906515e+01
-1.312348314911815983e+01,-8.586081965252796877e+00,-1.738837114416729435e+01
-1.262910586730866136e+01,-8.017866084688479944e+00,-1.703836248750851468e+01
-1.318401386994887758e+01,-5.143580711668401584e+00,-1.798946595460883913e+01
-1.254640900037620987e+01,-1.056878074382554189e+01,-1.533491670084033487e+01
-1.343770705135055721e+01,-6.812979909137673928e+00,-1.671265705755998709e+01
-1.255803812816796494e+01,-7.455408298691825308e+00,-1.742909843203369036e+01
-1.348884091460585211e+01,-5.765244663718104512e+00,-1.791441140443311753e+01
-1.428738527618931187e+01,1.556954878466595638e+00,-1.621523939145270532e+01
-1.351775878796965102e+01,-5.594088880809534814e+00,-1.834285377690882513e+01
-1.611132058850679982e+01,6.498543498196390544e+00,-1.199151710443942065e+01
-1.349940600515696154e+01,-6.258622569360970722e+00,-1.855021026627498770e+01
-1.322244988555497613e+01,-4.926268960892255855e+00,-1.685851868531270270e+01
-1.222177694201315923e+01,-9.053669666924420767e+00,-1.647987719247205618e+01
-1.458139982567740311e+01,-1.952750151131201761e+00,-1.817565637156737424e+01
-1.341255883800023874e+01,-3.097450718804315883e+00,-1.810340359212710482e+01
-1.440645453089172356e+01,2.211809790966401401e+00,-1.645264590932757542e+01
-1.193712862849979395e+01,-1.237945226200528381e+01,-1.368758206877894779e+01
-1.344127888533262549e+01,-4.377598654834610414e+00,-1.774819447180508902e+01
-1.317996302654562868e+01,-3.435345037556910786e+00,-1.757230974893919040e+01
-1.324898388668255045e+01,-7.165296665602514992e+00,-1.757765736519312583e+01
-1.342264739909429139e+01,-6.417527470248162835e+00,-1.860949410960960648e+01
-1.415539414286176623e+01,-2.918455349646705610e+00,-1.771344456362243847e+01
-1.317446839640384937e+01,-7.492185523074960329e+00,-1.658202177203352790e+01
-1.448469370495780240e+01,-3.135307771920590625e+00,-1.797651706441067887e+01
-1.528632568923078594e+01,4.685376883141234572e-01,-1.756151374331199833e+01
-1.227591044291007272e+01,-8.495114336733308846e+00,-1.711757562905923180e+01
-1.281750921075058791e+01,-8.040507294391296966e+00,-1.658582407193567221e+01
-1.245587464923643140e+01,-9.112571815236742978e+00,-1.730381438582104536e+01
-1.308926519824433754e+01,-7.451609674566151753e+00,-1.718920625486549625e+01
-1.645339418036515511e+01,7.382402687410285935e+00,-8.055091957390105861e+00
-1.656130476323728473e+01,7.479945989958263652e+00,-4.771677738454028983e+00
-1.661159484078974202e+01,8.097991079647375301e+00,-6.465974489448926832e+00
-1.694291363943615281e+01,7.938854924583669259e+00,-7.847019998962207588e+00
-1.705225493000251191e+01,8.273509580004388297e+00,-1.361801206319779745e+00
-1.592938542207729569e+01,5.861336844134489965e+00,-1.214191842613768380e+01
-1.632910661010952680e+01,8.804393876988289236e+00,-7.683946025594213580e+00
-1.585688555003061673e+01,8.823898454780499279e+00,-8.356045527166315878e+00
-1.404854614045483707e+01,-1.136973744008778375e+00,-1.782355206906638756e+01
-1.526535454391915714e+01,4.010538256846770011e+00,-1.451808590613034156e+01
-1.628659704246933515e+01,8.125295050890519732e+00,-8.314708226918344991e+00
-1.511479068472412379e+01,1.882088579887041924e+00,-1.644778803870357109e+01
-1.495400752484361107e+01,3.707654153524119423e+00,-1.489813925229233504e+01
-1.478930752003110349e+01,1.317740685608417728e+00,-1.690696819234760184e+01
-1.529173688776298334e+01,3.561915542459212602e+00,-1.581242245822763337e+01
-1.496910459162500118e+01,2.322187324756086468e-01,-1.695158903731445577e+01
-1.545219032234885326e+01,6.152730637187238116e+00,-1.247006494917788011e+01
-1.469145396954023397e+01,5.804330906336597096e+00,-1.309378413726908974e+01
-1.898788199784210562e+01,3.249560630185005294e+00,6.549281091303999602e+00
-1.571745465000396358e+01,2.237991282801172765e+00,-1.658722738839586697e+01
-1.511211284714100778e+01,1.127179634406377140e+00,-1.634529718745005411e+01
-1.539159575365048305e+01,6.937204305012953043e+00,-9.737695414897025614e+00
-1.807303515510734115e+01,4.757333386504440043e+00,3.957251423163308246e+00
-1.449158744148847866e+01,2.235837840250619379e+00,-1.675064609885996703e+01
-1.598771362217022762e+01,3.034584031342285826e+00,-1.538150885381962851e+01
-1.703702886188433041e+01,7.593521459021800979e+00,-1.262652376700381218e+00
-1.664789048431876495e+01,5.311025222618292574e+00,-1.426980047872935486e+01
-1.371936884998051909e+01,-4.664727020653710809e+00,-1.849533287710204377e+01
-1.676063811616221244e+01,9.878484513517387100e+00,-5.530127405782879535e+00
-1.511243535088700263e+01,4.566260339784321332e+00,-1.544922096299710113e+01
-1.684106044393793056e+01,8.787266912708210143e+00,-8.342009331795241067e+00
-1.506406276008835476e+01,5.867327091263700112e+00,-1.265316389733326119e+01
-1.546005539070945822e+01,7.108617947282439786e+00,-1.037810164161595061e+01
-1.638855564010735932e+01,6.065515949846437493e+00,-1.263173412340649371e+01
-1.853910408351196537e+01,4.214139932266830257e+00,5.116620730383008464e+00
-1.695180757997870913e+01,8.132997003042978790e+00,-7.202444267408105283e+00
-1.588221573901916805e+01,7.822845931449977641e+00,-9.821593761859555016e+00
-1.753177628346295336e+01,7.735486470816946181e+00,-2.468646595444683456e-01
-1.606867984753119671e+01,7.375700469287286509e+00,-1.106474944992303833e+01
-1.757863109350234510e+01,8.159362234680092030e+00,-8.418207623032834874e+00
-1.665412346818128952e+01,6.972634802158150791e+00,-9.887193189253990155e+00
-1.387542776782413867e+01,-3.206430777412592636e+00,-1.765501849252107291e+01
-1.668059461885076544e+01,8.881794620201031165e+00,-7.048970183217672769e+00
-1.469444031165007480e+01,1.969431270613339002e+00,-1.568862868881986827e+01
-1.594874492905061025e+01,7.779895227922397183e+00,-1.010928068288663084e+01
-1.436786482048101732e+01,1.530434859106996726e+00,-1.584429547932200677e+01
-1.638237963118461948e+01,8.192414124659862296e+00,-3.042694169529642778e+00
-1.600570520736174274e+01,4.996876052384335409e+00,-1.278601973171864081e+01
-1.616171446391154376e+01,4.091949164523896343e+00,-1.396517770926991275e+01
-1.513554289803591502e+01,1.484084610712073982e+00,-1.751786689080163484e+01
-1.477605331987120785e+01,-1.467919215284172019e+00,-1.780769004333539129e+01
-1.757193463550051504e+01,8.056675978082806111e+00,-5.462745008745203634e+00
-1.695380580274347082e+01,7.633945778535977666e+00,-9.355561616519098678e+00
-1.677622277187671784e+01,7.069768228772769447e+00,-1.125591046671367934e+01
-1.525526163669538349e+01,6.222541177290061398e+00,-1.263677035232336721e+01
-1.616707981912927039e+01,7.622146136872471445e+00,-8.766143078454049942e+00
-2.296359044322872833e+01,-2.316991974955748645e+01,2.071706138055439794e+00
-2.184343019210889025e+01,-2.326519724165115122e+01,2.406709435737475644e+00
-2.341798948840471084e+01,-2.512138862677182516e+01,-8.040050046342468448e+00
-2.134833938244103635e+01,-2.253114476509641406e+01,1.850427262628588920e+00
-2.112236377489577777e+01,-1.822738718336637120e+01,6.586017064502648566e+00
-2.140169601694480761e+01,-2.027269475361827844e+01,5.258768505564601625e+00
-1.877228097345865976e+01,4.982902187603093225e-01,7.916565910948589746e+00
-2.199738259802289519e+01,-2.547712281357617314e+01,-6.506855070403702257e+00
-2.160032292670828369e+01,-1.839895317118849505e+01,5.855063487398586730e+00
-2.201031494962639101e+01,-2.484870288497440072e+01,-3.029237897749075259e+00
-2.064329096048719947e+01,-1.268411298729742498e+01,9.241424582854142145e+00
-2.218532288756697213e+01,-2.290693958742515690e+01,1.052581387909075517e+00
-2.227736573802844333e+01,-1.849358102309743046e+01,6.001130968337715643e+00
-2.165757348224896006e+01,-1.870715573527809283e+01,6.652346721065390156e+00
-2.076458065493189054e+01,-1.982592446387534935e+01,5.789730045757707444e+00
-2.024448426913530952e+01,-1.574320900063249873e+01,7.229101673812197149e+00
-2.156857459526498033e+01,-2.054045176750033619e+01,4.564112079158643809e+00
-2.333440187548032441e+01,-2.595171045248289232e+01,-1.130360482477417428e+01
-2.258656528031731625e+01,-2.604504613646205513e+01,-9.408790284756381794e+00
-2.130834774661994402e+01,-2.013841735677001310e+01,4.266196272923430399e+00
-2.049663888756070307e+01,-1.571712573990078887e+01,7.501726870241967049e+00
-2.228065728292500580e+01,-2.572960754891156654e+01,-3.199480585653966092e+00
-2.120460109656314174e+01,-1.816441718402893457e+01,6.920400000318716494e+00
-2.195681766009772318e+01,-2.199529736637779109e+01,1.256915192457176644e+00
-2.201823837099016146e+01,-2.536548785460904298e+01,-7.730147302712683910e+00
-2.191232254550725500e+01,-2.262899038587625000e+01,6.268619023663628553e-01
-2.230974503566952905e+01,-2.580644757428363079e+01,-6.324530313668581982e+00
-2.142370693029285178e+01,-2.026886274530126997e+01,5.314775659652834605e+00
-1.965260860484254479e+01,-6.018209388722169706e+00,1.043062548484094343e+01
-2.121054172257165504e+01,-2.078600358730887265e+01,4.180813133424983619e+00
-2.267995853948431417e+01,-2.601352321476538521e+01,-8.216380826288411043e+00
-2.116253738932094564e+01,-1.980497517308850419e+01,5.755232310930471940e+00
-2.141267617355513408e+01,-2.238993563427020916e+01,1.512012774605178578e+00
-2.208466092280029969e+01,-2.284813441398870282e+01,1.807110938072760575e+00
-2.162322873943209345e+01,-2.016911113304284697e+01,4.060709540934650974e+00
-2.137929177206634890e+01,-2.335557217243398753e+01,-1.373994680270005375e-01
-2.022571474659641311e+01,-1.024682560613245919e+01,1.007090323086750239e+01
-2.297451970135233523e+01,-2.504358813195573674e+01,-4.359600035303495602e+00
-2.140509119621716749e+01,-2.237022054721911246e+01,1.241929891201520419e+00
-2.379048468235028935e+01,-2.184937727178267153e+01,-2.081215166065097932e+01
-2.108287713804223884e+01,-1.761971042371840213e+01,7.294940082264405490e+00
-2.267910244039433820e+01,-2.472180781042260378e+01,-2.996126791598650030e+00
-2.159433868019981517e+01,-1.989647825655822899e+01,3.684544847593317130e+00
-2.126073297645213600e+01,-1.866086985209446425e+01,6.584880764221512806e+00
-2.211698579238815654e+01,-2.384802886015779677e+01,6.796908563404846504e-01
-2.218684925429112553e+01,-1.694407942818845925e+01,6.197662542500848915e+00
-2.030683561678518956e+01,-6.426481060442648108e+00,9.596690860818073432e+00
-2.188917107351645797e+01,-2.102820621716719529e+01,3.027735236424064169e+00
-2.173271057200532752e+01,-2.382834097812880003e+01,-1.045245821052465551e+00
-2.201234834421086717e+01,-2.104728853507654307e+01,1.355780719869750683e+00
-2.345047161065107844e+01,-2.534337542845079128e+01,-1.204297824467470690e+01
-2.192101547619951418e+01,-2.389646709273769432e+01,-8.684406494161578394e-01
-2.081756794180137149e+01,-1.526137004877870673e+01,8.690106094713812013e+00
-2.043858724830730722e+01,-1.355857081852436608e+01,8.472750311409948054e+00
-2.408101567470776416e+01,-2.523692774724589327e+01,-1.267726475208434778e+01
-2.199324047807551352e+01,-1.949430300853566678e+01,5.735800194962589416e+00
-2.091441711027008310e+01,-9.437018367061078550e+00,9.608524790867077670e+00
-2.092422279781106553e+01,-8.245819367914005937e+00,1.045728452752925186e+01
-2.388671832860385535e+01,-2.608941496635303992e+01,-1.273025878016193602e+01
-2.480046511090974093e+01,-2.420636210663293753e+01,-1.484274544901062498e+01
-2.041831244763949726e+01,-1.517703690822252760e+01,8.062227306343656252e+00
-2.132962557634880696e+01,-2.225011225368936607e+01,3.363397839605919870e+00
-2.212528812501945552e+01,-2.251554071299918292e+01,-1.931815061803342282e+00
-2.040123031916628804e+01,-1.097886582435655711e+01,9.700909635296360634e+00
-2.580456151995164404e+01,-1.437712772899021729e+01,-2.691973088356861155e+01
-2.418016162138154002e+01,-2.034372992539833191e+01,-2.373874699070208294e+01
-2.393687502563621194e+01,-2.393873658027090556e+01,-1.929834210989234577e+01
-2.429105906728302955e+01,-1.358334006104800196e+01,-2.774229307970408342e+01
-2.298347278932940085e+01,-2.571218239453622090e+01,-1.226803408900074643e+01
-2.307607434424518900e+01,-2.564243564182613966e+01,-9.694602101597222799e+00
-2.364212608243864722e+01,-2.558886654877179012e+01,-1.330013287810668388e+01
-2.273562947326239225e+01,-2.529567592209023985e+01,-9.236445701190184820e+00
-2.402093827704013762e+01,-2.430611915291135006e+01,-1.663415994459370495e+01
-2.252418619017255708e+01,-2.496805946901873341e+01,-3.126407554013312051e+00
-2.319781893885000557e+01,-2.354012555635899417e+01,-1.680613288434327757e+01
-2.450553773745986064e+01,-1.619910550745199984e+01,-2.568206974882684790e+01
-2.240582474461039908e+01,-2.578463728330557814e+01,-1.004574535155576243e+01
-2.455609950178190104e+01,-1.934319529607305199e+01,-2.425350074179327464e+01
-2.436548957048902153e+01,-2.091737112472101501e+01,-2.224627098568040040e+01
-2.425362828020559292e+01,-2.469058973216790065e+01,-1.364218832111659552e+01
-2.393265836216282949e+01,-2.578288692673940830e+01,-1.214964966372184207e+01
-2.321468676588910540e+01,-2.511141645267787226e+01,-1.293161436483637949e+01
-2.279149804209653851e+01,-2.495417589318267204e+01,-1.542912035081367783e+01
-2.340089058837738634e+01,-2.456397497963765630e+01,-1.498155714379575976e+01
-2.499599307161682660e+01,-2.066441078346491622e+01,-2.423301063447068060e+01
-2.440607832674238864e+01,-2.333472725085637478e+01,-1.831131866602770586e+01
-2.328968380096867463e+01,-2.516646870521633161e+01,-1.134756100155570024e+01
-2.535871720657070938e+01,-1.953135355834352538e+01,-2.372382925460571812e+01
-2.358564076152469369e+01,-2.528010373022814861e+01,-1.320364432252458364e+01
-2.467039969914649333e+01,-2.045869131947891617e+01,-2.293463046671746497e+01
-2.154361217505673309e+01,-1.994131148479492666e+01,5.007621372466962484e+00
-2.291113835839421142e+01,-2.622646583487545513e+01,-1.041186851563811189e+01
-2.241312153973111521e+01,-2.485334868959381538e+01,-6.729881578395903396e+00
-2.372681353790398973e+01,-2.487506020013109520e+01,-1.506372714906544275e+01
-2.373518158438036352e+01,-2.526971819406776376e+01,-1.370637208755551839e+01
-2.269906081402751497e+01,-2.556912076443708060e+01,-1.094686370566043010e+01
-2.445059875153450690e+01,-2.136125882372177642e+01,-2.364691248539913460e+01
-2.272170233857012533e+01,-2.334516458696715802e+01,-5.564281986004084857e-01
-2.228236045808541022e+01,-2.374237420594234749e+01,-1.622933820191633458e+00
-2.363197545872582239e+01,-2.601905338343803464e+01,-9.118905376074529556e+00
-2.389913679633781385e+01,-2.342710545536563416e+01,-1.938059894142172013e+01
-2.466995018657652849e+01,-1.481900631176661953e+01,-2.775436768519973896e+01
-2.385976378648329188e+01,-2.433399965862594883e+01,-1.610582835780952848e+01
-2.493143230170545266e+01,-2.265657548725371129e+01,-1.946609675960931440e+01
-2.500184453095704029e+01,-1.986468934643995254e+01,-2.484616744219461992e+01
-2.383728576622739226e+01,-2.361271384202615309e+01,-1.703775275106067966e+01
-2.563320154403852058e+01,-2.050683397525197904e+01,-2.346573887840794725e+01
-2.401361809420738780e+01,-2.429544704622363582e+01,-1.616394300332300560e+01
-2.438126624520911534e+01,-2.329935745272958769e+01,-2.023942552232622916e+01
-2.168118169877426382e+01,-2.477896003438056738e+01,-3.320091652407336280e+00
-2.498452237488503158e+01,-2.145933383723118482e+01,-2.316114018891853021e+01
-2.404916792188872421e+01,-2.500622343780692347e+01,-1.678219588655666072e+01
-2.253073526596396192e+01,-2.609832328347219743e+01,-8.276341531692194664e+00
-2.660334839324570666e+01,3.154796922131613002e-01,-3.031659536282133871e+01
-2.662634717407331664e+01,1.958647243612976929e+00,-2.985683746464473387e+01
-2.573255246579507372e+01,-1.163406342430614515e+01,-2.864468076708158151e+01
-2.406243195854128913e+01,-2.484330767090132497e+01,-1.140440011958523314e+01
-2.654884244276905036e+01,2.126001819614392829e+00,-2.926748626699598077e+01
-2.770257030252795261e+01,6.948565951396881601e+00,-2.836931666418573172e+01
-2.562977448741007436e+01,-4.061658735403788967e+00,-3.004161973842064981e+01
-2.450111192727538878e+01,-1.542784643626145957e+01,-2.788494956704713701e+01
-2.566908658134365950e+01,1.177433276095776193e+00,-3.008095187301636741e+01
-2.492816059900121672e+01,-1.970670452114191562e+01,-2.319957472681966237e+01
-2.561810978684233575e+01,-9.355852577239360812e+00,-3.034310301210084759e+01
-2.531695338639963566e+01,-6.637480734348861766e+00,-3.027927041575528477e+01
-2.602561193023810659e+01,-1.351580428775205789e+00,-3.075454580157289541e+01
-2.579293620227478456e+01,-1.217014811115688389e+01,-2.868241117960560160e+01
-2.557749259081761650e+01,-1.208168191276528525e+01,-2.815481382999392679e+01
-2.698075246633476709e+01,9.483424000208026783e+00,-2.659065366931564256e+01
-2.712664021711685081e+01,3.305439012783379482e+00,-2.948290966444160688e+01
-2.583713255580311241e+01,-7.447434975397501766e+00,-3.048220451495397043e+01
-2.550047832073646958e+01,-1.065504042729559231e+01,-3.000408204181651683e+01
-2.701188758566963699e+01,5.689488230290582038e+00,-2.881903240281894796e+01
-2.492916584659752033e+01,-1.564880840851351884e+01,-2.607978351828969465e+01
-2.485304389821337878e+01,-1.008400746808790061e+01,-3.044925109706454691e+01
-2.568802244477453556e+01,-1.420779979831882578e+01,-2.831622704428171033e+01
-2.721765693759176230e+01,1.216632851114070668e+01,-2.384328778326518972e+01
-2.303298527970989795e+01,-2.317782336705361246e+01,-1.714092160090000760e+01
-2.638784042435533905e+01,2.099259284007446880e+00,-2.922269245200862997e+01
-2.624865362381293465e+01,-3.724719884032089645e+00,-2.998113172482596411e+01
-2.493388447411540909e+01,-1.857204131343311815e+01,-2.563285553330792510e+01
-2.628442402066710315e+01,-5.990407003640221717e+00,-2.987638032586152548e+01
-2.518492375408382955e+01,-1.655791214612232665e+01,-2.640305360379820598e+01
-2.470676708551136613e+01,-1.384804674712817985e+01,-2.773323632140176187e+01
-2.545991121770164511e+01,-1.567712397602648977e+01,-2.689114016344712610e+01
-2.411516901153554926e+01,-2.038715461456817124e+01,-2.383481742661471969e+01
-2.537867622506524867e+01,-4.630337276247908029e+00,-3.030095054025095891e+01
-2.600869588066692017e+01,-1.455468535518538964e+01,-2.851196982492563592e+01
-2.623345652322523236e+01,-1.002003177416990276e+01,-2.980437663387418468e+01
-2.596107414157103932e+01,-7.832635439771223673e+00,-2.978567388222689516e+01
-2.333083761918416954e+01,-2.479365120585386251e+01,-1.288695882561743211e+01
-2.733807216117158845e+01,3.675426208697039954e+00,-3.059382421899822191e+01
-2.612742612818355781e+01,4.102759095210952722e-01,-3.056068184466597870e+01
-2.582472653935734641e+01,-9.994117504537875618e+00,-2.940843156094427258e+01
-2.498030516657384226e+01,-1.757517516325876983e+01,-2.578666137670646918e+01
-2.718397366313713093e+01,1.282125168044421493e+01,-2.482776824238119673e+01
-2.524390522628411659e+01,-1.665887024870409761e+01,-2.632389136363828896e+01
-2.427321377757826326e+01,-2.181585714613408555e+01,-2.213654426135629905e+01
-2.822865553065143374e+01,1.027575921679436277e+01,-2.709155080772760016e+01
-2.783445809979478369e+01,1.155749130450795370e+01,-2.472909330684742457e+01
-2.589792523731228258e+01,-5.815642603612385386e+00,-3.082674832937700415e+01
-2.735206748723539150e+01,-1.654895068872628272e+00,-2.980705240831009206e+01
-2.792000183772815802e+01,7.116430885319008581e+00,-2.830961651975295013e+01
-2.802779872801178840e+01,1.097499362550357027e+01,-2.472330556768348231e+01
-2.604767322666315721e+01,-9.170409416638037214e+00,-2.879885449844666567e+01
-2.635717814932284142e+01,-1.634681735633828570e+00,-2.986070763941575734e+01
-2.819886839191068617e+01,1.090378700145044455e+01,-2.598361639664192069e+01
-2.800348363224804871e+01,1.212893064434568124e+01,-2.388674597698715019e+01
-2.712295078823364136e+01,1.236375217337750065e+01,-2.566603941969177782e+01
-2.755082092124272464e+01,8.737393707293122702e+00,-2.743532450241990261e+01
-2.703453660595289065e+01,7.584398539439501263e+00,-2.831522914117201140e+01
-2.771362498481308734e+01,7.467232153714469689e+00,-2.691245060150031776e+01
-2.812931842015370876e+01,4.155779841421759713e+00,-2.819617026608333532e+01
-2.726239787428324846e+01,7.927540014955891223e+00,-2.780215927500725570e+01
-2.804617721546156162e+01,1.424016417817234803e+01,-2.166153171018120105e+01
-2.738791592829496579e+01,6.500227115647193799e+00,-2.854149148467065800e+01
-2.686123024421294403e+01,-5.263932639424545812e+00,-3.002164033909289742e+01
-2.705151057083327260e+01,3.908207119342018032e+00,-2.956792441180240871e+01
-2.759820718404161255e+01,1.232196443318550116e+01,-2.369515477610941900e+01
-2.760745455056906650e+01,5.373035868737551013e+00,-2.838134626937095106e+01
-2.559365807435917262e+01,-6.408745497381122647e+00,-3.015045744622517532e+01
-2.695300118427521596e+01,7.769141218688591977e+00,-2.718707161753179946e+01
-2.797578137149367450e+01,1.163621790391164090e+01,-2.445734439670212623e+01
-2.675353365801597505e+01,1.073948282127522980e+01,-2.561659411295675426e+01
-2.638412100777211577e+01,9.142945441408238949e+00,-2.572150342477528540e+01
-2.815283827604533329e+01,1.020085529611552921e+01,-2.445536057984242717e+01
-2.697009398385699441e+01,-1.061344869159195348e+00,-3.029493340755773545e+01
-2.601201055039280874e+01,-5.950267103208248365e+00,-3.064450298680011997e+01
-2.716532600866198521e+01,4.987841178595598279e+00,-2.763482677010973276e+01
-2.706956391424163755e+01,-1.621923419888668949e+00,-2.990897705521074812e+01
-2.671496061837095226e+01,6.484378286892368948e+00,-2.872453443883717483e+01
-2.655664828496867003e+01,-5.978698862352223919e+00,-3.103614852311505246e+01
-2.760323951513204221e+01,1.280043685947881293e+01,-2.340991492241052896e+01
-2.889130018009085532e+01,1.309801153608050051e+01,-2.295024059951489903e+01
-2.697052325911059611e+01,7.161171353198541922e+00,-2.808600476721761652e+01
-2.798258721308376096e+01,1.394219742787011818e+01,-2.419652681730543264e+01
-2.504056123354465413e+01,-5.562245132830813787e+00,-3.130958362530562056e+01
-2.768812781096057662e+01,6.888244448998847247e+00,-2.689659929685236506e+01
-2.620788593394531318e+01,-1.061491906016868825e+00,-3.051434954278153100e+01
-2.702032455467734096e+01,4.253893439968221557e-01,-3.012724597576129071e+01
-2.699028916897978903e+01,-4.227146549636151107e+00,-2.974920994233877991e+01
-2.749557251632571209e+01,7.577694489253758547e+00,-2.730610388650458020e+01
-2.780559257709388632e+01,9.157339986904265317e+00,-2.804754097157310611e+01
-2.683158239377393173e+01,1.713230133339291861e+00,-2.991583647988129968e+01
-2.744850208293523153e+01,1.254407390450305293e+01,-2.498774780143790508e+01
-2.756213262623451499e+01,1.624881923611249945e+00,-2.935524708771626479e+01
-2.706705482756131786e+01,1.360854514729059339e+01,-2.363473821075596248e+01
-2.844758386596406297e+01,4.885627238651887083e+00,-2.905799269727151568e+01
-2.776611175995396863e+01,5.738431438325685363e+00,-2.755948060303403224e+01
-2.678708184457916985e+01,9.942560485715143059e+00,-2.560596290950687148e+01
-2.852643390382387167e+01,1.224003545136200621e+01,-2.499624405606923006e+01
-2.698752079825024097e+01,7.706313118782572857e+00,-2.842973471918411121e+01
+4.395250595036668706e+00,-4.322663868386681152e+00,-4.971164226449628742e+00
+5.464502063414679256e+00,-4.440635391753692041e+00,-5.655311415943845788e+00
+4.816082401592716167e+00,-3.760850775547923242e+00,-6.244057362492451801e+00
+4.745651181664434226e+00,-3.520985471737261285e+00,-6.425287235864297841e+00
+5.143417018105640892e+00,-3.769231601723258329e+00,-6.667001493987497085e+00
+4.682671393843319763e+00,-4.214836713990881556e+00,-7.263347824176770828e+00
+4.632631213160046002e+00,-3.244833835867647842e+00,-7.118236051895419969e+00
+4.031937727141903238e+00,-3.680862188183487760e+00,-6.577724542069433689e+00
+3.773553551336611633e+00,-4.709611143852578508e+00,-7.092710208142162465e+00
+6.035645899548843119e+00,-4.157390994574154952e+00,-4.537637138422331518e+00
+4.441820081212016547e+00,-3.757077437121850938e+00,-5.377318270987054838e+00
+4.019996924716306097e+00,-3.595435894698909784e+00,-7.472054943412725692e+00
+4.546973880381376176e+00,-4.705362330457607989e+00,-7.168970149921851664e+00
+4.218853456840061078e+00,-4.004649112098787711e+00,-5.689728936182667951e+00
+5.094352674240221646e+00,-3.312716352726931213e+00,-6.448881632377177375e+00
+4.976689714674379594e+00,-3.460792155550518334e+00,-5.736484596831427751e+00
+5.593090830375377465e+00,-3.677049303093503418e+00,-6.478883997405122663e+00
+3.743942389505838353e+00,-4.978315239030565387e+00,-6.382412467092967390e+00
+4.719851067643378251e+00,-3.564997910544921211e+00,-6.930491281523351255e+00
+3.509042320998985609e+00,-4.075031457567797055e+00,-7.529789903700861764e+00
+4.422154513908088447e+00,-4.073047695107685051e+00,-5.770936423537373017e+00
+5.903061369353857835e+00,-3.333470887820057182e+00,-5.149531069211041867e+00
+5.320061273013488190e+00,-4.900966278643878127e+00,-6.011214688346447232e+00
+4.386030844677042850e+00,-4.362466414500863365e+00,-5.867253157156456567e+00
+4.185189254387175595e+00,-4.439924987741166618e+00,-7.572141142042074335e+00
+4.942030220319173495e+00,-3.463824980279692323e+00,-5.902864229833759246e+00
+3.668413359819459707e+00,-4.546183564105624519e+00,-6.910565031961458438e+00
+5.311832290371190979e+00,-3.477423392958457704e+00,-6.355732706688390188e+00
+1.001623244718298089e+01,-1.248338026820153601e+01,-6.975115843194810594e+00
+9.746047524311890697e+00,-1.234602955463430973e+01,-5.789917664650237050e+00
+1.226313539578390355e+01,-1.221788971161849702e+01,-1.049925018831972245e+01
+1.074858711255845733e+01,-1.319460832729752298e+01,-7.044217943157934592e+00
+9.510610972292333543e+00,-1.053218118160822669e+01,-3.191987672990745928e+00
+1.075556831488009557e+01,-1.380605656435415085e+01,-9.681023588688230319e+00
+1.239984239604647520e+01,-1.130425900231670333e+01,-1.490606197102359332e+01
+9.886284250200747081e+00,-1.346505253961593240e+01,-7.480705471248404237e+00
+9.343375845911809918e+00,-1.118841666220255959e+01,-3.363274088290253427e+00
+9.173719526831138893e+00,-1.080471664309665947e+01,-4.572699446149313118e+00
+9.410657408812545199e+00,-1.245168042356199578e+01,-5.759540231959079826e+00
+1.036319024552942025e+01,-1.317108591702204201e+01,-7.002380547205122596e+00
+1.082365444353933093e+01,-1.282800038362785955e+01,-6.366720032462955814e+00
+9.812859452446542008e+00,-1.290800079730089500e+01,-7.656748215638626398e+00
+7.499149414234647537e+00,-7.769221077547984855e+00,-2.504820919063063478e+00
+1.141153828109480806e+01,-1.314418961705730915e+01,-1.032553736258267740e+01
+1.095853923999918678e+01,-1.298491757987332917e+01,-6.768323379190671396e+00
+8.672724450648097161e+00,-1.013328436035949665e+01,-3.128271773883745333e+00
+1.032622464401251605e+01,-1.310220476518617438e+01,-9.081164192728834905e+00
+9.889109234781914282e+00,-1.270394120633862656e+01,-4.065018695329629672e+00
+9.815268076722158952e+00,-1.295616014137147864e+01,-6.239129368279058951e+00
+8.892292357825327898e+00,-9.288905949172741927e+00,-3.551138605407810900e+00
+8.975744294190628025e+00,-9.295787711290845579e+00,-3.513719809478732969e+00
+8.379909104901010153e+00,-8.635166578746488852e+00,-1.879361369055306596e+00
+9.762884571397854927e+00,-1.023836563220016060e+01,-3.398738455820169868e+00
+8.731284177973209992e+00,-9.293783176422163450e+00,-2.766092812813486290e+00
+7.899911251126299661e+00,-9.506823880050692566e+00,-2.604402749314255416e+00
+9.731959157140854799e+00,-1.034000968358193795e+01,-3.435779939702835684e+00
+1.035719926870322105e+01,-1.308235357102338092e+01,-9.341539860265154260e+00
+7.654682114372681312e+00,-4.330253356305346912e+00,-2.987674829030328105e+00
+9.306203420390966485e+00,-1.406702220181735541e+01,-9.150251498175723697e+00
+1.014911150048022215e+01,-1.265435780392008169e+01,-6.247722507453955743e+00
+1.003190093143867401e+01,-1.299324923292024891e+01,-7.279288219316636166e+00
+9.011463401155614505e+00,-1.234406573494549875e+01,-4.987416593295200151e+00
+9.747876515955013588e+00,-1.356929033495655901e+01,-6.281615324604515216e+00
+1.095873265490255299e+01,-1.341215311515254527e+01,-8.072667583212597364e+00
+1.023313390484863561e+01,-1.285195814961189242e+01,-5.003435992934814891e+00
+9.560415276819307806e+00,-1.176390953557082852e+01,-4.840284594763478054e+00
+8.726491126080192728e+00,-1.064016230571775878e+01,-4.204087355889096322e+00
+8.746381188116510330e+00,-9.181624294424377553e+00,-3.095571632160803333e+00
+9.073694019185431614e+00,-1.041293984221182711e+01,-2.761047322707135265e+00
+9.080828775841769840e+00,-1.157967794373984205e+01,-4.875282134119531818e+00
+9.705168846735871213e+00,-1.395160253636398906e+01,-6.953602487585388126e+00
+1.060893835564072596e+01,-1.358143196579211320e+01,-7.331515016952955044e+00
+8.890633788856165509e+00,-8.549841352690226159e+00,-3.102810717366640603e+00
+7.689708342648051698e+00,-8.317816779351453249e+00,-3.673782492687565071e+00
+1.036648116944628306e+01,-1.273110720850786315e+01,-6.776974019740150013e+00
+1.036250513551251196e+01,-1.348174618267534264e+01,-7.813690311801156696e+00
+8.608686267366518763e+00,-8.401086558886060374e+00,-1.751645182339836460e+00
+1.021449314462090463e+01,-1.176300229511189599e+01,-7.094474648682265183e+00
+7.286065623640102018e+00,-6.371821818146274907e+00,-1.963986481598901435e+00
+9.650406516947663604e+00,-1.358609338205300787e+01,-8.632143621637300868e+00
+1.050290508583148430e+01,-1.292288438371390846e+01,-6.801667227988794195e+00
+1.017972627467378111e+01,-1.184768388328544653e+01,-4.764489523859370301e+00
+7.696346386977783283e+00,-5.832091720334171114e+00,-3.305916269236620408e+00
+8.972799883575337532e+00,-1.086033415740480201e+01,-3.077954171257880844e+00
+8.292488182000942842e+00,-8.704818157236919873e+00,-2.845082799917594940e+00
+1.107841080136359579e+01,-1.316655456044676242e+01,-9.302312517386928548e+00
+9.745359465449064729e+00,-1.231529300361775725e+01,-5.028936417917496904e+00
+8.478809339834770142e+00,-1.221600989547063065e+01,-4.459622869527334998e+00
+8.852500263772505207e+00,-9.007977612217839436e+00,-2.457086525620048256e+00
+7.551587982240722141e+00,-7.390924712159323562e+00,-2.465509969589359862e+00
+8.404382709847265431e+00,-8.736907374221489775e+00,-2.929705380523430769e+00
+1.005639414966485390e+01,-1.177873343078086066e+01,-5.837812672238696265e+00
+8.925463857406237267e+00,-9.788086679139645696e+00,-2.830254610270173110e+00
+1.032757821120249986e+01,-1.329956219406319207e+01,-7.851523401458935680e+00
+1.081958776732908412e+01,-1.320603629163440473e+01,-7.784668722969446897e+00
+7.584698305368953619e+00,-6.144443995298825456e+00,-1.964060351459080422e+00
+1.422440566345288104e+01,6.664656239356148149e-01,-1.748458449632873624e+01
+1.209211895314341945e+01,-1.395198990754988166e+01,-1.294512112936691572e+01
+1.204484132896206461e+01,-1.162847258283540697e+01,-1.349147052379273504e+01
+1.363309817471195196e+01,-4.690118982502275990e+00,-1.812698810422864426e+01
+1.321794691948816691e+01,-4.725842437851797584e+00,-1.682453206547122448e+01
+1.330138311704246235e+01,-1.028332373266535171e+01,-1.554599597718006798e+01
+1.299794660769330967e+01,-7.629650725764824060e+00,-1.740075707863643473e+01
+1.273508492167364636e+01,-9.940554485766080361e+00,-1.687214661600456367e+01
+1.211301819494347676e+01,-9.803996791212910011e+00,-1.601748581960441697e+01
+1.411067780523191573e+01,-6.565823475510969232e+00,-1.747617407053593297e+01
+1.251930561918896245e+01,-1.037615327945981392e+01,-1.695316723643325929e+01
+1.337049379021845574e+01,-4.944629667103464854e+00,-1.830385006109548485e+01
+1.591512523181550698e+01,5.230776523220260543e+00,-1.395055095972282544e+01
+1.343853436334039309e+01,-6.169476090609759211e+00,-1.829381003312731835e+01
+1.144814910437605704e+01,-1.352699163364047052e+01,-1.254816379143971261e+01
+1.452156408138628230e+01,3.224544127597482657e+00,-1.594468183501004610e+01
+1.443563928508468130e+01,-5.256380644623710019e+00,-1.760902093339744567e+01
+1.332207393146289043e+01,-2.036763707876132479e+00,-1.813326373217121557e+01
+1.382034832759745413e+01,-9.523074623212330891e+00,-1.564110570520793786e+01
+1.697481318573218800e+01,7.377017130819920609e+00,-9.281558563274238338e+00
+1.450597355019188939e+01,-3.837366278349945148e-01,-1.773154640754879807e+01
+1.314741597332643330e+01,-9.921472000309114136e+00,-1.463081694245978603e+01
+1.327433790167815353e+01,-2.337707503980743784e+00,-1.764863409683201922e+01
+1.515566226815671769e+01,3.235122009065914739e+00,-1.481951957903419625e+01
+1.283737809678832242e+01,-2.311194451897040647e+00,-1.803706541334578972e+01
+1.234507040648451692e+01,-1.148583282998043842e+01,-1.533048188863032735e+01
+1.403451864582015851e+01,-1.267330320629449503e+00,-1.723929668751237188e+01
+1.474395624404557736e+01,-3.509430616015811744e+00,-1.728353234207030908e+01
+1.312169581312165079e+01,-9.411084323360272563e+00,-1.660377278613343321e+01
+1.359355967399659981e+01,-1.791061369903209410e+00,-1.777786262748419688e+01
+1.298412052647757164e+01,-2.763773284403350239e+00,-1.864495588837796092e+01
+1.317564493368682577e+01,-1.099327049626182351e+01,-1.464418637422346592e+01
+1.331745860998589848e+01,-8.064170655338038785e+00,-1.815350606072040307e+01
+1.355490971140668144e+01,-3.668129628788647345e+00,-1.832575302085016489e+01
+1.341095543126219347e+01,-4.961370215759112412e+00,-1.727950749131285590e+01
+1.264544633259677830e+01,-6.238205236825889344e+00,-1.817043066121454586e+01
+1.304202522351826588e+01,-6.879516322041464349e+00,-1.763172217221836036e+01
+1.575372210259419070e+01,4.080489382037058022e+00,-1.550889800616303305e+01
+1.537214912549692158e+01,-4.023603523606151811e-01,-1.746618064396603387e+01
+1.468408596455508075e+01,-2.625262897804098383e+00,-1.699519195835906515e+01
+1.312348314911815983e+01,-8.586081965252796877e+00,-1.738837114416729435e+01
+1.262910586730866136e+01,-8.017866084688479944e+00,-1.703836248750851468e+01
+1.318401386994887758e+01,-5.143580711668401584e+00,-1.798946595460883913e+01
+1.254640900037620987e+01,-1.056878074382554189e+01,-1.533491670084033487e+01
+1.343770705135055721e+01,-6.812979909137673928e+00,-1.671265705755998709e+01
+1.255803812816796494e+01,-7.455408298691825308e+00,-1.742909843203369036e+01
+1.348884091460585211e+01,-5.765244663718104512e+00,-1.791441140443311753e+01
+1.428738527618931187e+01,1.556954878466595638e+00,-1.621523939145270532e+01
+1.351775878796965102e+01,-5.594088880809534814e+00,-1.834285377690882513e+01
+1.611132058850679982e+01,6.498543498196390544e+00,-1.199151710443942065e+01
+1.349940600515696154e+01,-6.258622569360970722e+00,-1.855021026627498770e+01
+1.322244988555497613e+01,-4.926268960892255855e+00,-1.685851868531270270e+01
+1.222177694201315923e+01,-9.053669666924420767e+00,-1.647987719247205618e+01
+1.458139982567740311e+01,-1.952750151131201761e+00,-1.817565637156737424e+01
+1.341255883800023874e+01,-3.097450718804315883e+00,-1.810340359212710482e+01
+1.440645453089172356e+01,2.211809790966401401e+00,-1.645264590932757542e+01
+1.193712862849979395e+01,-1.237945226200528381e+01,-1.368758206877894779e+01
+1.344127888533262549e+01,-4.377598654834610414e+00,-1.774819447180508902e+01
+1.317996302654562868e+01,-3.435345037556910786e+00,-1.757230974893919040e+01
+1.324898388668255045e+01,-7.165296665602514992e+00,-1.757765736519312583e+01
+1.342264739909429139e+01,-6.417527470248162835e+00,-1.860949410960960648e+01
+1.415539414286176623e+01,-2.918455349646705610e+00,-1.771344456362243847e+01
+1.317446839640384937e+01,-7.492185523074960329e+00,-1.658202177203352790e+01
+1.448469370495780240e+01,-3.135307771920590625e+00,-1.797651706441067887e+01
+1.528632568923078594e+01,4.685376883141234572e-01,-1.756151374331199833e+01
+1.227591044291007272e+01,-8.495114336733308846e+00,-1.711757562905923180e+01
+1.281750921075058791e+01,-8.040507294391296966e+00,-1.658582407193567221e+01
+1.245587464923643140e+01,-9.112571815236742978e+00,-1.730381438582104536e+01
+1.308926519824433754e+01,-7.451609674566151753e+00,-1.718920625486549625e+01
+1.645339418036515511e+01,7.382402687410285935e+00,-8.055091957390105861e+00
+1.656130476323728473e+01,7.479945989958263652e+00,-4.771677738454028983e+00
+1.661159484078974202e+01,8.097991079647375301e+00,-6.465974489448926832e+00
+1.694291363943615281e+01,7.938854924583669259e+00,-7.847019998962207588e+00
+1.705225493000251191e+01,8.273509580004388297e+00,-1.361801206319779745e+00
+1.592938542207729569e+01,5.861336844134489965e+00,-1.214191842613768380e+01
+1.632910661010952680e+01,8.804393876988289236e+00,-7.683946025594213580e+00
+1.585688555003061673e+01,8.823898454780499279e+00,-8.356045527166315878e+00
+1.404854614045483707e+01,-1.136973744008778375e+00,-1.782355206906638756e+01
+1.526535454391915714e+01,4.010538256846770011e+00,-1.451808590613034156e+01
+1.628659704246933515e+01,8.125295050890519732e+00,-8.314708226918344991e+00
+1.511479068472412379e+01,1.882088579887041924e+00,-1.644778803870357109e+01
+1.495400752484361107e+01,3.707654153524119423e+00,-1.489813925229233504e+01
+1.478930752003110349e+01,1.317740685608417728e+00,-1.690696819234760184e+01
+1.529173688776298334e+01,3.561915542459212602e+00,-1.581242245822763337e+01
+1.496910459162500118e+01,2.322187324756086468e-01,-1.695158903731445577e+01
+1.545219032234885326e+01,6.152730637187238116e+00,-1.247006494917788011e+01
+1.469145396954023397e+01,5.804330906336597096e+00,-1.309378413726908974e+01
+1.898788199784210562e+01,3.249560630185005294e+00,6.549281091303999602e+00
+1.571745465000396358e+01,2.237991282801172765e+00,-1.658722738839586697e+01
+1.511211284714100778e+01,1.127179634406377140e+00,-1.634529718745005411e+01
+1.539159575365048305e+01,6.937204305012953043e+00,-9.737695414897025614e+00
+1.807303515510734115e+01,4.757333386504440043e+00,3.957251423163308246e+00
+1.449158744148847866e+01,2.235837840250619379e+00,-1.675064609885996703e+01
+1.598771362217022762e+01,3.034584031342285826e+00,-1.538150885381962851e+01
+1.703702886188433041e+01,7.593521459021800979e+00,-1.262652376700381218e+00
+1.664789048431876495e+01,5.311025222618292574e+00,-1.426980047872935486e+01
+1.371936884998051909e+01,-4.664727020653710809e+00,-1.849533287710204377e+01
+1.676063811616221244e+01,9.878484513517387100e+00,-5.530127405782879535e+00
+1.511243535088700263e+01,4.566260339784321332e+00,-1.544922096299710113e+01
+1.684106044393793056e+01,8.787266912708210143e+00,-8.342009331795241067e+00
+1.506406276008835476e+01,5.867327091263700112e+00,-1.265316389733326119e+01
+1.546005539070945822e+01,7.108617947282439786e+00,-1.037810164161595061e+01
+1.638855564010735932e+01,6.065515949846437493e+00,-1.263173412340649371e+01
+1.853910408351196537e+01,4.214139932266830257e+00,5.116620730383008464e+00
+1.695180757997870913e+01,8.132997003042978790e+00,-7.202444267408105283e+00
+1.588221573901916805e+01,7.822845931449977641e+00,-9.821593761859555016e+00
+1.753177628346295336e+01,7.735486470816946181e+00,-2.468646595444683456e-01
+1.606867984753119671e+01,7.375700469287286509e+00,-1.106474944992303833e+01
+1.757863109350234510e+01,8.159362234680092030e+00,-8.418207623032834874e+00
+1.665412346818128952e+01,6.972634802158150791e+00,-9.887193189253990155e+00
+1.387542776782413867e+01,-3.206430777412592636e+00,-1.765501849252107291e+01
+1.668059461885076544e+01,8.881794620201031165e+00,-7.048970183217672769e+00
+1.469444031165007480e+01,1.969431270613339002e+00,-1.568862868881986827e+01
+1.594874492905061025e+01,7.779895227922397183e+00,-1.010928068288663084e+01
+1.436786482048101732e+01,1.530434859106996726e+00,-1.584429547932200677e+01
+1.638237963118461948e+01,8.192414124659862296e+00,-3.042694169529642778e+00
+1.600570520736174274e+01,4.996876052384335409e+00,-1.278601973171864081e+01
+1.616171446391154376e+01,4.091949164523896343e+00,-1.396517770926991275e+01
+1.513554289803591502e+01,1.484084610712073982e+00,-1.751786689080163484e+01
+1.477605331987120785e+01,-1.467919215284172019e+00,-1.780769004333539129e+01
+1.757193463550051504e+01,8.056675978082806111e+00,-5.462745008745203634e+00
+1.695380580274347082e+01,7.633945778535977666e+00,-9.355561616519098678e+00
+1.677622277187671784e+01,7.069768228772769447e+00,-1.125591046671367934e+01
+1.525526163669538349e+01,6.222541177290061398e+00,-1.263677035232336721e+01
+1.616707981912927039e+01,7.622146136872471445e+00,-8.766143078454049942e+00
+2.296359044322872833e+01,-2.316991974955748645e+01,2.071706138055439794e+00
+2.184343019210889025e+01,-2.326519724165115122e+01,2.406709435737475644e+00
+2.341798948840471084e+01,-2.512138862677182516e+01,-8.040050046342468448e+00
+2.134833938244103635e+01,-2.253114476509641406e+01,1.850427262628588920e+00
+2.112236377489577777e+01,-1.822738718336637120e+01,6.586017064502648566e+00
+2.140169601694480761e+01,-2.027269475361827844e+01,5.258768505564601625e+00
+1.877228097345865976e+01,4.982902187603093225e-01,7.916565910948589746e+00
+2.199738259802289519e+01,-2.547712281357617314e+01,-6.506855070403702257e+00
+2.160032292670828369e+01,-1.839895317118849505e+01,5.855063487398586730e+00
+2.201031494962639101e+01,-2.484870288497440072e+01,-3.029237897749075259e+00
+2.064329096048719947e+01,-1.268411298729742498e+01,9.241424582854142145e+00
+2.218532288756697213e+01,-2.290693958742515690e+01,1.052581387909075517e+00
+2.227736573802844333e+01,-1.849358102309743046e+01,6.001130968337715643e+00
+2.165757348224896006e+01,-1.870715573527809283e+01,6.652346721065390156e+00
+2.076458065493189054e+01,-1.982592446387534935e+01,5.789730045757707444e+00
+2.024448426913530952e+01,-1.574320900063249873e+01,7.229101673812197149e+00
+2.156857459526498033e+01,-2.054045176750033619e+01,4.564112079158643809e+00
+2.333440187548032441e+01,-2.595171045248289232e+01,-1.130360482477417428e+01
+2.258656528031731625e+01,-2.604504613646205513e+01,-9.408790284756381794e+00
+2.130834774661994402e+01,-2.013841735677001310e+01,4.266196272923430399e+00
+2.049663888756070307e+01,-1.571712573990078887e+01,7.501726870241967049e+00
+2.228065728292500580e+01,-2.572960754891156654e+01,-3.199480585653966092e+00
+2.120460109656314174e+01,-1.816441718402893457e+01,6.920400000318716494e+00
+2.195681766009772318e+01,-2.199529736637779109e+01,1.256915192457176644e+00
+2.201823837099016146e+01,-2.536548785460904298e+01,-7.730147302712683910e+00
+2.191232254550725500e+01,-2.262899038587625000e+01,6.268619023663628553e-01
+2.230974503566952905e+01,-2.580644757428363079e+01,-6.324530313668581982e+00
+2.142370693029285178e+01,-2.026886274530126997e+01,5.314775659652834605e+00
+1.965260860484254479e+01,-6.018209388722169706e+00,1.043062548484094343e+01
+2.121054172257165504e+01,-2.078600358730887265e+01,4.180813133424983619e+00
+2.267995853948431417e+01,-2.601352321476538521e+01,-8.216380826288411043e+00
+2.116253738932094564e+01,-1.980497517308850419e+01,5.755232310930471940e+00
+2.141267617355513408e+01,-2.238993563427020916e+01,1.512012774605178578e+00
+2.208466092280029969e+01,-2.284813441398870282e+01,1.807110938072760575e+00
+2.162322873943209345e+01,-2.016911113304284697e+01,4.060709540934650974e+00
+2.137929177206634890e+01,-2.335557217243398753e+01,-1.373994680270005375e-01
+2.022571474659641311e+01,-1.024682560613245919e+01,1.007090323086750239e+01
+2.297451970135233523e+01,-2.504358813195573674e+01,-4.359600035303495602e+00
+2.140509119621716749e+01,-2.237022054721911246e+01,1.241929891201520419e+00
+2.379048468235028935e+01,-2.184937727178267153e+01,-2.081215166065097932e+01
+2.108287713804223884e+01,-1.761971042371840213e+01,7.294940082264405490e+00
+2.267910244039433820e+01,-2.472180781042260378e+01,-2.996126791598650030e+00
+2.159433868019981517e+01,-1.989647825655822899e+01,3.684544847593317130e+00
+2.126073297645213600e+01,-1.866086985209446425e+01,6.584880764221512806e+00
+2.211698579238815654e+01,-2.384802886015779677e+01,6.796908563404846504e-01
+2.218684925429112553e+01,-1.694407942818845925e+01,6.197662542500848915e+00
+2.030683561678518956e+01,-6.426481060442648108e+00,9.596690860818073432e+00
+2.188917107351645797e+01,-2.102820621716719529e+01,3.027735236424064169e+00
+2.173271057200532752e+01,-2.382834097812880003e+01,-1.045245821052465551e+00
+2.201234834421086717e+01,-2.104728853507654307e+01,1.355780719869750683e+00
+2.345047161065107844e+01,-2.534337542845079128e+01,-1.204297824467470690e+01
+2.192101547619951418e+01,-2.389646709273769432e+01,-8.684406494161578394e-01
+2.081756794180137149e+01,-1.526137004877870673e+01,8.690106094713812013e+00
+2.043858724830730722e+01,-1.355857081852436608e+01,8.472750311409948054e+00
+2.408101567470776416e+01,-2.523692774724589327e+01,-1.267726475208434778e+01
+2.199324047807551352e+01,-1.949430300853566678e+01,5.735800194962589416e+00
+2.091441711027008310e+01,-9.437018367061078550e+00,9.608524790867077670e+00
+2.092422279781106553e+01,-8.245819367914005937e+00,1.045728452752925186e+01
+2.388671832860385535e+01,-2.608941496635303992e+01,-1.273025878016193602e+01
+2.480046511090974093e+01,-2.420636210663293753e+01,-1.484274544901062498e+01
+2.041831244763949726e+01,-1.517703690822252760e+01,8.062227306343656252e+00
+2.132962557634880696e+01,-2.225011225368936607e+01,3.363397839605919870e+00
+2.212528812501945552e+01,-2.251554071299918292e+01,-1.931815061803342282e+00
+2.040123031916628804e+01,-1.097886582435655711e+01,9.700909635296360634e+00
+2.580456151995164404e+01,-1.437712772899021729e+01,-2.691973088356861155e+01
+2.418016162138154002e+01,-2.034372992539833191e+01,-2.373874699070208294e+01
+2.393687502563621194e+01,-2.393873658027090556e+01,-1.929834210989234577e+01
+2.429105906728302955e+01,-1.358334006104800196e+01,-2.774229307970408342e+01
+2.298347278932940085e+01,-2.571218239453622090e+01,-1.226803408900074643e+01
+2.307607434424518900e+01,-2.564243564182613966e+01,-9.694602101597222799e+00
+2.364212608243864722e+01,-2.558886654877179012e+01,-1.330013287810668388e+01
+2.273562947326239225e+01,-2.529567592209023985e+01,-9.236445701190184820e+00
+2.402093827704013762e+01,-2.430611915291135006e+01,-1.663415994459370495e+01
+2.252418619017255708e+01,-2.496805946901873341e+01,-3.126407554013312051e+00
+2.319781893885000557e+01,-2.354012555635899417e+01,-1.680613288434327757e+01
+2.450553773745986064e+01,-1.619910550745199984e+01,-2.568206974882684790e+01
+2.240582474461039908e+01,-2.578463728330557814e+01,-1.004574535155576243e+01
+2.455609950178190104e+01,-1.934319529607305199e+01,-2.425350074179327464e+01
+2.436548957048902153e+01,-2.091737112472101501e+01,-2.224627098568040040e+01
+2.425362828020559292e+01,-2.469058973216790065e+01,-1.364218832111659552e+01
+2.393265836216282949e+01,-2.578288692673940830e+01,-1.214964966372184207e+01
+2.321468676588910540e+01,-2.511141645267787226e+01,-1.293161436483637949e+01
+2.279149804209653851e+01,-2.495417589318267204e+01,-1.542912035081367783e+01
+2.340089058837738634e+01,-2.456397497963765630e+01,-1.498155714379575976e+01
+2.499599307161682660e+01,-2.066441078346491622e+01,-2.423301063447068060e+01
+2.440607832674238864e+01,-2.333472725085637478e+01,-1.831131866602770586e+01
+2.328968380096867463e+01,-2.516646870521633161e+01,-1.134756100155570024e+01
+2.535871720657070938e+01,-1.953135355834352538e+01,-2.372382925460571812e+01
+2.358564076152469369e+01,-2.528010373022814861e+01,-1.320364432252458364e+01
+2.467039969914649333e+01,-2.045869131947891617e+01,-2.293463046671746497e+01
+2.154361217505673309e+01,-1.994131148479492666e+01,5.007621372466962484e+00
+2.291113835839421142e+01,-2.622646583487545513e+01,-1.041186851563811189e+01
+2.241312153973111521e+01,-2.485334868959381538e+01,-6.729881578395903396e+00
+2.372681353790398973e+01,-2.487506020013109520e+01,-1.506372714906544275e+01
+2.373518158438036352e+01,-2.526971819406776376e+01,-1.370637208755551839e+01
+2.269906081402751497e+01,-2.556912076443708060e+01,-1.094686370566043010e+01
+2.445059875153450690e+01,-2.136125882372177642e+01,-2.364691248539913460e+01
+2.272170233857012533e+01,-2.334516458696715802e+01,-5.564281986004084857e-01
+2.228236045808541022e+01,-2.374237420594234749e+01,-1.622933820191633458e+00
+2.363197545872582239e+01,-2.601905338343803464e+01,-9.118905376074529556e+00
+2.389913679633781385e+01,-2.342710545536563416e+01,-1.938059894142172013e+01
+2.466995018657652849e+01,-1.481900631176661953e+01,-2.775436768519973896e+01
+2.385976378648329188e+01,-2.433399965862594883e+01,-1.610582835780952848e+01
+2.493143230170545266e+01,-2.265657548725371129e+01,-1.946609675960931440e+01
+2.500184453095704029e+01,-1.986468934643995254e+01,-2.484616744219461992e+01
+2.383728576622739226e+01,-2.361271384202615309e+01,-1.703775275106067966e+01
+2.563320154403852058e+01,-2.050683397525197904e+01,-2.346573887840794725e+01
+2.401361809420738780e+01,-2.429544704622363582e+01,-1.616394300332300560e+01
+2.438126624520911534e+01,-2.329935745272958769e+01,-2.023942552232622916e+01
+2.168118169877426382e+01,-2.477896003438056738e+01,-3.320091652407336280e+00
+2.498452237488503158e+01,-2.145933383723118482e+01,-2.316114018891853021e+01
+2.404916792188872421e+01,-2.500622343780692347e+01,-1.678219588655666072e+01
+2.253073526596396192e+01,-2.609832328347219743e+01,-8.276341531692194664e+00
+2.660334839324570666e+01,3.154796922131613002e-01,-3.031659536282133871e+01
+2.662634717407331664e+01,1.958647243612976929e+00,-2.985683746464473387e+01
+2.573255246579507372e+01,-1.163406342430614515e+01,-2.864468076708158151e+01
+2.406243195854128913e+01,-2.484330767090132497e+01,-1.140440011958523314e+01
+2.654884244276905036e+01,2.126001819614392829e+00,-2.926748626699598077e+01
+2.770257030252795261e+01,6.948565951396881601e+00,-2.836931666418573172e+01
+2.562977448741007436e+01,-4.061658735403788967e+00,-3.004161973842064981e+01
+2.450111192727538878e+01,-1.542784643626145957e+01,-2.788494956704713701e+01
+2.566908658134365950e+01,1.177433276095776193e+00,-3.008095187301636741e+01
+2.492816059900121672e+01,-1.970670452114191562e+01,-2.319957472681966237e+01
+2.561810978684233575e+01,-9.355852577239360812e+00,-3.034310301210084759e+01
+2.531695338639963566e+01,-6.637480734348861766e+00,-3.027927041575528477e+01
+2.602561193023810659e+01,-1.351580428775205789e+00,-3.075454580157289541e+01
+2.579293620227478456e+01,-1.217014811115688389e+01,-2.868241117960560160e+01
+2.557749259081761650e+01,-1.208168191276528525e+01,-2.815481382999392679e+01
+2.698075246633476709e+01,9.483424000208026783e+00,-2.659065366931564256e+01
+2.712664021711685081e+01,3.305439012783379482e+00,-2.948290966444160688e+01
+2.583713255580311241e+01,-7.447434975397501766e+00,-3.048220451495397043e+01
+2.550047832073646958e+01,-1.065504042729559231e+01,-3.000408204181651683e+01
+2.701188758566963699e+01,5.689488230290582038e+00,-2.881903240281894796e+01
+2.492916584659752033e+01,-1.564880840851351884e+01,-2.607978351828969465e+01
+2.485304389821337878e+01,-1.008400746808790061e+01,-3.044925109706454691e+01
+2.568802244477453556e+01,-1.420779979831882578e+01,-2.831622704428171033e+01
+2.721765693759176230e+01,1.216632851114070668e+01,-2.384328778326518972e+01
+2.303298527970989795e+01,-2.317782336705361246e+01,-1.714092160090000760e+01
+2.638784042435533905e+01,2.099259284007446880e+00,-2.922269245200862997e+01
+2.624865362381293465e+01,-3.724719884032089645e+00,-2.998113172482596411e+01
+2.493388447411540909e+01,-1.857204131343311815e+01,-2.563285553330792510e+01
+2.628442402066710315e+01,-5.990407003640221717e+00,-2.987638032586152548e+01
+2.518492375408382955e+01,-1.655791214612232665e+01,-2.640305360379820598e+01
+2.470676708551136613e+01,-1.384804674712817985e+01,-2.773323632140176187e+01
+2.545991121770164511e+01,-1.567712397602648977e+01,-2.689114016344712610e+01
+2.411516901153554926e+01,-2.038715461456817124e+01,-2.383481742661471969e+01
+2.537867622506524867e+01,-4.630337276247908029e+00,-3.030095054025095891e+01
+2.600869588066692017e+01,-1.455468535518538964e+01,-2.851196982492563592e+01
+2.623345652322523236e+01,-1.002003177416990276e+01,-2.980437663387418468e+01
+2.596107414157103932e+01,-7.832635439771223673e+00,-2.978567388222689516e+01
+2.333083761918416954e+01,-2.479365120585386251e+01,-1.288695882561743211e+01
+2.733807216117158845e+01,3.675426208697039954e+00,-3.059382421899822191e+01
+2.612742612818355781e+01,4.102759095210952722e-01,-3.056068184466597870e+01
+2.582472653935734641e+01,-9.994117504537875618e+00,-2.940843156094427258e+01
+2.498030516657384226e+01,-1.757517516325876983e+01,-2.578666137670646918e+01
+2.718397366313713093e+01,1.282125168044421493e+01,-2.482776824238119673e+01
+2.524390522628411659e+01,-1.665887024870409761e+01,-2.632389136363828896e+01
+2.427321377757826326e+01,-2.181585714613408555e+01,-2.213654426135629905e+01
+2.822865553065143374e+01,1.027575921679436277e+01,-2.709155080772760016e+01
+2.783445809979478369e+01,1.155749130450795370e+01,-2.472909330684742457e+01
+2.589792523731228258e+01,-5.815642603612385386e+00,-3.082674832937700415e+01
+2.735206748723539150e+01,-1.654895068872628272e+00,-2.980705240831009206e+01
+2.792000183772815802e+01,7.116430885319008581e+00,-2.830961651975295013e+01
+2.802779872801178840e+01,1.097499362550357027e+01,-2.472330556768348231e+01
+2.604767322666315721e+01,-9.170409416638037214e+00,-2.879885449844666567e+01
+2.635717814932284142e+01,-1.634681735633828570e+00,-2.986070763941575734e+01
+2.819886839191068617e+01,1.090378700145044455e+01,-2.598361639664192069e+01
+2.800348363224804871e+01,1.212893064434568124e+01,-2.388674597698715019e+01
+2.712295078823364136e+01,1.236375217337750065e+01,-2.566603941969177782e+01
+2.755082092124272464e+01,8.737393707293122702e+00,-2.743532450241990261e+01
+2.703453660595289065e+01,7.584398539439501263e+00,-2.831522914117201140e+01
+2.771362498481308734e+01,7.467232153714469689e+00,-2.691245060150031776e+01
+2.812931842015370876e+01,4.155779841421759713e+00,-2.819617026608333532e+01
+2.726239787428324846e+01,7.927540014955891223e+00,-2.780215927500725570e+01
+2.804617721546156162e+01,1.424016417817234803e+01,-2.166153171018120105e+01
+2.738791592829496579e+01,6.500227115647193799e+00,-2.854149148467065800e+01
+2.686123024421294403e+01,-5.263932639424545812e+00,-3.002164033909289742e+01
+2.705151057083327260e+01,3.908207119342018032e+00,-2.956792441180240871e+01
+2.759820718404161255e+01,1.232196443318550116e+01,-2.369515477610941900e+01
+2.760745455056906650e+01,5.373035868737551013e+00,-2.838134626937095106e+01
+2.559365807435917262e+01,-6.408745497381122647e+00,-3.015045744622517532e+01
+2.695300118427521596e+01,7.769141218688591977e+00,-2.718707161753179946e+01
+2.797578137149367450e+01,1.163621790391164090e+01,-2.445734439670212623e+01
+2.675353365801597505e+01,1.073948282127522980e+01,-2.561659411295675426e+01
+2.638412100777211577e+01,9.142945441408238949e+00,-2.572150342477528540e+01
+2.815283827604533329e+01,1.020085529611552921e+01,-2.445536057984242717e+01
+2.697009398385699441e+01,-1.061344869159195348e+00,-3.029493340755773545e+01
+2.601201055039280874e+01,-5.950267103208248365e+00,-3.064450298680011997e+01
+2.716532600866198521e+01,4.987841178595598279e+00,-2.763482677010973276e+01
+2.706956391424163755e+01,-1.621923419888668949e+00,-2.990897705521074812e+01
+2.671496061837095226e+01,6.484378286892368948e+00,-2.872453443883717483e+01
+2.655664828496867003e+01,-5.978698862352223919e+00,-3.103614852311505246e+01
+2.760323951513204221e+01,1.280043685947881293e+01,-2.340991492241052896e+01
+2.889130018009085532e+01,1.309801153608050051e+01,-2.295024059951489903e+01
+2.697052325911059611e+01,7.161171353198541922e+00,-2.808600476721761652e+01
+2.798258721308376096e+01,1.394219742787011818e+01,-2.419652681730543264e+01
+2.504056123354465413e+01,-5.562245132830813787e+00,-3.130958362530562056e+01
+2.768812781096057662e+01,6.888244448998847247e+00,-2.689659929685236506e+01
+2.620788593394531318e+01,-1.061491906016868825e+00,-3.051434954278153100e+01
+2.702032455467734096e+01,4.253893439968221557e-01,-3.012724597576129071e+01
+2.699028916897978903e+01,-4.227146549636151107e+00,-2.974920994233877991e+01
+2.749557251632571209e+01,7.577694489253758547e+00,-2.730610388650458020e+01
+2.780559257709388632e+01,9.157339986904265317e+00,-2.804754097157310611e+01
+2.683158239377393173e+01,1.713230133339291861e+00,-2.991583647988129968e+01
+2.744850208293523153e+01,1.254407390450305293e+01,-2.498774780143790508e+01
+2.756213262623451499e+01,1.624881923611249945e+00,-2.935524708771626479e+01
+2.706705482756131786e+01,1.360854514729059339e+01,-2.363473821075596248e+01
+2.844758386596406297e+01,4.885627238651887083e+00,-2.905799269727151568e+01
+2.776611175995396863e+01,5.738431438325685363e+00,-2.755948060303403224e+01
+2.678708184457916985e+01,9.942560485715143059e+00,-2.560596290950687148e+01
+2.852643390382387167e+01,1.224003545136200621e+01,-2.499624405606923006e+01
+2.698752079825024097e+01,7.706313118782572857e+00,-2.842973471918411121e+01
```

### Comparing `transmorph-0.2.6b0/src/transmorph/datasets/data/spirals/spiralB.csv` & `transmorph-0.2.7/src/transmorph/datasets/data/spirals/spiralB.csv`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,663 +1,663 @@
-6.288231846863515884e+00,-9.957513016266172912e+00,2.052031744259442014e+00
-2.187664757190107423e+01,-2.079958410700529114e+01,-1.642695490698600480e+01
-1.721311050515630114e+01,1.981542489102370297e-01,1.113065406866879670e+01
-5.490379321544194724e+00,-9.319793538580666947e+00,1.982100537574760679e+00
-1.367134566400121187e+01,4.955666230517612014e+00,-4.334731738014916402e+00
-1.140264423563923479e+01,-9.660662994810005344e+00,-1.039035574446679178e+01
-5.342770846175468158e+00,-7.064787817268452841e+00,2.977920359528680727e+00
-2.369322651183931328e+01,-1.432866216139283289e+01,-2.203828131861419592e+01
-1.594011115481313468e+01,4.619151222971244586e+00,4.692307455549049600e+00
-6.499106497661962578e+00,-1.133153512055212886e+01,2.118913732934650351e+00
-1.080906507359198798e+01,-6.525758088272249680e+00,-1.026523466698498943e+01
-6.556333799011085262e+00,-1.061305377540915984e+01,2.144259048455944949e+00
-2.929075158039343041e+00,-5.953068741910248818e+00,-3.808203633364732887e-01
-1.297904638339607253e+01,1.456696610600034525e+00,-7.918572770092177748e+00
-6.309235265547667559e+00,-8.885855213093098115e+00,2.091471114828243216e+00
-6.968765080561007963e+00,-9.070070162589312091e+00,3.712899488857235752e+00
-8.905071442536065973e+00,-1.403150564629828168e+01,-3.195270741683479354e+00
-7.101847620133860062e+00,-1.063721392640442787e+01,1.874715573549484482e+00
-4.362535942741251560e+00,-5.713938190505494674e+00,1.350129942869185307e+00
-1.251581606957957682e+01,-2.633542356310522692e+00,-9.490944212634209620e+00
-7.636584994163911233e+00,-1.360049080457358173e+01,-1.287592759595214575e+00
-9.111226649569411862e+00,-1.428603507943711293e+01,-2.710415534797347981e+00
-1.501817630340857157e+01,3.870835309109950551e+00,6.830832270556736141e+00
-4.362217512730367730e+00,-6.466821492528233684e+00,8.138737040758132757e-01
-6.528393214210133522e+00,-1.157409016294481319e+01,2.182500134493769117e+00
-5.628186384095875461e+00,-8.393146065573059644e+00,1.914179067379764732e+00
-2.935506333229600973e+00,-6.654111818472083328e+00,6.521084254319517992e-01
-1.208946183241823391e+01,-3.587576163695978426e+00,-1.001890258092026720e+01
-2.485014687271074862e+01,-1.915279325613446382e+00,-2.258623614937050661e+01
-9.582160487921347780e+00,-1.399533056416461108e+01,-5.469072263978428161e+00
-1.447885245353093353e+01,3.058495539013807551e+00,-5.349600905983349364e+00
-1.875349824483936345e+01,-1.920579656913320576e+01,1.099209200710477319e+01
-1.050125911918851962e+01,-1.174595737959472252e+01,-7.282450329067729378e+00
-7.918319476895185005e+00,-1.209115225941405924e+01,1.676691757003101912e+00
-6.129831269207294042e+00,-8.515025349849473457e+00,2.551153877009085136e+00
-8.374151376459261442e+00,-1.318515109089289972e+01,-1.131063725662658337e+00
-1.258961111934922528e+01,-2.699437102445024550e+00,-1.034215723011696930e+01
-3.007843886718459370e+00,-6.807017696208778723e+00,-5.141797716607114932e-01
-2.434815117930565265e+01,1.560037429864643777e+00,-2.094721049017575609e+01
-1.252718372150153492e+01,1.079288140381623684e+00,-8.338216100559519006e+00
-1.890638368510957434e+01,-1.212067606210131210e+01,1.485897268385905967e+01
-9.154213841601890778e+00,-1.340203759110870863e+01,-7.120491082589706089e-01
-8.241832831426105344e+00,-1.334680345509104171e+01,-1.798901463017805513e+00
-3.590145287165296129e+00,-5.748355277727799972e+00,-4.129280893392439644e-02
-1.467808038914389179e+01,3.436740764410431304e+00,7.281320675425378752e+00
-7.191779635309993424e+00,-1.170530056957410636e+01,1.752096559517208441e+00
-5.917997997038180635e+00,-8.717297232945703911e+00,2.958915039140964431e+00
-1.658685913343362728e+01,-9.100033605054642649e-01,1.280023656196929061e+01
-4.505443027576931492e+00,-7.719297890604655876e+00,1.146344612089289505e+00
-1.382340354075000555e+01,3.978879263863341897e+00,-5.691816123194650245e+00
-6.145338428055142188e+00,-1.062385818698043138e+01,2.126365379001312395e+00
-4.671844005724754112e+00,-6.983735621911425717e+00,2.474887847836762411e+00
-3.759647875590362176e+00,-5.543208876407263119e+00,4.921790262517138359e-01
-5.631116239806615908e+00,-7.577183490976068470e+00,1.373779391459581056e+00
-1.486588424198012781e+01,4.155780650560180867e+00,6.539216165168409312e+00
-3.876845310323536964e+00,-6.642837223592044538e+00,1.897131845500823921e+00
-9.289743927251118194e+00,-1.185837903240850366e+01,-8.741309058475504656e+00
-1.470309078876212361e+01,5.817381448279863143e+00,-6.389239312667196469e-01
-1.481407430392839153e+01,5.979884169145234019e+00,9.518122053446136377e-01
-4.283763827989938378e+00,-6.793696241253256218e+00,1.382455937590880701e+00
-5.648843584229776837e+00,-9.039836497598384923e+00,3.425968137478218267e+00
-1.100272399725878536e+01,-1.308526907371931536e+01,-7.167445860198427887e+00
-1.250701454457395378e+01,-2.927283099328944260e+00,-1.104670206837754343e+01
-1.435676481254507308e+01,3.375590856754283386e+00,-5.485772334084739299e+00
-3.892387518184961870e+00,-6.427723531469395013e+00,1.130925125883621263e+00
-1.711716312151206054e+01,-1.345667991549055031e+00,1.300880191756870197e+01
-1.117275987792079661e+01,-1.016608282360414073e+01,-9.638058220150272248e+00
-1.349190566454513096e+01,3.389267610818401444e+00,-6.477109256481966781e+00
-8.125196416053059423e+00,-1.257422794220364537e+01,5.613509653592598792e-01
-1.303580314071839297e+01,-2.600656400794147061e+00,-1.010716496228548245e+01
-1.308796646243636097e+01,-1.544300413165842656e+00,-9.980404664705064377e+00
-2.210371524183499403e+01,-2.191756252246287318e+01,-1.522202248229947408e+01
-8.873170643369704180e+00,-1.419491142348207191e+01,-4.106973078820706391e+00
-5.739769462145488887e+00,-9.103926384322090115e+00,3.558500146635495298e+00
-1.172262526179484787e+01,-1.008973272836288970e+01,-9.249416522744406066e+00
-1.367559813590182749e+01,6.343742755147462553e+00,-2.933647685524478188e+00
-5.684397012472857114e+00,-8.967159063322743151e+00,2.684440627664646861e+00
-3.983226351997968706e+00,-5.719860564705618877e+00,-5.974275299899820535e-01
-4.294522502377937201e+00,-6.327670804680986194e+00,2.036784089375571760e+00
-2.830898806006420187e+00,-6.800243103987262394e+00,-1.446615001642370668e-01
-7.340335075288143329e+00,-1.173182971443549683e+01,9.921456798524097564e-01
-1.932629014592209415e+01,-1.726170052376386010e+01,1.227922488893439912e+01
-7.735472089980362398e+00,-1.326203508515768092e+01,1.499185854272427232e+00
-9.074042821019613569e+00,-1.311154596880812662e+01,4.453231095429657227e-01
-1.437398913640947207e+01,5.386834763964327699e+00,-3.922267460296471331e-01
-1.033353063039244368e+01,-1.027545818320467319e+01,-8.468985099643802528e+00
-1.586397451677547998e+01,4.055606442420283564e+00,6.959247877529431747e+00
-4.423332904606439797e+00,-7.390556530175671490e+00,1.847390845237481649e+00
-7.405827607837018434e+00,-1.380198509430840836e+01,-6.095979270149837204e-01
-1.820925624054963521e+01,-1.612429224178954357e+01,1.299183710019139326e+01
-1.198306347674564876e+01,-5.449918947940652458e+00,-1.026000854988537192e+01
-1.120931348551781603e+01,-8.947237041990689477e+00,-1.001090126090539556e+01
-1.610995742168998035e+01,3.738312554357807294e+00,6.920898478724561542e+00
-1.114289282783514778e+01,-6.716707642935343614e+00,-1.089068485999379732e+01
-1.601936051661457583e+01,3.572010277191906447e+00,8.340622931303949272e+00
-1.518518242478363867e+01,5.576571903441664979e+00,4.166886417786272112e+00
-1.642649252676431004e+01,2.343898298882721498e+00,9.161233585409920721e+00
-7.672459454877483154e+00,-1.306642388414222822e+01,-6.668998104822975170e-01
-4.276403961706154000e+00,-6.393483146002679973e+00,2.402317439675574207e-01
-1.570516926639700195e+01,4.647155330378557103e+00,3.396035846838542760e+00
-9.237887443380884633e+00,-1.455551380540489959e+01,-2.845404108253942077e+00
-1.249513945337973020e+01,-8.230112389484476765e+00,-1.076660202069384908e+01
-1.964434692876406885e+01,-2.259236260103009286e+01,5.733264465392542419e+00
-6.303006848809401319e+00,-8.347166266150809477e+00,1.665504355958214777e+00
-1.281787255148432081e+01,-5.224692018566123863e-03,-1.055260212760212113e+01
-7.219796113336776955e+00,-1.207957002600227447e+01,2.451160326595247518e-01
-8.579077588577442626e+00,-1.348283863362243196e+01,-7.426859169127066895e-01
-4.826526601611774048e+00,-7.117734150992354181e+00,1.933431092629225745e+00
-4.559589670612213652e+00,-7.110805106779777951e+00,2.106079372001381067e+00
-1.021487878891790935e+01,-1.239875094509357112e+01,-7.677021918229092634e+00
-1.048707044468682348e+01,-1.163221937329391054e+01,-8.639500823643146532e+00
-1.980273600101304865e+01,-1.638600099845477231e+01,1.366655321107174892e+01
-4.018089628903101840e+00,-5.837454387667815325e+00,9.743005378353535306e-01
-8.098588765257280997e+00,-1.173671689521261996e+01,1.485991596029467843e+00
-8.427082222064147032e+00,-1.378528772961098170e+01,-3.181054589478969241e+00
-9.322568470666540819e+00,-1.340201995900376986e+01,-3.710527207448443221e+00
-6.666376930668615586e+00,-9.925115956850365961e+00,2.553476875280018099e+00
-2.188237508154312394e+01,-2.349026482478387123e+01,-1.427711996186906518e+01
-5.284014163308377476e+00,-8.731298087641270911e+00,2.472381872985603746e+00
-4.548046387661584866e+00,-6.340970228718106227e+00,7.856428523594769509e-01
-5.902534960824100452e+00,-8.118731992659188990e+00,2.838554375406613595e+00
-1.848215528957479847e+01,-9.456450182415228056e+00,1.523357722845421414e+01
-7.535978785765470533e+00,-1.315098278358261474e+01,-2.644542177412284589e-01
-2.361753490982256665e+01,-1.343549961855449304e+01,-2.212281722451863430e+01
-4.497382620636345862e+00,-6.939294130683157924e+00,1.528323164442504822e+00
-4.305118675751666402e+00,-6.556853119098221327e+00,1.085208960893526253e+00
-8.105667354739068742e+00,-1.312631563387509814e+01,1.032351781776261745e-01
-6.091499616848219389e+00,-1.255939655758127316e+01,5.725002494928068675e-01
-2.302160300044360497e+01,-9.764154001049179854e+00,-2.267057961909715402e+01
-5.283130741876920666e+00,-7.188925875135224963e+00,2.018514604952407865e+00
-1.592060098048794181e+01,3.660903952763528757e+00,6.870656400785579265e+00
-5.918501407067909170e+00,-8.570562731133316348e+00,2.645541786051554656e+00
-7.285833388948418587e+00,-1.111060752272113916e+01,9.995651523122903725e-01
-1.287265166435936870e+01,-1.006055072379429483e+00,-9.866361103650090669e+00
-1.046779275055465774e+01,-8.976018613372293231e+00,-1.071755766355496853e+01
-1.676226949768923191e+01,-1.922944232974677092e+00,1.307529484852322632e+01
-1.145906797399837984e+01,-6.487302837138908984e+00,-1.138764455896726524e+01
-7.151818352915512378e+00,-9.897444842835772860e+00,3.323889676124068160e+00
-1.492682536749237521e+01,4.899228609609994400e+00,-2.138315517671940391e+00
-2.526545713448393826e+01,-5.074810203482307713e+00,-2.362008570416118403e+01
-1.913257306249501966e+01,-1.954165415444724729e+01,1.058761833454834722e+01
-9.247847000990926603e+00,-1.422126187057345348e+01,-3.706895212594904621e+00
-1.432540837141248247e+01,2.900369822101661832e+00,-7.277477335569630057e+00
-2.522570590584081174e+01,8.576980579674533089e+00,-1.847178489859147987e+01
-1.294948794273073034e+01,9.156830687877537400e-02,-9.048140663569022024e+00
-1.948117885537541838e+01,-2.072980823357816149e+01,9.713160238902872834e+00
-1.132026369529352827e+01,-1.030926652955173495e+01,-8.678811022438761569e+00
-6.835554611203875197e+00,-1.096235229983621018e+01,2.163750442509330352e+00
-1.291940998826090414e+01,9.242819873298122602e-01,-8.937411717094109420e+00
-1.889628904789808672e+01,-8.762613455100002113e+00,1.438615483426989705e+01
-7.879328655098058576e+00,-1.222359507265064948e+01,1.718890316927780937e+00
-1.172351517644431773e+01,-1.267483318448358709e+00,-9.860716156238341412e+00
-1.375771950939861021e+01,3.826096763832210534e+00,-6.062768091351983912e+00
-3.531740362129893285e+00,-6.178850834692473981e+00,1.214953886730141264e-01
-6.659197399447933208e+00,-1.167992691757933699e+01,2.230679018771349664e+00
-6.163432582219554590e+00,-1.103106017366014946e+01,1.872160448398864308e+00
-2.091682423874258134e+01,-2.566597640921174417e+01,3.127564084656944132e-01
-1.268438555744256746e+01,-2.637779770846764293e-01,-9.135649420463956005e+00
-9.217486743061419574e+00,-1.317271850968544555e+01,-6.194888685878982670e+00
-2.675784018062661218e+01,1.363167737802547563e+01,-1.278390249101688170e+01
-4.004060646190088946e+00,-7.066653880632068230e+00,8.383367375519945597e-01
-8.004330115704085813e+00,-1.287243114645671227e+01,9.152107162027300902e-03
-2.403822452804752885e+01,-2.777757821565844942e+00,-2.413393157934739719e+01
-3.892754298611562191e+00,-7.014147694214142525e+00,5.450102185646805708e-01
-1.176989451460309510e+01,-2.059750602530852071e+00,-1.016574878383989677e+01
-1.384918723223139025e+01,4.964763631285319612e+00,-4.303772365165183800e+00
-9.933321400996526052e+00,-1.243101230075391328e+01,-7.256277127261917315e+00
-1.514420156679158858e+01,6.605452410224585513e+00,1.451443649066798791e+00
-2.038936323491558866e+01,-2.421323289630234399e+01,3.284862009127122562e+00
-1.638110360096398921e+01,2.920542563244526768e+00,8.088870699147950205e+00
-2.116560842379331220e+01,-2.433112408862368525e+01,-1.141728662065358257e+01
-1.343114702900522239e+01,1.217658065889410501e+00,-8.648474746917585776e+00
-1.195006682447781721e+01,-6.779871326826201638e+00,-1.077873733983841653e+01
-7.496794719472667623e+00,-1.311344201589071901e+01,1.297072111327940647e+00
-9.193691530380222687e+00,-1.359284603547153480e+01,-3.310192327020687664e+00
-1.577354947873274327e+01,5.183774174743304819e+00,-6.536052847391198295e-01
-1.757521011323161275e+01,-7.579942903961741862e+00,1.482292117793057074e+01
-2.185030578139933155e+01,-2.014323991946699266e+01,-1.709578771698129174e+01
-1.227791524540583623e+01,-2.749617883304248167e+00,-1.060483815263587282e+01
-1.274997019533938492e+01,-2.888399674020094565e-01,-9.231027566219742297e+00
-9.671344151869130101e+00,-1.448014309491348328e+01,-4.104111641976896152e+00
-2.232083427932682440e+01,-2.347530070580327788e+01,-1.362474281700582601e+01
-6.640274452332277200e+00,-1.030451957713977151e+01,2.538979289382405025e+00
-4.212834299205295174e+00,-7.545217094190256546e+00,7.640711758909268791e-01
-5.382551484740540459e+00,-6.204416121425348152e+00,9.962294852635551479e-01
-6.716275072067601215e+00,-1.193217044796193527e+01,1.535643786068982664e+00
-2.442932852098493868e+01,-9.337197157310217932e+00,-2.192751930116482129e+01
-1.516820442385497358e+01,4.655749710251229523e+00,5.879205105204414750e+00
-1.559635883258893152e+01,3.644934466153547881e+00,7.813634860516906144e+00
-5.315656723352200075e+00,-1.014782853717897382e+01,3.033372293754389659e+00
-1.483389044870980022e+01,4.699604991824201328e+00,4.897061155584160552e+00
-6.769781119059002705e+00,-8.459694351200159446e+00,3.071225236228865008e+00
-6.602948443480380014e+00,-8.635017365676093348e+00,1.972659373269798344e+00
-1.927714325065320367e+01,-1.843374957368938638e+01,1.077668429503120429e+01
-2.157478170026825026e+01,-2.625888468724086167e+01,-4.651077848881957522e+00
-2.304105750511821782e+01,-1.578879861552753994e+01,-2.005607161899573754e+01
-8.867345976250527784e+00,-1.365573705057889420e+01,-4.054767345909004561e+00
-2.142752399112806572e+01,-2.456888933758835236e+01,-1.103061582737206159e+01
-2.105295785240834405e+01,-2.610572166155633766e+01,-3.733238867635881864e+00
-1.694722417638339707e+01,-5.590925228671679292e+00,1.528646021312083825e+01
-8.946543439661132524e+00,-1.399095291563432397e+01,-2.309889364703663350e+00
-5.401977224088858165e+00,-8.722030563649443735e+00,2.968939580843279913e+00
-4.049856943533734821e+00,-5.997064896880079488e+00,6.222478103884605538e-01
-2.058681761882220940e+01,-2.587966952480747906e+01,1.923249164768669139e+00
-1.835190203907615114e+01,-1.263236346359370899e+01,1.438351419947290921e+01
-2.316453254434501119e+01,-1.161149692357674645e+01,-2.251428254598699397e+01
-1.614681632512299458e+01,3.992063041452600380e+00,7.001877173251736863e+00
-1.692535297941225991e+01,-3.588960912838104811e+00,1.323066822992836045e+01
-6.455646955041943968e+00,-1.168003371252856937e+01,2.735485348778316617e+00
-9.977076433480387863e+00,-1.320428004163239777e+01,-4.325379620730562813e+00
-1.738078463110154814e+01,-1.567201086165675328e+00,1.197193212011233499e+01
-1.975690775801262689e+01,-2.085945167679798118e+01,1.073542629428292727e+01
-2.411666962390230751e+01,-4.949284350503271313e-01,-2.255909851970879032e+01
-2.212731878264988694e+01,-2.368163296077458924e+01,-1.222118935764122938e+01
-5.275444888912607766e+00,-9.217254317767155314e+00,2.716314760025122510e+00
-2.603866679789941330e+01,1.255708067211281787e+01,-1.607734813615578773e+01
-1.663231240922786824e+01,3.009800643558340205e+00,9.573376926059433245e+00
-7.356480069677280298e+00,-1.245286850419223867e+01,9.655705429989165367e-01
-1.865351338179617002e+01,-1.928768092735901618e+01,1.031077721901173305e+01
-1.616192666763953412e+01,6.765700799671137133e-02,1.243238184235547550e+01
-1.542866292700658093e+01,5.958051995196595563e+00,-2.106599301597515961e+00
-2.113603395821421671e+01,-2.451370420292253627e+01,5.000879889333602613e+00
-1.030822259203822533e+01,-8.986287843219637139e+00,-9.692475997258899412e+00
-6.234561473638162710e+00,-9.759385822771850627e+00,2.545186700604142427e+00
-8.096533205215189710e+00,-1.329014914250574719e+01,4.395487421450807730e-01
-8.296520222873414951e+00,-1.388798675819212747e+01,-9.710791128828140106e-01
-1.819114235606220120e+01,-1.540515376479361720e+01,1.347027400652728168e+01
-7.057089643802001433e+00,-1.326421432521019028e+01,3.518798550989958862e-01
-9.732115949206388450e+00,-1.435959918980491068e+01,-5.185351596562727039e+00
-1.185694685957471783e+01,-5.057996720673837210e+00,-1.108943935606792230e+01
-4.530400784272819337e+00,-6.256372857316624625e+00,6.586791399703511019e-01
-3.349812065588268162e+00,-6.779397634002383377e+00,-1.240286714673597857e+00
-2.146341648139993197e+01,-2.660777124457761644e+01,-3.389762562866063700e+00
-1.308237306424228485e+01,4.352320420073632512e+00,-5.350499308728395853e+00
-1.800373151033933183e+01,-1.285774377312631778e+01,1.478866223856763895e+01
-1.018648335611039712e+01,-1.283365905594977008e+01,-7.511617015082380888e+00
-6.924615076669036640e+00,-9.797280052931242267e+00,2.236129806542396015e+00
-7.432926965748006154e+00,-1.369962705481234266e+01,-1.173955482613406653e+00
-1.057642079885968300e+01,-9.074320833752832272e+00,-9.381515398935764694e+00
-8.310079901938806302e+00,-1.228694456736275598e+01,9.001210538958508423e-01
-1.908861216936588789e+01,-1.985382830051395686e+01,1.132181237257862350e+01
-7.608766580205125862e+00,-1.323780709723172144e+01,-1.458528837184169591e+00
-1.540201235615190534e+01,4.808021136397685247e+00,5.645811741397412931e+00
-1.784608758683472018e+01,-1.537607585012980849e+01,1.252475874716186333e+01
-1.535810960133968450e+01,5.332182149309660169e+00,-1.018371338679251004e+00
-1.264912413941907765e+01,-2.391541051031203402e+00,-1.084924617517901169e+01
-1.391433731541126662e+01,5.166950367235631170e+00,-4.780744703437450838e+00
-9.563446090624756479e+00,-1.335704122179495812e+01,-4.963050430276335412e+00
-1.686508753241843195e+01,4.575450534383049828e-01,1.082972299063093935e+01
-1.054329231894819685e+01,-1.141705317447024193e+01,-8.273241151233284185e+00
-2.303320968798100310e+01,-6.201085005790710980e+00,-2.222523507704035950e+01
-1.080258498001853873e+01,-6.244715700622299082e+00,-1.062284955630264704e+01
-4.587845809211865244e+00,-6.550370794511183981e+00,1.532502025716993010e+00
-8.084370059733993585e+00,-1.343543213269004610e+01,4.691028945591577681e-01
-1.787579348156884507e+01,-9.332585837803719642e+00,1.497599947128181874e+01
-1.124427403634775935e+01,-1.007962423321477807e+01,-9.063620017544558038e+00
-7.799746796327159615e+00,-1.385798120134865385e+01,-1.425022216799118002e+00
-1.507239651303152783e+01,4.939261739857516709e+00,5.146613539189506703e+00
-1.739695700836085379e+01,-3.178956579554215622e+00,1.300900704644130279e+01
-1.290591895909028253e+01,-1.493057928959551361e-02,-8.858213548206691712e+00
-1.666597223636445335e+01,-9.594520374240111948e-02,1.318253093102315354e+01
-6.278041897447139696e+00,-8.924910011142356936e+00,2.608785299661021018e+00
-1.314385300518510213e+01,3.948360671057609572e+00,-7.040527392736676937e+00
-7.552098014464831977e+00,-1.099904009994869725e+01,2.719063595523874000e+00
-2.044655519539495714e+01,-2.668793147665486032e+01,-2.415341813578053554e+00
-2.007305352280492272e+01,-2.102848573071651828e+01,9.908056523333272025e+00
-1.560617285690837797e+01,3.950061643555016211e+00,7.709647521675821125e+00
-1.267485903113503198e+01,3.406524304738596243e-01,-9.875588326728069077e+00
-1.789623270738916005e+01,-8.502000367654853008e+00,1.497805746641985358e+01
-1.319745580478087099e+01,-5.787126412757448435e-02,-9.620904531638734269e+00
-2.326205682132209418e+01,-2.117885373478931044e+01,-1.548282609951922417e+01
-2.004398025559033414e+01,-2.267562946414561509e+01,6.519035029705677609e+00
-8.876592494157177882e+00,-1.338345096216514563e+01,-1.157434678727616850e+00
-1.622967206312772248e+01,1.240736974842318041e+00,1.159223460029143737e+01
-2.466435567898806269e+01,1.449598889586996897e+00,-2.292637852703687429e+01
-7.569343502746830765e+00,-1.199896204122193311e+01,-2.042951303879747549e-02
-1.918039414902924378e+01,-2.296026826032343493e+01,7.695938964401673132e+00
-7.742116571145245985e+00,-1.207038051323297267e+01,-1.045523723622201029e+00
-1.954844697756890781e+01,-2.497747114942972857e+01,3.952796794391016277e+00
-1.632427519780853942e+01,-1.783078568638595485e+00,1.412767282896855470e+01
-1.409727647945056361e+01,3.873100726490512180e+00,-3.577401371992735335e+00
-1.031884754955862427e+01,-1.262216056454711044e+01,-7.134917344974503806e+00
-2.937458513883744793e+00,-6.765288902987050434e+00,-2.221560622287870324e-01
-1.085263562130505122e+01,-1.014624561361925359e+01,-9.795169759143107058e+00
-5.826389637659663556e+00,-9.153196310421051862e+00,2.627246911971151455e+00
-1.514377478176687930e+01,4.512784479882667732e+00,-3.337757641539422782e+00
-2.484038927267795316e+01,1.217744048381815247e+01,-1.511872807152568576e+01
-1.851631613994898018e+01,-1.026987847102076756e+01,1.413782392054822523e+01
-1.406607403714526328e+01,1.381349956154383385e+00,-8.803572034282003855e+00
-1.152052869369916444e+01,-3.447819071847617600e+00,-1.103757569461125065e+01
-1.120468256631661852e+01,-7.368015102201546540e+00,-1.051437023945115534e+01
-1.332094856423278451e+01,-4.764051555049769071e+00,-1.038435617552582713e+01
-1.247388343970132674e+01,2.746724186812557811e+00,-5.739848149657846399e+00
-1.478179881016299824e+01,5.550117913368130651e+00,-2.633744008712073370e-01
-1.924121134888230600e+01,-1.253280795188469732e+01,1.445388466258891569e+01
-2.266183447260117134e+01,-2.310117242247675051e+01,-1.500941277311370392e+01
-6.020817089602879868e+00,-8.010772181906260059e+00,1.618174629146450716e+00
-2.146858878343033794e+01,-2.566067087017313497e+01,-7.218945277621401146e+00
-1.621256315922986957e+01,5.919355100845893780e+00,4.528911125540989069e+00
-1.197503561018772089e+01,-2.154366725714136344e+00,-1.082257403592566725e+01
-2.260205125172374707e+01,-8.268643692696924674e+00,-2.294178621022025055e+01
-2.004461859943096513e+01,-2.436965450312537129e+01,2.937884862741822367e+00
-1.567606010710446540e+01,5.344252917539971115e+00,2.040208019968922315e+00
-2.169422551370177388e+01,-2.106789008152881237e+01,-1.587971612052708004e+01
-2.221965699456329801e+01,-2.588664956883840063e+01,-6.771008754194609125e+00
-2.085741094550907704e+01,-2.605311242369706548e+01,4.557028347666771673e-01
-1.074590033931101196e+01,-1.270706431596138763e+01,-8.047059739424870628e+00
-1.735484497851404484e+01,-1.250824704150740985e+00,1.199064945858849462e+01
-2.445933549648849947e+01,-4.118481382849403794e+00,-2.297878133734609918e+01
-1.014323127900081012e+01,-1.187611179979089648e+01,-8.403026356414832421e+00
-2.260904573600389256e+01,-1.863161453443731119e+01,-1.909024576376092597e+01
-2.145067552974443714e+01,-2.317859466533477786e+01,-1.212906041132544921e+01
-1.982425240820114709e+01,-2.282094286210035960e+01,7.420015285746851319e+00
-7.327613982080942279e+00,-1.107305804113166481e+01,2.066667338340721471e+00
-2.555153850102290036e+01,6.180383615763603622e+00,-2.102182077582616415e+01
-1.010697896581174682e+01,-1.258935117940922055e+01,-7.175211844356872426e+00
-2.154766513879960144e+01,-2.611031196747577710e+01,-5.346359265526682281e-01
-9.496625848582096907e+00,-1.410778795569997257e+01,-5.968105287310561557e+00
-6.140069449915493749e+00,-1.022186404165284657e+01,1.716588144442932951e+00
-2.006398435122285306e+01,-2.572118106724387232e+01,3.073294019530954380e+00
-1.634210110038220520e+01,2.411386924941541388e+00,9.539566218726717395e+00
-1.333723542256096017e+01,-5.987427015427559951e-02,-8.088827329609149075e+00
-1.283700502012248990e+01,-1.689074747536980503e+00,-1.068989404373356678e+01
-2.310573782779740171e+01,-1.729058651112188372e+01,-1.909006285753892485e+01
-5.304777440068442651e+00,-8.130126364332484812e+00,1.750262709010497630e+00
-2.252858568549002882e+01,-2.372640349761774559e+01,-1.232975866943885457e+01
-2.208418114146449085e+01,-2.028370712760799321e+01,-1.695770381091592327e+01
-1.996927680529851656e+01,-2.287761180674238304e+01,7.078070894113842826e+00
-1.162251991464229661e+01,-4.718992903388377513e+00,-1.107152990939307635e+01
-6.428318122441837090e+00,-9.868145229349664760e+00,2.752442290572005845e+00
-2.303719699520223330e+01,-1.387290489523010706e+01,-2.190364096787549641e+01
-1.470593111242053830e+01,5.908486490501513977e+00,2.730773799320538764e+00
-1.411680731443424008e+01,5.397611975436901410e+00,2.474768750828486574e+00
-1.355850624968552154e+01,2.443457423942230200e+00,-7.695788590747113744e+00
-1.120676749642655068e+01,-5.570864006448433159e+00,-1.024452388559919491e+01
-8.691923485842419694e+00,-1.462767666864503724e+01,-2.188972930889909740e+00
-2.518115028719757476e+01,1.215851110385398570e+01,-1.519615810617602669e+01
-1.890933598233750956e+01,-1.619827022668360783e+01,1.343000528578523145e+01
-2.055448295269335901e+01,-2.654261260327181304e+01,8.321203577417006780e-01
-2.243057567024769483e+01,-2.387056591223324631e+01,-1.243294891769894228e+01
-1.519004865572293994e+01,6.168149322069871765e+00,1.579605541963419402e+00
-7.803139098699933385e+00,-1.187290142245653435e+01,1.218277795002848940e+00
-1.837140427362895778e+01,-1.744744651221009235e+01,1.153390362701948924e+01
-4.134863094071127065e+00,-6.182302608878023520e+00,-2.213789348070631657e-01
-6.544053333615087453e+00,-1.006556234584045662e+01,2.914355995508532082e+00
-7.820180475908495410e+00,-1.330239558372155528e+01,-7.588846193196074896e-01
-5.372584408457768745e+00,-8.819357855259688961e+00,3.235939946687333979e+00
-2.286377763416580322e+01,-1.765191665693305723e+01,-2.027646530523981738e+01
-8.056307689539272232e+00,-1.364611708005502066e+01,-1.040532892853164748e+00
-2.600976152592165036e+01,1.269663433014256171e+01,-1.285699486202717523e+01
-9.940668257046679557e+00,-1.014383127056241207e+01,-1.005082842541397170e+01
-6.574758807114739589e+00,-1.136817086323861226e+01,2.785048798150224325e+00
-6.369261158515968191e+00,-7.943204395371625814e+00,2.957743211633388825e+00
-2.606360939411646527e+01,1.422140106999828646e+01,-1.180268130805715465e+01
-9.012430006743267441e+00,-1.376117257492106205e+01,-1.572921304338365189e+00
-2.295966359104549426e+01,-1.996047796099093219e+01,-1.765791743066063191e+01
-1.241351129673464726e+01,2.101316146321847711e-01,-7.731090973179729708e+00
-1.963097992002737513e+01,-1.905828544243102129e+01,1.180537728672040743e+01
-2.411233048153641434e+01,-7.183212962803311896e+00,-2.410767467382302698e+01
-2.253297924065808999e+01,-2.547951871682246150e+01,-4.624078443846567410e+00
-1.513536096375898055e+01,5.241752333011606702e+00,9.483876988222101900e-01
-1.937963886323884566e+01,-2.417531196867813748e+01,5.352943612762063097e+00
-2.228539007655298221e+01,-1.969341740923589157e+01,-1.828596072354638835e+01
-8.189519961118961078e+00,-1.413583843012129471e+01,-2.070776080929076279e+00
-8.727764168634033481e+00,-1.352830841420886543e+01,-3.529263129994613113e+00
-2.051230003833839888e+01,-2.611849087780997536e+01,1.865159573028842388e+00
-3.926271882453408413e+00,-5.752096378302901769e+00,-2.677184075298010280e-01
-1.611559207664653570e+01,1.568581967629328666e+00,8.144646646921355426e+00
-4.344650508285765156e+00,-7.254256633761306361e+00,1.191899550041862987e+00
-1.476276238952588038e+01,5.714416346904468647e+00,-3.169914330750125853e+00
-1.200397207704018676e+01,-9.817620591742697300e-01,-1.145867620924562580e+01
-4.490847332300337058e+00,-6.293705266938934173e+00,1.381139407157638832e+00
-2.346540651556653856e+01,-3.934336763083390309e+00,-2.381999810272223783e+01
-5.814343584659583897e+00,-7.221266268386170140e+00,1.144062159828406422e+00
-1.171299681733527365e+01,-7.074753794871936563e+00,-1.098999308272407838e+01
-6.757423901690621904e+00,-9.135381974823129525e+00,2.618165125446557440e+00
-2.214758774109295558e+01,-2.090085068222564146e+01,-1.668425931786434546e+01
-2.150984395551909500e+01,-2.552209603002873450e+01,-5.421972340492052567e+00
-2.619234089989640424e+01,1.579553883051059771e+01,-8.241139126873921583e+00
-3.660743059926329757e+00,-5.558203873922593630e+00,1.894669290098610848e+00
-2.274068271626153503e+01,-1.547939021787257019e+01,-2.039722667304535264e+01
-5.415970524385222973e+00,-9.012901930175438281e+00,2.589761883319367186e+00
-1.375977899697920392e+01,4.300219957350324584e+00,-4.254886591257382555e+00
-6.905830163223500406e+00,-1.149875398671117388e+01,2.132586697383511698e+00
-1.700640818295847723e+01,-5.741444477684074954e+00,1.370167499120037746e+01
-1.420336862032664271e+01,4.053527896125662444e+00,-4.514147740919165486e+00
-2.141727526128607906e+01,-2.614292271913464560e+01,-1.861854534335793732e+00
-1.344877849252288193e+01,1.582781494894556218e-01,-8.818973822700286291e+00
-1.036491562453851145e+01,-8.943700672690336972e+00,-9.873658612949256508e+00
-2.573593731721301836e+01,7.560287275386760264e+00,-1.930020715846036694e+01
-1.436134828034665922e+01,6.115002230910394410e+00,4.976206164045708924e-01
-1.142219912645135516e+01,-7.185156908378232288e+00,-1.121111731985273963e+01
-1.195529737073526810e+01,-2.905812972811709471e+00,-1.008431664735532962e+01
-1.149081485861253427e+01,-1.115954035822642076e+01,-8.650606950801510209e+00
-2.417261289879074937e+01,-3.492455184616749087e+00,-2.323556101387963224e+01
-1.177802250054865318e+01,-8.332203738393664239e+00,-1.017820988979364571e+01
-1.373497658884353356e+01,-2.700480995789344973e-01,-9.464090776641770120e+00
-2.152704765736172732e+01,-2.344858663440417601e+01,-1.323309251430787725e+01
-1.384914686628341940e+01,1.783346535357503093e+00,-7.641983367288610829e+00
-1.580745021393452099e+01,2.868352997211364830e+00,8.254973744418835579e+00
-5.706443707247517594e+00,-7.088941595804350904e+00,6.207023962635940251e-01
-1.042439783809316367e+01,-1.072242817210399579e+01,-9.230449121451632877e+00
-9.155633357772419600e+00,-1.302522463613280479e+01,-2.140737549715580279e+00
-5.618876757550852474e+00,-7.062180682240769336e+00,2.312431458133238138e+00
-9.406666130707060702e+00,-1.343964908951016390e+01,-4.860304384624765106e+00
-1.676731795417415327e+01,-4.737193813489671612e+00,1.378436120540708743e+01
-1.695329152296762487e+01,-3.006724904370758011e+00,1.368326442054545033e+01
-1.312033120070528724e+01,1.900623582474310069e-01,-8.944644944556923605e+00
-1.608757631590937720e+01,2.355885062506741789e-01,1.136776235125385170e+01
-1.154874864832947523e+01,-8.559654253984671612e+00,-1.016263144265091078e+01
-1.166891807930378633e+01,-8.444221035425533373e+00,-9.699911153927244456e+00
-2.457659789454210042e+01,5.598583367487428575e-01,-2.261664699667650069e+01
-2.075437602466496045e+01,-2.483565044189185400e+01,2.199623915982989342e+00
-2.685143565702432866e+01,1.686817486700240565e+01,-7.388017870346942573e+00
-2.134682298489288499e+01,-2.722862334944046481e+01,-4.144509326962807272e+00
-2.318353753772999326e+01,-1.651606298559597974e+01,-2.048273521535046626e+01
-1.326959036710392859e+01,2.368462582872120414e+00,-8.144275356931142795e+00
-4.046237088802604021e+00,-6.547436703799695223e+00,1.320427605345359190e+00
-1.346283255024571979e+01,2.525295005896233569e+00,-7.512172642262189726e+00
-2.199036093205726061e+01,-2.528661685409227289e+01,-9.718852110966340163e+00
-1.837265922542116670e+01,-1.748057946613262459e+01,1.284465499197332328e+01
-1.926520136917274684e+01,-2.190309771714446185e+01,8.220488962923797160e+00
-1.514428800522444618e+01,5.483726771845106818e+00,3.521974003103575335e+00
-1.458570537094653830e+01,4.834081378752377312e+00,-2.028768550078621224e+00
-2.178352453464813365e+01,-2.444383458084961447e+01,-1.008930925699115022e+01
-1.754000838178522415e+01,-5.102946298347888821e+00,1.484907239367638887e+01
-1.848138672102928126e+01,-3.685909693195588588e+00,1.410956567511424353e+01
-8.490056753706092252e+00,-1.399387560633241279e+01,-3.184614855211155948e+00
-1.593399702611558233e+01,3.471860802704106241e+00,8.600079893442066137e+00
-2.407251145979249074e+01,-7.275314599565289697e+00,-2.293056341124427178e+01
-1.674062446819076655e+01,3.229096180334520838e-01,1.117455835242325790e+01
-2.318127904916508086e+01,-1.799868130264278321e+01,-2.001899437270137838e+01
-1.950173304683986331e+01,-2.384171968365481220e+01,5.219354714995962041e+00
-1.965210941325579341e+01,-2.287669379624462707e+01,8.100994143573656103e+00
-1.469344728774298225e+01,5.212563538731541435e+00,1.598701742430525652e+00
-5.346173693169625096e+00,-8.319401231280000530e+00,1.194088321693766108e+00
-5.110591289743826593e+00,-6.997531052589042844e+00,2.157163858721566463e+00
-1.443178869012463572e+01,5.515670387612275682e+00,-1.735841800585647077e+00
-7.565199111351599726e+00,-1.260704881821683898e+01,1.124178289514855322e+00
-1.164067433415608654e+01,-2.610287265168273585e+00,-1.039228261371419570e+01
-1.740487215868784077e+01,-6.511306261435822584e+00,1.488785078831362974e+01
-6.834885784505054573e+00,-1.093743100544909908e+01,2.320005463001990176e+00
-9.144855924113519663e+00,-1.401964303614456853e+01,-2.138005378872123163e+00
-1.586235800599064838e+01,4.778534523520366228e+00,7.274253445721596378e+00
-9.148031070109642116e+00,-1.348698655243187794e+01,-2.100658987607335160e+00
-1.404664595027373863e+01,6.192260803135337888e+00,-2.640193020971708826e+00
-1.591777613058741458e+01,2.359485362839534695e+00,8.758307168235621276e+00
-1.834881731932261673e+01,-1.581595398885556847e+01,1.339976709661184984e+01
-2.533975326385773030e+01,1.106271223788852609e+01,-1.625033146410964946e+01
-1.211897280971400015e+01,-4.283172979347898313e+00,-1.137089778754230984e+01
-1.881070214214910763e+01,-2.112689295714271509e+01,1.026357360928932749e+01
-1.551625352738800068e+01,5.337816302659873280e+00,2.714653795052834884e+00
-1.992612429376245942e+01,-2.067497187014286908e+01,9.229301963058745173e+00
-1.301077012640076624e+01,1.874017247512113293e+00,-7.879441181951912121e+00
-2.103040013645074424e+01,-2.620814018238652565e+01,-4.987010539490871253e+00
-2.343682922868167751e+01,-8.965896590435001201e+00,-2.274414014640029791e+01
-1.591036310395064746e+01,1.668039854149161449e+00,8.721806624841301314e+00
-2.107423059849663005e+01,-2.444883676074177359e+01,-1.239793422074283313e+01
-1.011944366862372924e+01,-1.239294726155507576e+01,-7.559240297673714970e+00
-2.047255955100037639e+01,-2.578645203183630841e+01,-3.244903615313937451e+00
-2.617190568366683223e+01,6.225627451056479522e+00,-2.049007250998361229e+01
-2.482861620317560991e+01,7.216136007521627427e+00,-1.977306215073611639e+01
-2.471378090179000253e+01,9.503117979314019692e+00,-1.756960639987511286e+01
-2.525486694104066387e+01,1.596594399662877706e+01,-1.049568444805337997e+01
-1.439272813773745163e+01,4.366053161670669702e+00,-3.649759661751583284e+00
-1.635759280915426928e+01,4.031987925356458113e+00,7.767877271182909382e+00
-2.356198070123604182e+01,-1.822954817147143558e+01,-1.896024799305326525e+01
-2.235984099275620451e+01,-2.171092298182126967e+01,-1.614928214096586601e+01
-1.231588686790117038e+01,-4.738422573257817128e+00,-1.065588623787593470e+01
-2.328591774017433380e+01,-1.435695467409254888e+01,-2.182094160420029283e+01
-1.995312579795000829e+01,-2.440100209300568679e+01,4.946117771382794182e+00
-1.348041423580614406e+01,3.276257422221878990e+00,-6.421842598117234679e+00
-2.188766005590647978e+01,-2.398774153560882638e+01,-1.320312262336140030e+01
-1.102446289076129027e+01,-7.570488681308882306e+00,-1.093550140324746245e+01
-1.196874207185018335e+01,-2.745031332381755895e+00,-1.000715935701159331e+01
-1.424399871419267960e+01,3.505045400301617597e+00,-6.079064877201169281e+00
-2.397922359666646486e+01,-1.296537512259452818e+01,-2.179293936565116496e+01
-1.336533167075202400e+01,4.603436355560464044e+00,-3.373879340115852443e+00
-5.938607938211756476e+00,-7.683512989569407203e+00,2.038761651845470091e+00
-1.980799998129430506e+01,-2.389792816372647266e+01,4.656594621077291052e+00
-9.675417472144237863e+00,-1.386926557863174736e+01,-5.113922205504518814e+00
-2.356265868702679356e+01,-1.645651021807132608e+01,-2.096977909413447350e+01
-6.324787403454191548e+00,-1.210174153949093601e+01,1.207578850941470439e+00
-1.987608245310292432e+01,-2.491779585406550979e+01,3.476832096257118643e+00
-2.166577332205659800e+01,-2.588683754544189242e+01,-7.662473641644264255e+00
-1.777791658847976208e+01,-1.733874005808248242e+00,1.292781460709049135e+01
-1.915675138440426295e+01,-1.574542699556009850e+01,1.298079466846799690e+01
-1.936133839447892413e+01,-2.258549612512778992e+01,8.932596615713553234e+00
-2.508224380307736823e+01,9.326140559975229394e+00,-1.731136423179978578e+01
-1.033153225912175266e+01,-1.322798655280663382e+01,-3.755390409371381022e+00
-2.273624498405809646e+01,-2.372688928811433939e+01,-1.299385610502396737e+01
-1.281159418393686167e+01,2.345679902572524789e+00,-6.755005604810242481e+00
-2.087337640845328224e+01,-2.578531874126039014e+01,1.146283800838699296e+00
-1.497918575942056307e+01,6.304899421829968098e+00,-1.391397209818867164e+00
-1.685316037526309429e+01,-7.731630158540535369e+00,1.505736578244114376e+01
-4.816848230152659838e+00,-7.750396459533855698e+00,3.000555204229509165e-01
-9.230077114576102915e+00,-1.426845895826724053e+01,-4.178769101199424796e+00
-1.651160409690649544e+01,3.263921521465877440e+00,7.199048956468736549e+00
-1.249212150104483143e+01,-9.019591941644033994e-01,-9.542055152861269818e+00
-1.518538046542044384e+01,4.550891139085806891e+00,9.212176538977243645e-01
-1.736980297190575939e+01,-5.425910891778216616e+00,1.461729866570997416e+01
-2.538919219967998941e+01,1.454172297412333847e+01,-1.037648205588952166e+01
-2.194266140642715612e+01,-2.700004337951372335e+01,-4.571966439612294764e+00
-1.693820151115191308e+01,-3.350957884659627961e+00,1.334577316904475452e+01
-1.972508113054781020e+01,-2.448981549856138784e+01,6.972184227882037177e+00
-2.114640405397779332e+01,-2.526490958564891187e+01,6.294405030680498836e-01
-2.026684435570955500e+01,-2.410053076486639867e+01,4.823298534617702416e+00
-2.054563130721570374e+01,-2.381046802047153221e+01,4.505289725573802251e+00
-1.413262987179951402e+01,5.356208577396571080e+00,2.107904807204953990e+00
-8.371088352783994324e+00,-1.287717515405282498e+01,1.688852401958146121e+00
-1.982009133905154741e+01,-2.472690303757821084e+01,3.826025210174446300e+00
-1.494284654692304315e+01,4.850093485455801989e+00,4.335101641582176590e+00
-1.192213701262360814e+01,-3.501344234853501103e+00,-1.114254194934554931e+01
-1.233125195761659754e+01,-8.626258161535549362e-01,-1.061759428889177848e+01
-2.638839236734244764e+01,1.834452674876221678e+01,-6.999820692063727812e+00
-1.412397515453787911e+01,4.441732843787595364e+00,-5.517895724700044857e-01
-4.994824099780398541e+00,-7.261416708424443200e+00,1.260607884431212522e+00
-1.110064285975399656e+01,-6.620883852693684624e+00,-1.173676778265741127e+01
-1.855707569312059135e+01,-8.920363398032657543e+00,1.364393162557992234e+01
-1.978070282394129720e+01,-2.035478665156414380e+01,1.004620212823427927e+01
-1.572779598008688851e+01,5.554710985947908242e-01,1.123561803361210920e+01
-1.470697866715481972e+01,5.435173225054987789e+00,-2.062569184868013217e+00
-1.293061332723554102e+01,-4.685140869903676730e+00,-1.089962554432043085e+01
-2.241035207182362754e+01,-2.399378848098107397e+01,-1.189840913936498801e+01
-1.125993631758902680e+01,-1.207155524718314510e+01,-5.962420331831191689e+00
-1.531584927794298956e+01,3.061669515235398542e+00,7.163400228070599951e+00
-1.920738614237074771e+01,-2.414166517817354318e+01,4.692921273099221580e+00
-2.374613099988856035e+01,-8.195621953135528770e+00,-2.273139334049360372e+01
-2.589645733174912223e+01,1.629021518787582323e+01,-7.093422758445099952e+00
-8.401498436674268433e+00,-1.375333963384859182e+01,-1.526590180308619704e+00
-1.586639494505238623e+01,6.006716052845892939e+00,4.315000450142298050e+00
-2.513654507694387163e+01,1.968634505849039762e+00,-2.311989977173310251e+01
-1.809923627117503031e+01,-4.719864513570952269e+00,1.374649989926335714e+01
-1.864401842156636846e+01,-2.102054923980609402e+01,9.377730542984135553e+00
-1.939743784762634249e+01,-2.232957098451484512e+01,8.396294876585335132e+00
-6.189757914907195513e+00,-9.104834579712303366e+00,2.300321804968418427e+00
-2.426912514320380510e+01,-1.257603916733168958e+00,-2.235223539902650458e+01
-4.385945785902803706e+00,-6.020456244686851477e+00,7.209501608316684074e-01
-1.752114654911539660e+01,-6.018537008577111713e+00,1.454175432476469432e+01
-2.156129079745074861e+01,-2.640390757720264858e+01,-1.613852437426660735e+00
-1.455680215858329696e+01,5.236741018159229988e+00,-1.488454555034077753e+00
-2.619923939777534017e+01,1.484866306750926412e+01,-1.181042587901669272e+01
-1.705440259833099148e+01,-8.244656415078146949e+00,1.374964385274364354e+01
-1.080153365534254917e+01,-9.683647671249412170e+00,-8.989563743717930322e+00
-1.939268890837919201e+01,-2.548357895886853441e+01,3.517011595359853970e+00
-1.791315200899453330e+01,-1.510750957582581577e+01,1.358471692980101153e+01
-2.370137948008053641e+01,-9.259651195862208084e+00,-2.257335784680862645e+01
-2.543812305418260067e+01,1.309718143086379172e+01,-1.445957355987915172e+01
-9.675745852056484964e+00,-1.351672692400412856e+01,-4.102153151661007691e+00
-3.562233324218383679e+00,-5.926985926816761285e+00,-1.381561208221213644e-01
-1.932128103412230757e+01,-1.968452249925336517e+01,1.077223160678077640e+01
-8.478193983471308925e+00,-1.117119337743558916e+01,1.385156770313188623e+00
-1.810490221456069193e+01,-1.237342421336984266e+01,1.413672831435098232e+01
-1.528368910781727763e+01,4.818825764667333367e+00,4.849977460912127114e+00
-2.658573070843726782e+01,1.770688487574752656e+01,-5.828596864892722884e+00
-1.339346592897467936e+01,5.240770276693830887e+00,-2.949411944642311934e+00
-2.087361754167300276e+01,-2.529008986983027185e+01,-9.056942649094953168e+00
-2.455422212869780907e+01,2.616510307857105921e+00,-2.172615902846477098e+01
-1.902070105076570883e+01,-2.263886737796014970e+01,8.420564772554000044e+00
-2.527377626624629059e+01,8.374927252351710649e+00,-1.826049177166931514e+01
-2.628169339837640450e+01,1.383684441492921025e+01,-1.251458237250198025e+01
-2.119693917636971037e+01,-2.555942930923443512e+01,4.012111483905216325e-01
-2.263666765791331059e+01,-1.970368613436385985e+01,-1.671772466938027080e+01
-1.804141541097152412e+01,-8.461943245659396595e+00,1.352662153520397048e+01
-1.874792423780163375e+01,-2.103387313582268092e+01,9.307922198149290338e+00
-2.090805364583402337e+01,-2.544519391541260944e+01,1.431894941073290184e+00
-1.870416924915054580e+01,-1.332562212510831401e+01,1.310645060560786135e+01
-2.670410961206907885e+01,1.635935294860294675e+01,-5.561533850067672091e+00
-2.661641054630572967e+01,1.621457304123468646e+01,-9.001407978243616270e+00
-1.757398433184464892e+01,-7.339404394859850633e+00,1.443033385079859876e+01
-1.754747881493114647e+01,-4.144721857408338650e+00,1.360067587365037056e+01
-1.718421179237487095e+01,-2.988453632785307512e+00,1.365579728223067590e+01
-1.445302845037893391e+01,6.504977689999114965e+00,1.049455131217200243e+00
-2.514203303839694925e+01,2.100934095051690598e+00,-2.138964893013869073e+01
-1.462087223024265015e+01,5.731317779403812374e+00,1.072510489729729954e+00
-1.723046503318723666e+01,-2.060815661550527089e+00,1.197201202633523565e+01
-1.340466975572003960e+01,-1.234611707301389139e+00,-1.016839919287774308e+01
-2.127560429156662636e+01,-2.593942714722985698e+01,-1.187111503594445949e+00
-1.746324131747647712e+01,-7.311422990095265639e+00,1.464599213321039883e+01
-1.993560849490860676e+01,-2.090348994318480891e+01,1.075555268253570773e+01
-7.638469377559760076e+00,-1.268195232816358597e+01,5.018570059805065320e-01
-2.385432293392500469e+01,-9.963009128057283448e+00,-2.331031261340206129e+01
-1.133054212698301733e+01,-8.192475635926486532e+00,-1.011757458401461562e+01
-7.494620485987201874e+00,-1.295863403921326551e+01,1.545094465835450848e+00
-1.967677668432564886e+01,-1.913027294056395533e+01,1.148326616798142297e+01
-1.923668568746521501e+01,-1.260224840252439193e+01,1.441667731003316710e+01
-2.246520538455834526e+01,-2.621201998499466868e+01,-6.470950115760444987e+00
-2.471914090975780809e+01,-1.768178453888226365e+00,-2.157038603308539848e+01
-7.435199307165166971e+00,-1.200506094789014888e+01,1.451093811805416856e+00
-2.581364644679286258e+01,1.160065633335593560e+01,-1.556437603488778088e+01
-2.162524493232928791e+01,-2.561889480923573359e+01,-6.599768179724442518e+00
-2.558104538331870259e+01,6.038256943281870015e+00,-2.144167203683432632e+01
-2.051658077269308222e+01,-2.633362517895839261e+01,3.709260337434128196e-02
-4.938047559673222509e+00,-7.147856578053565002e+00,1.879307635610208305e+00
-2.239577772728431526e+01,-2.444446218459414766e+01,-1.188063944678044237e+01
-5.414179412726998208e+00,-7.682703213544816556e+00,2.088781840202358797e+00
-2.112859735411380768e+01,-2.459629545000203876e+01,-1.145295621808573472e+01
-1.885333068470767870e+01,-2.183916671060952908e+01,9.401207128951051928e+00
-2.421132464566532150e+01,-3.935730645589023968e+00,-2.336864962840157744e+01
-1.206020262603299642e+01,-5.065351968902742641e-01,-9.792602190405750306e+00
-2.468568725636113825e+01,3.322011953546867069e+00,-2.131221738420153144e+01
-2.235877571572716960e+01,-2.116280535855354117e+01,-1.663432908783774877e+01
-9.453304426202329580e+00,-1.336618033301169994e+01,-6.947726434666460449e+00
-1.951982111259196984e+01,-1.982512898884142061e+01,1.168821505935973626e+01
-1.380786147525128449e+01,2.296157115368532509e+00,-7.963788272971132010e+00
-1.629076430939239017e+01,-2.011042016403104427e+00,1.319261740755360179e+01
-2.199220212690133280e+01,-2.586589133179847622e+01,-2.243436891808469724e+00
-2.486509972065838880e+01,8.885375939253705724e+00,-1.764686177552493263e+01
-9.262216704199971673e+00,-1.457673436558977542e+01,-1.421147656495748812e+00
-2.265686173130742986e+01,-2.540279881120788019e+01,-1.064263991704245882e+01
-2.528926509631806496e+01,7.876282434112353847e+00,-1.899884356304903577e+01
-2.174124479787587561e+01,-2.582917137102553440e+01,-9.039713057945650831e+00
-2.606373133903819195e+01,1.253240524356625230e+01,-1.389308140114126111e+01
-1.964003667383432727e+01,-2.048658127374620719e+01,8.928204049326204483e+00
-1.621157228674842088e+01,1.350655339574911018e+00,1.081343639535893075e+01
-1.565935190747207884e+01,2.811394350390323815e+00,9.292806315020158081e+00
-2.097877746103495866e+01,-2.491270915590614266e+01,3.455756327161361163e+00
-2.097136260699557653e+01,-2.468210048800793643e+01,3.293143939006740517e+00
-2.581946439776644553e+01,1.785021044451976024e+01,-4.879026458799026855e+00
-5.377013781098723300e+00,-8.856008563756073926e+00,2.317097449855962665e+00
-1.510693040645124796e+01,4.701540744398914562e+00,5.282082480462396923e+00
-2.546826427071196619e+01,4.549811003070890258e+00,-2.125644532632559702e+01
-7.341696513224130527e+00,-1.145830254395111680e+01,1.972034154540442508e+00
-2.245830541721123552e+01,-2.483415315969391557e+01,-1.115825686096097158e+01
-2.551753367344477752e+01,6.762650241879920365e+00,-1.952051681734236865e+01
-1.464455903800639369e+01,5.326728163785118930e+00,-3.553170888014037132e+00
-1.063321973957261157e+01,-8.992246457676619897e+00,-9.975421183052016971e+00
-1.530000725556413599e+01,5.101844962992619692e+00,-9.188724914814785372e-01
-2.540687271364042488e+01,9.473514715245386242e+00,-1.696110244895483277e+01
-8.198666498090684485e+00,-1.378548704173702077e+01,-4.911752274273016639e+00
-1.572986550804393779e+01,2.846878348088725197e+00,8.298194295697189915e+00
-2.029741634705190023e+01,-2.587077253483554884e+01,4.790251610927698245e-01
-1.813907543037277037e+01,-1.822792700624311024e+01,1.248696196688529980e+01
-2.580999574825163378e+01,1.161044416937404833e+01,-1.551079718000966068e+01
-1.586235695390923084e+01,3.887414422108860457e+00,4.776448543070914710e+00
-2.519655465233795866e+01,-9.017265225481260416e+00,-2.298176485406207092e+01
-2.471010832751492359e+01,-6.592459442765898459e+00,-2.293831898722635287e+01
-2.449467567175208771e+01,-8.567370750619147657e-01,-2.285983210996698034e+01
-9.960230181439836628e+00,-1.227227613819709617e+01,-6.346030696773343749e+00
-1.846703276591660270e+01,-1.135070131073076993e+01,1.398154733043795872e+01
-1.093463363304534752e+01,-4.933371061817548586e+00,-1.031745292549059734e+01
-2.304315238562634960e+01,-1.599328918790850906e+01,-2.036755501341412611e+01
-1.052802713381784550e+01,-9.196555665029098492e+00,-1.120933002873744933e+01
-2.333404696641204268e+01,-1.327207208758834511e+01,-2.167099340107120753e+01
-2.148057940478388161e+01,-2.322916256514355737e+01,-1.390143530443905284e+01
-1.953070502494668048e+01,-2.491147985424986189e+01,5.174280318261995859e+00
-2.456506235036209773e+01,-4.530217416105457140e+00,-2.353940483003152195e+01
-9.160844475883656912e+00,-1.352642830644638394e+01,-5.325184892158300265e+00
-1.150867978980838302e+01,-3.886184338854294928e+00,-9.253397216282344573e+00
-2.558698802774866010e+01,1.514452157180459935e+01,-1.148958485979931865e+01
-1.533278111660303722e+01,5.689119138391936836e+00,3.105152045176828857e+00
-3.176250365714620827e+00,-6.745153865379862168e+00,-6.323997746955005717e-01
-2.624135454850302196e+01,1.449761777314100542e+01,-1.046802057760974947e+01
-1.142992224270783197e+01,-8.461000773740524394e+00,-1.040279173201102303e+01
-2.041232477576469151e+01,-2.522550129027365884e+01,-5.123015956210185129e-01
-2.419059803106427253e+01,3.447520851032373379e+00,-2.158746673808884964e+01
-2.160877640047978332e+01,-2.501880882350765489e+01,-7.364530242511582614e+00
-2.656708798627344592e+01,1.627064431966952895e+01,-7.767922182091026251e+00
-2.164092009693748153e+01,-2.662741372758210900e+01,-4.184209908426014479e+00
-6.581392776941481060e+00,-1.079802001828051949e+01,2.543134247841539519e+00
-2.733118796526959571e+01,1.069265969992130749e+01,-1.693345150683806821e+01
-4.380606945618692016e+00,-6.951838930503489777e+00,1.280163859347801747e+00
-1.204722405349341940e+01,1.050121972104467893e+00,-8.915908770873940625e+00
+6.288231846863515884e+00,-9.957513016266172912e+00,2.052031744259442014e+00
+2.187664757190107423e+01,-2.079958410700529114e+01,-1.642695490698600480e+01
+1.721311050515630114e+01,1.981542489102370297e-01,1.113065406866879670e+01
+5.490379321544194724e+00,-9.319793538580666947e+00,1.982100537574760679e+00
+1.367134566400121187e+01,4.955666230517612014e+00,-4.334731738014916402e+00
+1.140264423563923479e+01,-9.660662994810005344e+00,-1.039035574446679178e+01
+5.342770846175468158e+00,-7.064787817268452841e+00,2.977920359528680727e+00
+2.369322651183931328e+01,-1.432866216139283289e+01,-2.203828131861419592e+01
+1.594011115481313468e+01,4.619151222971244586e+00,4.692307455549049600e+00
+6.499106497661962578e+00,-1.133153512055212886e+01,2.118913732934650351e+00
+1.080906507359198798e+01,-6.525758088272249680e+00,-1.026523466698498943e+01
+6.556333799011085262e+00,-1.061305377540915984e+01,2.144259048455944949e+00
+2.929075158039343041e+00,-5.953068741910248818e+00,-3.808203633364732887e-01
+1.297904638339607253e+01,1.456696610600034525e+00,-7.918572770092177748e+00
+6.309235265547667559e+00,-8.885855213093098115e+00,2.091471114828243216e+00
+6.968765080561007963e+00,-9.070070162589312091e+00,3.712899488857235752e+00
+8.905071442536065973e+00,-1.403150564629828168e+01,-3.195270741683479354e+00
+7.101847620133860062e+00,-1.063721392640442787e+01,1.874715573549484482e+00
+4.362535942741251560e+00,-5.713938190505494674e+00,1.350129942869185307e+00
+1.251581606957957682e+01,-2.633542356310522692e+00,-9.490944212634209620e+00
+7.636584994163911233e+00,-1.360049080457358173e+01,-1.287592759595214575e+00
+9.111226649569411862e+00,-1.428603507943711293e+01,-2.710415534797347981e+00
+1.501817630340857157e+01,3.870835309109950551e+00,6.830832270556736141e+00
+4.362217512730367730e+00,-6.466821492528233684e+00,8.138737040758132757e-01
+6.528393214210133522e+00,-1.157409016294481319e+01,2.182500134493769117e+00
+5.628186384095875461e+00,-8.393146065573059644e+00,1.914179067379764732e+00
+2.935506333229600973e+00,-6.654111818472083328e+00,6.521084254319517992e-01
+1.208946183241823391e+01,-3.587576163695978426e+00,-1.001890258092026720e+01
+2.485014687271074862e+01,-1.915279325613446382e+00,-2.258623614937050661e+01
+9.582160487921347780e+00,-1.399533056416461108e+01,-5.469072263978428161e+00
+1.447885245353093353e+01,3.058495539013807551e+00,-5.349600905983349364e+00
+1.875349824483936345e+01,-1.920579656913320576e+01,1.099209200710477319e+01
+1.050125911918851962e+01,-1.174595737959472252e+01,-7.282450329067729378e+00
+7.918319476895185005e+00,-1.209115225941405924e+01,1.676691757003101912e+00
+6.129831269207294042e+00,-8.515025349849473457e+00,2.551153877009085136e+00
+8.374151376459261442e+00,-1.318515109089289972e+01,-1.131063725662658337e+00
+1.258961111934922528e+01,-2.699437102445024550e+00,-1.034215723011696930e+01
+3.007843886718459370e+00,-6.807017696208778723e+00,-5.141797716607114932e-01
+2.434815117930565265e+01,1.560037429864643777e+00,-2.094721049017575609e+01
+1.252718372150153492e+01,1.079288140381623684e+00,-8.338216100559519006e+00
+1.890638368510957434e+01,-1.212067606210131210e+01,1.485897268385905967e+01
+9.154213841601890778e+00,-1.340203759110870863e+01,-7.120491082589706089e-01
+8.241832831426105344e+00,-1.334680345509104171e+01,-1.798901463017805513e+00
+3.590145287165296129e+00,-5.748355277727799972e+00,-4.129280893392439644e-02
+1.467808038914389179e+01,3.436740764410431304e+00,7.281320675425378752e+00
+7.191779635309993424e+00,-1.170530056957410636e+01,1.752096559517208441e+00
+5.917997997038180635e+00,-8.717297232945703911e+00,2.958915039140964431e+00
+1.658685913343362728e+01,-9.100033605054642649e-01,1.280023656196929061e+01
+4.505443027576931492e+00,-7.719297890604655876e+00,1.146344612089289505e+00
+1.382340354075000555e+01,3.978879263863341897e+00,-5.691816123194650245e+00
+6.145338428055142188e+00,-1.062385818698043138e+01,2.126365379001312395e+00
+4.671844005724754112e+00,-6.983735621911425717e+00,2.474887847836762411e+00
+3.759647875590362176e+00,-5.543208876407263119e+00,4.921790262517138359e-01
+5.631116239806615908e+00,-7.577183490976068470e+00,1.373779391459581056e+00
+1.486588424198012781e+01,4.155780650560180867e+00,6.539216165168409312e+00
+3.876845310323536964e+00,-6.642837223592044538e+00,1.897131845500823921e+00
+9.289743927251118194e+00,-1.185837903240850366e+01,-8.741309058475504656e+00
+1.470309078876212361e+01,5.817381448279863143e+00,-6.389239312667196469e-01
+1.481407430392839153e+01,5.979884169145234019e+00,9.518122053446136377e-01
+4.283763827989938378e+00,-6.793696241253256218e+00,1.382455937590880701e+00
+5.648843584229776837e+00,-9.039836497598384923e+00,3.425968137478218267e+00
+1.100272399725878536e+01,-1.308526907371931536e+01,-7.167445860198427887e+00
+1.250701454457395378e+01,-2.927283099328944260e+00,-1.104670206837754343e+01
+1.435676481254507308e+01,3.375590856754283386e+00,-5.485772334084739299e+00
+3.892387518184961870e+00,-6.427723531469395013e+00,1.130925125883621263e+00
+1.711716312151206054e+01,-1.345667991549055031e+00,1.300880191756870197e+01
+1.117275987792079661e+01,-1.016608282360414073e+01,-9.638058220150272248e+00
+1.349190566454513096e+01,3.389267610818401444e+00,-6.477109256481966781e+00
+8.125196416053059423e+00,-1.257422794220364537e+01,5.613509653592598792e-01
+1.303580314071839297e+01,-2.600656400794147061e+00,-1.010716496228548245e+01
+1.308796646243636097e+01,-1.544300413165842656e+00,-9.980404664705064377e+00
+2.210371524183499403e+01,-2.191756252246287318e+01,-1.522202248229947408e+01
+8.873170643369704180e+00,-1.419491142348207191e+01,-4.106973078820706391e+00
+5.739769462145488887e+00,-9.103926384322090115e+00,3.558500146635495298e+00
+1.172262526179484787e+01,-1.008973272836288970e+01,-9.249416522744406066e+00
+1.367559813590182749e+01,6.343742755147462553e+00,-2.933647685524478188e+00
+5.684397012472857114e+00,-8.967159063322743151e+00,2.684440627664646861e+00
+3.983226351997968706e+00,-5.719860564705618877e+00,-5.974275299899820535e-01
+4.294522502377937201e+00,-6.327670804680986194e+00,2.036784089375571760e+00
+2.830898806006420187e+00,-6.800243103987262394e+00,-1.446615001642370668e-01
+7.340335075288143329e+00,-1.173182971443549683e+01,9.921456798524097564e-01
+1.932629014592209415e+01,-1.726170052376386010e+01,1.227922488893439912e+01
+7.735472089980362398e+00,-1.326203508515768092e+01,1.499185854272427232e+00
+9.074042821019613569e+00,-1.311154596880812662e+01,4.453231095429657227e-01
+1.437398913640947207e+01,5.386834763964327699e+00,-3.922267460296471331e-01
+1.033353063039244368e+01,-1.027545818320467319e+01,-8.468985099643802528e+00
+1.586397451677547998e+01,4.055606442420283564e+00,6.959247877529431747e+00
+4.423332904606439797e+00,-7.390556530175671490e+00,1.847390845237481649e+00
+7.405827607837018434e+00,-1.380198509430840836e+01,-6.095979270149837204e-01
+1.820925624054963521e+01,-1.612429224178954357e+01,1.299183710019139326e+01
+1.198306347674564876e+01,-5.449918947940652458e+00,-1.026000854988537192e+01
+1.120931348551781603e+01,-8.947237041990689477e+00,-1.001090126090539556e+01
+1.610995742168998035e+01,3.738312554357807294e+00,6.920898478724561542e+00
+1.114289282783514778e+01,-6.716707642935343614e+00,-1.089068485999379732e+01
+1.601936051661457583e+01,3.572010277191906447e+00,8.340622931303949272e+00
+1.518518242478363867e+01,5.576571903441664979e+00,4.166886417786272112e+00
+1.642649252676431004e+01,2.343898298882721498e+00,9.161233585409920721e+00
+7.672459454877483154e+00,-1.306642388414222822e+01,-6.668998104822975170e-01
+4.276403961706154000e+00,-6.393483146002679973e+00,2.402317439675574207e-01
+1.570516926639700195e+01,4.647155330378557103e+00,3.396035846838542760e+00
+9.237887443380884633e+00,-1.455551380540489959e+01,-2.845404108253942077e+00
+1.249513945337973020e+01,-8.230112389484476765e+00,-1.076660202069384908e+01
+1.964434692876406885e+01,-2.259236260103009286e+01,5.733264465392542419e+00
+6.303006848809401319e+00,-8.347166266150809477e+00,1.665504355958214777e+00
+1.281787255148432081e+01,-5.224692018566123863e-03,-1.055260212760212113e+01
+7.219796113336776955e+00,-1.207957002600227447e+01,2.451160326595247518e-01
+8.579077588577442626e+00,-1.348283863362243196e+01,-7.426859169127066895e-01
+4.826526601611774048e+00,-7.117734150992354181e+00,1.933431092629225745e+00
+4.559589670612213652e+00,-7.110805106779777951e+00,2.106079372001381067e+00
+1.021487878891790935e+01,-1.239875094509357112e+01,-7.677021918229092634e+00
+1.048707044468682348e+01,-1.163221937329391054e+01,-8.639500823643146532e+00
+1.980273600101304865e+01,-1.638600099845477231e+01,1.366655321107174892e+01
+4.018089628903101840e+00,-5.837454387667815325e+00,9.743005378353535306e-01
+8.098588765257280997e+00,-1.173671689521261996e+01,1.485991596029467843e+00
+8.427082222064147032e+00,-1.378528772961098170e+01,-3.181054589478969241e+00
+9.322568470666540819e+00,-1.340201995900376986e+01,-3.710527207448443221e+00
+6.666376930668615586e+00,-9.925115956850365961e+00,2.553476875280018099e+00
+2.188237508154312394e+01,-2.349026482478387123e+01,-1.427711996186906518e+01
+5.284014163308377476e+00,-8.731298087641270911e+00,2.472381872985603746e+00
+4.548046387661584866e+00,-6.340970228718106227e+00,7.856428523594769509e-01
+5.902534960824100452e+00,-8.118731992659188990e+00,2.838554375406613595e+00
+1.848215528957479847e+01,-9.456450182415228056e+00,1.523357722845421414e+01
+7.535978785765470533e+00,-1.315098278358261474e+01,-2.644542177412284589e-01
+2.361753490982256665e+01,-1.343549961855449304e+01,-2.212281722451863430e+01
+4.497382620636345862e+00,-6.939294130683157924e+00,1.528323164442504822e+00
+4.305118675751666402e+00,-6.556853119098221327e+00,1.085208960893526253e+00
+8.105667354739068742e+00,-1.312631563387509814e+01,1.032351781776261745e-01
+6.091499616848219389e+00,-1.255939655758127316e+01,5.725002494928068675e-01
+2.302160300044360497e+01,-9.764154001049179854e+00,-2.267057961909715402e+01
+5.283130741876920666e+00,-7.188925875135224963e+00,2.018514604952407865e+00
+1.592060098048794181e+01,3.660903952763528757e+00,6.870656400785579265e+00
+5.918501407067909170e+00,-8.570562731133316348e+00,2.645541786051554656e+00
+7.285833388948418587e+00,-1.111060752272113916e+01,9.995651523122903725e-01
+1.287265166435936870e+01,-1.006055072379429483e+00,-9.866361103650090669e+00
+1.046779275055465774e+01,-8.976018613372293231e+00,-1.071755766355496853e+01
+1.676226949768923191e+01,-1.922944232974677092e+00,1.307529484852322632e+01
+1.145906797399837984e+01,-6.487302837138908984e+00,-1.138764455896726524e+01
+7.151818352915512378e+00,-9.897444842835772860e+00,3.323889676124068160e+00
+1.492682536749237521e+01,4.899228609609994400e+00,-2.138315517671940391e+00
+2.526545713448393826e+01,-5.074810203482307713e+00,-2.362008570416118403e+01
+1.913257306249501966e+01,-1.954165415444724729e+01,1.058761833454834722e+01
+9.247847000990926603e+00,-1.422126187057345348e+01,-3.706895212594904621e+00
+1.432540837141248247e+01,2.900369822101661832e+00,-7.277477335569630057e+00
+2.522570590584081174e+01,8.576980579674533089e+00,-1.847178489859147987e+01
+1.294948794273073034e+01,9.156830687877537400e-02,-9.048140663569022024e+00
+1.948117885537541838e+01,-2.072980823357816149e+01,9.713160238902872834e+00
+1.132026369529352827e+01,-1.030926652955173495e+01,-8.678811022438761569e+00
+6.835554611203875197e+00,-1.096235229983621018e+01,2.163750442509330352e+00
+1.291940998826090414e+01,9.242819873298122602e-01,-8.937411717094109420e+00
+1.889628904789808672e+01,-8.762613455100002113e+00,1.438615483426989705e+01
+7.879328655098058576e+00,-1.222359507265064948e+01,1.718890316927780937e+00
+1.172351517644431773e+01,-1.267483318448358709e+00,-9.860716156238341412e+00
+1.375771950939861021e+01,3.826096763832210534e+00,-6.062768091351983912e+00
+3.531740362129893285e+00,-6.178850834692473981e+00,1.214953886730141264e-01
+6.659197399447933208e+00,-1.167992691757933699e+01,2.230679018771349664e+00
+6.163432582219554590e+00,-1.103106017366014946e+01,1.872160448398864308e+00
+2.091682423874258134e+01,-2.566597640921174417e+01,3.127564084656944132e-01
+1.268438555744256746e+01,-2.637779770846764293e-01,-9.135649420463956005e+00
+9.217486743061419574e+00,-1.317271850968544555e+01,-6.194888685878982670e+00
+2.675784018062661218e+01,1.363167737802547563e+01,-1.278390249101688170e+01
+4.004060646190088946e+00,-7.066653880632068230e+00,8.383367375519945597e-01
+8.004330115704085813e+00,-1.287243114645671227e+01,9.152107162027300902e-03
+2.403822452804752885e+01,-2.777757821565844942e+00,-2.413393157934739719e+01
+3.892754298611562191e+00,-7.014147694214142525e+00,5.450102185646805708e-01
+1.176989451460309510e+01,-2.059750602530852071e+00,-1.016574878383989677e+01
+1.384918723223139025e+01,4.964763631285319612e+00,-4.303772365165183800e+00
+9.933321400996526052e+00,-1.243101230075391328e+01,-7.256277127261917315e+00
+1.514420156679158858e+01,6.605452410224585513e+00,1.451443649066798791e+00
+2.038936323491558866e+01,-2.421323289630234399e+01,3.284862009127122562e+00
+1.638110360096398921e+01,2.920542563244526768e+00,8.088870699147950205e+00
+2.116560842379331220e+01,-2.433112408862368525e+01,-1.141728662065358257e+01
+1.343114702900522239e+01,1.217658065889410501e+00,-8.648474746917585776e+00
+1.195006682447781721e+01,-6.779871326826201638e+00,-1.077873733983841653e+01
+7.496794719472667623e+00,-1.311344201589071901e+01,1.297072111327940647e+00
+9.193691530380222687e+00,-1.359284603547153480e+01,-3.310192327020687664e+00
+1.577354947873274327e+01,5.183774174743304819e+00,-6.536052847391198295e-01
+1.757521011323161275e+01,-7.579942903961741862e+00,1.482292117793057074e+01
+2.185030578139933155e+01,-2.014323991946699266e+01,-1.709578771698129174e+01
+1.227791524540583623e+01,-2.749617883304248167e+00,-1.060483815263587282e+01
+1.274997019533938492e+01,-2.888399674020094565e-01,-9.231027566219742297e+00
+9.671344151869130101e+00,-1.448014309491348328e+01,-4.104111641976896152e+00
+2.232083427932682440e+01,-2.347530070580327788e+01,-1.362474281700582601e+01
+6.640274452332277200e+00,-1.030451957713977151e+01,2.538979289382405025e+00
+4.212834299205295174e+00,-7.545217094190256546e+00,7.640711758909268791e-01
+5.382551484740540459e+00,-6.204416121425348152e+00,9.962294852635551479e-01
+6.716275072067601215e+00,-1.193217044796193527e+01,1.535643786068982664e+00
+2.442932852098493868e+01,-9.337197157310217932e+00,-2.192751930116482129e+01
+1.516820442385497358e+01,4.655749710251229523e+00,5.879205105204414750e+00
+1.559635883258893152e+01,3.644934466153547881e+00,7.813634860516906144e+00
+5.315656723352200075e+00,-1.014782853717897382e+01,3.033372293754389659e+00
+1.483389044870980022e+01,4.699604991824201328e+00,4.897061155584160552e+00
+6.769781119059002705e+00,-8.459694351200159446e+00,3.071225236228865008e+00
+6.602948443480380014e+00,-8.635017365676093348e+00,1.972659373269798344e+00
+1.927714325065320367e+01,-1.843374957368938638e+01,1.077668429503120429e+01
+2.157478170026825026e+01,-2.625888468724086167e+01,-4.651077848881957522e+00
+2.304105750511821782e+01,-1.578879861552753994e+01,-2.005607161899573754e+01
+8.867345976250527784e+00,-1.365573705057889420e+01,-4.054767345909004561e+00
+2.142752399112806572e+01,-2.456888933758835236e+01,-1.103061582737206159e+01
+2.105295785240834405e+01,-2.610572166155633766e+01,-3.733238867635881864e+00
+1.694722417638339707e+01,-5.590925228671679292e+00,1.528646021312083825e+01
+8.946543439661132524e+00,-1.399095291563432397e+01,-2.309889364703663350e+00
+5.401977224088858165e+00,-8.722030563649443735e+00,2.968939580843279913e+00
+4.049856943533734821e+00,-5.997064896880079488e+00,6.222478103884605538e-01
+2.058681761882220940e+01,-2.587966952480747906e+01,1.923249164768669139e+00
+1.835190203907615114e+01,-1.263236346359370899e+01,1.438351419947290921e+01
+2.316453254434501119e+01,-1.161149692357674645e+01,-2.251428254598699397e+01
+1.614681632512299458e+01,3.992063041452600380e+00,7.001877173251736863e+00
+1.692535297941225991e+01,-3.588960912838104811e+00,1.323066822992836045e+01
+6.455646955041943968e+00,-1.168003371252856937e+01,2.735485348778316617e+00
+9.977076433480387863e+00,-1.320428004163239777e+01,-4.325379620730562813e+00
+1.738078463110154814e+01,-1.567201086165675328e+00,1.197193212011233499e+01
+1.975690775801262689e+01,-2.085945167679798118e+01,1.073542629428292727e+01
+2.411666962390230751e+01,-4.949284350503271313e-01,-2.255909851970879032e+01
+2.212731878264988694e+01,-2.368163296077458924e+01,-1.222118935764122938e+01
+5.275444888912607766e+00,-9.217254317767155314e+00,2.716314760025122510e+00
+2.603866679789941330e+01,1.255708067211281787e+01,-1.607734813615578773e+01
+1.663231240922786824e+01,3.009800643558340205e+00,9.573376926059433245e+00
+7.356480069677280298e+00,-1.245286850419223867e+01,9.655705429989165367e-01
+1.865351338179617002e+01,-1.928768092735901618e+01,1.031077721901173305e+01
+1.616192666763953412e+01,6.765700799671137133e-02,1.243238184235547550e+01
+1.542866292700658093e+01,5.958051995196595563e+00,-2.106599301597515961e+00
+2.113603395821421671e+01,-2.451370420292253627e+01,5.000879889333602613e+00
+1.030822259203822533e+01,-8.986287843219637139e+00,-9.692475997258899412e+00
+6.234561473638162710e+00,-9.759385822771850627e+00,2.545186700604142427e+00
+8.096533205215189710e+00,-1.329014914250574719e+01,4.395487421450807730e-01
+8.296520222873414951e+00,-1.388798675819212747e+01,-9.710791128828140106e-01
+1.819114235606220120e+01,-1.540515376479361720e+01,1.347027400652728168e+01
+7.057089643802001433e+00,-1.326421432521019028e+01,3.518798550989958862e-01
+9.732115949206388450e+00,-1.435959918980491068e+01,-5.185351596562727039e+00
+1.185694685957471783e+01,-5.057996720673837210e+00,-1.108943935606792230e+01
+4.530400784272819337e+00,-6.256372857316624625e+00,6.586791399703511019e-01
+3.349812065588268162e+00,-6.779397634002383377e+00,-1.240286714673597857e+00
+2.146341648139993197e+01,-2.660777124457761644e+01,-3.389762562866063700e+00
+1.308237306424228485e+01,4.352320420073632512e+00,-5.350499308728395853e+00
+1.800373151033933183e+01,-1.285774377312631778e+01,1.478866223856763895e+01
+1.018648335611039712e+01,-1.283365905594977008e+01,-7.511617015082380888e+00
+6.924615076669036640e+00,-9.797280052931242267e+00,2.236129806542396015e+00
+7.432926965748006154e+00,-1.369962705481234266e+01,-1.173955482613406653e+00
+1.057642079885968300e+01,-9.074320833752832272e+00,-9.381515398935764694e+00
+8.310079901938806302e+00,-1.228694456736275598e+01,9.001210538958508423e-01
+1.908861216936588789e+01,-1.985382830051395686e+01,1.132181237257862350e+01
+7.608766580205125862e+00,-1.323780709723172144e+01,-1.458528837184169591e+00
+1.540201235615190534e+01,4.808021136397685247e+00,5.645811741397412931e+00
+1.784608758683472018e+01,-1.537607585012980849e+01,1.252475874716186333e+01
+1.535810960133968450e+01,5.332182149309660169e+00,-1.018371338679251004e+00
+1.264912413941907765e+01,-2.391541051031203402e+00,-1.084924617517901169e+01
+1.391433731541126662e+01,5.166950367235631170e+00,-4.780744703437450838e+00
+9.563446090624756479e+00,-1.335704122179495812e+01,-4.963050430276335412e+00
+1.686508753241843195e+01,4.575450534383049828e-01,1.082972299063093935e+01
+1.054329231894819685e+01,-1.141705317447024193e+01,-8.273241151233284185e+00
+2.303320968798100310e+01,-6.201085005790710980e+00,-2.222523507704035950e+01
+1.080258498001853873e+01,-6.244715700622299082e+00,-1.062284955630264704e+01
+4.587845809211865244e+00,-6.550370794511183981e+00,1.532502025716993010e+00
+8.084370059733993585e+00,-1.343543213269004610e+01,4.691028945591577681e-01
+1.787579348156884507e+01,-9.332585837803719642e+00,1.497599947128181874e+01
+1.124427403634775935e+01,-1.007962423321477807e+01,-9.063620017544558038e+00
+7.799746796327159615e+00,-1.385798120134865385e+01,-1.425022216799118002e+00
+1.507239651303152783e+01,4.939261739857516709e+00,5.146613539189506703e+00
+1.739695700836085379e+01,-3.178956579554215622e+00,1.300900704644130279e+01
+1.290591895909028253e+01,-1.493057928959551361e-02,-8.858213548206691712e+00
+1.666597223636445335e+01,-9.594520374240111948e-02,1.318253093102315354e+01
+6.278041897447139696e+00,-8.924910011142356936e+00,2.608785299661021018e+00
+1.314385300518510213e+01,3.948360671057609572e+00,-7.040527392736676937e+00
+7.552098014464831977e+00,-1.099904009994869725e+01,2.719063595523874000e+00
+2.044655519539495714e+01,-2.668793147665486032e+01,-2.415341813578053554e+00
+2.007305352280492272e+01,-2.102848573071651828e+01,9.908056523333272025e+00
+1.560617285690837797e+01,3.950061643555016211e+00,7.709647521675821125e+00
+1.267485903113503198e+01,3.406524304738596243e-01,-9.875588326728069077e+00
+1.789623270738916005e+01,-8.502000367654853008e+00,1.497805746641985358e+01
+1.319745580478087099e+01,-5.787126412757448435e-02,-9.620904531638734269e+00
+2.326205682132209418e+01,-2.117885373478931044e+01,-1.548282609951922417e+01
+2.004398025559033414e+01,-2.267562946414561509e+01,6.519035029705677609e+00
+8.876592494157177882e+00,-1.338345096216514563e+01,-1.157434678727616850e+00
+1.622967206312772248e+01,1.240736974842318041e+00,1.159223460029143737e+01
+2.466435567898806269e+01,1.449598889586996897e+00,-2.292637852703687429e+01
+7.569343502746830765e+00,-1.199896204122193311e+01,-2.042951303879747549e-02
+1.918039414902924378e+01,-2.296026826032343493e+01,7.695938964401673132e+00
+7.742116571145245985e+00,-1.207038051323297267e+01,-1.045523723622201029e+00
+1.954844697756890781e+01,-2.497747114942972857e+01,3.952796794391016277e+00
+1.632427519780853942e+01,-1.783078568638595485e+00,1.412767282896855470e+01
+1.409727647945056361e+01,3.873100726490512180e+00,-3.577401371992735335e+00
+1.031884754955862427e+01,-1.262216056454711044e+01,-7.134917344974503806e+00
+2.937458513883744793e+00,-6.765288902987050434e+00,-2.221560622287870324e-01
+1.085263562130505122e+01,-1.014624561361925359e+01,-9.795169759143107058e+00
+5.826389637659663556e+00,-9.153196310421051862e+00,2.627246911971151455e+00
+1.514377478176687930e+01,4.512784479882667732e+00,-3.337757641539422782e+00
+2.484038927267795316e+01,1.217744048381815247e+01,-1.511872807152568576e+01
+1.851631613994898018e+01,-1.026987847102076756e+01,1.413782392054822523e+01
+1.406607403714526328e+01,1.381349956154383385e+00,-8.803572034282003855e+00
+1.152052869369916444e+01,-3.447819071847617600e+00,-1.103757569461125065e+01
+1.120468256631661852e+01,-7.368015102201546540e+00,-1.051437023945115534e+01
+1.332094856423278451e+01,-4.764051555049769071e+00,-1.038435617552582713e+01
+1.247388343970132674e+01,2.746724186812557811e+00,-5.739848149657846399e+00
+1.478179881016299824e+01,5.550117913368130651e+00,-2.633744008712073370e-01
+1.924121134888230600e+01,-1.253280795188469732e+01,1.445388466258891569e+01
+2.266183447260117134e+01,-2.310117242247675051e+01,-1.500941277311370392e+01
+6.020817089602879868e+00,-8.010772181906260059e+00,1.618174629146450716e+00
+2.146858878343033794e+01,-2.566067087017313497e+01,-7.218945277621401146e+00
+1.621256315922986957e+01,5.919355100845893780e+00,4.528911125540989069e+00
+1.197503561018772089e+01,-2.154366725714136344e+00,-1.082257403592566725e+01
+2.260205125172374707e+01,-8.268643692696924674e+00,-2.294178621022025055e+01
+2.004461859943096513e+01,-2.436965450312537129e+01,2.937884862741822367e+00
+1.567606010710446540e+01,5.344252917539971115e+00,2.040208019968922315e+00
+2.169422551370177388e+01,-2.106789008152881237e+01,-1.587971612052708004e+01
+2.221965699456329801e+01,-2.588664956883840063e+01,-6.771008754194609125e+00
+2.085741094550907704e+01,-2.605311242369706548e+01,4.557028347666771673e-01
+1.074590033931101196e+01,-1.270706431596138763e+01,-8.047059739424870628e+00
+1.735484497851404484e+01,-1.250824704150740985e+00,1.199064945858849462e+01
+2.445933549648849947e+01,-4.118481382849403794e+00,-2.297878133734609918e+01
+1.014323127900081012e+01,-1.187611179979089648e+01,-8.403026356414832421e+00
+2.260904573600389256e+01,-1.863161453443731119e+01,-1.909024576376092597e+01
+2.145067552974443714e+01,-2.317859466533477786e+01,-1.212906041132544921e+01
+1.982425240820114709e+01,-2.282094286210035960e+01,7.420015285746851319e+00
+7.327613982080942279e+00,-1.107305804113166481e+01,2.066667338340721471e+00
+2.555153850102290036e+01,6.180383615763603622e+00,-2.102182077582616415e+01
+1.010697896581174682e+01,-1.258935117940922055e+01,-7.175211844356872426e+00
+2.154766513879960144e+01,-2.611031196747577710e+01,-5.346359265526682281e-01
+9.496625848582096907e+00,-1.410778795569997257e+01,-5.968105287310561557e+00
+6.140069449915493749e+00,-1.022186404165284657e+01,1.716588144442932951e+00
+2.006398435122285306e+01,-2.572118106724387232e+01,3.073294019530954380e+00
+1.634210110038220520e+01,2.411386924941541388e+00,9.539566218726717395e+00
+1.333723542256096017e+01,-5.987427015427559951e-02,-8.088827329609149075e+00
+1.283700502012248990e+01,-1.689074747536980503e+00,-1.068989404373356678e+01
+2.310573782779740171e+01,-1.729058651112188372e+01,-1.909006285753892485e+01
+5.304777440068442651e+00,-8.130126364332484812e+00,1.750262709010497630e+00
+2.252858568549002882e+01,-2.372640349761774559e+01,-1.232975866943885457e+01
+2.208418114146449085e+01,-2.028370712760799321e+01,-1.695770381091592327e+01
+1.996927680529851656e+01,-2.287761180674238304e+01,7.078070894113842826e+00
+1.162251991464229661e+01,-4.718992903388377513e+00,-1.107152990939307635e+01
+6.428318122441837090e+00,-9.868145229349664760e+00,2.752442290572005845e+00
+2.303719699520223330e+01,-1.387290489523010706e+01,-2.190364096787549641e+01
+1.470593111242053830e+01,5.908486490501513977e+00,2.730773799320538764e+00
+1.411680731443424008e+01,5.397611975436901410e+00,2.474768750828486574e+00
+1.355850624968552154e+01,2.443457423942230200e+00,-7.695788590747113744e+00
+1.120676749642655068e+01,-5.570864006448433159e+00,-1.024452388559919491e+01
+8.691923485842419694e+00,-1.462767666864503724e+01,-2.188972930889909740e+00
+2.518115028719757476e+01,1.215851110385398570e+01,-1.519615810617602669e+01
+1.890933598233750956e+01,-1.619827022668360783e+01,1.343000528578523145e+01
+2.055448295269335901e+01,-2.654261260327181304e+01,8.321203577417006780e-01
+2.243057567024769483e+01,-2.387056591223324631e+01,-1.243294891769894228e+01
+1.519004865572293994e+01,6.168149322069871765e+00,1.579605541963419402e+00
+7.803139098699933385e+00,-1.187290142245653435e+01,1.218277795002848940e+00
+1.837140427362895778e+01,-1.744744651221009235e+01,1.153390362701948924e+01
+4.134863094071127065e+00,-6.182302608878023520e+00,-2.213789348070631657e-01
+6.544053333615087453e+00,-1.006556234584045662e+01,2.914355995508532082e+00
+7.820180475908495410e+00,-1.330239558372155528e+01,-7.588846193196074896e-01
+5.372584408457768745e+00,-8.819357855259688961e+00,3.235939946687333979e+00
+2.286377763416580322e+01,-1.765191665693305723e+01,-2.027646530523981738e+01
+8.056307689539272232e+00,-1.364611708005502066e+01,-1.040532892853164748e+00
+2.600976152592165036e+01,1.269663433014256171e+01,-1.285699486202717523e+01
+9.940668257046679557e+00,-1.014383127056241207e+01,-1.005082842541397170e+01
+6.574758807114739589e+00,-1.136817086323861226e+01,2.785048798150224325e+00
+6.369261158515968191e+00,-7.943204395371625814e+00,2.957743211633388825e+00
+2.606360939411646527e+01,1.422140106999828646e+01,-1.180268130805715465e+01
+9.012430006743267441e+00,-1.376117257492106205e+01,-1.572921304338365189e+00
+2.295966359104549426e+01,-1.996047796099093219e+01,-1.765791743066063191e+01
+1.241351129673464726e+01,2.101316146321847711e-01,-7.731090973179729708e+00
+1.963097992002737513e+01,-1.905828544243102129e+01,1.180537728672040743e+01
+2.411233048153641434e+01,-7.183212962803311896e+00,-2.410767467382302698e+01
+2.253297924065808999e+01,-2.547951871682246150e+01,-4.624078443846567410e+00
+1.513536096375898055e+01,5.241752333011606702e+00,9.483876988222101900e-01
+1.937963886323884566e+01,-2.417531196867813748e+01,5.352943612762063097e+00
+2.228539007655298221e+01,-1.969341740923589157e+01,-1.828596072354638835e+01
+8.189519961118961078e+00,-1.413583843012129471e+01,-2.070776080929076279e+00
+8.727764168634033481e+00,-1.352830841420886543e+01,-3.529263129994613113e+00
+2.051230003833839888e+01,-2.611849087780997536e+01,1.865159573028842388e+00
+3.926271882453408413e+00,-5.752096378302901769e+00,-2.677184075298010280e-01
+1.611559207664653570e+01,1.568581967629328666e+00,8.144646646921355426e+00
+4.344650508285765156e+00,-7.254256633761306361e+00,1.191899550041862987e+00
+1.476276238952588038e+01,5.714416346904468647e+00,-3.169914330750125853e+00
+1.200397207704018676e+01,-9.817620591742697300e-01,-1.145867620924562580e+01
+4.490847332300337058e+00,-6.293705266938934173e+00,1.381139407157638832e+00
+2.346540651556653856e+01,-3.934336763083390309e+00,-2.381999810272223783e+01
+5.814343584659583897e+00,-7.221266268386170140e+00,1.144062159828406422e+00
+1.171299681733527365e+01,-7.074753794871936563e+00,-1.098999308272407838e+01
+6.757423901690621904e+00,-9.135381974823129525e+00,2.618165125446557440e+00
+2.214758774109295558e+01,-2.090085068222564146e+01,-1.668425931786434546e+01
+2.150984395551909500e+01,-2.552209603002873450e+01,-5.421972340492052567e+00
+2.619234089989640424e+01,1.579553883051059771e+01,-8.241139126873921583e+00
+3.660743059926329757e+00,-5.558203873922593630e+00,1.894669290098610848e+00
+2.274068271626153503e+01,-1.547939021787257019e+01,-2.039722667304535264e+01
+5.415970524385222973e+00,-9.012901930175438281e+00,2.589761883319367186e+00
+1.375977899697920392e+01,4.300219957350324584e+00,-4.254886591257382555e+00
+6.905830163223500406e+00,-1.149875398671117388e+01,2.132586697383511698e+00
+1.700640818295847723e+01,-5.741444477684074954e+00,1.370167499120037746e+01
+1.420336862032664271e+01,4.053527896125662444e+00,-4.514147740919165486e+00
+2.141727526128607906e+01,-2.614292271913464560e+01,-1.861854534335793732e+00
+1.344877849252288193e+01,1.582781494894556218e-01,-8.818973822700286291e+00
+1.036491562453851145e+01,-8.943700672690336972e+00,-9.873658612949256508e+00
+2.573593731721301836e+01,7.560287275386760264e+00,-1.930020715846036694e+01
+1.436134828034665922e+01,6.115002230910394410e+00,4.976206164045708924e-01
+1.142219912645135516e+01,-7.185156908378232288e+00,-1.121111731985273963e+01
+1.195529737073526810e+01,-2.905812972811709471e+00,-1.008431664735532962e+01
+1.149081485861253427e+01,-1.115954035822642076e+01,-8.650606950801510209e+00
+2.417261289879074937e+01,-3.492455184616749087e+00,-2.323556101387963224e+01
+1.177802250054865318e+01,-8.332203738393664239e+00,-1.017820988979364571e+01
+1.373497658884353356e+01,-2.700480995789344973e-01,-9.464090776641770120e+00
+2.152704765736172732e+01,-2.344858663440417601e+01,-1.323309251430787725e+01
+1.384914686628341940e+01,1.783346535357503093e+00,-7.641983367288610829e+00
+1.580745021393452099e+01,2.868352997211364830e+00,8.254973744418835579e+00
+5.706443707247517594e+00,-7.088941595804350904e+00,6.207023962635940251e-01
+1.042439783809316367e+01,-1.072242817210399579e+01,-9.230449121451632877e+00
+9.155633357772419600e+00,-1.302522463613280479e+01,-2.140737549715580279e+00
+5.618876757550852474e+00,-7.062180682240769336e+00,2.312431458133238138e+00
+9.406666130707060702e+00,-1.343964908951016390e+01,-4.860304384624765106e+00
+1.676731795417415327e+01,-4.737193813489671612e+00,1.378436120540708743e+01
+1.695329152296762487e+01,-3.006724904370758011e+00,1.368326442054545033e+01
+1.312033120070528724e+01,1.900623582474310069e-01,-8.944644944556923605e+00
+1.608757631590937720e+01,2.355885062506741789e-01,1.136776235125385170e+01
+1.154874864832947523e+01,-8.559654253984671612e+00,-1.016263144265091078e+01
+1.166891807930378633e+01,-8.444221035425533373e+00,-9.699911153927244456e+00
+2.457659789454210042e+01,5.598583367487428575e-01,-2.261664699667650069e+01
+2.075437602466496045e+01,-2.483565044189185400e+01,2.199623915982989342e+00
+2.685143565702432866e+01,1.686817486700240565e+01,-7.388017870346942573e+00
+2.134682298489288499e+01,-2.722862334944046481e+01,-4.144509326962807272e+00
+2.318353753772999326e+01,-1.651606298559597974e+01,-2.048273521535046626e+01
+1.326959036710392859e+01,2.368462582872120414e+00,-8.144275356931142795e+00
+4.046237088802604021e+00,-6.547436703799695223e+00,1.320427605345359190e+00
+1.346283255024571979e+01,2.525295005896233569e+00,-7.512172642262189726e+00
+2.199036093205726061e+01,-2.528661685409227289e+01,-9.718852110966340163e+00
+1.837265922542116670e+01,-1.748057946613262459e+01,1.284465499197332328e+01
+1.926520136917274684e+01,-2.190309771714446185e+01,8.220488962923797160e+00
+1.514428800522444618e+01,5.483726771845106818e+00,3.521974003103575335e+00
+1.458570537094653830e+01,4.834081378752377312e+00,-2.028768550078621224e+00
+2.178352453464813365e+01,-2.444383458084961447e+01,-1.008930925699115022e+01
+1.754000838178522415e+01,-5.102946298347888821e+00,1.484907239367638887e+01
+1.848138672102928126e+01,-3.685909693195588588e+00,1.410956567511424353e+01
+8.490056753706092252e+00,-1.399387560633241279e+01,-3.184614855211155948e+00
+1.593399702611558233e+01,3.471860802704106241e+00,8.600079893442066137e+00
+2.407251145979249074e+01,-7.275314599565289697e+00,-2.293056341124427178e+01
+1.674062446819076655e+01,3.229096180334520838e-01,1.117455835242325790e+01
+2.318127904916508086e+01,-1.799868130264278321e+01,-2.001899437270137838e+01
+1.950173304683986331e+01,-2.384171968365481220e+01,5.219354714995962041e+00
+1.965210941325579341e+01,-2.287669379624462707e+01,8.100994143573656103e+00
+1.469344728774298225e+01,5.212563538731541435e+00,1.598701742430525652e+00
+5.346173693169625096e+00,-8.319401231280000530e+00,1.194088321693766108e+00
+5.110591289743826593e+00,-6.997531052589042844e+00,2.157163858721566463e+00
+1.443178869012463572e+01,5.515670387612275682e+00,-1.735841800585647077e+00
+7.565199111351599726e+00,-1.260704881821683898e+01,1.124178289514855322e+00
+1.164067433415608654e+01,-2.610287265168273585e+00,-1.039228261371419570e+01
+1.740487215868784077e+01,-6.511306261435822584e+00,1.488785078831362974e+01
+6.834885784505054573e+00,-1.093743100544909908e+01,2.320005463001990176e+00
+9.144855924113519663e+00,-1.401964303614456853e+01,-2.138005378872123163e+00
+1.586235800599064838e+01,4.778534523520366228e+00,7.274253445721596378e+00
+9.148031070109642116e+00,-1.348698655243187794e+01,-2.100658987607335160e+00
+1.404664595027373863e+01,6.192260803135337888e+00,-2.640193020971708826e+00
+1.591777613058741458e+01,2.359485362839534695e+00,8.758307168235621276e+00
+1.834881731932261673e+01,-1.581595398885556847e+01,1.339976709661184984e+01
+2.533975326385773030e+01,1.106271223788852609e+01,-1.625033146410964946e+01
+1.211897280971400015e+01,-4.283172979347898313e+00,-1.137089778754230984e+01
+1.881070214214910763e+01,-2.112689295714271509e+01,1.026357360928932749e+01
+1.551625352738800068e+01,5.337816302659873280e+00,2.714653795052834884e+00
+1.992612429376245942e+01,-2.067497187014286908e+01,9.229301963058745173e+00
+1.301077012640076624e+01,1.874017247512113293e+00,-7.879441181951912121e+00
+2.103040013645074424e+01,-2.620814018238652565e+01,-4.987010539490871253e+00
+2.343682922868167751e+01,-8.965896590435001201e+00,-2.274414014640029791e+01
+1.591036310395064746e+01,1.668039854149161449e+00,8.721806624841301314e+00
+2.107423059849663005e+01,-2.444883676074177359e+01,-1.239793422074283313e+01
+1.011944366862372924e+01,-1.239294726155507576e+01,-7.559240297673714970e+00
+2.047255955100037639e+01,-2.578645203183630841e+01,-3.244903615313937451e+00
+2.617190568366683223e+01,6.225627451056479522e+00,-2.049007250998361229e+01
+2.482861620317560991e+01,7.216136007521627427e+00,-1.977306215073611639e+01
+2.471378090179000253e+01,9.503117979314019692e+00,-1.756960639987511286e+01
+2.525486694104066387e+01,1.596594399662877706e+01,-1.049568444805337997e+01
+1.439272813773745163e+01,4.366053161670669702e+00,-3.649759661751583284e+00
+1.635759280915426928e+01,4.031987925356458113e+00,7.767877271182909382e+00
+2.356198070123604182e+01,-1.822954817147143558e+01,-1.896024799305326525e+01
+2.235984099275620451e+01,-2.171092298182126967e+01,-1.614928214096586601e+01
+1.231588686790117038e+01,-4.738422573257817128e+00,-1.065588623787593470e+01
+2.328591774017433380e+01,-1.435695467409254888e+01,-2.182094160420029283e+01
+1.995312579795000829e+01,-2.440100209300568679e+01,4.946117771382794182e+00
+1.348041423580614406e+01,3.276257422221878990e+00,-6.421842598117234679e+00
+2.188766005590647978e+01,-2.398774153560882638e+01,-1.320312262336140030e+01
+1.102446289076129027e+01,-7.570488681308882306e+00,-1.093550140324746245e+01
+1.196874207185018335e+01,-2.745031332381755895e+00,-1.000715935701159331e+01
+1.424399871419267960e+01,3.505045400301617597e+00,-6.079064877201169281e+00
+2.397922359666646486e+01,-1.296537512259452818e+01,-2.179293936565116496e+01
+1.336533167075202400e+01,4.603436355560464044e+00,-3.373879340115852443e+00
+5.938607938211756476e+00,-7.683512989569407203e+00,2.038761651845470091e+00
+1.980799998129430506e+01,-2.389792816372647266e+01,4.656594621077291052e+00
+9.675417472144237863e+00,-1.386926557863174736e+01,-5.113922205504518814e+00
+2.356265868702679356e+01,-1.645651021807132608e+01,-2.096977909413447350e+01
+6.324787403454191548e+00,-1.210174153949093601e+01,1.207578850941470439e+00
+1.987608245310292432e+01,-2.491779585406550979e+01,3.476832096257118643e+00
+2.166577332205659800e+01,-2.588683754544189242e+01,-7.662473641644264255e+00
+1.777791658847976208e+01,-1.733874005808248242e+00,1.292781460709049135e+01
+1.915675138440426295e+01,-1.574542699556009850e+01,1.298079466846799690e+01
+1.936133839447892413e+01,-2.258549612512778992e+01,8.932596615713553234e+00
+2.508224380307736823e+01,9.326140559975229394e+00,-1.731136423179978578e+01
+1.033153225912175266e+01,-1.322798655280663382e+01,-3.755390409371381022e+00
+2.273624498405809646e+01,-2.372688928811433939e+01,-1.299385610502396737e+01
+1.281159418393686167e+01,2.345679902572524789e+00,-6.755005604810242481e+00
+2.087337640845328224e+01,-2.578531874126039014e+01,1.146283800838699296e+00
+1.497918575942056307e+01,6.304899421829968098e+00,-1.391397209818867164e+00
+1.685316037526309429e+01,-7.731630158540535369e+00,1.505736578244114376e+01
+4.816848230152659838e+00,-7.750396459533855698e+00,3.000555204229509165e-01
+9.230077114576102915e+00,-1.426845895826724053e+01,-4.178769101199424796e+00
+1.651160409690649544e+01,3.263921521465877440e+00,7.199048956468736549e+00
+1.249212150104483143e+01,-9.019591941644033994e-01,-9.542055152861269818e+00
+1.518538046542044384e+01,4.550891139085806891e+00,9.212176538977243645e-01
+1.736980297190575939e+01,-5.425910891778216616e+00,1.461729866570997416e+01
+2.538919219967998941e+01,1.454172297412333847e+01,-1.037648205588952166e+01
+2.194266140642715612e+01,-2.700004337951372335e+01,-4.571966439612294764e+00
+1.693820151115191308e+01,-3.350957884659627961e+00,1.334577316904475452e+01
+1.972508113054781020e+01,-2.448981549856138784e+01,6.972184227882037177e+00
+2.114640405397779332e+01,-2.526490958564891187e+01,6.294405030680498836e-01
+2.026684435570955500e+01,-2.410053076486639867e+01,4.823298534617702416e+00
+2.054563130721570374e+01,-2.381046802047153221e+01,4.505289725573802251e+00
+1.413262987179951402e+01,5.356208577396571080e+00,2.107904807204953990e+00
+8.371088352783994324e+00,-1.287717515405282498e+01,1.688852401958146121e+00
+1.982009133905154741e+01,-2.472690303757821084e+01,3.826025210174446300e+00
+1.494284654692304315e+01,4.850093485455801989e+00,4.335101641582176590e+00
+1.192213701262360814e+01,-3.501344234853501103e+00,-1.114254194934554931e+01
+1.233125195761659754e+01,-8.626258161535549362e-01,-1.061759428889177848e+01
+2.638839236734244764e+01,1.834452674876221678e+01,-6.999820692063727812e+00
+1.412397515453787911e+01,4.441732843787595364e+00,-5.517895724700044857e-01
+4.994824099780398541e+00,-7.261416708424443200e+00,1.260607884431212522e+00
+1.110064285975399656e+01,-6.620883852693684624e+00,-1.173676778265741127e+01
+1.855707569312059135e+01,-8.920363398032657543e+00,1.364393162557992234e+01
+1.978070282394129720e+01,-2.035478665156414380e+01,1.004620212823427927e+01
+1.572779598008688851e+01,5.554710985947908242e-01,1.123561803361210920e+01
+1.470697866715481972e+01,5.435173225054987789e+00,-2.062569184868013217e+00
+1.293061332723554102e+01,-4.685140869903676730e+00,-1.089962554432043085e+01
+2.241035207182362754e+01,-2.399378848098107397e+01,-1.189840913936498801e+01
+1.125993631758902680e+01,-1.207155524718314510e+01,-5.962420331831191689e+00
+1.531584927794298956e+01,3.061669515235398542e+00,7.163400228070599951e+00
+1.920738614237074771e+01,-2.414166517817354318e+01,4.692921273099221580e+00
+2.374613099988856035e+01,-8.195621953135528770e+00,-2.273139334049360372e+01
+2.589645733174912223e+01,1.629021518787582323e+01,-7.093422758445099952e+00
+8.401498436674268433e+00,-1.375333963384859182e+01,-1.526590180308619704e+00
+1.586639494505238623e+01,6.006716052845892939e+00,4.315000450142298050e+00
+2.513654507694387163e+01,1.968634505849039762e+00,-2.311989977173310251e+01
+1.809923627117503031e+01,-4.719864513570952269e+00,1.374649989926335714e+01
+1.864401842156636846e+01,-2.102054923980609402e+01,9.377730542984135553e+00
+1.939743784762634249e+01,-2.232957098451484512e+01,8.396294876585335132e+00
+6.189757914907195513e+00,-9.104834579712303366e+00,2.300321804968418427e+00
+2.426912514320380510e+01,-1.257603916733168958e+00,-2.235223539902650458e+01
+4.385945785902803706e+00,-6.020456244686851477e+00,7.209501608316684074e-01
+1.752114654911539660e+01,-6.018537008577111713e+00,1.454175432476469432e+01
+2.156129079745074861e+01,-2.640390757720264858e+01,-1.613852437426660735e+00
+1.455680215858329696e+01,5.236741018159229988e+00,-1.488454555034077753e+00
+2.619923939777534017e+01,1.484866306750926412e+01,-1.181042587901669272e+01
+1.705440259833099148e+01,-8.244656415078146949e+00,1.374964385274364354e+01
+1.080153365534254917e+01,-9.683647671249412170e+00,-8.989563743717930322e+00
+1.939268890837919201e+01,-2.548357895886853441e+01,3.517011595359853970e+00
+1.791315200899453330e+01,-1.510750957582581577e+01,1.358471692980101153e+01
+2.370137948008053641e+01,-9.259651195862208084e+00,-2.257335784680862645e+01
+2.543812305418260067e+01,1.309718143086379172e+01,-1.445957355987915172e+01
+9.675745852056484964e+00,-1.351672692400412856e+01,-4.102153151661007691e+00
+3.562233324218383679e+00,-5.926985926816761285e+00,-1.381561208221213644e-01
+1.932128103412230757e+01,-1.968452249925336517e+01,1.077223160678077640e+01
+8.478193983471308925e+00,-1.117119337743558916e+01,1.385156770313188623e+00
+1.810490221456069193e+01,-1.237342421336984266e+01,1.413672831435098232e+01
+1.528368910781727763e+01,4.818825764667333367e+00,4.849977460912127114e+00
+2.658573070843726782e+01,1.770688487574752656e+01,-5.828596864892722884e+00
+1.339346592897467936e+01,5.240770276693830887e+00,-2.949411944642311934e+00
+2.087361754167300276e+01,-2.529008986983027185e+01,-9.056942649094953168e+00
+2.455422212869780907e+01,2.616510307857105921e+00,-2.172615902846477098e+01
+1.902070105076570883e+01,-2.263886737796014970e+01,8.420564772554000044e+00
+2.527377626624629059e+01,8.374927252351710649e+00,-1.826049177166931514e+01
+2.628169339837640450e+01,1.383684441492921025e+01,-1.251458237250198025e+01
+2.119693917636971037e+01,-2.555942930923443512e+01,4.012111483905216325e-01
+2.263666765791331059e+01,-1.970368613436385985e+01,-1.671772466938027080e+01
+1.804141541097152412e+01,-8.461943245659396595e+00,1.352662153520397048e+01
+1.874792423780163375e+01,-2.103387313582268092e+01,9.307922198149290338e+00
+2.090805364583402337e+01,-2.544519391541260944e+01,1.431894941073290184e+00
+1.870416924915054580e+01,-1.332562212510831401e+01,1.310645060560786135e+01
+2.670410961206907885e+01,1.635935294860294675e+01,-5.561533850067672091e+00
+2.661641054630572967e+01,1.621457304123468646e+01,-9.001407978243616270e+00
+1.757398433184464892e+01,-7.339404394859850633e+00,1.443033385079859876e+01
+1.754747881493114647e+01,-4.144721857408338650e+00,1.360067587365037056e+01
+1.718421179237487095e+01,-2.988453632785307512e+00,1.365579728223067590e+01
+1.445302845037893391e+01,6.504977689999114965e+00,1.049455131217200243e+00
+2.514203303839694925e+01,2.100934095051690598e+00,-2.138964893013869073e+01
+1.462087223024265015e+01,5.731317779403812374e+00,1.072510489729729954e+00
+1.723046503318723666e+01,-2.060815661550527089e+00,1.197201202633523565e+01
+1.340466975572003960e+01,-1.234611707301389139e+00,-1.016839919287774308e+01
+2.127560429156662636e+01,-2.593942714722985698e+01,-1.187111503594445949e+00
+1.746324131747647712e+01,-7.311422990095265639e+00,1.464599213321039883e+01
+1.993560849490860676e+01,-2.090348994318480891e+01,1.075555268253570773e+01
+7.638469377559760076e+00,-1.268195232816358597e+01,5.018570059805065320e-01
+2.385432293392500469e+01,-9.963009128057283448e+00,-2.331031261340206129e+01
+1.133054212698301733e+01,-8.192475635926486532e+00,-1.011757458401461562e+01
+7.494620485987201874e+00,-1.295863403921326551e+01,1.545094465835450848e+00
+1.967677668432564886e+01,-1.913027294056395533e+01,1.148326616798142297e+01
+1.923668568746521501e+01,-1.260224840252439193e+01,1.441667731003316710e+01
+2.246520538455834526e+01,-2.621201998499466868e+01,-6.470950115760444987e+00
+2.471914090975780809e+01,-1.768178453888226365e+00,-2.157038603308539848e+01
+7.435199307165166971e+00,-1.200506094789014888e+01,1.451093811805416856e+00
+2.581364644679286258e+01,1.160065633335593560e+01,-1.556437603488778088e+01
+2.162524493232928791e+01,-2.561889480923573359e+01,-6.599768179724442518e+00
+2.558104538331870259e+01,6.038256943281870015e+00,-2.144167203683432632e+01
+2.051658077269308222e+01,-2.633362517895839261e+01,3.709260337434128196e-02
+4.938047559673222509e+00,-7.147856578053565002e+00,1.879307635610208305e+00
+2.239577772728431526e+01,-2.444446218459414766e+01,-1.188063944678044237e+01
+5.414179412726998208e+00,-7.682703213544816556e+00,2.088781840202358797e+00
+2.112859735411380768e+01,-2.459629545000203876e+01,-1.145295621808573472e+01
+1.885333068470767870e+01,-2.183916671060952908e+01,9.401207128951051928e+00
+2.421132464566532150e+01,-3.935730645589023968e+00,-2.336864962840157744e+01
+1.206020262603299642e+01,-5.065351968902742641e-01,-9.792602190405750306e+00
+2.468568725636113825e+01,3.322011953546867069e+00,-2.131221738420153144e+01
+2.235877571572716960e+01,-2.116280535855354117e+01,-1.663432908783774877e+01
+9.453304426202329580e+00,-1.336618033301169994e+01,-6.947726434666460449e+00
+1.951982111259196984e+01,-1.982512898884142061e+01,1.168821505935973626e+01
+1.380786147525128449e+01,2.296157115368532509e+00,-7.963788272971132010e+00
+1.629076430939239017e+01,-2.011042016403104427e+00,1.319261740755360179e+01
+2.199220212690133280e+01,-2.586589133179847622e+01,-2.243436891808469724e+00
+2.486509972065838880e+01,8.885375939253705724e+00,-1.764686177552493263e+01
+9.262216704199971673e+00,-1.457673436558977542e+01,-1.421147656495748812e+00
+2.265686173130742986e+01,-2.540279881120788019e+01,-1.064263991704245882e+01
+2.528926509631806496e+01,7.876282434112353847e+00,-1.899884356304903577e+01
+2.174124479787587561e+01,-2.582917137102553440e+01,-9.039713057945650831e+00
+2.606373133903819195e+01,1.253240524356625230e+01,-1.389308140114126111e+01
+1.964003667383432727e+01,-2.048658127374620719e+01,8.928204049326204483e+00
+1.621157228674842088e+01,1.350655339574911018e+00,1.081343639535893075e+01
+1.565935190747207884e+01,2.811394350390323815e+00,9.292806315020158081e+00
+2.097877746103495866e+01,-2.491270915590614266e+01,3.455756327161361163e+00
+2.097136260699557653e+01,-2.468210048800793643e+01,3.293143939006740517e+00
+2.581946439776644553e+01,1.785021044451976024e+01,-4.879026458799026855e+00
+5.377013781098723300e+00,-8.856008563756073926e+00,2.317097449855962665e+00
+1.510693040645124796e+01,4.701540744398914562e+00,5.282082480462396923e+00
+2.546826427071196619e+01,4.549811003070890258e+00,-2.125644532632559702e+01
+7.341696513224130527e+00,-1.145830254395111680e+01,1.972034154540442508e+00
+2.245830541721123552e+01,-2.483415315969391557e+01,-1.115825686096097158e+01
+2.551753367344477752e+01,6.762650241879920365e+00,-1.952051681734236865e+01
+1.464455903800639369e+01,5.326728163785118930e+00,-3.553170888014037132e+00
+1.063321973957261157e+01,-8.992246457676619897e+00,-9.975421183052016971e+00
+1.530000725556413599e+01,5.101844962992619692e+00,-9.188724914814785372e-01
+2.540687271364042488e+01,9.473514715245386242e+00,-1.696110244895483277e+01
+8.198666498090684485e+00,-1.378548704173702077e+01,-4.911752274273016639e+00
+1.572986550804393779e+01,2.846878348088725197e+00,8.298194295697189915e+00
+2.029741634705190023e+01,-2.587077253483554884e+01,4.790251610927698245e-01
+1.813907543037277037e+01,-1.822792700624311024e+01,1.248696196688529980e+01
+2.580999574825163378e+01,1.161044416937404833e+01,-1.551079718000966068e+01
+1.586235695390923084e+01,3.887414422108860457e+00,4.776448543070914710e+00
+2.519655465233795866e+01,-9.017265225481260416e+00,-2.298176485406207092e+01
+2.471010832751492359e+01,-6.592459442765898459e+00,-2.293831898722635287e+01
+2.449467567175208771e+01,-8.567370750619147657e-01,-2.285983210996698034e+01
+9.960230181439836628e+00,-1.227227613819709617e+01,-6.346030696773343749e+00
+1.846703276591660270e+01,-1.135070131073076993e+01,1.398154733043795872e+01
+1.093463363304534752e+01,-4.933371061817548586e+00,-1.031745292549059734e+01
+2.304315238562634960e+01,-1.599328918790850906e+01,-2.036755501341412611e+01
+1.052802713381784550e+01,-9.196555665029098492e+00,-1.120933002873744933e+01
+2.333404696641204268e+01,-1.327207208758834511e+01,-2.167099340107120753e+01
+2.148057940478388161e+01,-2.322916256514355737e+01,-1.390143530443905284e+01
+1.953070502494668048e+01,-2.491147985424986189e+01,5.174280318261995859e+00
+2.456506235036209773e+01,-4.530217416105457140e+00,-2.353940483003152195e+01
+9.160844475883656912e+00,-1.352642830644638394e+01,-5.325184892158300265e+00
+1.150867978980838302e+01,-3.886184338854294928e+00,-9.253397216282344573e+00
+2.558698802774866010e+01,1.514452157180459935e+01,-1.148958485979931865e+01
+1.533278111660303722e+01,5.689119138391936836e+00,3.105152045176828857e+00
+3.176250365714620827e+00,-6.745153865379862168e+00,-6.323997746955005717e-01
+2.624135454850302196e+01,1.449761777314100542e+01,-1.046802057760974947e+01
+1.142992224270783197e+01,-8.461000773740524394e+00,-1.040279173201102303e+01
+2.041232477576469151e+01,-2.522550129027365884e+01,-5.123015956210185129e-01
+2.419059803106427253e+01,3.447520851032373379e+00,-2.158746673808884964e+01
+2.160877640047978332e+01,-2.501880882350765489e+01,-7.364530242511582614e+00
+2.656708798627344592e+01,1.627064431966952895e+01,-7.767922182091026251e+00
+2.164092009693748153e+01,-2.662741372758210900e+01,-4.184209908426014479e+00
+6.581392776941481060e+00,-1.079802001828051949e+01,2.543134247841539519e+00
+2.733118796526959571e+01,1.069265969992130749e+01,-1.693345150683806821e+01
+4.380606945618692016e+00,-6.951838930503489777e+00,1.280163859347801747e+00
+1.204722405349341940e+01,1.050121972104467893e+00,-8.915908770873940625e+00
```

### Comparing `transmorph-0.2.6b0/src/transmorph/datasets/databank_api.py` & `transmorph-0.2.7/src/transmorph/datasets/databank_api.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import base64
-import hashlib
-import json
-import logging
-import os
-import time
-import urllib.request
-import zipfile
-
-from os import path
-from socket import error as SocketError
-from typing import Dict, Optional
-from warnings import warn
-
-from ..utils.file import adapt_path
-from .._logging import logger
-
-CALLBACK = 30
-DATASETS_JSON = "datasets.json"
-DATA_PATH = f"{path.dirname(__file__)}/data/"
-
-
-def check_md5_file(file_path: str, target_hash: str) -> bool:
-    # Returns a md5 hash to quality check
-    file_hash = hashlib.md5(open(adapt_path(file_path), "rb").read()).hexdigest()
-    return file_hash == target_hash
-
-
-def remove_dataset(dataset_name: str) -> None:
-    # Removes all files from data/$dataset_name
-    logger.log(logging.DEBUG, f"databank_api > Removing dataset {dataset_name}...")
-    if not path.exists(adapt_path(f"{DATA_PATH}{dataset_name}")):
-        logger.log(logging.DEBUG, "databank_api > Nothing to do.")
-        return
-    for fname in os.listdir(adapt_path(f"{DATA_PATH}{dataset_name}/")):
-        os.remove(adapt_path(f"{DATA_PATH}{dataset_name}/{fname}"))
-    os.rmdir(adapt_path(f"{DATA_PATH}{dataset_name}"))
-
-
-def unzip_file(zip_path: str, dataset_name: str) -> None:
-    # Unzips $zip_path at data/$dataset_name/
-    logger.log(logging.DEBUG, f"databank_api > Unzipping file {zip_path}...")
-    with zipfile.ZipFile(zip_path, "r") as fzip:
-        fzip.extractall(adapt_path(f"{DATA_PATH}{dataset_name}/"))
-    os.remove(adapt_path(zip_path))
-
-
-def check_files(dataset_name: str) -> bool:
-    # Check if all files from a dataset are present
-    logger.log(logging.DEBUG, f"databank_api > Checking files from {dataset_name}...")
-    with open(adapt_path(f"{path.dirname(__file__)}/{DATASETS_JSON}"), "r") as f:
-        all_datasets = json.load(f)
-        dataset: Optional[Dict] = None
-        for ds in all_datasets:
-            if ds["name"] == dataset_name:
-                dataset = ds
-                break
-        if dataset is None:
-            warn(f"Dataset {dataset_name} not found in database.")
-            return False
-        for fname in dataset["files"]:
-            if not path.exists(
-                adapt_path(f"{path.dirname(__file__)}/data/{dataset_name}/{fname}")
-            ):
-                return False
-    return True
-
-
-# From https://towardsdatascience.com/
-#      how-to-get-onedrive-direct-download-link-ecb52a62fee4
-def url_to_dllink(onedrive_link: str) -> str:
-    # Converts a "share" link to a direct download link
-    data_bytes64 = base64.b64encode(bytes(onedrive_link, "utf-8"))
-    data_bytes64_String = (
-        data_bytes64.decode("utf-8").replace("/", "_").replace("+", "-").rstrip("=")
-    )
-    resultUrl = (
-        f"https://api.onedrive.com/v1.0/shares/u!{data_bytes64_String}/root/content"
-    )
-    return resultUrl
-
-
-def print_download_state(blocks_received: int, block_size: int, file_size: int) -> None:
-    percent = int(blocks_received * block_size / file_size * 100)
-    print(f"databank_api > Downloading bank: {percent}%", end="\r")
-
-
-def download_dataset(dataset_name: str) -> str:
-    # Downloads a dataset from onedrive
-    # using data from datasets.json
-    # TODO print -> log
-
-    datasets_root = adapt_path(f"{path.dirname(__file__)}/")
-
-    # Ensuring dataset exists
-    f = open(adapt_path(f"{datasets_root}{DATASETS_JSON}"), "r")
-    all_datasets = json.load(f)
-    dataset = None
-    for ds in all_datasets:
-        if ds["name"] == dataset_name:
-            dataset = ds
-            break
-    assert dataset is not None, f"databank_api > Unknown dataset: {dataset_name}."
-    logger.log(logging.INFO, f"databank_api > Loading dataset {dataset_name}...")
-    logger.log(logging.INFO, f"databank_api > Reference: {dataset['reference']}")
-    logger.log(logging.INFO, f"databank_api > Type: {dataset['type']}")
-    logger.log(logging.INFO, f"databank_api > Number of files: {dataset['n_files']}")
-
-    # Preparing dir structure
-    if not path.exists(adapt_path(f"{datasets_root}data/")):
-        logger.log(logging.DEBUG, "databank_api > data/ not found, creating it.")
-        os.mkdir(adapt_path(f"{datasets_root}data/"))
-    data_path = adapt_path(f"{datasets_root}data/{dataset_name}/")
-    if not path.exists(data_path):
-        logger.log(
-            logging.DEBUG,
-            f"databank_api > data/{dataset_name}/ not found, creating it.",
-        )
-        os.mkdir(data_path)
-
-    # Loading dataset
-    dl_url = url_to_dllink(dataset["zip_link"])
-    zip_path = adapt_path(f"{data_path}{dataset['zip_name']}")
-    try:
-        urllib.request.urlretrieve(dl_url, zip_path, print_download_state)
-        logger.log(logging.DEBUG, "")
-    except SocketError as e:
-        f.close()
-        logger.log(logging.DEBUG, "")
-        logger.log(logging.INFO, f"databank_api > # ERROR # {e}")
-        logger.log(logging.INFO, f"databank_api > Retrying in {CALLBACK} seconds.")
-        logger.log(
-            logging.INFO,
-            "databank_api > Please make sure you're running the "
-            "latest package version.",
-        )
-        time.sleep(CALLBACK)
-        return download_dataset(dataset_name)
-
-    logger.log(logging.DEBUG, "databank_api > Checking md5 sums...")
-    if not check_md5_file(zip_path, dataset["md5_hash"]):
-        f.close()
-        os.remove(zip_path)
-        logger.log(
-            logging.DEBUG, "databank_api > # ERROR # Errors detected in the file."
-        )
-        logger.log(logging.INFO, f"databank_api > Retrying in {CALLBACK} seconds.")
-        time.sleep(CALLBACK)
-        return download_dataset(dataset_name)
-
-    f.close()
-    logger.log(
-        logging.INFO, f"databank_api > Dataset {dataset_name} successfully downloaded."
-    )
-    return zip_path
+import base64
+import hashlib
+import json
+import logging
+import os
+import time
+import urllib.request
+import zipfile
+
+from os import path
+from socket import error as SocketError
+from typing import Dict, Optional
+from warnings import warn
+
+from ..utils.file import adapt_path
+from .._logging import logger
+
+CALLBACK = 30
+DATASETS_JSON = "datasets.json"
+DATA_PATH = f"{path.dirname(__file__)}/data/"
+
+
+def check_md5_file(file_path: str, target_hash: str) -> bool:
+    # Returns a md5 hash to quality check
+    file_hash = hashlib.md5(open(adapt_path(file_path), "rb").read()).hexdigest()
+    return file_hash == target_hash
+
+
+def remove_dataset(dataset_name: str) -> None:
+    # Removes all files from data/$dataset_name
+    logger.log(logging.DEBUG, f"databank_api > Removing dataset {dataset_name}...")
+    if not path.exists(adapt_path(f"{DATA_PATH}{dataset_name}")):
+        logger.log(logging.DEBUG, "databank_api > Nothing to do.")
+        return
+    for fname in os.listdir(adapt_path(f"{DATA_PATH}{dataset_name}/")):
+        os.remove(adapt_path(f"{DATA_PATH}{dataset_name}/{fname}"))
+    os.rmdir(adapt_path(f"{DATA_PATH}{dataset_name}"))
+
+
+def unzip_file(zip_path: str, dataset_name: str) -> None:
+    # Unzips $zip_path at data/$dataset_name/
+    logger.log(logging.DEBUG, f"databank_api > Unzipping file {zip_path}...")
+    with zipfile.ZipFile(zip_path, "r") as fzip:
+        fzip.extractall(adapt_path(f"{DATA_PATH}{dataset_name}/"))
+    os.remove(adapt_path(zip_path))
+
+
+def check_files(dataset_name: str) -> bool:
+    # Check if all files from a dataset are present
+    logger.log(logging.DEBUG, f"databank_api > Checking files from {dataset_name}...")
+    with open(adapt_path(f"{path.dirname(__file__)}/{DATASETS_JSON}"), "r") as f:
+        all_datasets = json.load(f)
+        dataset: Optional[Dict] = None
+        for ds in all_datasets:
+            if ds["name"] == dataset_name:
+                dataset = ds
+                break
+        if dataset is None:
+            warn(f"Dataset {dataset_name} not found in database.")
+            return False
+        for fname in dataset["files"]:
+            if not path.exists(
+                adapt_path(f"{path.dirname(__file__)}/data/{dataset_name}/{fname}")
+            ):
+                return False
+    return True
+
+
+# From https://towardsdatascience.com/
+#      how-to-get-onedrive-direct-download-link-ecb52a62fee4
+def url_to_dllink(onedrive_link: str) -> str:
+    # Converts a "share" link to a direct download link
+    data_bytes64 = base64.b64encode(bytes(onedrive_link, "utf-8"))
+    data_bytes64_String = (
+        data_bytes64.decode("utf-8").replace("/", "_").replace("+", "-").rstrip("=")
+    )
+    resultUrl = (
+        f"https://api.onedrive.com/v1.0/shares/u!{data_bytes64_String}/root/content"
+    )
+    return resultUrl
+
+
+def print_download_state(blocks_received: int, block_size: int, file_size: int) -> None:
+    percent = int(blocks_received * block_size / file_size * 100)
+    print(f"databank_api > Downloading bank: {percent}%", end="\r")
+
+
+def download_dataset(dataset_name: str) -> str:
+    # Downloads a dataset from onedrive
+    # using data from datasets.json
+    # TODO print -> log
+
+    datasets_root = adapt_path(f"{path.dirname(__file__)}/")
+
+    # Ensuring dataset exists
+    f = open(adapt_path(f"{datasets_root}{DATASETS_JSON}"), "r")
+    all_datasets = json.load(f)
+    dataset = None
+    for ds in all_datasets:
+        if ds["name"] == dataset_name:
+            dataset = ds
+            break
+    assert dataset is not None, f"databank_api > Unknown dataset: {dataset_name}."
+    logger.log(logging.INFO, f"databank_api > Loading dataset {dataset_name}...")
+    logger.log(logging.INFO, f"databank_api > Reference: {dataset['reference']}")
+    logger.log(logging.INFO, f"databank_api > Type: {dataset['type']}")
+    logger.log(logging.INFO, f"databank_api > Number of files: {dataset['n_files']}")
+
+    # Preparing dir structure
+    if not path.exists(adapt_path(f"{datasets_root}data/")):
+        logger.log(logging.DEBUG, "databank_api > data/ not found, creating it.")
+        os.mkdir(adapt_path(f"{datasets_root}data/"))
+    data_path = adapt_path(f"{datasets_root}data/{dataset_name}/")
+    if not path.exists(data_path):
+        logger.log(
+            logging.DEBUG,
+            f"databank_api > data/{dataset_name}/ not found, creating it.",
+        )
+        os.mkdir(data_path)
+
+    # Loading dataset
+    dl_url = url_to_dllink(dataset["zip_link"])
+    zip_path = adapt_path(f"{data_path}{dataset['zip_name']}")
+    try:
+        urllib.request.urlretrieve(dl_url, zip_path, print_download_state)
+        logger.log(logging.DEBUG, "")
+    except SocketError as e:
+        f.close()
+        logger.log(logging.DEBUG, "")
+        logger.log(logging.INFO, f"databank_api > # ERROR # {e}")
+        logger.log(logging.INFO, f"databank_api > Retrying in {CALLBACK} seconds.")
+        logger.log(
+            logging.INFO,
+            "databank_api > Please make sure you're running the "
+            "latest package version.",
+        )
+        time.sleep(CALLBACK)
+        return download_dataset(dataset_name)
+
+    logger.log(logging.DEBUG, "databank_api > Checking md5 sums...")
+    if not check_md5_file(zip_path, dataset["md5_hash"]):
+        f.close()
+        os.remove(zip_path)
+        logger.log(
+            logging.DEBUG, "databank_api > # ERROR # Errors detected in the file."
+        )
+        logger.log(logging.INFO, f"databank_api > Retrying in {CALLBACK} seconds.")
+        time.sleep(CALLBACK)
+        return download_dataset(dataset_name)
+
+    f.close()
+    logger.log(
+        logging.INFO, f"databank_api > Dataset {dataset_name} successfully downloaded."
+    )
+    return zip_path
```

### Comparing `transmorph-0.2.6b0/src/transmorph/datasets/datasets.json` & `transmorph-0.2.7/src/transmorph/datasets/datasets.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {'1': "{'zip_link': 'https://1drv.ms/u/s!Al03Ky07bKkGhe1zpM95A6_RSlXi5w?e=o1DRJv', 'md5_hash': "*

 * *      "'7bb3471fc4a69e999d68f28b815157d3'}"}*

```diff
@@ -28,20 +28,20 @@
         "files": [
             "patient_1.h5ad",
             "patient_2.h5ad",
             "patient_3.h5ad",
             "patient_4.h5ad",
             "patient_5.h5ad"
         ],
-        "md5_hash": "b1e5a3498d0a93ff9304644d91e2ecb2",
+        "md5_hash": "7bb3471fc4a69e999d68f28b815157d3",
         "n_files": 5,
         "name": "pal_10x",
         "reference": "https://embopress.org/doi/full/10.15252/embj.2020107333",
         "type": "single-cell RNA-seq 10x",
-        "zip_link": "https://1drv.ms/u/s!Al03Ky07bKkGheMM3FETrabb7Iv3Rw?e=iQp4cS",
+        "zip_link": "https://1drv.ms/u/s!Al03Ky07bKkGhe1zpM95A6_RSlXi5w?e=o1DRJv",
         "zip_name": "pal_10x.zip"
     },
     {
         "files": [
             "lung_P1.h5ad",
             "lung_P2.h5ad",
             "lung_P3.h5ad"
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/lisi.py` & `transmorph-0.2.7/src/transmorph/engine/checking/algorithms/lisi.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from typing import List
-
-from ..checking import Checking
-from ....stats.lisi import compute_lisi
-
-
-class LISI(Checking):
-    """
-    LISI statistic measures how heterogeneous a sample neighborhood
-    is for a certain label. Is is notably used in the Harmony [1]
-    integration pipeline to measure how well integrated datasets
-    are. Here, we use it to measure how many batches are found
-    on average in each sample's neighborhood.
-
-    Parameters
-    ----------
-    threshold: float, default = 0.5
-        Minimum average heterogeneity to reach to accept
-        an integration, after dividing by the number of
-        datasets.
-
-    perplexity: float, default = 30.0
-        Scales the neighborhood size to consider.
-
-    References
-    ----------
-    [1] Korsunsky, Ilya, et al. "Fast, sensitive and accurate integration
-        of single-cell data with Harmony." Nature methods 16.12 (2019): 1289-1296.
-    """
-
-    def __init__(self, threshold: float = 0.5, perplexity: float = 15.0):
-        Checking.__init__(self, str_identifier="LISI")
-        self.threshold = threshold
-        self.perplexity = perplexity
-
-    def check(self, datasets: List[np.ndarray]) -> bool:
-        """
-        Computes LISI after concatenating datasets, then
-        compares with threshold.
-        """
-        X_all = np.concatenate(datasets, axis=0)
-        labels = np.array(sum([[i] * X.shape[0] for i, X in enumerate(datasets)], []))
-        lisi = compute_lisi(X_all, labels, self.perplexity)
-        self.score = lisi.mean()
-        return self.score >= self.threshold
+#!/usr/bin/env python3
+
+import numpy as np
+
+from typing import List
+
+from ..checking import Checking
+from ....stats.lisi import compute_lisi
+
+
+class LISI(Checking):
+    """
+    LISI statistic measures how heterogeneous a sample neighborhood
+    is for a certain label. Is is notably used in the Harmony [1]
+    integration pipeline to measure how well integrated datasets
+    are. Here, we use it to measure how many batches are found
+    on average in each sample's neighborhood.
+
+    Parameters
+    ----------
+    threshold: float, default = 0.5
+        Minimum average heterogeneity to reach to accept
+        an integration, after dividing by the number of
+        datasets.
+
+    perplexity: float, default = 30.0
+        Scales the neighborhood size to consider.
+
+    References
+    ----------
+    [1] Korsunsky, Ilya, et al. "Fast, sensitive and accurate integration
+        of single-cell data with Harmony." Nature methods 16.12 (2019): 1289-1296.
+    """
+
+    def __init__(self, threshold: float = 0.5, perplexity: float = 15.0):
+        Checking.__init__(self, str_identifier="LISI")
+        self.threshold = threshold
+        self.perplexity = perplexity
+
+    def check(self, datasets: List[np.ndarray]) -> bool:
+        """
+        Computes LISI after concatenating datasets, then
+        compares with threshold.
+        """
+        X_all = np.concatenate(datasets, axis=0)
+        labels = np.array(sum([[i] * X.shape[0] for i, X in enumerate(datasets)], []))
+        lisi = compute_lisi(X_all, labels, self.perplexity)
+        self.score = lisi.mean()
+        return self.score >= self.threshold
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/checking/algorithms/neighborentropy.py` & `transmorph-0.2.7/src/transmorph/engine/checking/algorithms/neighborentropy.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from typing import List
-
-from ..checking import Checking
-from ...traits.isprofilable import profile_method
-from ....stats.entropy import label_entropy
-
-
-class NeighborEntropy(Checking):
-    """
-    Uses a neighborhood criterion to provide a numerical estimation
-    of neighborhood sanity after integration. Intuitively, it attributes
-    a score to each sample, that penalizes points whose neighbors in
-    the embedding space come from the same dataset.
-
-    For a set of datasets D = {X1, ..., XN} embedded in the same space
-    using a projector f,
-
-    NE(S) = (|X1| + ... + |XN|)^{-1}
-            \\times \\sum_{Xi \\in S} \\sum_{x \\in xi}
-            H_k(NN(f(x), f(X1) \\cup ... \\cup f(XN))),
-
-    Where H_k(x, S) is the Shannon entropy of labels in the k-nearest
-    neighbors of x (including x).
-
-    Parameters
-    ----------
-    n_neighbors: int, default = 15
-        Number of nearest neighbors to take into account when computing
-        label entropy.
-
-    threshold: float, default = 0.5
-        check() is accepted if neighbor entropy is above this threshold.
-    """
-
-    def __init__(self, n_neighbors: int = 15, threshold: float = 0.5):
-        Checking.__init__(self, str_identifier="NEIGHBOR_ENTROPY")
-        self.n_neighbors = n_neighbors
-        self.threshold = threshold
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Checks correct common dimensionality of the embeddings.
-        """
-        assert len(datasets) > 0
-        dimensionality = datasets[0].shape[1]
-        assert all(X.shape[1] == dimensionality for X in datasets)
-
-    @profile_method
-    def check(self, datasets: List[np.ndarray]) -> bool:
-        """
-        Computes label entropy, and returns true if it is above threshold.
-        """
-        # Concatenating datasets and labels
-        X_all = np.concatenate(datasets, axis=0)
-        N = X_all.shape[0]
-
-        labels = np.zeros(N)
-        offset = 0
-        for i, X in enumerate(datasets, 1):
-            n_obs = X.shape[0]
-            labels[offset : offset + n_obs] = i
-            offset += n_obs
-
-        self.score = label_entropy(X_all, labels, self.n_neighbors)
-        return self.score >= self.threshold
+#!/usr/bin/env python3
+
+import numpy as np
+
+from typing import List
+
+from ..checking import Checking
+from ...traits.isprofilable import profile_method
+from ....stats.entropy import label_entropy
+
+
+class NeighborEntropy(Checking):
+    """
+    Uses a neighborhood criterion to provide a numerical estimation
+    of neighborhood sanity after integration. Intuitively, it attributes
+    a score to each sample, that penalizes points whose neighbors in
+    the embedding space come from the same dataset.
+
+    For a set of datasets D = {X1, ..., XN} embedded in the same space
+    using a projector f,
+
+    NE(S) = (|X1| + ... + |XN|)^{-1}
+            \\times \\sum_{Xi \\in S} \\sum_{x \\in xi}
+            H_k(NN(f(x), f(X1) \\cup ... \\cup f(XN))),
+
+    Where H_k(x, S) is the Shannon entropy of labels in the k-nearest
+    neighbors of x (including x).
+
+    Parameters
+    ----------
+    n_neighbors: int, default = 15
+        Number of nearest neighbors to take into account when computing
+        label entropy.
+
+    threshold: float, default = 0.5
+        check() is accepted if neighbor entropy is above this threshold.
+    """
+
+    def __init__(self, n_neighbors: int = 15, threshold: float = 0.5):
+        Checking.__init__(self, str_identifier="NEIGHBOR_ENTROPY")
+        self.n_neighbors = n_neighbors
+        self.threshold = threshold
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Checks correct common dimensionality of the embeddings.
+        """
+        assert len(datasets) > 0
+        dimensionality = datasets[0].shape[1]
+        assert all(X.shape[1] == dimensionality for X in datasets)
+
+    @profile_method
+    def check(self, datasets: List[np.ndarray]) -> bool:
+        """
+        Computes label entropy, and returns true if it is above threshold.
+        """
+        # Concatenating datasets and labels
+        X_all = np.concatenate(datasets, axis=0)
+        N = X_all.shape[0]
+
+        labels = np.zeros(N)
+        offset = 0
+        for i, X in enumerate(datasets, 1):
+            n_obs = X.shape[0]
+            labels[offset : offset + n_obs] = i
+            offset += n_obs
+
+        self.score = label_entropy(X_all, labels, self.n_neighbors)
+        return self.score >= self.threshold
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/checking/checking.py` & `transmorph-0.2.7/src/transmorph/engine/checking/checking.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from abc import ABC, abstractmethod
-from typing import List
-
-from ..traits.canlog import CanLog
-from ..traits.isprofilable import IsProfilable
-
-
-class Checking(ABC, CanLog, IsProfilable):
-    """
-    Checking is the abstract class used to describe checking algorithms.
-    A "checking" is a function that takes as input a set of datasets
-    endowed with their respective embeddings, and provides a boolean
-    answer to "are these datasets satisfyingly integrated?". All checking
-    algorithms must inherit Checking, in addition to their own traits.
-
-    Parameters
-    ----------
-    str_identifier: str
-        Small string to identify the algorithm in logging.
-    """
-
-    def __init__(self, str_identifier: str):
-        CanLog.__init__(self, str_identifier=f"CHECKING_{str_identifier}")
-        IsProfilable.__init__(self)
-        self.score = 0.0
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Checks input validity, can be overriden at the condition to
-        start by calling the base verify_input inside.
-        """
-        pass
-
-    @abstractmethod
-    def check(self, datasets: List[np.ndarray]) -> bool:
-        """
-        Performs the checking over a list of AnnData, returns if the
-        statistical test is considered accepted given specified threshold.
-        This method should not be overriden, see $evaluate_metric instead.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of target datasets.
-
-        X_kw: str, default = ""
-            Target embeddings location in AnnDatas.
-        """
-        pass
+#!/usr/bin/env python3
+
+import numpy as np
+
+from abc import ABC, abstractmethod
+from typing import List
+
+from ..traits.canlog import CanLog
+from ..traits.isprofilable import IsProfilable
+
+
+class Checking(ABC, CanLog, IsProfilable):
+    """
+    Checking is the abstract class used to describe checking algorithms.
+    A "checking" is a function that takes as input a set of datasets
+    endowed with their respective embeddings, and provides a boolean
+    answer to "are these datasets satisfyingly integrated?". All checking
+    algorithms must inherit Checking, in addition to their own traits.
+
+    Parameters
+    ----------
+    str_identifier: str
+        Small string to identify the algorithm in logging.
+    """
+
+    def __init__(self, str_identifier: str):
+        CanLog.__init__(self, str_identifier=f"CHECKING_{str_identifier}")
+        IsProfilable.__init__(self)
+        self.score = 0.0
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Checks input validity, can be overriden at the condition to
+        start by calling the base verify_input inside.
+        """
+        pass
+
+    @abstractmethod
+    def check(self, datasets: List[np.ndarray]) -> bool:
+        """
+        Performs the checking over a list of AnnData, returns if the
+        statistical test is considered accepted given specified threshold.
+        This method should not be overriden, see $evaluate_metric instead.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of target datasets.
+
+        X_kw: str, default = ""
+            Target embeddings location in AnnDatas.
+        """
+        pass
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/evaluators/matching_evaluators.py` & `transmorph-0.2.7/src/transmorph/engine/evaluators/matching_evaluators.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from anndata import AnnData
-from typing import Callable, List
-
-from ...engine.layers import LayerMatching
-from ...stats.matching import edge_accuracy, edge_penalty
-
-
-def evaluate_matching_layer(
-    layer: LayerMatching,
-    datasets: List[AnnData],
-    evaluator: Callable,
-) -> np.ndarray:
-    """
-    layer: LayerMatching
-        LayerMatching which has been fit, containing matchings to
-        evaluate.
-
-    datasets: List[AnnData]
-        List of AnnData objects that have been passed to Model.fit().
-
-    evaluator: Callable
-        Evaluation metric f : AnnData, AnnData, csr_matrix -> float
-        to use.
-    """
-    ndatasets = len(datasets)
-    results = np.zeros((ndatasets, ndatasets), dtype=np.float32)
-    matchings = layer.get_matchings()
-    for i in range(ndatasets):
-        for j in range(i + 1, ndatasets):
-            results[i, j] = results[j, i] = evaluator(
-                datasets[i], datasets[j], matchings[i, j]
-            )
-    return results
-
-
-def matching_edge_accuracy_discrete(label: str) -> Callable:
-    """
-    This evaluator measures the frequency of edges in a matching
-    between two datasets that bind samples from the same class.
-
-    Parameters
-    ----------
-    label: str
-        .obs column entry containing labels.
-    """
-    return lambda a1, a2, T: 1.0 if a1 is a2 else edge_accuracy(a1, a2, T, label)
-
-
-def matching_edge_penalty_continuous(label: str) -> Callable:
-    """
-    This evaluator measures the frequency of edges in a matching
-    between two datasets that bind samples from the same class.
-
-    Parameters
-    ----------
-    label: str
-        .obs column entry containing labels.
-    """
-    return lambda a1, a2, T: 0.0 if a1 is a2 else edge_penalty(a1, a2, T, label)
+#!/usr/bin/env python3
+
+import numpy as np
+
+from anndata import AnnData
+from typing import Callable, List
+
+from ...engine.layers import LayerMatching
+from ...stats.matching import edge_accuracy, edge_penalty
+
+
+def evaluate_matching_layer(
+    layer: LayerMatching,
+    datasets: List[AnnData],
+    evaluator: Callable,
+) -> np.ndarray:
+    """
+    layer: LayerMatching
+        LayerMatching which has been fit, containing matchings to
+        evaluate.
+
+    datasets: List[AnnData]
+        List of AnnData objects that have been passed to Model.fit().
+
+    evaluator: Callable
+        Evaluation metric f : AnnData, AnnData, csr_matrix -> float
+        to use.
+    """
+    ndatasets = len(datasets)
+    results = np.zeros((ndatasets, ndatasets), dtype=np.float32)
+    matchings = layer.get_matchings()
+    for i in range(ndatasets):
+        for j in range(i + 1, ndatasets):
+            results[i, j] = results[j, i] = evaluator(
+                datasets[i], datasets[j], matchings[i, j]
+            )
+    return results
+
+
+def matching_edge_accuracy_discrete(label: str) -> Callable:
+    """
+    This evaluator measures the frequency of edges in a matching
+    between two datasets that bind samples from the same class.
+
+    Parameters
+    ----------
+    label: str
+        .obs column entry containing labels.
+    """
+    return lambda a1, a2, T: 1.0 if a1 is a2 else edge_accuracy(a1, a2, T, label)
+
+
+def matching_edge_penalty_continuous(label: str) -> Callable:
+    """
+    This evaluator measures the frequency of edges in a matching
+    between two datasets that bind samples from the same class.
+
+    Parameters
+    ----------
+    label: str
+        .obs column entry containing labels.
+    """
+    return lambda a1, a2, T: 0.0 if a1 is a2 else edge_penalty(a1, a2, T, label)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/layers/layer.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from anndata import AnnData
-from typing import List, Optional, Type
-
-from ..traits import CanLog, IsRepresentable, assert_trait
-from ...utils.misc import assert_type
-
-
-class Layer(ABC, CanLog):
-    """
-    A Layer is a structural object which wraps an algorithmic module,
-    and manages connections with other layers. All Layers derive from
-    this class, and can be enriched using traits. Layers are the deepest
-    objects in the architecture allowed to manipulate AnnData objects
-    without using traits.
-
-    Layers are not supposed to be manipulated for non-developement purposes.
-
-    Attributes
-    ----------
-    _embedding_reference: Optional[IsRepresentable], default = None
-        Layer able to provide a representation of datasets that
-        this layer will use as a reference.
-
-    compatible_inputs: List[Type], default = []
-        List of layer types that can connect this class of layer.
-
-    input_layer: Optional[Layer], default = None
-        Incoming layer if any.
-
-    layer_id: int
-        Unique integer identifier, facilitates debugging.
-
-    output_layers: List[Layer], default = []
-        List of layers that receive information from this layer.
-    """
-
-    # Provides a unique ID to each layer
-    LayerID = 0
-
-    def __init__(
-        self,
-        compatible_inputs: List[Type] = [],
-        str_identifier: str = "BASE",
-    ) -> None:
-        CanLog.__init__(self, str_identifier=f"LAYER_{str_identifier}#{Layer.LayerID}")
-        self.compatible_inputs = compatible_inputs
-        self._embedding_reference: Optional[IsRepresentable] = None
-        self.input_layer: Optional[Layer] = None
-        self.layer_id = Layer.LayerID
-        Layer.LayerID += 1
-        self.output_layers: List[Layer] = []
-        self.log("Initialized.")
-
-    def connect(self, layer: Layer) -> None:
-        """
-        Connects the current layer to an output layer, after
-        checking if they are compatible.
-
-        Parameters
-        ----------
-        layer: Layer
-            Output layer of compatible type.
-        """
-        assert_type(layer, Layer)
-        assert_type(self, tuple(layer.compatible_inputs))
-        assert layer not in self.output_layers, f"{self} already connected to {layer}."
-        assert layer.input_layer is None, f"{layer} has already a predecessor."
-        layer.input_layer = self
-        self.output_layers.append(layer)
-        self.log(f"Connected to layer {layer}.")
-        # Setting default embedding reference if needed
-        if layer._embedding_reference is None:
-            if not isinstance(self, IsRepresentable):
-                reference = self.embedding_reference
-            else:
-                reference = self
-            self.log(f"{reference} chosen as default embedding reference for {layer}.")
-            layer.embedding_reference = reference
-
-    @abstractmethod
-    def fit(self, datasets: List[AnnData]) -> List[Layer]:
-        """
-        This is the computational method, running an internal algorithm.
-        It then returns a list of downstream layers, to call next. It is
-        the deepest method in the architecture allowed to manipulate
-        AnnData objects without using traits.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of AnnData datasets to process.
-        """
-        pass
-
-    @property
-    def embedding_reference(self) -> IsRepresentable:
-        """
-        Retrieves closest IsRepresentable layer upstream from current layer.
-        """
-        if self._embedding_reference is None:
-            if self.input_layer is None:
-                self.raise_error(
-                    ValueError,
-                    "Input layer is None. Please make sure the "
-                    "pipeline contains at least an input layer.",
-                )
-            self._embedding_reference = self.input_layer.embedding_reference
-        return self._embedding_reference
-
-    @embedding_reference.setter
-    def embedding_reference(self, reference: IsRepresentable) -> None:
-        """
-        Sets a IsRepresentable layer to be the one providing matrix
-        representations of datasets.
-        """
-        assert_trait(reference, IsRepresentable)
-        self._embedding_reference = reference
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from anndata import AnnData
+from typing import List, Optional, Type
+
+from ..traits import CanLog, IsRepresentable, assert_trait
+from ...utils.misc import assert_type
+
+
+class Layer(ABC, CanLog):
+    """
+    A Layer is a structural object which wraps an algorithmic module,
+    and manages connections with other layers. All Layers derive from
+    this class, and can be enriched using traits. Layers are the deepest
+    objects in the architecture allowed to manipulate AnnData objects
+    without using traits.
+
+    Layers are not supposed to be manipulated for non-developement purposes.
+
+    Attributes
+    ----------
+    _embedding_reference: Optional[IsRepresentable], default = None
+        Layer able to provide a representation of datasets that
+        this layer will use as a reference.
+
+    compatible_inputs: List[Type], default = []
+        List of layer types that can connect this class of layer.
+
+    input_layer: Optional[Layer], default = None
+        Incoming layer if any.
+
+    layer_id: int
+        Unique integer identifier, facilitates debugging.
+
+    output_layers: List[Layer], default = []
+        List of layers that receive information from this layer.
+    """
+
+    # Provides a unique ID to each layer
+    LayerID = 0
+
+    def __init__(
+        self,
+        compatible_inputs: List[Type] = [],
+        str_identifier: str = "BASE",
+    ) -> None:
+        CanLog.__init__(self, str_identifier=f"LAYER_{str_identifier}#{Layer.LayerID}")
+        self.compatible_inputs = compatible_inputs
+        self._embedding_reference: Optional[IsRepresentable] = None
+        self.input_layer: Optional[Layer] = None
+        self.layer_id = Layer.LayerID
+        Layer.LayerID += 1
+        self.output_layers: List[Layer] = []
+        self.log("Initialized.")
+
+    def connect(self, layer: Layer) -> None:
+        """
+        Connects the current layer to an output layer, after
+        checking if they are compatible.
+
+        Parameters
+        ----------
+        layer: Layer
+            Output layer of compatible type.
+        """
+        assert_type(layer, Layer)
+        assert_type(self, tuple(layer.compatible_inputs))
+        assert layer not in self.output_layers, f"{self} already connected to {layer}."
+        assert layer.input_layer is None, f"{layer} has already a predecessor."
+        layer.input_layer = self
+        self.output_layers.append(layer)
+        self.log(f"Connected to layer {layer}.")
+        # Setting default embedding reference if needed
+        if layer._embedding_reference is None:
+            if not isinstance(self, IsRepresentable):
+                reference = self.embedding_reference
+            else:
+                reference = self
+            self.log(f"{reference} chosen as default embedding reference for {layer}.")
+            layer.embedding_reference = reference
+
+    @abstractmethod
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        This is the computational method, running an internal algorithm.
+        It then returns a list of downstream layers, to call next. It is
+        the deepest method in the architecture allowed to manipulate
+        AnnData objects without using traits.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of AnnData datasets to process.
+        """
+        pass
+
+    @property
+    def embedding_reference(self) -> IsRepresentable:
+        """
+        Retrieves closest IsRepresentable layer upstream from current layer.
+        """
+        if self._embedding_reference is None:
+            if self.input_layer is None:
+                self.raise_error(
+                    ValueError,
+                    "Input layer is None. Please make sure the "
+                    "pipeline contains at least an input layer.",
+                )
+            self._embedding_reference = self.input_layer.embedding_reference
+        return self._embedding_reference
+
+    @embedding_reference.setter
+    def embedding_reference(self, reference: IsRepresentable) -> None:
+        """
+        Sets a IsRepresentable layer to be the one providing matrix
+        representations of datasets.
+        """
+        assert_trait(reference, IsRepresentable)
+        self._embedding_reference = reference
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/layers/layerchecking.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layerchecking.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-#!/usr/bin/env python3
-
-import logging
-
-from anndata import AnnData
-from typing import List, Optional
-
-from . import Layer
-from ..checking import Checking
-from ..traits import (
-    CanCatchChecking,
-    ContainsTransformations,
-    IsProfilable,
-    profile_method,
-    IsRepresentable,
-    UsesSubsampling,
-    assert_trait,
-)
-from ..traits.utils import preprocess_traits
-from ..subsampling import Subsampling
-
-
-class LayerChecking(
-    Layer,
-    IsProfilable,
-    IsRepresentable,
-    UsesSubsampling,
-    ContainsTransformations,
-    CanCatchChecking,
-):
-    """
-    A checking layer is a layer that encapsulates a checking algorithm.
-    It is used to create logic branchings in Models, and has two
-    ouputs:
-
-    - Forward output, containing the next pipeline step if the
-      checking is accepted.
-
-    - Rejected output, containing the fallback step to carry out
-      if checking is rejected.
-
-    A checking layer can be used to create iterative procedures in
-    a model, playing the role of a while loop ("while the checking
-    is rejected, go back to an earlier pipeline step"). Temporary
-    transformations can be loaded in a checking layer to be carried
-    out before the checking algorithm.
-
-    Parameters
-    ----------
-    checking : Checking
-        Checking algorithm contained in the layer. This object is
-        endowed with a check() method, that will be called by the
-        layer. Model execution will then continue according to
-        the result.
-
-    min_score_variation : float, default = 0.01
-        Minimum score improvement between two checkings necessary
-        to avoid early exit.
-
-    n_checks_min : int, default = 3
-        Minuimum number of checkings to be carried out by the layer
-        before taking into account score improvement.
-
-    n_checks_max : int, default = 10
-        Maximum number of checkings to be carried out by the layer.
-        Beyond this number, it will automatically accept to avoid
-        endless looping.
-
-    subsampling : Optional[Subsampling], default = None
-        Subsampling algorithm to use before the checking, can help
-        for performance when dealing with large datasets.
-    """
-
-    # TODO: remove IsRepresentable trait from LayerChecking
-    #
-    # Attributes
-    # ----------
-    # check_is_valid: Optional[bool]
-    #     Contains validity of the last check, useful for logging
-    #     purposes.
-
-    # n_checks: int
-    #     Number of checkings that have been carried out by the layer.
-
-    # rejected_layer: Optional[CanCatchChecking]
-    #     Reference to the rejected output. This output must be an
-    #     instance of CanCatchChecking, meaning it is equipped to
-    #     receive information of a LayerChecking in case of
-    #     rejection.
-
-    # rejected_layer_ref: Optional[IsRepresentable]
-    #     Used to temporarily store the embedding reference of
-    #     rejected layer, that will be swapped during the loop with
-    #     this CheckingLayer.
-    def __init__(
-        self,
-        checking: Checking,
-        min_score_variation: float = 0.01,
-        n_checks_min: int = 3,
-        n_checks_max: int = 10,
-        subsampling: Optional[Subsampling] = None,
-    ) -> None:
-        Layer.__init__(
-            self,
-            compatible_inputs=[IsRepresentable],
-            str_identifier="CHECKING",
-        )
-        IsProfilable.__init__(self)
-        IsRepresentable.__init__(self, repr_key=f"{self}#{self.layer_id}")
-        UsesSubsampling.__init__(self, subsampling)
-        ContainsTransformations.__init__(self)
-        CanCatchChecking.__init__(self)
-        self.check_is_valid: Optional[bool] = None
-        self.checking = checking
-        self.min_score_variation = min_score_variation
-        self.n_checks_min = n_checks_min  # Min checks before early stop
-        self.n_checks_max = n_checks_max  # Max checks allowed
-        self.n_checks = 0  # Numbers of checkings done
-        self.rejected_layer: Optional[CanCatchChecking] = None
-        self.rejected_layer_ref: Optional[IsRepresentable] = None
-        self.scores: List[float] = []
-
-    def connect_rejected(self, layer: CanCatchChecking):
-        """
-        Connects this layer to another layer which will be called
-        in case of rejection. Target layer can be upstream in the
-        pipeline. It must inherit CanCatchChecking trait. A
-        LayerChecking can only have one target rejected layer.
-
-        Parameters
-        ----------
-        layer: CanCatchChecking
-            Target layer to call in the rejected case.
-        """
-        assert_trait(layer, CanCatchChecking)
-        assert isinstance(layer, Layer)
-        layer.catch_checking_rejected(self)
-        self.rejected_layer = layer
-
-    @profile_method
-    def fit(self, datasets: List[AnnData]) -> List[Layer]:
-        """
-        Runs the internal algorithm after carrying out the
-        appropriate preprocessings. Then, returns either the
-        rejected layer or standard output layers depending
-        on checking result.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            Datasets to run checking on.
-        """
-        assert self.rejected_layer is not None, "A rejected layer must be specified."
-        # Writing previous output for next layers to use
-        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
-        Xs = [self.embedding_reference.get_representation(adata) for adata in datasets]
-        is_feature_space = self.embedding_reference.is_feature_space
-        assert is_feature_space is not None
-        for adata, X in zip(datasets, Xs):
-            self.write_representation(
-                adata,
-                X,
-                is_feature_space,
-            )
-        # Preprocessing for self.checking if necessary
-        if self.has_transformations:
-            self.log("Calling preprocessings.", level=logging.INFO)
-        Xs = self.transform(datasets, self.embedding_reference)
-        # Subsampling if necessary
-        self.compute_subsampling(
-            datasets=datasets,
-            matrices=Xs,
-            is_feature_space=is_feature_space,
-            log_callback=self.log,
-        )
-        Xs = self.subsample_matrices(Xs)
-        # Retrieving metadata and common features if asked by
-        # self.checking
-        preprocess_traits(self.checking, datasets, is_feature_space)
-        # Performing actual checking
-        self.n_checks += 1
-        check_passed = self.checking.check(Xs)
-
-        self.scores.append(self.checking.score)
-
-        insufficient_variation, variation = False, 0.0
-        if len(self.scores) > 1:
-            variation = abs(self.scores[-1] - self.scores[-2]) / self.scores[-2]
-            insufficient_variation = variation < self.min_score_variation
-
-        self.info(f"Checking score: {self.scores[-1]}")
-
-        self.check_is_valid = (
-            check_passed
-            or insufficient_variation
-            and self.n_checks >= self.n_checks_min
-            or self.n_checks >= self.n_checks_max
-        )
-
-        # Routing accordingly
-        if self.check_is_valid:
-            if self.n_checks >= self.n_checks_max:
-                self.info("Maximum number of checks reached. Continuing.")
-            if insufficient_variation:
-                self.info(
-                    f"Insufficient improvement ({variation} < "
-                    f"{self.min_score_variation}). Continuing."
-                )
-            return self.output_layers
-        else:
-            self.log("Checking failed. Continuing.", level=logging.INFO)
-            self.rejected_layer.called_by_checking = True
-            assert isinstance(self.rejected_layer, Layer)
-            return [self.rejected_layer]
+#!/usr/bin/env python3
+
+import logging
+
+from anndata import AnnData
+from typing import List, Optional
+
+from . import Layer
+from ..checking import Checking
+from ..traits import (
+    CanCatchChecking,
+    ContainsTransformations,
+    IsProfilable,
+    profile_method,
+    IsRepresentable,
+    UsesSubsampling,
+    assert_trait,
+)
+from ..traits.utils import preprocess_traits
+from ..subsampling import Subsampling
+
+
+class LayerChecking(
+    Layer,
+    IsProfilable,
+    IsRepresentable,
+    UsesSubsampling,
+    ContainsTransformations,
+    CanCatchChecking,
+):
+    """
+    A checking layer is a layer that encapsulates a checking algorithm.
+    It is used to create logic branchings in Models, and has two
+    ouputs:
+
+    - Forward output, containing the next pipeline step if the
+      checking is accepted.
+
+    - Rejected output, containing the fallback step to carry out
+      if checking is rejected.
+
+    A checking layer can be used to create iterative procedures in
+    a model, playing the role of a while loop ("while the checking
+    is rejected, go back to an earlier pipeline step"). Temporary
+    transformations can be loaded in a checking layer to be carried
+    out before the checking algorithm.
+
+    Parameters
+    ----------
+    checking : Checking
+        Checking algorithm contained in the layer. This object is
+        endowed with a check() method, that will be called by the
+        layer. Model execution will then continue according to
+        the result.
+
+    min_score_variation : float, default = 0.01
+        Minimum score improvement between two checkings necessary
+        to avoid early exit.
+
+    n_checks_min : int, default = 3
+        Minuimum number of checkings to be carried out by the layer
+        before taking into account score improvement.
+
+    n_checks_max : int, default = 10
+        Maximum number of checkings to be carried out by the layer.
+        Beyond this number, it will automatically accept to avoid
+        endless looping.
+
+    subsampling : Optional[Subsampling], default = None
+        Subsampling algorithm to use before the checking, can help
+        for performance when dealing with large datasets.
+    """
+
+    # TODO: remove IsRepresentable trait from LayerChecking
+    #
+    # Attributes
+    # ----------
+    # check_is_valid: Optional[bool]
+    #     Contains validity of the last check, useful for logging
+    #     purposes.
+
+    # n_checks: int
+    #     Number of checkings that have been carried out by the layer.
+
+    # rejected_layer: Optional[CanCatchChecking]
+    #     Reference to the rejected output. This output must be an
+    #     instance of CanCatchChecking, meaning it is equipped to
+    #     receive information of a LayerChecking in case of
+    #     rejection.
+
+    # rejected_layer_ref: Optional[IsRepresentable]
+    #     Used to temporarily store the embedding reference of
+    #     rejected layer, that will be swapped during the loop with
+    #     this CheckingLayer.
+    def __init__(
+        self,
+        checking: Checking,
+        min_score_variation: float = 0.01,
+        n_checks_min: int = 3,
+        n_checks_max: int = 10,
+        subsampling: Optional[Subsampling] = None,
+    ) -> None:
+        Layer.__init__(
+            self,
+            compatible_inputs=[IsRepresentable],
+            str_identifier="CHECKING",
+        )
+        IsProfilable.__init__(self)
+        IsRepresentable.__init__(self, repr_key=f"{self}#{self.layer_id}")
+        UsesSubsampling.__init__(self, subsampling)
+        ContainsTransformations.__init__(self)
+        CanCatchChecking.__init__(self)
+        self.check_is_valid: Optional[bool] = None
+        self.checking = checking
+        self.min_score_variation = min_score_variation
+        self.n_checks_min = n_checks_min  # Min checks before early stop
+        self.n_checks_max = n_checks_max  # Max checks allowed
+        self.n_checks = 0  # Numbers of checkings done
+        self.rejected_layer: Optional[CanCatchChecking] = None
+        self.rejected_layer_ref: Optional[IsRepresentable] = None
+        self.scores: List[float] = []
+
+    def connect_rejected(self, layer: CanCatchChecking):
+        """
+        Connects this layer to another layer which will be called
+        in case of rejection. Target layer can be upstream in the
+        pipeline. It must inherit CanCatchChecking trait. A
+        LayerChecking can only have one target rejected layer.
+
+        Parameters
+        ----------
+        layer: CanCatchChecking
+            Target layer to call in the rejected case.
+        """
+        assert_trait(layer, CanCatchChecking)
+        assert isinstance(layer, Layer)
+        layer.catch_checking_rejected(self)
+        self.rejected_layer = layer
+
+    @profile_method
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        Runs the internal algorithm after carrying out the
+        appropriate preprocessings. Then, returns either the
+        rejected layer or standard output layers depending
+        on checking result.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to run checking on.
+        """
+        assert self.rejected_layer is not None, "A rejected layer must be specified."
+        # Writing previous output for next layers to use
+        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
+        Xs = [self.embedding_reference.get_representation(adata) for adata in datasets]
+        is_feature_space = self.embedding_reference.is_feature_space
+        assert is_feature_space is not None
+        for adata, X in zip(datasets, Xs):
+            self.write_representation(
+                adata,
+                X,
+                is_feature_space,
+            )
+        # Preprocessing for self.checking if necessary
+        if self.has_transformations:
+            self.log("Calling preprocessings.", level=logging.INFO)
+        Xs = self.transform(datasets, self.embedding_reference)
+        # Subsampling if necessary
+        self.compute_subsampling(
+            datasets=datasets,
+            matrices=Xs,
+            is_feature_space=is_feature_space,
+            log_callback=self.log,
+        )
+        Xs = self.subsample_matrices(Xs)
+        # Retrieving metadata and common features if asked by
+        # self.checking
+        preprocess_traits(self.checking, datasets, is_feature_space)
+        # Performing actual checking
+        self.n_checks += 1
+        check_passed = self.checking.check(Xs)
+
+        self.scores.append(self.checking.score)
+
+        insufficient_variation, variation = False, 0.0
+        if len(self.scores) > 1:
+            variation = abs(self.scores[-1] - self.scores[-2]) / self.scores[-2]
+            insufficient_variation = variation < self.min_score_variation
+
+        self.info(f"Checking score: {self.scores[-1]}")
+
+        self.check_is_valid = (
+            check_passed
+            or insufficient_variation
+            and self.n_checks >= self.n_checks_min
+            or self.n_checks >= self.n_checks_max
+        )
+
+        # Routing accordingly
+        if self.check_is_valid:
+            if self.n_checks >= self.n_checks_max:
+                self.info("Maximum number of checks reached. Continuing.")
+            if insufficient_variation:
+                self.info(
+                    f"Insufficient improvement ({variation} < "
+                    f"{self.min_score_variation}). Continuing."
+                )
+            return self.output_layers
+        else:
+            self.log("Checking failed. Continuing.", level=logging.INFO)
+            self.rejected_layer.called_by_checking = True
+            assert isinstance(self.rejected_layer, Layer)
+            return [self.rejected_layer]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/layers/layerinput.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layerinput.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import List
-
-from . import Layer
-from ..traits import IsRepresentable
-from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
-
-
-class LayerInput(Layer, IsRepresentable):
-    """
-    Every integration pipeline must contain exactly one input layer,
-    followed by an arbitrary network structure. Every
-    pipeline is initialized using this input layer. This
-    layer is the first to be called by any model. Its role
-    is just to check all representations are present, and
-    call subsequent layers. This layer can provide AnnData
-    matrix representations.
-    """
-
-    def __init__(self) -> None:
-        Layer.__init__(self, compatible_inputs=[], str_identifier="INPUT")
-        IsRepresentable.__init__(
-            self, repr_key=AnnDataKeyIdentifiers.BaseRepresentation
-        )
-
-    def fit(self, datasets: List[AnnData]) -> List[Layer]:
-        """
-        Simply checks dataset representations are at the right
-        place, and call downstream layers.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            Datasets to run checking on.
-        """
-        self.log("Checking if all representations are present.")
-        # Detecting if datasets are in feature space
-        self.is_feature_space = True
-        for adata in datasets:
-            X = adm.get_value(adata, self.repr_key)
-            assert X is not None, f"Representation {self.repr_key} missing in {adata}."
-            if X is not adata.X:
-                self.is_feature_space = False
-        self.log(
-            f"All representations found, in feature space: {self.is_feature_space}."
-        )
-        return self.output_layers
-
-    @property
-    def embedding_reference(self) -> IsRepresentable:
-        """
-        Each layer input is its own embedding reference, for
-        obvious structural reasons.
-        """
-        return self
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import List
+
+from . import Layer
+from ..traits import IsRepresentable
+from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
+
+
+class LayerInput(Layer, IsRepresentable):
+    """
+    Every integration pipeline must contain exactly one input layer,
+    followed by an arbitrary network structure. Every
+    pipeline is initialized using this input layer. This
+    layer is the first to be called by any model. Its role
+    is just to check all representations are present, and
+    call subsequent layers. This layer can provide AnnData
+    matrix representations.
+    """
+
+    def __init__(self) -> None:
+        Layer.__init__(self, compatible_inputs=[], str_identifier="INPUT")
+        IsRepresentable.__init__(
+            self, repr_key=AnnDataKeyIdentifiers.BaseRepresentation
+        )
+
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        Simply checks dataset representations are at the right
+        place, and call downstream layers.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to run checking on.
+        """
+        self.log("Checking if all representations are present.")
+        # Detecting if datasets are in feature space
+        self.is_feature_space = True
+        for adata in datasets:
+            X = adm.get_value(adata, self.repr_key)
+            assert X is not None, f"Representation {self.repr_key} missing in {adata}."
+            if X is not adata.X:
+                self.is_feature_space = False
+        self.log(
+            f"All representations found, in feature space: {self.is_feature_space}."
+        )
+        return self.output_layers
+
+    @property
+    def embedding_reference(self) -> IsRepresentable:
+        """
+        Each layer input is its own embedding reference, for
+        obvious structural reasons.
+        """
+        return self
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/layers/layermatching.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layermatching.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-from anndata import AnnData
-from scipy.sparse import csr_matrix
-from typing import List, Literal, Optional
-
-
-from . import Layer
-from ..matching import Matching, _TypeMatchingSet
-from ..subsampling import Subsampling
-from ..traits import (
-    CanCatchChecking,
-    ContainsTransformations,
-    IsProfilable,
-    profile_method,
-    UsesSubsampling,
-    IsRepresentable,
-    UsesSampleLabels,
-)
-from ..traits.utils import preprocess_traits
-from ...utils.graph import (
-    prune_edges_supervised,
-)
-
-
-class LayerMatching(
-    Layer,
-    CanCatchChecking,
-    ContainsTransformations,
-    IsProfilable,
-    UsesSubsampling,
-):
-    """
-    A LayerMatching encapsulates a matching algorithm, used to assess
-    similarity between samples across datasets. It then stores matching
-    results internally, and provides them upon request to a LayerMerging.
-    Merings use this information to build a common embedding between
-    datasets. Temporary transformations can be loaded in LayerMatching
-    to be carried out before the matching algorithm.
-
-    Parameters
-    ----------
-    matching: Matching
-        Matching algorithm contained in the layer. This object is
-        endowed with a fit() method, that will be called by the
-        layer.
-
-    subsampling: Optional[Subsampling], default = None
-        Subsampling algorithm to use before the matching, can help
-        for performance when dealing with large datasets. Note it
-        tends to greatly reduce the number of matching edges.
-
-    obs_class: Optional[str], default = None
-        Provides the AnnData.obs key where sample type is stored. If
-        specified, matching edges between samples of different class
-        are pruned.
-    """
-
-    def __init__(
-        self,
-        matching: Matching,
-        subsampling: Optional[Subsampling] = None,
-        obs_class: Optional[str] = None,
-        unsubsampling_scheme: Literal["raw", "transitive"] = "transitive",
-    ) -> None:
-        Layer.__init__(
-            self,
-            compatible_inputs=[IsRepresentable],
-            str_identifier="MATCHING",
-        )
-        CanCatchChecking.__init__(self)
-        ContainsTransformations.__init__(self)
-        IsProfilable.__init__(self)
-        UsesSubsampling.__init__(self, subsampling)
-        self.matching = matching
-        self.matching_matrices: Optional[_TypeMatchingSet] = None
-        self.obs_class = obs_class
-        self.unsubsampling_scheme = unsubsampling_scheme
-
-    @profile_method
-    def fit(self, datasets: List[AnnData]) -> List[Layer]:
-        """
-        Runs the internal algorithm after carrying out the
-        appropriate preprocessings. Then, returns next layers
-        in the model.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            Datasets to run matching on.
-        """
-        self.datasets = datasets.copy()  # Keeping a copy to preserve order
-
-        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
-
-        # Preprocessing if any
-        Xs = self.transform(
-            datasets=datasets,
-            representer=self.embedding_reference,
-            log_callback=self.log,
-        )
-
-        # Loading anndata information
-        is_feature_space = (
-            self.embedding_reference.is_feature_space and self.preserves_space
-        )
-        assert is_feature_space is not None
-        preprocess_traits(self.matching, datasets, is_feature_space)
-
-        # Subsampling
-        if self.has_subsampling:
-            self.info("Subsampling datasets...")
-
-        self.compute_subsampling(
-            datasets=datasets,
-            matrices=Xs,
-            is_feature_space=is_feature_space,
-            log_callback=self.log,
-        )
-        Xs = self.subsample_matrices(matrices=Xs)
-        if isinstance(self.matching, UsesSampleLabels):
-            # FIXME this will cause trouble if we update USL trait
-            self.matching.labels = self.subsample_matrices(self.matching.labels)
-
-        self.matching.check_input(Xs)
-
-        # Matching then supersampling matrices
-        self.info(f"Calling matching {self.matching}.")
-        self.matching_matrices = {}
-        for key, T in self.matching.fit(Xs).items():
-            i, j = key
-            if self.is_subsampled:
-                if self.unsubsampling_scheme == "raw":
-                    T = self.unsubsample_matrix_exact(T, i, j)
-                elif self.unsubsampling_scheme == "transitive":
-                    T = self.unsubsample_matrix_transitive(T, datasets[i], datasets[j])
-                else:
-                    self.raise_error(
-                        f"Unknown unsubsampling scheme: {self.unsubsampling_scheme}"
-                    )
-            assert isinstance(T, csr_matrix)
-            self.matching_matrices[i, j] = T
-            self.log(f"Datasets {key}, found {T.data.shape[0]} edges.")
-
-        # if some labels are available, prune edges
-        if self.obs_class is not None:
-            self.info(f"Pruning matching edges using {self.obs_class} labels...")
-            labels = [datasets[i].obs[self.obs_class] for i in range(len(datasets))]
-            self.matching_matrices = prune_edges_supervised(
-                self.matching_matrices,
-                labels,
-            )
-        return self.output_layers
-
-    def get_matchings(self) -> _TypeMatchingSet:
-        """
-        Returns computed matchings for read-only purposes.
-        get_matchings()[i, j] is the matching between datasets
-        i and j.
-        """
-        assert self.matching_matrices is not None, "Layer is not fit."
-        return self.matching_matrices
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+from anndata import AnnData
+from scipy.sparse import csr_matrix
+from typing import List, Literal, Optional
+
+
+from . import Layer
+from ..matching import Matching, _TypeMatchingSet
+from ..subsampling import Subsampling
+from ..traits import (
+    CanCatchChecking,
+    ContainsTransformations,
+    IsProfilable,
+    profile_method,
+    UsesSubsampling,
+    IsRepresentable,
+    UsesSampleLabels,
+)
+from ..traits.utils import preprocess_traits
+from ...utils.graph import (
+    prune_edges_supervised,
+)
+
+
+class LayerMatching(
+    Layer,
+    CanCatchChecking,
+    ContainsTransformations,
+    IsProfilable,
+    UsesSubsampling,
+):
+    """
+    A LayerMatching encapsulates a matching algorithm, used to assess
+    similarity between samples across datasets. It then stores matching
+    results internally, and provides them upon request to a LayerMerging.
+    Merings use this information to build a common embedding between
+    datasets. Temporary transformations can be loaded in LayerMatching
+    to be carried out before the matching algorithm.
+
+    Parameters
+    ----------
+    matching: Matching
+        Matching algorithm contained in the layer. This object is
+        endowed with a fit() method, that will be called by the
+        layer.
+
+    subsampling: Optional[Subsampling], default = None
+        Subsampling algorithm to use before the matching, can help
+        for performance when dealing with large datasets. Note it
+        tends to greatly reduce the number of matching edges.
+
+    obs_class: Optional[str], default = None
+        Provides the AnnData.obs key where sample type is stored. If
+        specified, matching edges between samples of different class
+        are pruned.
+    """
+
+    def __init__(
+        self,
+        matching: Matching,
+        subsampling: Optional[Subsampling] = None,
+        obs_class: Optional[str] = None,
+        unsubsampling_scheme: Literal["raw", "transitive"] = "transitive",
+    ) -> None:
+        Layer.__init__(
+            self,
+            compatible_inputs=[IsRepresentable],
+            str_identifier="MATCHING",
+        )
+        CanCatchChecking.__init__(self)
+        ContainsTransformations.__init__(self)
+        IsProfilable.__init__(self)
+        UsesSubsampling.__init__(self, subsampling)
+        self.matching = matching
+        self.matching_matrices: Optional[_TypeMatchingSet] = None
+        self.obs_class = obs_class
+        self.unsubsampling_scheme = unsubsampling_scheme
+
+    @profile_method
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        Runs the internal algorithm after carrying out the
+        appropriate preprocessings. Then, returns next layers
+        in the model.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to run matching on.
+        """
+        self.datasets = datasets.copy()  # Keeping a copy to preserve order
+
+        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
+
+        # Preprocessing if any
+        Xs = self.transform(
+            datasets=datasets,
+            representer=self.embedding_reference,
+            log_callback=self.log,
+        )
+
+        # Loading anndata information
+        is_feature_space = (
+            self.embedding_reference.is_feature_space and self.preserves_space
+        )
+        assert is_feature_space is not None
+        preprocess_traits(self.matching, datasets, is_feature_space)
+
+        # Subsampling
+        if self.has_subsampling:
+            self.info("Subsampling datasets...")
+
+        self.compute_subsampling(
+            datasets=datasets,
+            matrices=Xs,
+            is_feature_space=is_feature_space,
+            log_callback=self.log,
+        )
+        Xs = self.subsample_matrices(matrices=Xs)
+        if isinstance(self.matching, UsesSampleLabels):
+            # FIXME this will cause trouble if we update USL trait
+            self.matching.labels = self.subsample_matrices(self.matching.labels)
+
+        self.matching.check_input(Xs)
+
+        # Matching then supersampling matrices
+        self.info(f"Calling matching {self.matching}.")
+        self.matching_matrices = {}
+        for key, T in self.matching.fit(Xs).items():
+            i, j = key
+            if self.is_subsampled:
+                if self.unsubsampling_scheme == "raw":
+                    T = self.unsubsample_matrix_exact(T, i, j)
+                elif self.unsubsampling_scheme == "transitive":
+                    T = self.unsubsample_matrix_transitive(T, datasets[i], datasets[j])
+                else:
+                    self.raise_error(
+                        f"Unknown unsubsampling scheme: {self.unsubsampling_scheme}"
+                    )
+            assert isinstance(T, csr_matrix)
+            self.matching_matrices[i, j] = T
+            self.log(f"Datasets {key}, found {T.data.shape[0]} edges.")
+
+        # if some labels are available, prune edges
+        if self.obs_class is not None:
+            self.info(f"Pruning matching edges using {self.obs_class} labels...")
+            labels = [datasets[i].obs[self.obs_class] for i in range(len(datasets))]
+            self.matching_matrices = prune_edges_supervised(
+                self.matching_matrices,
+                labels,
+            )
+        return self.output_layers
+
+    def get_matchings(self) -> _TypeMatchingSet:
+        """
+        Returns computed matchings for read-only purposes.
+        get_matchings()[i, j] is the matching between datasets
+        i and j.
+        """
+        assert self.matching_matrices is not None, "Layer is not fit."
+        return self.matching_matrices
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/layers/layermerging.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layermerging.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import List
-
-from . import Layer, LayerMatching
-from ..merging import Merging
-from ..traits import (
-    ContainsTransformations,
-    IsProfilable,
-    profile_method,
-    IsRepresentable,
-)
-from ..traits.utils import preprocess_traits
-
-
-class LayerMerging(
-    Layer,
-    ContainsTransformations,
-    IsProfilable,
-    IsRepresentable,
-):
-    """
-    A LayerMerging encapsulates a merging algorithms, used to leverage
-    matching information to embed several datasets in a common integration
-    space. It can only follow a LayerMatching, and is able to provide
-    matrix representation of AnnData datasets. Temporary transformations
-    can be loaded in LayerMatching to be carried out before the matching
-    algorithm.
-
-    Parameters
-    ----------
-    merging: Merging
-        Merging algorithm contained in the layer. This object is
-        endowed with a transform() method, that will be called by the
-        layer.
-    """
-
-    def __init__(self, merging: Merging) -> None:
-        Layer.__init__(
-            self, compatible_inputs=[LayerMatching], str_identifier="MERGING"
-        )
-        ContainsTransformations.__init__(self)
-        IsProfilable.__init__(self)
-        IsRepresentable.__init__(self, repr_key=f"{self}_{self.layer_id}")
-        self.merging = merging
-
-    @profile_method
-    def fit(self, datasets: List[AnnData]) -> List[Layer]:
-        """
-        Runs the internal algorithm after carrying out the
-        appropriate preprocessings. Then, returns next layers
-        in the model.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            Datasets to run merging on.
-        """
-        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
-        Xs = self.transform(
-            datasets=datasets,
-            representer=self.embedding_reference,
-            log_callback=self.log,
-        )
-        is_feature_space = (
-            self.embedding_reference.is_feature_space  # Original matrices
-            and self.preserves_space  # Internal transformations
-            and self.merging.preserves_space  # Internal matching
-        )
-        preprocess_traits(self.merging, datasets, is_feature_space)
-        assert isinstance(self.input_layer, LayerMatching)
-        self.merging.set_matchings(self.input_layer.get_matchings())
-        self.info(f"Running merging {self.merging}...")
-        Xs_transform = self.merging.transform(datasets, Xs)
-        for adata, X_after in zip(datasets, Xs_transform):
-            self.write_representation(adata, X_after, is_feature_space=is_feature_space)
-        return self.output_layers
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import List
+
+from . import Layer, LayerMatching
+from ..merging import Merging
+from ..traits import (
+    ContainsTransformations,
+    IsProfilable,
+    profile_method,
+    IsRepresentable,
+)
+from ..traits.utils import preprocess_traits
+
+
+class LayerMerging(
+    Layer,
+    ContainsTransformations,
+    IsProfilable,
+    IsRepresentable,
+):
+    """
+    A LayerMerging encapsulates a merging algorithms, used to leverage
+    matching information to embed several datasets in a common integration
+    space. It can only follow a LayerMatching, and is able to provide
+    matrix representation of AnnData datasets. Temporary transformations
+    can be loaded in LayerMatching to be carried out before the matching
+    algorithm.
+
+    Parameters
+    ----------
+    merging: Merging
+        Merging algorithm contained in the layer. This object is
+        endowed with a transform() method, that will be called by the
+        layer.
+    """
+
+    def __init__(self, merging: Merging) -> None:
+        Layer.__init__(
+            self, compatible_inputs=[LayerMatching], str_identifier="MERGING"
+        )
+        ContainsTransformations.__init__(self)
+        IsProfilable.__init__(self)
+        IsRepresentable.__init__(self, repr_key=f"{self}_{self.layer_id}")
+        self.merging = merging
+
+    @profile_method
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        Runs the internal algorithm after carrying out the
+        appropriate preprocessings. Then, returns next layers
+        in the model.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to run merging on.
+        """
+        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
+        Xs = self.transform(
+            datasets=datasets,
+            representer=self.embedding_reference,
+            log_callback=self.log,
+        )
+        is_feature_space = (
+            self.embedding_reference.is_feature_space  # Original matrices
+            and self.preserves_space  # Internal transformations
+            and self.merging.preserves_space  # Internal matching
+        )
+        preprocess_traits(self.merging, datasets, is_feature_space)
+        assert isinstance(self.input_layer, LayerMatching)
+        self.merging.set_matchings(self.input_layer.get_matchings())
+        self.info(f"Running merging {self.merging}...")
+        Xs_transform = self.merging.transform(datasets, Xs)
+        for adata, X_after in zip(datasets, Xs_transform):
+            self.write_representation(adata, X_after, is_feature_space=is_feature_space)
+        return self.output_layers
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/bknn.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/bknn.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from scipy.sparse import csr_matrix
-from typing import Dict, List, Literal, Optional
-
-from ..matching import Matching, _TypeMatchingSet
-from ...traits.isprofilable import profile_method
-from ...traits.usescommonfeatures import UsesCommonFeatures
-from ...traits.usesreference import UsesReference
-from ....utils.graph import (
-    generate_qtree,
-    qtree_k_nearest_neighbors,
-    nearest_neighbors_custom,
-)
-
-
-class BKNN(Matching, UsesCommonFeatures, UsesReference):
-    """
-    Batch k-nearest neighbors matching. x from batch X is matched with
-    y from batch Y if y belongs to the k nearest neighbors of x in Y.
-
-    We propose two solvers,
-
-    - An exact solver, which computes all pairwise distances between
-      batches, computes exact nearest neighbors and makes the intersection
-    - An approximate solver, that leverages NNDescent algorithm to
-      compute approximate nearest neighbors using projection trees.
-      This allows MNN to scale to large, high dimensional datasets.
-
-    Parameters
-    ----------
-    metric: str or Callable, default = "sqeuclidean"
-        Scipy-compatible metric for kNN computation.
-
-    metric_kwargs: dict, default = {}
-        Additional metric parameters.
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use between batches.
-
-    common_features_mode: Literal["pairwise", "total"], default = "pairwise"
-        Uses pairwise common features, or total common features. Use "total"
-        for a small number of datasets, and "pairwise" if the features
-        intersection is too small. Ignored if datasets are not in feature
-        space, set to "total" if solver = "pynndescent".
-
-    solver: Literal["auto", "exact", "pynndescent"], default = "auto"
-        Solver to use.
-    """
-
-    def __init__(
-        self,
-        metric: str = "sqeuclidean",
-        metric_kwargs: Optional[Dict] = None,
-        n_neighbors: int = 10,
-        common_features_mode: Literal["pairwise", "total"] = "pairwise",
-    ):
-        Matching.__init__(self, str_identifier="MNN")
-        UsesCommonFeatures.__init__(self, mode=common_features_mode)
-        UsesReference.__init__(self)
-        self.metric = metric
-        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
-        self.n_neighbors = n_neighbors
-
-    @profile_method
-    def fit(
-        self,
-        datasets: List[np.ndarray],
-    ) -> _TypeMatchingSet:
-        """
-        Computes BKNN between pairs of datasets.
-        """
-        ndatasets = len(datasets)
-        results: _TypeMatchingSet = {}
-        reference = self.reference_index
-        if reference is None:
-            target_indices = np.arange(ndatasets)
-        else:
-            target_indices = [reference]
-        small_scale_problem = all(X.shape[0] < 100 for X in datasets)
-        if not small_scale_problem:
-            qtrees = [
-                generate_qtree(X, self.metric, self.metric_kwargs) for X in datasets
-            ]
-        for i in range(ndatasets):
-            for j in target_indices:
-                if i == j:
-                    continue
-                Xi, Yi = self.slice_features(
-                    X1=datasets[i],
-                    X2=datasets[j],
-                    idx_1=i,
-                    idx_2=j,
-                )
-                if small_scale_problem:
-                    Tij = nearest_neighbors_custom(
-                        Xi, mode="edges", n_neighbors=self.n_neighbors, Y=Yi
-                    )
-                else:
-                    Tij = qtree_k_nearest_neighbors(
-                        Xi,
-                        qtrees[j],
-                        n_neighbors=self.n_neighbors,
-                    )
-                results[i, j] = csr_matrix(Tij)
-        return results
+#!/usr/bin/env python3
+
+import numpy as np
+
+from scipy.sparse import csr_matrix
+from typing import Dict, List, Literal, Optional
+
+from ..matching import Matching, _TypeMatchingSet
+from ...traits.isprofilable import profile_method
+from ...traits.usescommonfeatures import UsesCommonFeatures
+from ...traits.usesreference import UsesReference
+from ....utils.graph import (
+    generate_qtree,
+    qtree_k_nearest_neighbors,
+    nearest_neighbors_custom,
+)
+
+
+class BKNN(Matching, UsesCommonFeatures, UsesReference):
+    """
+    Batch k-nearest neighbors matching. x from batch X is matched with
+    y from batch Y if y belongs to the k nearest neighbors of x in Y.
+
+    We propose two solvers,
+
+    - An exact solver, which computes all pairwise distances between
+      batches, computes exact nearest neighbors and makes the intersection
+    - An approximate solver, that leverages NNDescent algorithm to
+      compute approximate nearest neighbors using projection trees.
+      This allows MNN to scale to large, high dimensional datasets.
+
+    Parameters
+    ----------
+    metric: str or Callable, default = "sqeuclidean"
+        Scipy-compatible metric for kNN computation.
+
+    metric_kwargs: dict, default = {}
+        Additional metric parameters.
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use between batches.
+
+    common_features_mode: Literal["pairwise", "total"], default = "pairwise"
+        Uses pairwise common features, or total common features. Use "total"
+        for a small number of datasets, and "pairwise" if the features
+        intersection is too small. Ignored if datasets are not in feature
+        space, set to "total" if solver = "pynndescent".
+
+    solver: Literal["auto", "exact", "pynndescent"], default = "auto"
+        Solver to use.
+    """
+
+    def __init__(
+        self,
+        metric: str = "sqeuclidean",
+        metric_kwargs: Optional[Dict] = None,
+        n_neighbors: int = 10,
+        common_features_mode: Literal["pairwise", "total"] = "pairwise",
+    ):
+        Matching.__init__(self, str_identifier="MNN")
+        UsesCommonFeatures.__init__(self, mode=common_features_mode)
+        UsesReference.__init__(self)
+        self.metric = metric
+        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
+        self.n_neighbors = n_neighbors
+
+    @profile_method
+    def fit(
+        self,
+        datasets: List[np.ndarray],
+    ) -> _TypeMatchingSet:
+        """
+        Computes BKNN between pairs of datasets.
+        """
+        ndatasets = len(datasets)
+        results: _TypeMatchingSet = {}
+        reference = self.reference_index
+        if reference is None:
+            target_indices = np.arange(ndatasets)
+        else:
+            target_indices = [reference]
+        small_scale_problem = all(X.shape[0] < 100 for X in datasets)
+        if not small_scale_problem:
+            qtrees = [
+                generate_qtree(X, self.metric, self.metric_kwargs) for X in datasets
+            ]
+        for i in range(ndatasets):
+            for j in target_indices:
+                if i == j:
+                    continue
+                Xi, Yi = self.slice_features(
+                    X1=datasets[i],
+                    X2=datasets[j],
+                    idx_1=i,
+                    idx_2=j,
+                )
+                if small_scale_problem:
+                    Tij = nearest_neighbors_custom(
+                        Xi, mode="edges", n_neighbors=self.n_neighbors, Y=Yi
+                    )
+                else:
+                    Tij = qtree_k_nearest_neighbors(
+                        Xi,
+                        qtrees[j],
+                        n_neighbors=self.n_neighbors,
+                    )
+                results[i, j] = csr_matrix(Tij)
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/combinematching.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/combinematching.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from typing import List, Literal
-
-from ..matching import Matching, _TypeMatchingSet
-
-
-class CombineMatching(Matching):
-    def __init__(self, rule: Literal["and", "or", "min", "max"], *matchings):
-        Matching.__init__(self, str_identifier="COMBINE_MATCHING")
-        assert rule in [
-            "and",
-            "or",
-            "min",
-            "max",
-        ], f"Unrecognized rule: {rule}. Expected 'and', 'or', 'min' or 'max'."
-        self.rule = rule
-        self.matchings: List[Matching] = [matching for matching in matchings]
-        assert all(
-            isinstance(matching, Matching) for matching in self.matchings
-        ), "Non-matching object detected."
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        for matching in self.matchings:
-            matching.check_input(datasets)
-
-    def fit(self, datasets: List[np.ndarray]) -> _TypeMatchingSet:
-        matching_results: List[_TypeMatchingSet] = []
-        for matching in self.matchings:
-            matching_results.append(matching.fit(datasets))
-        result = {}
-        for (i, j) in matching_results[0]:
-            result_mtx = matching_results[0][i, j].copy()
-            for matching_result in matching_results[1:]:
-                if self.rule == "and":
-                    result_mtx = result_mtx * matching_result[i, j]
-                elif self.rule == "or":
-                    result_mtx = result_mtx + matching_result[i, j]
-                elif self.rule == "min":
-                    result_mtx = result_mtx.minimum(matching_result)[i, j]
-                elif self.rule == "max":
-                    result_mtx = result_mtx.maximum(matching_result)[i, j]
-                else:
-                    raise ValueError(f"Unrecognized rule: {self.rule}")
-            result[i, j] = result_mtx
-        return result
+#!/usr/bin/env python3
+
+import numpy as np
+
+from typing import List, Literal
+
+from ..matching import Matching, _TypeMatchingSet
+
+
+class CombineMatching(Matching):
+    def __init__(self, rule: Literal["and", "or", "min", "max"], *matchings):
+        Matching.__init__(self, str_identifier="COMBINE_MATCHING")
+        assert rule in [
+            "and",
+            "or",
+            "min",
+            "max",
+        ], f"Unrecognized rule: {rule}. Expected 'and', 'or', 'min' or 'max'."
+        self.rule = rule
+        self.matchings: List[Matching] = [matching for matching in matchings]
+        assert all(
+            isinstance(matching, Matching) for matching in self.matchings
+        ), "Non-matching object detected."
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        for matching in self.matchings:
+            matching.check_input(datasets)
+
+    def fit(self, datasets: List[np.ndarray]) -> _TypeMatchingSet:
+        matching_results: List[_TypeMatchingSet] = []
+        for matching in self.matchings:
+            matching_results.append(matching.fit(datasets))
+        result = {}
+        for (i, j) in matching_results[0]:
+            result_mtx = matching_results[0][i, j].copy()
+            for matching_result in matching_results[1:]:
+                if self.rule == "and":
+                    result_mtx = result_mtx * matching_result[i, j]
+                elif self.rule == "or":
+                    result_mtx = result_mtx + matching_result[i, j]
+                elif self.rule == "min":
+                    result_mtx = result_mtx.minimum(matching_result)[i, j]
+                elif self.rule == "max":
+                    result_mtx = result_mtx.maximum(matching_result)[i, j]
+                else:
+                    raise ValueError(f"Unrecognized rule: {self.rule}")
+            result[i, j] = result_mtx
+        return result
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/gw.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/gw.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from scipy.sparse import csr_matrix
-from scipy.spatial.distance import cdist
-from typing import Dict, List, Literal, Optional
-from ot.gromov import gromov_wasserstein, entropic_gromov_wasserstein
-
-from ..matching import Matching, _TypeMatchingSet
-from ...traits.isprofilable import profile_method
-from ...traits.usesmetric import UsesMetric
-from ...traits.usesreference import UsesReference
-
-
-class GW(Matching, UsesMetric, UsesReference):
-    """
-    Gromov-Wasserstein-based matching. Embeds the gromov_wasserstein class of
-    methods from POT:
-
-        https://github.com/PythonOT/POT
-
-    Gromov-Wasserstein(GW) computes a transport plan between two distributions,
-    and does not require them to be defined in the same space. It rather use
-    relative topology of each distribution in its own metric space to define a
-    cost that assumes similar locations to have similar relative positions with
-    respect to the other regions. This combinatorial cost is typically more
-    expansive than the optimal transport alternative, but comes very handy when
-    a ground cost is difficult (or impossible) to compute between distributions.
-    It is unfortunately prone to overfitting, and is sensitive to class
-    imbalance between datasets.
-
-    Parameters
-    ----------
-    optimizer: Literal["GW", "GWEntropic"], default = "GW"
-        Uses the exact (GW) or entropy regularized (GWEntropic) problem
-        formulation.
-
-    default_metric: str or callable, default = "sqeuclidean"
-        Scipy-compatible metric to use for datasets in which metric
-        is not specified as a backup.
-
-    default_metric_kwargs: dict, default = {}
-        Additional metric parameters for backup metric.
-
-    GW_loss: str, default = "square_loss"
-        Loss to use in the Gromov-Wasserstein problem. Valid options
-        are "square_loss", "kl_loss".
-
-    entropy_epsilon: Optional[float]
-        If optimizer is GWEntropic, this is the regularization parameter.
-        Decreasing it will improve result quality, but it will decrease
-        convergence speed.
-
-    max_iter: int, default = 1e6
-        Maximum number of iterations to solve the optimization problem.
-
-    References
-    ----------
-    [1] Gabriel Peyré, Marco Cuturi, and Justin Solomon,
-        "Gromov-Wasserstein averaging of kernel and distance matrices."
-        International Conference on Machine Learning (ICML). 2016.
-    [2] Mémoli, Facundo. Gromov–Wasserstein distances and the
-        metric approach to object matching. Foundations of computational
-        mathematics 11.4 (2011): 417-487.
-    """
-
-    def __init__(
-        self,
-        optimizer: Literal["gw", "entropic_gw"] = "gw",
-        default_metric: str = "sqeuclidean",
-        default_metric_kwargs: Optional[Dict] = None,
-        GW_loss: str = "square_loss",
-        entropy_epsilon: Optional[float] = None,
-        max_iter: int = int(1e6),
-    ):
-        Matching.__init__(self, str_identifier="GW")
-        UsesMetric.__init__(
-            self,
-            default_metric=default_metric,
-            default_kwargs=default_metric_kwargs,
-        )
-        UsesReference.__init__(self)
-        assert optimizer in ("gw", "entropic_gw"), f"Unknown optimizer: {optimizer}."
-        self.optimizer = optimizer
-        self.GW_loss = GW_loss
-        if entropy_epsilon is not None and optimizer == "gw":
-            self.warn("Epsilon specified has no effect on gw optimizer.")
-        if entropy_epsilon is None:
-            entropy_epsilon = 1e-2
-        self.entropy_epsilon = entropy_epsilon
-        self.max_iter = int(max_iter)
-
-    @profile_method
-    def fit(
-        self,
-        datasets: List[np.ndarray],
-    ) -> _TypeMatchingSet:
-        """
-        Compute optimal transport plan for the FGW problem.
-        TODO: specific strategy if reference is set
-        """
-        # Precomputes weights and internal distances
-        all_w = [np.ones(X.shape[0]) / X.shape[0] for X in datasets]
-        all_metrics = [self.get_metric(i) for i in range(len(datasets))]
-        all_C = [
-            cdist(Xi, Xi, metric, **kwargs)
-            for Xi, (metric, kwargs) in zip(datasets, all_metrics)
-        ]
-        all_C = [C / C.max() for C in all_C]
-        # Selects optimizer
-        if self.optimizer == "gw":
-            optimizer = gromov_wasserstein
-            kwargs = {"numItermax": self.max_iter}
-        elif self.optimizer == "entropic_gw":
-            optimizer = entropic_gromov_wasserstein
-            kwargs = {"epsilon": self.entropy_epsilon, "max_iter": self.max_iter}
-        else:
-            raise ValueError(f"Unknown optimizer: {self.optimizer}.")
-        # Compute pairwise GW
-        ndatasets = len(datasets)
-        result: _TypeMatchingSet = {}
-        ndatasets = len(datasets)
-        reference = self.reference_index
-        if reference is None:
-            target_indices = np.arange(ndatasets)
-        else:
-            target_indices = [reference]
-        for i in range(ndatasets):
-            for j in target_indices:
-                if (i, j) in result:
-                    continue
-                Tij = optimizer(
-                    C1=all_C[i],
-                    C2=all_C[j],
-                    p=all_w[i],
-                    q=all_w[j],
-                    loss_fun=self.GW_loss,
-                    **kwargs,
-                )
-                result[i, j] = csr_matrix(Tij)
-                result[j, i] = csr_matrix(Tij.T)
-        return result
+#!/usr/bin/env python3
+
+import numpy as np
+
+from scipy.sparse import csr_matrix
+from scipy.spatial.distance import cdist
+from typing import Dict, List, Literal, Optional
+from ot.gromov import gromov_wasserstein, entropic_gromov_wasserstein
+
+from ..matching import Matching, _TypeMatchingSet
+from ...traits.isprofilable import profile_method
+from ...traits.usesmetric import UsesMetric
+from ...traits.usesreference import UsesReference
+
+
+class GW(Matching, UsesMetric, UsesReference):
+    """
+    Gromov-Wasserstein-based matching. Embeds the gromov_wasserstein class of
+    methods from POT:
+
+        https://github.com/PythonOT/POT
+
+    Gromov-Wasserstein(GW) computes a transport plan between two distributions,
+    and does not require them to be defined in the same space. It rather use
+    relative topology of each distribution in its own metric space to define a
+    cost that assumes similar locations to have similar relative positions with
+    respect to the other regions. This combinatorial cost is typically more
+    expansive than the optimal transport alternative, but comes very handy when
+    a ground cost is difficult (or impossible) to compute between distributions.
+    It is unfortunately prone to overfitting, and is sensitive to class
+    imbalance between datasets.
+
+    Parameters
+    ----------
+    optimizer: Literal["GW", "GWEntropic"], default = "GW"
+        Uses the exact (GW) or entropy regularized (GWEntropic) problem
+        formulation.
+
+    default_metric: str or callable, default = "sqeuclidean"
+        Scipy-compatible metric to use for datasets in which metric
+        is not specified as a backup.
+
+    default_metric_kwargs: dict, default = {}
+        Additional metric parameters for backup metric.
+
+    GW_loss: str, default = "square_loss"
+        Loss to use in the Gromov-Wasserstein problem. Valid options
+        are "square_loss", "kl_loss".
+
+    entropy_epsilon: Optional[float]
+        If optimizer is GWEntropic, this is the regularization parameter.
+        Decreasing it will improve result quality, but it will decrease
+        convergence speed.
+
+    max_iter: int, default = 1e6
+        Maximum number of iterations to solve the optimization problem.
+
+    References
+    ----------
+    [1] Gabriel Peyré, Marco Cuturi, and Justin Solomon,
+        "Gromov-Wasserstein averaging of kernel and distance matrices."
+        International Conference on Machine Learning (ICML). 2016.
+    [2] Mémoli, Facundo. Gromov–Wasserstein distances and the
+        metric approach to object matching. Foundations of computational
+        mathematics 11.4 (2011): 417-487.
+    """
+
+    def __init__(
+        self,
+        optimizer: Literal["gw", "entropic_gw"] = "gw",
+        default_metric: str = "sqeuclidean",
+        default_metric_kwargs: Optional[Dict] = None,
+        GW_loss: str = "square_loss",
+        entropy_epsilon: Optional[float] = None,
+        max_iter: int = int(1e6),
+    ):
+        Matching.__init__(self, str_identifier="GW")
+        UsesMetric.__init__(
+            self,
+            default_metric=default_metric,
+            default_kwargs=default_metric_kwargs,
+        )
+        UsesReference.__init__(self)
+        assert optimizer in ("gw", "entropic_gw"), f"Unknown optimizer: {optimizer}."
+        self.optimizer = optimizer
+        self.GW_loss = GW_loss
+        if entropy_epsilon is not None and optimizer == "gw":
+            self.warn("Epsilon specified has no effect on gw optimizer.")
+        if entropy_epsilon is None:
+            entropy_epsilon = 1e-2
+        self.entropy_epsilon = entropy_epsilon
+        self.max_iter = int(max_iter)
+
+    @profile_method
+    def fit(
+        self,
+        datasets: List[np.ndarray],
+    ) -> _TypeMatchingSet:
+        """
+        Compute optimal transport plan for the FGW problem.
+        TODO: specific strategy if reference is set
+        """
+        # Precomputes weights and internal distances
+        all_w = [np.ones(X.shape[0]) / X.shape[0] for X in datasets]
+        all_metrics = [self.get_metric(i) for i in range(len(datasets))]
+        all_C = [
+            cdist(Xi, Xi, metric, **kwargs)
+            for Xi, (metric, kwargs) in zip(datasets, all_metrics)
+        ]
+        all_C = [C / C.max() for C in all_C]
+        # Selects optimizer
+        if self.optimizer == "gw":
+            optimizer = gromov_wasserstein
+            kwargs = {"numItermax": self.max_iter}
+        elif self.optimizer == "entropic_gw":
+            optimizer = entropic_gromov_wasserstein
+            kwargs = {"epsilon": self.entropy_epsilon, "max_iter": self.max_iter}
+        else:
+            raise ValueError(f"Unknown optimizer: {self.optimizer}.")
+        # Compute pairwise GW
+        ndatasets = len(datasets)
+        result: _TypeMatchingSet = {}
+        ndatasets = len(datasets)
+        reference = self.reference_index
+        if reference is None:
+            target_indices = np.arange(ndatasets)
+        else:
+            target_indices = [reference]
+        for i in range(ndatasets):
+            for j in target_indices:
+                if (i, j) in result:
+                    continue
+                Tij = optimizer(
+                    C1=all_C[i],
+                    C2=all_C[j],
+                    p=all_w[i],
+                    q=all_w[j],
+                    loss_fun=self.GW_loss,
+                    **kwargs,
+                )
+                result[i, j] = csr_matrix(Tij)
+                result[j, i] = csr_matrix(Tij.T)
+        return result
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/labels.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/labels.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from scipy.sparse import csr_matrix
-from typing import List
-
-from ..matching import Matching, _TypeMatchingSet
-from ...traits.isprofilable import profile_method
-from ...traits.usessamplelabels import UsesSampleLabels
-
-
-class Labels(Matching, UsesSampleLabels):
-    """
-    Supervised, label-based boolean matching that matches every pair
-    of samples that share the same label. Does not depend on dataset
-    dimensionality, and will typically generate a lot -- O(n^2) -- of
-    edges.
-
-    Parameters
-    ----------
-    label_obs: str
-        AnnData.obs entry containing categorical labels.
-    """
-
-    def __init__(self, label_obs: str):
-        Matching.__init__(self, str_identifier="LABELS")
-        UsesSampleLabels.__init__(self, label_obs=label_obs)
-
-    @profile_method
-    def fit(
-        self,
-        datasets: List[np.ndarray],
-    ) -> _TypeMatchingSet:
-        """
-        Collects label matching matrices using UsesSampleLabels
-        trait, then computes the matching.
-        """
-        ndatasets = len(datasets)
-        results: _TypeMatchingSet = {}
-        for i in range(ndatasets):
-            for j in range(ndatasets):
-                if j >= i:
-                    continue
-                T = self.get_matching_matrix(i, j)
-                results[i, j] = T
-                results[j, i] = csr_matrix(T.T)
-        return results
+#!/usr/bin/env python3
+
+import numpy as np
+
+from scipy.sparse import csr_matrix
+from typing import List
+
+from ..matching import Matching, _TypeMatchingSet
+from ...traits.isprofilable import profile_method
+from ...traits.usessamplelabels import UsesSampleLabels
+
+
+class Labels(Matching, UsesSampleLabels):
+    """
+    Supervised, label-based boolean matching that matches every pair
+    of samples that share the same label. Does not depend on dataset
+    dimensionality, and will typically generate a lot -- O(n^2) -- of
+    edges.
+
+    Parameters
+    ----------
+    label_obs: str
+        AnnData.obs entry containing categorical labels.
+    """
+
+    def __init__(self, label_obs: str):
+        Matching.__init__(self, str_identifier="LABELS")
+        UsesSampleLabels.__init__(self, label_obs=label_obs)
+
+    @profile_method
+    def fit(
+        self,
+        datasets: List[np.ndarray],
+    ) -> _TypeMatchingSet:
+        """
+        Collects label matching matrices using UsesSampleLabels
+        trait, then computes the matching.
+        """
+        ndatasets = len(datasets)
+        results: _TypeMatchingSet = {}
+        for i in range(ndatasets):
+            for j in range(ndatasets):
+                if j >= i:
+                    continue
+                T = self.get_matching_matrix(i, j)
+                results[i, j] = T
+                results[j, i] = csr_matrix(T.T)
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/mnn.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/mnn.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from scipy.sparse import csr_matrix
-from typing import Dict, List, Literal, Optional
-
-from ..matching import Matching, _TypeMatchingSet
-from ...traits.isprofilable import profile_method
-from ...traits.usescommonfeatures import UsesCommonFeatures
-from ...traits.usesreference import UsesReference
-from ....utils.graph import (
-    generate_qtree,
-    raw_mutual_nearest_neighbors,
-    qtree_mutual_nearest_neighbors,
-)
-
-
-class MNN(Matching, UsesCommonFeatures, UsesReference):
-    """
-    Mutual Nearest Neighbors (MNN) matching. Two samples xi and yj
-    from batches X and Y are matched if xi belongs to the k-nearest neighbors
-    (kNNs) of yj in X and vice-versa. All batches must be able to be
-    embedded in the same space, at least pairwisely.
-
-    We propose two solvers,
-
-    - An exact solver, which computes all pairwise distances between
-      batches, computes exact nearest neighbors and makes the intersection
-    - An approximate solver, that leverages NNDescent algorithm to
-      compute approximate nearest neighbors using projection trees.
-      This allows MNN to scale to large, high dimensional datasets.
-
-    Parameters
-    ----------
-    metric: str or Callable, default = "sqeuclidean"
-        Scipy-compatible metric for kNN computation.
-
-    metric_kwargs: dict, default = {}
-        Additional metric parameters.
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use between datasets before computing the
-        intersection. The more samples, the higher this number must be
-        to have a chance to get nonempty intersections. Using a subsampling
-        algorithm greatly helps keeping this number of neighbors low.
-
-    common_features_mode: Literal["pairwise", "total"], default = "pairwise"
-        Uses pairwise common features, or total common features. Use "total"
-        for a small number of datasets, and "pairwise" if the features
-        intersection is too small. Ignored if datasets are not in feature
-        space, set to "total" if solver = "pynndescent".
-
-    solver: Literal["auto", "exact", "pynndescent"], default = "auto"
-        Solver to use.
-
-    References
-    ----------
-    [1] Haghverdi, Laleh, et al. "Batch effects in single-cell RNA-sequencing
-        data are corrected by matching mutual nearest neighbors." Nature
-        biotechnology 36.5 (2018): 421-427.
-    """
-
-    def __init__(
-        self,
-        metric: str = "sqeuclidean",
-        metric_kwargs: Optional[Dict] = None,
-        n_neighbors: int = 10,
-        common_features_mode: Literal["pairwise", "total"] = "pairwise",
-        solver: Literal["auto", "exact", "nndescent"] = "auto",
-    ):
-        Matching.__init__(self, str_identifier="MNN")
-        UsesCommonFeatures.__init__(self, mode=common_features_mode)
-        UsesReference.__init__(self)
-        self.metric = metric
-        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
-        self.n_neighbors = n_neighbors
-        self.solver = solver
-
-    @profile_method
-    def fit(
-        self,
-        datasets: List[np.ndarray],
-        reference: Optional[int] = None,
-    ) -> _TypeMatchingSet:
-        """
-        Computes MNN between pairs of datasets.
-        """
-        from .... import settings
-
-        # We can only use qtrees if datasets are in the same space.
-        small_data = any(
-            X.shape[0] < settings.small_dataset_threshold for X in datasets
-        )
-        large_data = any(
-            X.shape[0] > settings.large_dataset_threshold for X in datasets
-        )
-        if small_data and large_data:
-            self.warn(
-                "Very disproportionate datasets can be an obstacle to the MNN solver."
-            )
-        if self.solver == "auto":
-            if small_data:
-                self.solver = "exact"
-            else:
-                self.solver = "nndescent"
-        if self.solver == "exact" and large_data:
-            self.warn("Using exact solver with large datasets is discouraged.")
-        if self.solver == "nndescent" and small_data:
-            self.warn("Using nndescent solver with small datasets is discouraged")
-
-        qtrees = []
-        if self.solver == "nndescent":
-            qtrees = [
-                generate_qtree(X, self.metric, self.metric_kwargs) for X in datasets
-            ]
-        ndatasets = len(datasets)
-        results: _TypeMatchingSet = {}
-        reference = self.reference_index
-        if reference is None:
-            target_indices = np.arange(ndatasets)
-        else:
-            target_indices = [reference]
-        for i in range(ndatasets):
-            for j in target_indices:
-                if (i, j) in results:
-                    continue
-                Xi, Xj = self.slice_features(
-                    X1=datasets[i],
-                    X2=datasets[j],
-                    idx_1=i,
-                    idx_2=j,
-                )
-                if self.solver == "nndescent":
-                    Tij = qtree_mutual_nearest_neighbors(
-                        Xi,
-                        Xj,
-                        qtrees[i],
-                        qtrees[j],
-                        n_neighbors=self.n_neighbors,
-                    )
-                else:
-                    Tij = raw_mutual_nearest_neighbors(
-                        Xi,
-                        Xj,
-                        metric=self.metric,
-                        metric_kwargs=self.metric_kwargs,
-                        n_neighbors=self.n_neighbors,
-                    )
-                results[i, j] = csr_matrix(Tij)
-                results[j, i] = csr_matrix(Tij.T)
-        return results
+#!/usr/bin/env python3
+
+import numpy as np
+
+from scipy.sparse import csr_matrix
+from typing import Dict, List, Literal, Optional
+
+from ..matching import Matching, _TypeMatchingSet
+from ...traits.isprofilable import profile_method
+from ...traits.usescommonfeatures import UsesCommonFeatures
+from ...traits.usesreference import UsesReference
+from ....utils.graph import (
+    generate_qtree,
+    raw_mutual_nearest_neighbors,
+    qtree_mutual_nearest_neighbors,
+)
+
+
+class MNN(Matching, UsesCommonFeatures, UsesReference):
+    """
+    Mutual Nearest Neighbors (MNN) matching. Two samples xi and yj
+    from batches X and Y are matched if xi belongs to the k-nearest neighbors
+    (kNNs) of yj in X and vice-versa. All batches must be able to be
+    embedded in the same space, at least pairwisely.
+
+    We propose two solvers,
+
+    - An exact solver, which computes all pairwise distances between
+      batches, computes exact nearest neighbors and makes the intersection
+    - An approximate solver, that leverages NNDescent algorithm to
+      compute approximate nearest neighbors using projection trees.
+      This allows MNN to scale to large, high dimensional datasets.
+
+    Parameters
+    ----------
+    metric: str or Callable, default = "sqeuclidean"
+        Scipy-compatible metric for kNN computation.
+
+    metric_kwargs: dict, default = {}
+        Additional metric parameters.
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use between datasets before computing the
+        intersection. The more samples, the higher this number must be
+        to have a chance to get nonempty intersections. Using a subsampling
+        algorithm greatly helps keeping this number of neighbors low.
+
+    common_features_mode: Literal["pairwise", "total"], default = "pairwise"
+        Uses pairwise common features, or total common features. Use "total"
+        for a small number of datasets, and "pairwise" if the features
+        intersection is too small. Ignored if datasets are not in feature
+        space, set to "total" if solver = "pynndescent".
+
+    solver: Literal["auto", "exact", "pynndescent"], default = "auto"
+        Solver to use.
+
+    References
+    ----------
+    [1] Haghverdi, Laleh, et al. "Batch effects in single-cell RNA-sequencing
+        data are corrected by matching mutual nearest neighbors." Nature
+        biotechnology 36.5 (2018): 421-427.
+    """
+
+    def __init__(
+        self,
+        metric: str = "sqeuclidean",
+        metric_kwargs: Optional[Dict] = None,
+        n_neighbors: int = 10,
+        common_features_mode: Literal["pairwise", "total"] = "pairwise",
+        solver: Literal["auto", "exact", "nndescent"] = "auto",
+    ):
+        Matching.__init__(self, str_identifier="MNN")
+        UsesCommonFeatures.__init__(self, mode=common_features_mode)
+        UsesReference.__init__(self)
+        self.metric = metric
+        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
+        self.n_neighbors = n_neighbors
+        self.solver = solver
+
+    @profile_method
+    def fit(
+        self,
+        datasets: List[np.ndarray],
+        reference: Optional[int] = None,
+    ) -> _TypeMatchingSet:
+        """
+        Computes MNN between pairs of datasets.
+        """
+        from .... import settings
+
+        # We can only use qtrees if datasets are in the same space.
+        small_data = any(
+            X.shape[0] < settings.small_dataset_threshold for X in datasets
+        )
+        large_data = any(
+            X.shape[0] > settings.large_dataset_threshold for X in datasets
+        )
+        if small_data and large_data:
+            self.warn(
+                "Very disproportionate datasets can be an obstacle to the MNN solver."
+            )
+        if self.solver == "auto":
+            if small_data:
+                self.solver = "exact"
+            else:
+                self.solver = "nndescent"
+        if self.solver == "exact" and large_data:
+            self.warn("Using exact solver with large datasets is discouraged.")
+        if self.solver == "nndescent" and small_data:
+            self.warn("Using nndescent solver with small datasets is discouraged")
+
+        qtrees = []
+        if self.solver == "nndescent":
+            qtrees = [
+                generate_qtree(X, self.metric, self.metric_kwargs) for X in datasets
+            ]
+        ndatasets = len(datasets)
+        results: _TypeMatchingSet = {}
+        reference = self.reference_index
+        if reference is None:
+            target_indices = np.arange(ndatasets)
+        else:
+            target_indices = [reference]
+        for i in range(ndatasets):
+            for j in target_indices:
+                if (i, j) in results:
+                    continue
+                Xi, Xj = self.slice_features(
+                    X1=datasets[i],
+                    X2=datasets[j],
+                    idx_1=i,
+                    idx_2=j,
+                )
+                if self.solver == "nndescent":
+                    Tij = qtree_mutual_nearest_neighbors(
+                        Xi,
+                        Xj,
+                        qtrees[i],
+                        qtrees[j],
+                        n_neighbors=self.n_neighbors,
+                    )
+                else:
+                    Tij = raw_mutual_nearest_neighbors(
+                        Xi,
+                        Xj,
+                        metric=self.metric,
+                        metric_kwargs=self.metric_kwargs,
+                        n_neighbors=self.n_neighbors,
+                    )
+                results[i, j] = csr_matrix(Tij)
+                results[j, i] = csr_matrix(Tij.T)
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/algorithms/ot.py` & `transmorph-0.2.7/src/transmorph/engine/matching/algorithms/ot.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from ot import emd
-from ot.partial import partial_wasserstein
-from ot.bregman import sinkhorn_stabilized
-from ot.unbalanced import sinkhorn_stabilized_unbalanced
-from scipy.sparse import csr_matrix
-from scipy.spatial.distance import cdist
-from typing import Dict, List, Literal, Optional, Union
-
-from ..matching import Matching, _TypeMatchingSet
-from ...traits.isprofilable import profile_method
-from ...traits.usescommonfeatures import UsesCommonFeatures
-from ...traits.usesreference import UsesReference
-
-
-class OT(Matching, UsesCommonFeatures, UsesReference):
-    """
-    Optimal transport-based matching. Wraps a selection of optimal
-    transport-derived methods from POT package:
-
-        https://github.com/PythonOT/POT
-
-    Optimal transport is an optimization problem seeking to move
-    mass from a source ptobability distribution to a target probability
-    distribution embedded in the same metric space at minimal cost,
-    where cost is both proportional to mass moved and distance moved.
-    We assume optimal transport can yield relevant matchings, being
-    more likely to move samples of one class towards samples of the
-    same class in the other dataset. There exists many variants of the
-    optimal transport problem, to help scalability or deal with
-    dataset class imbalance.
-
-    We wrapped four solvers:
-
-    - Earth Mover's Distance (EMD) which solves the exact
-      optimal transport problem [1].
-
-    - Sinkhorn-Knopp solver for the entropy-regularized
-      optimal transport problem [2], which can help for larger
-      datasets. We use a log-stabilized implementation for
-      more reliable convergence [3, 4].
-
-    - Partial optimal transport solver, which adds dummy
-      points to each datasets [5]. These dummy points are supposed
-      to attract dataset-specific classes, but need to have their
-      mass parametrized. This mass can be parametrized as a float,
-      or on a per-dataset basis.
-
-    - Unbalanced solver, which introduces mass conservation as
-      a penalty instead of a constraint [6]. This relaxation allows
-      a better handling of class imbalanced datasets, but is
-      typically longer and less likely to converge to a good optimal
-      transport plan in practice.
-
-    Parameters
-    ----------
-    solver: Literal["emd", "sinkhorn", "partial", "unbalanced"], default = "emd"
-        Solver to use.
-
-    metric: str, default = "sqeuclidean"
-        Scipy-compatible metric to compute cost matrix.
-
-    metric_kwargs: Optional[Dict]
-        Additional metric parameters if necessary.
-
-    common_features_mode: Literal["pairwise", "total"]
-        Uses pairwise common features, or total common features. Use "total"
-        for a small number of datasets, and "pairwise" if the features
-        intersection is too small.
-
-    sinkhorn_reg: Optional[float]
-        Entropy regularizer to use for Sinkhorn-Knopp-based solvers. Increasing
-        it will increase rate of convergence, but decrease optimal transport
-        estimation accuracy. If not specified, uses 10^-2.
-
-    partial_transport_mass: Optional[Union[float, List[float]]]
-        Fraction of mass attributed to dummy points, must be between 0 and 1.
-        If a float is provided, will be used for all datasets. If a list of
-        float is provided, each dataset will have its own mass.
-
-    partial_n_dummies: Optional[Union[float, List[float]]]
-        Number of dummies to use in the partial formulation.
-        If an integer is provided, will be used for all datasets. If a list of
-        integers is provided, each dataset will have its own n dummies.
-
-    unbalanced_reg: Optional[float]
-        Mass conservation regularizer to use in the unbalanced optimal
-        transport formulation. The higher, the closer result is from
-        constrained optimal transport. The lower, the better the matching
-        will be dealing with unbalanced datasets, but convergence will be
-        harder. Will be set to 1e-1 by default.
-
-    max_iter: int, default = 1e6
-        Maximum number of iterations to solve the optimization problem.
-
-    References
-    ----------
-    [1] Bonneel, N., Van De Panne, M., Paris, S., & Heidrich, W. (2011, December).
-        Displacement interpolation using Lagrangian mass transport. In ACM Transactions
-        on Graphics (TOG) (Vol. 30, No. 6, p. 158). ACM.
-
-    [2] M. Cuturi, Sinkhorn Distances : Lightspeed Computation of Optimal Transport,
-        Advances in Neural Information Processing Systems (NIPS) 26, 2013
-
-    [3] Schmitzer, B. (2016). Stabilized Sparse Scaling Algorithms for Entropy
-        Regularized Transport Problems. arXiv preprint arXiv:1610.06519.
-
-    [4] Chizat, L., Peyré, G., Schmitzer, B., & Vialard, F. X. (2016). Scaling
-        algorithms for unbalanced transport problems. arXiv preprint arXiv:1607.05816.
-
-    [5] Benamou, J. D., Carlier, G., Cuturi, M., Nenna, L., & Peyré, G. (2015).
-        Iterative Bregman projections for regularized transportation problems.
-        SIAM Journal on Scientific Computing, 37(2), A1111-A1138.
-
-    [6] Frogner C., Zhang C., Mobahi H., Araya-Polo M., Poggio T. : Learning with a
-        Wasserstein Loss, Advances in Neural Information Processing Systems (NIPS) 2015
-    """
-
-    def __init__(
-        self,
-        solver: Literal["emd", "sinkhorn", "partial", "unbalanced"] = "emd",
-        metric: str = "sqeuclidean",
-        metric_kwargs: Optional[Dict] = None,
-        common_features_mode: Literal["pairwise", "total"] = "pairwise",
-        sinkhorn_reg: Optional[float] = None,
-        partial_transport_mass: Optional[Union[float, List[float]]] = None,
-        partial_n_dummies: Optional[Union[int, List[int]]] = None,
-        unbalanced_reg: Optional[float] = None,
-        max_iter: int = int(1e6),
-    ):
-        Matching.__init__(self, str_identifier="OT")
-        UsesCommonFeatures.__init__(self, mode=common_features_mode)
-        UsesReference.__init__(self)
-
-        # Sanity checks
-        assert solver in (
-            "emd",
-            "sinkhorn",
-            "partial",
-            "unbalanced",
-        ), f"Unknown solver: {solver}."
-
-        # General parameters
-        self.solver = solver
-        self.metric = metric
-        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
-        self.max_iter = int(max_iter)
-
-        # Sinkhorn parameters
-        if sinkhorn_reg is None:
-            sinkhorn_reg = 1e-2
-        self.sinkhorn_reg = sinkhorn_reg
-
-        # Partial parameters
-        if partial_transport_mass is None:
-            partial_transport_mass = 0.5
-        if isinstance(partial_transport_mass, float):
-            assert 0.0 <= partial_transport_mass <= 1.0, (
-                "Partial transport mass must be between 0.0 and 1.0, "
-                f"found {partial_transport_mass}."
-            )
-        if isinstance(partial_transport_mass, List):
-            for pm in partial_transport_mass:
-                assert 0.0 <= pm <= 1.0, (
-                    "Partial transport mass must be between 0.0 and 1.0, "
-                    f"found {pm}."
-                )
-        if partial_n_dummies is None:
-            partial_n_dummies = 1
-        self.partial_transport_mass = partial_transport_mass
-        self.partial_n_dummies = partial_n_dummies
-
-        # Unbalanced parameters
-        if unbalanced_reg is None:
-            unbalanced_reg = 1e-1
-        self.unbalanced_reg = unbalanced_reg
-
-    @profile_method
-    def fit(
-        self,
-        datasets: List[np.ndarray],
-        reference: Optional[int] = None,
-    ) -> _TypeMatchingSet:
-        """
-        Computes OT between pairs of datasets with the right solver.
-        """
-        ndatasets = len(datasets)
-        results: _TypeMatchingSet = {}
-        ndatasets = len(datasets)
-        reference = self.reference_index
-        if reference is None:
-            target_indices = np.arange(ndatasets)
-        else:
-            target_indices = [reference]
-        for i in range(ndatasets):
-            for j in target_indices:
-                if (i, j) in results:
-                    continue
-                kwargs = {}
-                if self.solver == "emd":
-                    solver = emd
-                elif self.solver == "sinkhorn":
-                    solver = sinkhorn_stabilized
-                    kwargs = {"reg": self.sinkhorn_reg}
-                elif self.solver == "partial":
-                    solver = partial_wasserstein
-                    if isinstance(self.partial_transport_mass, List):
-                        partial_mass = self.partial_transport_mass[i]
-                    else:
-                        partial_mass = self.partial_transport_mass
-                    if isinstance(self.partial_n_dummies, List):
-                        partial_dummies = self.partial_n_dummies[i]
-                    else:
-                        partial_dummies = self.partial_n_dummies
-                    kwargs = {
-                        "m": partial_mass,
-                        "nb_dummies": partial_dummies,
-                    }
-                elif self.solver == "unbalanced":
-                    solver = sinkhorn_stabilized_unbalanced
-                    kwargs = {"reg": self.sinkhorn_reg, "reg_m": self.unbalanced_reg}
-                else:
-                    raise ValueError(f"Unknown solver: {self.solver}")
-                Xi, Xj = datasets[i], datasets[j]
-                ni, nj = Xi.shape[0], Xj.shape[0]
-                wi, wj = np.ones(ni) / ni, np.ones(nj) / nj
-                Xi, Xj = self.slice_features(X1=Xi, X2=Xj, idx_1=i, idx_2=j)
-                M = cdist(Xi, Xj, metric=self.metric, **self.metric_kwargs)
-                M /= M.max()
-                Tij = solver(a=wi, b=wj, M=M, numItermax=self.max_iter, **kwargs)
-                results[i, j] = csr_matrix(Tij)
-                results[j, i] = csr_matrix(Tij.T)
-        return results
+#!/usr/bin/env python3
+
+import numpy as np
+
+from ot import emd
+from ot.partial import partial_wasserstein
+from ot.bregman import sinkhorn_stabilized
+from ot.unbalanced import sinkhorn_stabilized_unbalanced
+from scipy.sparse import csr_matrix
+from scipy.spatial.distance import cdist
+from typing import Dict, List, Literal, Optional, Union
+
+from ..matching import Matching, _TypeMatchingSet
+from ...traits.isprofilable import profile_method
+from ...traits.usescommonfeatures import UsesCommonFeatures
+from ...traits.usesreference import UsesReference
+
+
+class OT(Matching, UsesCommonFeatures, UsesReference):
+    """
+    Optimal transport-based matching. Wraps a selection of optimal
+    transport-derived methods from POT package:
+
+        https://github.com/PythonOT/POT
+
+    Optimal transport is an optimization problem seeking to move
+    mass from a source ptobability distribution to a target probability
+    distribution embedded in the same metric space at minimal cost,
+    where cost is both proportional to mass moved and distance moved.
+    We assume optimal transport can yield relevant matchings, being
+    more likely to move samples of one class towards samples of the
+    same class in the other dataset. There exists many variants of the
+    optimal transport problem, to help scalability or deal with
+    dataset class imbalance.
+
+    We wrapped four solvers:
+
+    - Earth Mover's Distance (EMD) which solves the exact
+      optimal transport problem [1].
+
+    - Sinkhorn-Knopp solver for the entropy-regularized
+      optimal transport problem [2], which can help for larger
+      datasets. We use a log-stabilized implementation for
+      more reliable convergence [3, 4].
+
+    - Partial optimal transport solver, which adds dummy
+      points to each datasets [5]. These dummy points are supposed
+      to attract dataset-specific classes, but need to have their
+      mass parametrized. This mass can be parametrized as a float,
+      or on a per-dataset basis.
+
+    - Unbalanced solver, which introduces mass conservation as
+      a penalty instead of a constraint [6]. This relaxation allows
+      a better handling of class imbalanced datasets, but is
+      typically longer and less likely to converge to a good optimal
+      transport plan in practice.
+
+    Parameters
+    ----------
+    solver: Literal["emd", "sinkhorn", "partial", "unbalanced"], default = "emd"
+        Solver to use.
+
+    metric: str, default = "sqeuclidean"
+        Scipy-compatible metric to compute cost matrix.
+
+    metric_kwargs: Optional[Dict]
+        Additional metric parameters if necessary.
+
+    common_features_mode: Literal["pairwise", "total"]
+        Uses pairwise common features, or total common features. Use "total"
+        for a small number of datasets, and "pairwise" if the features
+        intersection is too small.
+
+    sinkhorn_reg: Optional[float]
+        Entropy regularizer to use for Sinkhorn-Knopp-based solvers. Increasing
+        it will increase rate of convergence, but decrease optimal transport
+        estimation accuracy. If not specified, uses 10^-2.
+
+    partial_transport_mass: Optional[Union[float, List[float]]]
+        Fraction of mass attributed to dummy points, must be between 0 and 1.
+        If a float is provided, will be used for all datasets. If a list of
+        float is provided, each dataset will have its own mass.
+
+    partial_n_dummies: Optional[Union[float, List[float]]]
+        Number of dummies to use in the partial formulation.
+        If an integer is provided, will be used for all datasets. If a list of
+        integers is provided, each dataset will have its own n dummies.
+
+    unbalanced_reg: Optional[float]
+        Mass conservation regularizer to use in the unbalanced optimal
+        transport formulation. The higher, the closer result is from
+        constrained optimal transport. The lower, the better the matching
+        will be dealing with unbalanced datasets, but convergence will be
+        harder. Will be set to 1e-1 by default.
+
+    max_iter: int, default = 1e6
+        Maximum number of iterations to solve the optimization problem.
+
+    References
+    ----------
+    [1] Bonneel, N., Van De Panne, M., Paris, S., & Heidrich, W. (2011, December).
+        Displacement interpolation using Lagrangian mass transport. In ACM Transactions
+        on Graphics (TOG) (Vol. 30, No. 6, p. 158). ACM.
+
+    [2] M. Cuturi, Sinkhorn Distances : Lightspeed Computation of Optimal Transport,
+        Advances in Neural Information Processing Systems (NIPS) 26, 2013
+
+    [3] Schmitzer, B. (2016). Stabilized Sparse Scaling Algorithms for Entropy
+        Regularized Transport Problems. arXiv preprint arXiv:1610.06519.
+
+    [4] Chizat, L., Peyré, G., Schmitzer, B., & Vialard, F. X. (2016). Scaling
+        algorithms for unbalanced transport problems. arXiv preprint arXiv:1607.05816.
+
+    [5] Benamou, J. D., Carlier, G., Cuturi, M., Nenna, L., & Peyré, G. (2015).
+        Iterative Bregman projections for regularized transportation problems.
+        SIAM Journal on Scientific Computing, 37(2), A1111-A1138.
+
+    [6] Frogner C., Zhang C., Mobahi H., Araya-Polo M., Poggio T. : Learning with a
+        Wasserstein Loss, Advances in Neural Information Processing Systems (NIPS) 2015
+    """
+
+    def __init__(
+        self,
+        solver: Literal["emd", "sinkhorn", "partial", "unbalanced"] = "emd",
+        metric: str = "sqeuclidean",
+        metric_kwargs: Optional[Dict] = None,
+        common_features_mode: Literal["pairwise", "total"] = "pairwise",
+        sinkhorn_reg: Optional[float] = None,
+        partial_transport_mass: Optional[Union[float, List[float]]] = None,
+        partial_n_dummies: Optional[Union[int, List[int]]] = None,
+        unbalanced_reg: Optional[float] = None,
+        max_iter: int = int(1e6),
+    ):
+        Matching.__init__(self, str_identifier="OT")
+        UsesCommonFeatures.__init__(self, mode=common_features_mode)
+        UsesReference.__init__(self)
+
+        # Sanity checks
+        assert solver in (
+            "emd",
+            "sinkhorn",
+            "partial",
+            "unbalanced",
+        ), f"Unknown solver: {solver}."
+
+        # General parameters
+        self.solver = solver
+        self.metric = metric
+        self.metric_kwargs = {} if metric_kwargs is None else metric_kwargs
+        self.max_iter = int(max_iter)
+
+        # Sinkhorn parameters
+        if sinkhorn_reg is None:
+            sinkhorn_reg = 1e-2
+        self.sinkhorn_reg = sinkhorn_reg
+
+        # Partial parameters
+        if partial_transport_mass is None:
+            partial_transport_mass = 0.5
+        if isinstance(partial_transport_mass, float):
+            assert 0.0 <= partial_transport_mass <= 1.0, (
+                "Partial transport mass must be between 0.0 and 1.0, "
+                f"found {partial_transport_mass}."
+            )
+        if isinstance(partial_transport_mass, List):
+            for pm in partial_transport_mass:
+                assert 0.0 <= pm <= 1.0, (
+                    "Partial transport mass must be between 0.0 and 1.0, "
+                    f"found {pm}."
+                )
+        if partial_n_dummies is None:
+            partial_n_dummies = 1
+        self.partial_transport_mass = partial_transport_mass
+        self.partial_n_dummies = partial_n_dummies
+
+        # Unbalanced parameters
+        if unbalanced_reg is None:
+            unbalanced_reg = 1e-1
+        self.unbalanced_reg = unbalanced_reg
+
+    @profile_method
+    def fit(
+        self,
+        datasets: List[np.ndarray],
+        reference: Optional[int] = None,
+    ) -> _TypeMatchingSet:
+        """
+        Computes OT between pairs of datasets with the right solver.
+        """
+        ndatasets = len(datasets)
+        results: _TypeMatchingSet = {}
+        ndatasets = len(datasets)
+        reference = self.reference_index
+        if reference is None:
+            target_indices = np.arange(ndatasets)
+        else:
+            target_indices = [reference]
+        for i in range(ndatasets):
+            for j in target_indices:
+                if (i, j) in results:
+                    continue
+                kwargs = {}
+                if self.solver == "emd":
+                    solver = emd
+                elif self.solver == "sinkhorn":
+                    solver = sinkhorn_stabilized
+                    kwargs = {"reg": self.sinkhorn_reg}
+                elif self.solver == "partial":
+                    solver = partial_wasserstein
+                    if isinstance(self.partial_transport_mass, List):
+                        partial_mass = self.partial_transport_mass[i]
+                    else:
+                        partial_mass = self.partial_transport_mass
+                    if isinstance(self.partial_n_dummies, List):
+                        partial_dummies = self.partial_n_dummies[i]
+                    else:
+                        partial_dummies = self.partial_n_dummies
+                    kwargs = {
+                        "m": partial_mass,
+                        "nb_dummies": partial_dummies,
+                    }
+                elif self.solver == "unbalanced":
+                    solver = sinkhorn_stabilized_unbalanced
+                    kwargs = {"reg": self.sinkhorn_reg, "reg_m": self.unbalanced_reg}
+                else:
+                    raise ValueError(f"Unknown solver: {self.solver}")
+                Xi, Xj = datasets[i], datasets[j]
+                ni, nj = Xi.shape[0], Xj.shape[0]
+                wi, wj = np.ones(ni) / ni, np.ones(nj) / nj
+                Xi, Xj = self.slice_features(X1=Xi, X2=Xj, idx_1=i, idx_2=j)
+                M = cdist(Xi, Xj, metric=self.metric, **self.metric_kwargs)
+                M /= M.max()
+                Tij = solver(a=wi, b=wj, M=M, numItermax=self.max_iter, **kwargs)
+                results[i, j] = csr_matrix(Tij)
+                results[j, i] = csr_matrix(Tij.T)
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/matching/matching.py` & `transmorph-0.2.7/src/transmorph/engine/matching/matching.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-import numpy as np
-
-from abc import ABC, abstractmethod
-from scipy.sparse import csr_matrix
-from typing import Dict, List, Tuple
-
-from ..traits.canlog import CanLog
-from ..traits.isprofilable import IsProfilable
-
-# This is the low-level type of a matching set
-# between datasets, we shortcut it as it is quite
-# often used.
-_TypeMatchingSet = Dict[Tuple[int, int], csr_matrix]
-
-
-class Matching(ABC, IsProfilable, CanLog):
-    """
-    A Matching is an algorithm that is used to assess similarity between
-    samples across datasets. Mergings use this information to build a
-    common embedding between datasets. In our framework a matching between
-    two datasets is represented as a sparse matrix whose value i,j represent
-    matching strength between sample i from the first dataset and sample
-    j from the second dataset.
-
-    Every matching algorithm must inherit from the Matching class, and at
-    least implement a fit() method. This method takes as input a list of
-    matrices representing datasets to match, and returns a dictionary D
-    where D[i, j] contains the sparse matching between datasets i and j.
-    Access to other type of metadata can be granted by inheriting specific
-    traits, and implementing their methods.
-    """
-
-    def __init__(
-        self,
-        str_identifier: str = "DEFAULT",
-    ):
-        CanLog.__init__(self, str_identifier=f"MATCHING_{str_identifier}")
-        IsProfilable.__init__(self)
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Takes a list of np.ndarray representing datasets to match,
-        and verifies their validity. Should raise warnings or
-        errors in case of unexpected input. Will be called before
-        carrying out the matching task. Can be overrode by child
-        classes.
-        """
-        pass
-
-    @abstractmethod
-    def fit(self, datasets: List[np.ndarray]) -> _TypeMatchingSet:
-        """
-        Computes pairwise matchings between a set of numpy ndarrays, and
-        returns these matchings as a dictionary of int tuples -> csr_matrix.
-        Must be implemented in each Matching child class.
-
-        Parameters:
-        -----------
-        datasets: List[np.ndarray]
-            List of numpy ndarray datasets.
-        """
-        pass
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+import numpy as np
+
+from abc import ABC, abstractmethod
+from scipy.sparse import csr_matrix
+from typing import Dict, List, Tuple
+
+from ..traits.canlog import CanLog
+from ..traits.isprofilable import IsProfilable
+
+# This is the low-level type of a matching set
+# between datasets, we shortcut it as it is quite
+# often used.
+_TypeMatchingSet = Dict[Tuple[int, int], csr_matrix]
+
+
+class Matching(ABC, IsProfilable, CanLog):
+    """
+    A Matching is an algorithm that is used to assess similarity between
+    samples across datasets. Mergings use this information to build a
+    common embedding between datasets. In our framework a matching between
+    two datasets is represented as a sparse matrix whose value i,j represent
+    matching strength between sample i from the first dataset and sample
+    j from the second dataset.
+
+    Every matching algorithm must inherit from the Matching class, and at
+    least implement a fit() method. This method takes as input a list of
+    matrices representing datasets to match, and returns a dictionary D
+    where D[i, j] contains the sparse matching between datasets i and j.
+    Access to other type of metadata can be granted by inheriting specific
+    traits, and implementing their methods.
+    """
+
+    def __init__(
+        self,
+        str_identifier: str = "DEFAULT",
+    ):
+        CanLog.__init__(self, str_identifier=f"MATCHING_{str_identifier}")
+        IsProfilable.__init__(self)
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Takes a list of np.ndarray representing datasets to match,
+        and verifies their validity. Should raise warnings or
+        errors in case of unexpected input. Will be called before
+        carrying out the matching task. Can be overrode by child
+        classes.
+        """
+        pass
+
+    @abstractmethod
+    def fit(self, datasets: List[np.ndarray]) -> _TypeMatchingSet:
+        """
+        Computes pairwise matchings between a set of numpy ndarrays, and
+        returns these matchings as a dictionary of int tuples -> csr_matrix.
+        Must be implemented in each Matching child class.
+
+        Parameters:
+        -----------
+        datasets: List[np.ndarray]
+            List of numpy ndarray datasets.
+        """
+        pass
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/barycenter.py` & `transmorph-0.2.7/src/transmorph/engine/merging/algorithms/barycenter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-
-from typing import List
-
-from ..merging import Merging
-from ...traits.usesreference import UsesReference
-
-
-class Barycenter(Merging, UsesReference):
-    """
-    Barycentric merging is the most naive way of merging datasets.
-    Given n vectorized datasets X1, ..., Xk, a reference dataset Y,
-    and n row-normalized matchings T1, ..., Tk from Xis to Y, the
-    barycentric merging f of Xi to Y through Ti is given by
-
-        bary_Y(Xi, Ti) = Ti @ Y
-
-    In other terms, every sample from Xi is projected to the weighted sum
-    of its matches in Y. This merging is limited to complete matchings,
-    where all points from Xi are matched to at least one point in Y, as
-    unmatched points are naturally projected to the origin. In this case,
-    LinearCorrection can circumvent this issue to a certain extent.
-    """
-
-    def __init__(self):
-        Merging.__init__(
-            self,
-            preserves_space=False,
-            str_identifier="BARYCENTER",
-            matching_mode="normalized",
-        )
-        UsesReference.__init__(self)
-
-    def transform(
-        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
-    ) -> List[np.ndarray]:
-        """
-        Combines datasets and matching to return a representation
-        of all datasets in reference space.
-        """
-        k_ref = self.reference_index
-        assert k_ref is not None, "Reference dataset must be set."
-        X_ref = self.get_reference_item(embeddings)
-        result = []
-        for k, X in enumerate(embeddings):
-            if X is X_ref:
-                result.append(X_ref)
-                continue
-            T = self.get_matching(k, k_ref)
-            result.append(T @ X_ref)
-        return result
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+
+from typing import List
+
+from ..merging import Merging
+from ...traits.usesreference import UsesReference
+
+
+class Barycenter(Merging, UsesReference):
+    """
+    Barycentric merging is the most naive way of merging datasets.
+    Given n vectorized datasets X1, ..., Xk, a reference dataset Y,
+    and n row-normalized matchings T1, ..., Tk from Xis to Y, the
+    barycentric merging f of Xi to Y through Ti is given by
+
+        bary_Y(Xi, Ti) = Ti @ Y
+
+    In other terms, every sample from Xi is projected to the weighted sum
+    of its matches in Y. This merging is limited to complete matchings,
+    where all points from Xi are matched to at least one point in Y, as
+    unmatched points are naturally projected to the origin. In this case,
+    LinearCorrection can circumvent this issue to a certain extent.
+    """
+
+    def __init__(self):
+        Merging.__init__(
+            self,
+            preserves_space=False,
+            str_identifier="BARYCENTER",
+            matching_mode="normalized",
+        )
+        UsesReference.__init__(self)
+
+    def transform(
+        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
+    ) -> List[np.ndarray]:
+        """
+        Combines datasets and matching to return a representation
+        of all datasets in reference space.
+        """
+        k_ref = self.reference_index
+        assert k_ref is not None, "Reference dataset must be set."
+        X_ref = self.get_reference_item(embeddings)
+        result = []
+        for k, X in enumerate(embeddings):
+            if X is X_ref:
+                result.append(X_ref)
+                continue
+            T = self.get_matching(k, k_ref)
+            result.append(T @ X_ref)
+        return result
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/merging/algorithms/linearcorrection.py` & `transmorph-0.2.7/src/transmorph/engine/merging/algorithms/linearcorrection.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-
-from scipy.sparse import csr_matrix
-from typing import List
-
-from ..merging import Merging
-from ...traits.usesreference import UsesReference
-from ....utils.graph import (
-    get_nearest_vertex_from_set,
-    nearest_neighbors,
-    smooth_correction_vectors,
-)
-from ....utils.matrix import sort_sparse_matrix
-
-
-class LinearCorrection(Merging, UsesReference):
-    """
-    LinearCorrection is a way to merge vectorized datasets embedded
-    in the same vector space onto a reference, aiming to solve issues
-    of barycentric merging with partial matchings and overfitting.
-    LinearCorrection requires all datasets to be already embedded in
-    a common features space.
-
-    Starting from two datasets X (source) and Y (reference) and a
-    row-normalized matching T where Tij > 0 iff xi and yj are matched,
-    we compute correction vectors c(Xm) between matched points Xm and the
-    barycenter of their matches,
-
-    c(Xm) = bary_Y(Xm, Tm) - Xm
-
-    We end up with a set of correction vectors c(Xm), and need to
-    define c(Xu) for unmatched samples.
-
-    Then, all matched points are associated with the correction vector of
-    their nearest corrected neigbhbor.
-
-    Parameters
-    ----------
-    n_neighbors: int, default = 10
-        Number of neighbors to use to compute the correction extrapolation
-        graph.
-
-    transformation_rate: float, default = 1.0
-        Output merging is interpolated as a linear combination of
-        original embedding and merged embedding, with 0.0 being the
-        original embedding and 1.0 being the merged embedding.
-    """
-
-    def __init__(self, n_neighbors: int = 10, transformation_rate: float = 1.0):
-        Merging.__init__(
-            self,
-            preserves_space=True,
-            str_identifier="LINEAR_CORRECTION",
-            matching_mode="normalized",
-            transformation_rate=transformation_rate,
-        )
-        UsesReference.__init__(self)
-        self.n_neighbors = n_neighbors
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Checks if all datasets are of same dimensionality.
-        """
-        dref = datasets[0].shape[1]
-        assert np.all(
-            [X.shape[1] == dref for X in datasets]
-        ), "All datasets must be embedded in the same space to perform LinearCorrection"
-
-    def project(
-        self,
-        X_src: np.ndarray,
-        X_ref: np.ndarray,
-        nn_src: csr_matrix,
-        T: csr_matrix,
-    ) -> np.ndarray:
-        """
-        Returns the projected view of X onto Y given the matching T
-        """
-        nsamples = X_src.shape[0]
-
-        corrected_idx = np.array(T.sum(axis=1))[:, 0] > 0
-        ncorrected = sum(corrected_idx)
-        self.log(f"Corrected samples: {ncorrected} ({int(100*ncorrected/nsamples)}%).")
-
-        ref_locations = T @ X_ref
-        corr_vectors = np.zeros(X_src.shape, dtype=np.float32)
-        corr_vectors[corrected_idx] = (
-            ref_locations[corrected_idx] - X_src[corrected_idx]
-        )
-
-        indices, distances = sort_sparse_matrix(nn_src, fill_empty=True)
-        references = get_nearest_vertex_from_set(indices, distances, corrected_idx)
-        unreferenced = references == -1
-        nunreferenced = sum(unreferenced)
-        nreferenced = nsamples - nunreferenced - ncorrected
-        self.log(
-            f"Newly corrected samples: {nreferenced} "
-            f"(+{int(100*nreferenced/nsamples)}%)."
-        )
-        self.log(
-            f"Unreferenced samples: {nunreferenced} "
-            f"({int(100*nunreferenced/nsamples)}%)."
-        )
-        if nunreferenced / nsamples > 0.1:
-            self.warn(
-                "More than 10% of samples are not matched, and are disconnected "
-                "from any matched samples. Please make sure the reference dataset "
-                "is comprehensive enough, and number of neighbors is high enough."
-            )
-        references[unreferenced] = np.arange(X_src.shape[0])[unreferenced]
-        corr_vectors = smooth_correction_vectors(
-            X_src,
-            corr_vectors[references],
-            indices,
-            distances,
-        )
-
-        return X_src + corr_vectors * self.transformation_rate
-
-    def transform(
-        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
-    ) -> List[np.ndarray]:
-        """
-        Computes correction vectors, then transforms.
-        """
-        k_ref = self.reference_index
-        assert k_ref is not None, "No reference provided."
-        X_ref = self.get_reference_item(embeddings)
-        assert X_ref is not None, "No reference provided."
-        result = []
-        for k, (adata, X) in enumerate(zip(datasets, embeddings)):
-            if X is X_ref:
-                result.append(X_ref)
-                continue
-            T = self.get_matching(k, k_ref)
-            nn_src = nearest_neighbors(
-                adata,
-                mode="distances",
-                n_neighbors=self.n_neighbors,
-            )
-            projection = self.project(X, X_ref, nn_src, T)
-            result.append(projection)
-        return result
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+
+from scipy.sparse import csr_matrix
+from typing import List
+
+from ..merging import Merging
+from ...traits.usesreference import UsesReference
+from ....utils.graph import (
+    get_nearest_vertex_from_set,
+    nearest_neighbors,
+    smooth_correction_vectors,
+)
+from ....utils.matrix import sort_sparse_matrix
+
+
+class LinearCorrection(Merging, UsesReference):
+    """
+    LinearCorrection is a way to merge vectorized datasets embedded
+    in the same vector space onto a reference, aiming to solve issues
+    of barycentric merging with partial matchings and overfitting.
+    LinearCorrection requires all datasets to be already embedded in
+    a common features space.
+
+    Starting from two datasets X (source) and Y (reference) and a
+    row-normalized matching T where Tij > 0 iff xi and yj are matched,
+    we compute correction vectors c(Xm) between matched points Xm and the
+    barycenter of their matches,
+
+    c(Xm) = bary_Y(Xm, Tm) - Xm
+
+    We end up with a set of correction vectors c(Xm), and need to
+    define c(Xu) for unmatched samples.
+
+    Then, all matched points are associated with the correction vector of
+    their nearest corrected neigbhbor.
+
+    Parameters
+    ----------
+    n_neighbors: int, default = 10
+        Number of neighbors to use to compute the correction extrapolation
+        graph.
+
+    transformation_rate: float, default = 1.0
+        Output merging is interpolated as a linear combination of
+        original embedding and merged embedding, with 0.0 being the
+        original embedding and 1.0 being the merged embedding.
+    """
+
+    def __init__(self, n_neighbors: int = 10, transformation_rate: float = 1.0):
+        Merging.__init__(
+            self,
+            preserves_space=True,
+            str_identifier="LINEAR_CORRECTION",
+            matching_mode="normalized",
+            transformation_rate=transformation_rate,
+        )
+        UsesReference.__init__(self)
+        self.n_neighbors = n_neighbors
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Checks if all datasets are of same dimensionality.
+        """
+        dref = datasets[0].shape[1]
+        assert np.all(
+            [X.shape[1] == dref for X in datasets]
+        ), "All datasets must be embedded in the same space to perform LinearCorrection"
+
+    def project(
+        self,
+        X_src: np.ndarray,
+        X_ref: np.ndarray,
+        nn_src: csr_matrix,
+        T: csr_matrix,
+    ) -> np.ndarray:
+        """
+        Returns the projected view of X onto Y given the matching T
+        """
+        nsamples = X_src.shape[0]
+
+        corrected_idx = np.array(T.sum(axis=1))[:, 0] > 0
+        ncorrected = sum(corrected_idx)
+        self.log(f"Corrected samples: {ncorrected} ({int(100*ncorrected/nsamples)}%).")
+
+        ref_locations = T @ X_ref
+        corr_vectors = np.zeros(X_src.shape, dtype=np.float32)
+        corr_vectors[corrected_idx] = (
+            ref_locations[corrected_idx] - X_src[corrected_idx]
+        )
+
+        indices, distances = sort_sparse_matrix(nn_src, fill_empty=True)
+        references = get_nearest_vertex_from_set(indices, distances, corrected_idx)
+        unreferenced = references == -1
+        nunreferenced = sum(unreferenced)
+        nreferenced = nsamples - nunreferenced - ncorrected
+        self.log(
+            f"Newly corrected samples: {nreferenced} "
+            f"(+{int(100*nreferenced/nsamples)}%)."
+        )
+        self.log(
+            f"Unreferenced samples: {nunreferenced} "
+            f"({int(100*nunreferenced/nsamples)}%)."
+        )
+        if nunreferenced / nsamples > 0.1:
+            self.warn(
+                "More than 10% of samples are not matched, and are disconnected "
+                "from any matched samples. Please make sure the reference dataset "
+                "is comprehensive enough, and number of neighbors is high enough."
+            )
+        references[unreferenced] = np.arange(X_src.shape[0])[unreferenced]
+        corr_vectors = smooth_correction_vectors(
+            X_src,
+            corr_vectors[references],
+            indices,
+            distances,
+        )
+
+        return X_src + corr_vectors * self.transformation_rate
+
+    def transform(
+        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
+    ) -> List[np.ndarray]:
+        """
+        Computes correction vectors, then transforms.
+        """
+        k_ref = self.reference_index
+        assert k_ref is not None, "No reference provided."
+        X_ref = self.get_reference_item(embeddings)
+        assert X_ref is not None, "No reference provided."
+        result = []
+        for k, (adata, X) in enumerate(zip(datasets, embeddings)):
+            if X is X_ref:
+                result.append(X_ref)
+                continue
+            T = self.get_matching(k, k_ref)
+            nn_src = nearest_neighbors(
+                adata,
+                mode="distances",
+                n_neighbors=self.n_neighbors,
+            )
+            projection = self.project(X, X_ref, nn_src, T)
+            result.append(projection)
+        return result
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/merging/merging.py` & `transmorph-0.2.7/src/transmorph/engine/merging/merging.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-#!/usr/bin/env python3
-
-from ..traits.usesmatching import UsesMatching, _TypeMatchingModes
-from ..transforming import Transformation
-
-
-class Merging(Transformation, UsesMatching):
-    """
-    A Merging is an algorithm that is used to embed several datasets
-    in a joint space, combining dataset geometry and inter-dataset
-    matchings. In practice, it takes a set of matrix representations
-    as input and returns a set of matrix representations in output,
-    which justifies its Transformation inheritance. All Merging
-    algorithms must inherit Merging.
-
-    There are two main merging types: (1) mergings which operate in
-    a space where datasets are already embedded, shifting samples in
-    order to bring them together. (2) mergings which learn a new
-    embedding space for datasets.
-
-    For mergings of type (1), it is possible to use a transformation
-    rate coefficient, which determines by how much samples of moved,
-    0.0 meaning no movement at all and 1.0 meaning complete movement.
-    This parameter can be used to design pipelines with iterative
-    matchings and mergings.
-
-    Parameters
-    ----------
-    preserves_space: bool, default = False
-        Determines if the merging preserves both the embedding space
-        and its basis.
-
-    str_identifier: str, default = "DEFAULT"
-        Merging name, for logging purposes
-
-    matching_mode: Literal["raw", "normalized", "bool"]
-        Determines the preprocessing to apply to input matching
-        matrices.
-
-        - raw: Matching matrices are left untouched
-        - normalized: Matching matrices are row-normalized to sum
-          to 1.
-        - bool: Matching matrices are simplified to 1 = match and
-          0 = no match.
-
-    transformation_rate: float, default = 1.0
-        This parameter only applies if the merging preserves space.
-        Output merging is then interpolated as a linear combination of
-        original embedding and merged embedding, with 0.0 being the
-        original embedding and 1.0 being the merged embedding.
-    """
-
-    def __init__(
-        self,
-        preserves_space: bool = False,
-        str_identifier: str = "DEFAULT",
-        matching_mode: _TypeMatchingModes = "raw",
-        transformation_rate: float = 1.0,
-    ):
-        Transformation.__init__(
-            self,
-            preserves_space=preserves_space,
-            str_identifier=f"MERGING_{str_identifier}",
-            transformation_rate=transformation_rate,
-        )
-        # Removes TRANSFORMATION_
-        self.str_identifier = f"MERGING_{str_identifier}"
-        UsesMatching.__init__(self, mode=matching_mode)
+#!/usr/bin/env python3
+
+from ..traits.usesmatching import UsesMatching, _TypeMatchingModes
+from ..transforming import Transformation
+
+
+class Merging(Transformation, UsesMatching):
+    """
+    A Merging is an algorithm that is used to embed several datasets
+    in a joint space, combining dataset geometry and inter-dataset
+    matchings. In practice, it takes a set of matrix representations
+    as input and returns a set of matrix representations in output,
+    which justifies its Transformation inheritance. All Merging
+    algorithms must inherit Merging.
+
+    There are two main merging types: (1) mergings which operate in
+    a space where datasets are already embedded, shifting samples in
+    order to bring them together. (2) mergings which learn a new
+    embedding space for datasets.
+
+    For mergings of type (1), it is possible to use a transformation
+    rate coefficient, which determines by how much samples of moved,
+    0.0 meaning no movement at all and 1.0 meaning complete movement.
+    This parameter can be used to design pipelines with iterative
+    matchings and mergings.
+
+    Parameters
+    ----------
+    preserves_space: bool, default = False
+        Determines if the merging preserves both the embedding space
+        and its basis.
+
+    str_identifier: str, default = "DEFAULT"
+        Merging name, for logging purposes
+
+    matching_mode: Literal["raw", "normalized", "bool"]
+        Determines the preprocessing to apply to input matching
+        matrices.
+
+        - raw: Matching matrices are left untouched
+        - normalized: Matching matrices are row-normalized to sum
+          to 1.
+        - bool: Matching matrices are simplified to 1 = match and
+          0 = no match.
+
+    transformation_rate: float, default = 1.0
+        This parameter only applies if the merging preserves space.
+        Output merging is then interpolated as a linear combination of
+        original embedding and merged embedding, with 0.0 being the
+        original embedding and 1.0 being the merged embedding.
+    """
+
+    def __init__(
+        self,
+        preserves_space: bool = False,
+        str_identifier: str = "DEFAULT",
+        matching_mode: _TypeMatchingModes = "raw",
+        transformation_rate: float = 1.0,
+    ):
+        Transformation.__init__(
+            self,
+            preserves_space=preserves_space,
+            str_identifier=f"MERGING_{str_identifier}",
+            transformation_rate=transformation_rate,
+        )
+        # Removes TRANSFORMATION_
+        self.str_identifier = f"MERGING_{str_identifier}"
+        UsesMatching.__init__(self, mode=matching_mode)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/model.py` & `transmorph-0.2.7/src/transmorph/engine/model.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-#!/usr/bin/env python3
-
-import gc
-
-from anndata import AnnData
-from typing import Dict, List, Optional, TypeVar, Union
-
-from .layers import Layer, LayerChecking, LayerInput, LayerOutput
-from .traits import CanLog, CanCatchChecking, IsProfilable, UsesReference
-from .. import profiler
-from ..utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
-
-T = TypeVar("T")
-
-
-class Model(CanLog):
-    """
-    A Model wraps and manages a network of Layers, allowing to articulate
-    integration modules together. Layers are expected to be already
-    connected to one another, with exactly one input and one output layer.
-
-    Parameters
-    ----------
-    input_layer : LayerInput
-        Input layer of the network, which is assumed to be already
-        connected. The Model will then automatically gather all
-        layers connected to the network, which is expected to have
-        exactly one output layer.
-
-    str_identifier : str, default = "CUSTOM_MODEL"
-        Model custom name for logging purpose.
-
-    Example
-    -------
-    >>> from transmorph.engine.layers import (
-    ...     LayerInput,
-    ...     LayerMatching,
-    ...     LayerMerging,
-    ...     LayerOutput
-    ... )
-    >>> from transmorph.engine import Model
-
-    We can then create custom layers starting from an input
-    layer, and load them with algorithms (see Layers section).
-
-    >>> layer_input = LayerInput()
-    >>> # other layers and algorithms instanciation...
-
-    A model can eventually be instanciated, and can operate
-    integration after being provided a list of AnnData objects.
-
-    >>> print(adata1)
-    AnnData object with n_obs × n_vars = 200 × 10
-        obs: 'class'
-        uns: 'hvg', 'log1p', 'pca'
-
-    >>> m = Model(layer_input)
-    >>> datasets = [adata1, adata2, adata3]
-    >>> m.fit(datasets)
-
-    Integration result for every dataset has been written under
-    'transmorph' entry of the .obsm field, as a numpy ndarray.
-
-    >>> print(adata1.obsm['X_transmorph'])
-    [[-0.06452738, -0.15287925],
-    [-0.06452738,  0.17531697],
-    [-0.06452738,  0.9535402],
-    ...,
-    [-0.06452738, -0.15287925],
-    [-0.06452738, -0.15287925],
-    [-0.06452738,  0.69629896]]
-    """
-
-    def __init__(
-        self,
-        input_layer: LayerInput,
-        str_identifier: str = "CUSTOM_MODEL",
-    ) -> None:
-        CanLog.__init__(self, str_identifier=str_identifier)
-        self.output_layers = []
-        self.layers: List[Layer] = []
-        assert isinstance(
-            input_layer, LayerInput
-        ), f"LayerInput expected, {type(input_layer)} found."
-        self.input_layer = input_layer
-        self._initialize()
-
-    def _initialize(self):
-        """
-        Loads the network and checks basic layout properties.
-        Is called by __init__.
-        """
-        self.log("Fetching pipeline layers...")
-        layers_to_visit: List[Layer] = [self.input_layer]
-        self.layers = [self.input_layer]
-        while len(layers_to_visit) > 0:
-            current_layer = layers_to_visit.pop(0)
-            self.log(f"Branching from layer {current_layer}.")
-
-            # Retrieving output layers
-            output_layers = current_layer.output_layers.copy()
-            # Checking layers have an extra output
-            if (
-                isinstance(current_layer, LayerChecking)
-                and current_layer.rejected_layer is not None
-            ):
-                assert isinstance(current_layer.rejected_layer, Layer)
-                output_layers.append(current_layer.rejected_layer)
-
-            # Registering non-visited output layers
-            for output_layer in output_layers:
-                if output_layer in self.layers:
-                    self.log(f"Ignored connection to {output_layer}.")
-                    continue
-                if isinstance(output_layer, LayerOutput):
-                    self.output_layers.append(output_layer)
-                self.log(f"Found connection to {output_layer}.")
-                layers_to_visit.append(output_layer)
-                self.layers.append(output_layer)
-
-        # Verifying structure is correct
-        if len(self.output_layers) == 0:
-            self.warn(
-                "No output layer reachable from input. This pipeline will not "
-                "write results in AnnData objects."
-            )
-
-        noutputs = len(self.output_layers)
-        assert noutputs <= 1, f"At most one output allowed, found {noutputs}."
-        self.log(
-            f"Pipeline initialized -- {len(self.layers)} layers found, "
-            f"{len(self.output_layers)} outputs found.",
-        )
-
-    def get_layers_by_type(self, layer_type: T) -> List[T]:
-        """
-        Returns all layers whose type if layer_type.
-        """
-        return [layer for layer in self.layers if isinstance(layer, layer_type)]
-
-    def fit(
-        self,
-        datasets: Union[List[AnnData], Dict[str, AnnData]],
-        reference: Optional[AnnData] = None,
-        use_representation: Optional[str] = None,
-        output_representation: Optional[str] = None,
-    ):
-        """
-        Runs the Model given a list of AnnData datasets, and writes integration
-        results in each AnnData object under the entry .obsm['X_transmorph']. A
-        reference dataset, or a specific dataset .obsm representation can be
-        set if needed.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            Datasets to integrate at the AnnData format. Basic preprocessing such
-            as sample filtering is expected at this stage, even if additional
-            transformation steps can be integrated in a Model. If you expect
-            the Model to work with datasets in a common feature space, please
-            ensure var_names are common between datasets -- not necessarily
-            all identical and in the same order, but at least with common names.
-
-        reference: AnnData
-            If some parts of the pipeline (typically mergings) are expected
-            to work with a reference, you must provide the reference AnnData
-            using this parameter (it must also be part of datasets list).
-            TODO: Automatically detect at initialization if reference is needed,
-            to avoid useless computations before raising an error.
-
-        use_representation: str
-            Matrix representation to use during the pipeline, useful to provide
-            a low-dimensional representation of data.
-            If None, use AnnData.X. Otherwise, uses the provided .obsm key.
-
-        output_representation: str
-            .obsm destination key, "transmorph" by default.
-
-        Returns
-        -------
-        fit() will write the datasets at entry .obsm["transmorph"] with
-        integrated embeddings.
-        """
-        if isinstance(datasets, Dict):
-            datasets = list(datasets.values())
-
-        # Sanity checks
-        assert len(datasets) > 0, "No dataset provided."
-        assert self.input_layer is not None, "Pipeline must be initialized first."
-        assert all(isinstance(adata, AnnData) for adata in datasets), (
-            "Only AnnData objects can be processed by a Model. "
-            "You can create one from a numpy ndarray using "
-            "AnnData(X: np.ndarray). Note that in this case, "
-            "observations and variables metadata will be attributed "
-            "automatically, and may cause incompatibilities for some "
-            "pipeline steps."
-        )
-
-        self.info("Transmorph model is initializing.")
-
-        # Flags reference dataset as such if any
-        if reference is not None:
-            assert isinstance(
-                reference, AnnData
-            ), "Reference must be an AnnData object."
-        for i, adata in enumerate(datasets):
-            self.log(f"Flagging dataset {i} as reference: {adata is reference}.")
-            if adata is reference:
-                UsesReference.write_is_reference(adata)
-
-        # Setting base representation if needed
-        if use_representation is not None:
-            self.log(f"Setting base representation to {use_representation}.")
-            for adata in datasets:
-                adm.set_value(
-                    adata=adata,
-                    key=AnnDataKeyIdentifiers.BaseRepresentation,
-                    field="obsm",
-                    value=adata.obsm[use_representation],
-                    persist="pipeline",
-                )
-
-        if output_representation is None:
-            output_representation = AnnDataKeyIdentifiers.TransmorphRepresentation.value
-        for layer in self.output_layers:
-            layer.repr_key = output_representation
-
-        # Logging some info
-        ndatasets = len(datasets)
-        nsamples = sum([adata.n_obs for adata in datasets])
-        self.info(
-            f"Ready to start the integration of {ndatasets} datasets,"
-            f" {nsamples} total samples.",
-        )
-
-        # Running
-        layers_to_run = [self.input_layer]
-        while len(layers_to_run) > 0:
-            called = layers_to_run.pop(0)
-            self.info(f"Running layer {called}.")
-            output_layers = called.fit(datasets)
-
-            # Invalid checking -> layer rejected
-            if isinstance(called, LayerChecking) and called.check_is_valid:
-                assert len(output_layers) == 1
-                output_layer = output_layers[0]
-                assert isinstance(output_layer, CanCatchChecking)
-                output_layer.called_by_checking = True
-            # Rejected layer was computed, can fall back to
-            # previous representation
-            if isinstance(called, CanCatchChecking) and called.called_by_checking:
-                called.called_by_checking = False
-
-            layers_to_run += output_layers
-            adm.clean(datasets, "layer")
-            if isinstance(called, IsProfilable):
-                self.log(f"Layer {called} terminated in {called.get_time_spent()}")
-
-        # Cleaning anndatas, LayerOutput has saved the result
-        adm.clean(datasets, "pipeline")
-
-        # Logging summary
-        if len(self.output_layers) >= 1:
-            loutput = self.output_layers[0]
-            npoints = sum(adata.n_obs for adata in datasets)
-            ndims = loutput.get_representation(datasets[0]).shape[1]
-            self.info(f"Terminated. Total embedding shape: {(npoints, ndims)}")
-            self.info(
-                f"Results have been written in AnnData.obsm['{output_representation}']."
-            )
-        self.log(
-            "### REPORT_START ###\n"
-            + profiler.log_stats()
-            + "\n"
-            + profiler.log_tasks()
-        )
-        self.log("### REPORT_END ###")
-
-        # We let python clean what it can
-        gc.collect()
+#!/usr/bin/env python3
+
+import gc
+
+from anndata import AnnData
+from typing import Dict, List, Optional, TypeVar, Union
+
+from .layers import Layer, LayerChecking, LayerInput, LayerOutput
+from .traits import CanLog, CanCatchChecking, IsProfilable, UsesReference
+from .. import profiler
+from ..utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
+
+T = TypeVar("T")
+
+
+class Model(CanLog):
+    """
+    A Model wraps and manages a network of Layers, allowing to articulate
+    integration modules together. Layers are expected to be already
+    connected to one another, with exactly one input and one output layer.
+
+    Parameters
+    ----------
+    input_layer : LayerInput
+        Input layer of the network, which is assumed to be already
+        connected. The Model will then automatically gather all
+        layers connected to the network, which is expected to have
+        exactly one output layer.
+
+    str_identifier : str, default = "CUSTOM_MODEL"
+        Model custom name for logging purpose.
+
+    Example
+    -------
+    >>> from transmorph.engine.layers import (
+    ...     LayerInput,
+    ...     LayerMatching,
+    ...     LayerMerging,
+    ...     LayerOutput
+    ... )
+    >>> from transmorph.engine import Model
+
+    We can then create custom layers starting from an input
+    layer, and load them with algorithms (see Layers section).
+
+    >>> layer_input = LayerInput()
+    >>> # other layers and algorithms instanciation...
+
+    A model can eventually be instanciated, and can operate
+    integration after being provided a list of AnnData objects.
+
+    >>> print(adata1)
+    AnnData object with n_obs × n_vars = 200 × 10
+        obs: 'class'
+        uns: 'hvg', 'log1p', 'pca'
+
+    >>> m = Model(layer_input)
+    >>> datasets = [adata1, adata2, adata3]
+    >>> m.fit(datasets)
+
+    Integration result for every dataset has been written under
+    'transmorph' entry of the .obsm field, as a numpy ndarray.
+
+    >>> print(adata1.obsm['X_transmorph'])
+    [[-0.06452738, -0.15287925],
+    [-0.06452738,  0.17531697],
+    [-0.06452738,  0.9535402],
+    ...,
+    [-0.06452738, -0.15287925],
+    [-0.06452738, -0.15287925],
+    [-0.06452738,  0.69629896]]
+    """
+
+    def __init__(
+        self,
+        input_layer: LayerInput,
+        str_identifier: str = "CUSTOM_MODEL",
+    ) -> None:
+        CanLog.__init__(self, str_identifier=str_identifier)
+        self.output_layers = []
+        self.layers: List[Layer] = []
+        assert isinstance(
+            input_layer, LayerInput
+        ), f"LayerInput expected, {type(input_layer)} found."
+        self.input_layer = input_layer
+        self._initialize()
+
+    def _initialize(self):
+        """
+        Loads the network and checks basic layout properties.
+        Is called by __init__.
+        """
+        self.log("Fetching pipeline layers...")
+        layers_to_visit: List[Layer] = [self.input_layer]
+        self.layers = [self.input_layer]
+        while len(layers_to_visit) > 0:
+            current_layer = layers_to_visit.pop(0)
+            self.log(f"Branching from layer {current_layer}.")
+
+            # Retrieving output layers
+            output_layers = current_layer.output_layers.copy()
+            # Checking layers have an extra output
+            if (
+                isinstance(current_layer, LayerChecking)
+                and current_layer.rejected_layer is not None
+            ):
+                assert isinstance(current_layer.rejected_layer, Layer)
+                output_layers.append(current_layer.rejected_layer)
+
+            # Registering non-visited output layers
+            for output_layer in output_layers:
+                if output_layer in self.layers:
+                    self.log(f"Ignored connection to {output_layer}.")
+                    continue
+                if isinstance(output_layer, LayerOutput):
+                    self.output_layers.append(output_layer)
+                self.log(f"Found connection to {output_layer}.")
+                layers_to_visit.append(output_layer)
+                self.layers.append(output_layer)
+
+        # Verifying structure is correct
+        if len(self.output_layers) == 0:
+            self.warn(
+                "No output layer reachable from input. This pipeline will not "
+                "write results in AnnData objects."
+            )
+
+        noutputs = len(self.output_layers)
+        assert noutputs <= 1, f"At most one output allowed, found {noutputs}."
+        self.log(
+            f"Pipeline initialized -- {len(self.layers)} layers found, "
+            f"{len(self.output_layers)} outputs found.",
+        )
+
+    def get_layers_by_type(self, layer_type: T) -> List[T]:
+        """
+        Returns all layers whose type if layer_type.
+        """
+        return [layer for layer in self.layers if isinstance(layer, layer_type)]
+
+    def fit(
+        self,
+        datasets: Union[List[AnnData], Dict[str, AnnData]],
+        reference: Optional[AnnData] = None,
+        use_representation: Optional[str] = None,
+        output_representation: Optional[str] = None,
+    ):
+        """
+        Runs the Model given a list of AnnData datasets, and writes integration
+        results in each AnnData object under the entry .obsm['X_transmorph']. A
+        reference dataset, or a specific dataset .obsm representation can be
+        set if needed.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to integrate at the AnnData format. Basic preprocessing such
+            as sample filtering is expected at this stage, even if additional
+            transformation steps can be integrated in a Model. If you expect
+            the Model to work with datasets in a common feature space, please
+            ensure var_names are common between datasets -- not necessarily
+            all identical and in the same order, but at least with common names.
+
+        reference: AnnData
+            If some parts of the pipeline (typically mergings) are expected
+            to work with a reference, you must provide the reference AnnData
+            using this parameter (it must also be part of datasets list).
+            TODO: Automatically detect at initialization if reference is needed,
+            to avoid useless computations before raising an error.
+
+        use_representation: str
+            Matrix representation to use during the pipeline, useful to provide
+            a low-dimensional representation of data.
+            If None, use AnnData.X. Otherwise, uses the provided .obsm key.
+
+        output_representation: str
+            .obsm destination key, "transmorph" by default.
+
+        Returns
+        -------
+        fit() will write the datasets at entry .obsm["transmorph"] with
+        integrated embeddings.
+        """
+        if isinstance(datasets, Dict):
+            datasets = list(datasets.values())
+
+        # Sanity checks
+        assert len(datasets) > 0, "No dataset provided."
+        assert self.input_layer is not None, "Pipeline must be initialized first."
+        assert all(isinstance(adata, AnnData) for adata in datasets), (
+            "Only AnnData objects can be processed by a Model. "
+            "You can create one from a numpy ndarray using "
+            "AnnData(X: np.ndarray). Note that in this case, "
+            "observations and variables metadata will be attributed "
+            "automatically, and may cause incompatibilities for some "
+            "pipeline steps."
+        )
+
+        self.info("Transmorph model is initializing.")
+
+        # Flags reference dataset as such if any
+        if reference is not None:
+            assert isinstance(
+                reference, AnnData
+            ), "Reference must be an AnnData object."
+        for i, adata in enumerate(datasets):
+            self.log(f"Flagging dataset {i} as reference: {adata is reference}.")
+            if adata is reference:
+                UsesReference.write_is_reference(adata)
+
+        # Setting base representation if needed
+        if use_representation is not None:
+            self.log(f"Setting base representation to {use_representation}.")
+            for adata in datasets:
+                adm.set_value(
+                    adata=adata,
+                    key=AnnDataKeyIdentifiers.BaseRepresentation,
+                    field="obsm",
+                    value=adata.obsm[use_representation],
+                    persist="pipeline",
+                )
+
+        if output_representation is None:
+            output_representation = AnnDataKeyIdentifiers.TransmorphRepresentation.value
+        for layer in self.output_layers:
+            layer.repr_key = output_representation
+
+        # Logging some info
+        ndatasets = len(datasets)
+        nsamples = sum([adata.n_obs for adata in datasets])
+        self.info(
+            f"Ready to start the integration of {ndatasets} datasets,"
+            f" {nsamples} total samples.",
+        )
+
+        # Running
+        layers_to_run = [self.input_layer]
+        while len(layers_to_run) > 0:
+            called = layers_to_run.pop(0)
+            self.info(f"Running layer {called}.")
+            output_layers = called.fit(datasets)
+
+            # Invalid checking -> layer rejected
+            if isinstance(called, LayerChecking) and called.check_is_valid:
+                assert len(output_layers) == 1
+                output_layer = output_layers[0]
+                assert isinstance(output_layer, CanCatchChecking)
+                output_layer.called_by_checking = True
+            # Rejected layer was computed, can fall back to
+            # previous representation
+            if isinstance(called, CanCatchChecking) and called.called_by_checking:
+                called.called_by_checking = False
+
+            layers_to_run += output_layers
+            adm.clean(datasets, "layer")
+            if isinstance(called, IsProfilable):
+                self.log(f"Layer {called} terminated in {called.get_time_spent()}")
+
+        # Cleaning anndatas, LayerOutput has saved the result
+        adm.clean(datasets, "pipeline")
+
+        # Logging summary
+        if len(self.output_layers) >= 1:
+            loutput = self.output_layers[0]
+            npoints = sum(adata.n_obs for adata in datasets)
+            ndims = loutput.get_representation(datasets[0]).shape[1]
+            self.info(f"Terminated. Total embedding shape: {(npoints, ndims)}")
+            self.info(
+                f"Results have been written in AnnData.obsm['{output_representation}']."
+            )
+        self.log(
+            "### REPORT_START ###\n"
+            + profiler.log_stats()
+            + "\n"
+            + profiler.log_tasks()
+        )
+        self.log("### REPORT_END ###")
+
+        # We let python clean what it can
+        gc.collect()
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/keepall.py` & `transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/keepall.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-
-from typing import List
-
-from ..subsampling import Subsampling, _TypeSubsampling
-
-
-class KeepAll(Subsampling):
-    """
-    This is the identity subsampling, which does nothing and serves
-    as a placeholder when no subsampling is needed.
-    """
-
-    def __init__(self):
-        Subsampling.__init__(self, str_identifier="KEEPALL")
-
-    def subsample(
-        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
-    ) -> List[_TypeSubsampling]:
-        """
-        Selects all points, and defines each point as its own anchor.
-        """
-        return [np.arange(X.shape[0]) for X in datasets]
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+
+from typing import List
+
+from ..subsampling import Subsampling, _TypeSubsampling
+
+
+class KeepAll(Subsampling):
+    """
+    This is the identity subsampling, which does nothing and serves
+    as a placeholder when no subsampling is needed.
+    """
+
+    def __init__(self):
+        Subsampling.__init__(self, str_identifier="KEEPALL")
+
+    def subsample(
+        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
+    ) -> List[_TypeSubsampling]:
+        """
+        Selects all points, and defines each point as its own anchor.
+        """
+        return [np.arange(X.shape[0]) for X in datasets]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/subsampling/algorithms/vertexcover.py` & `transmorph-0.2.7/src/transmorph/engine/subsampling/algorithms/vertexcover.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-import sccover
-
-from typing import List, Optional
-
-from ..subsampling import Subsampling, _TypeSubsampling
-from ....utils.graph import nearest_neighbors
-
-
-class VertexCover(Subsampling):
-    """
-    Subsamples the dataset by computing a vertex cover, where every point
-    in the dataset either belongs to the subsampling or is neighbor to a
-    subsampled point (in the sense of neighborhood graph). We use a heuristic
-    in O(n) that returns in worst case scenario a vertex cover twice as big
-    as the smallest one.
-
-    Parameters
-    ----------
-    n_hops: int, default = 1
-        Maximal geodesic distance a point is allowed to be to the cover.
-
-    n_neighbors: int, default = 5
-        Number of neighbors to use to build the kNN-graph along which is
-        computed the vertex cover. On average, a dataset with n samples
-        will have a subsampled size of n / n_neighbors.
-    """
-
-    def __init__(self, n_hops: int = 1, n_neighbors: Optional[int] = None):
-        from .... import settings, use_setting
-
-        Subsampling.__init__(self, str_identifier="VERTEX_COVER")
-        self.n_hops = n_hops
-        self.n_neighbors = use_setting(n_neighbors, settings.vertexcover_n_neighbors)
-
-    def subsample(
-        self,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-    ) -> List[_TypeSubsampling]:
-        """
-        Simply retrieves neighbor graphs, and uses it to compute vertex covers.
-        """
-        results = []
-        for adata in datasets:
-            Adj = nearest_neighbors(adata, "edges", n_neighbors=self.n_neighbors)
-            references = sccover.vertex_cover_base(Adj)
-            anchors = np.array(
-                [int(ref == i) for i, ref in enumerate(references)], dtype=bool
-            )
-            results.append((anchors, references))
-        return results
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+import sccover
+
+from typing import List, Optional
+
+from ..subsampling import Subsampling, _TypeSubsampling
+from ....utils.graph import nearest_neighbors
+
+
+class VertexCover(Subsampling):
+    """
+    Subsamples the dataset by computing a vertex cover, where every point
+    in the dataset either belongs to the subsampling or is neighbor to a
+    subsampled point (in the sense of neighborhood graph). We use a heuristic
+    in O(n) that returns in worst case scenario a vertex cover twice as big
+    as the smallest one.
+
+    Parameters
+    ----------
+    n_hops: int, default = 1
+        Maximal geodesic distance a point is allowed to be to the cover.
+
+    n_neighbors: int, default = 5
+        Number of neighbors to use to build the kNN-graph along which is
+        computed the vertex cover. On average, a dataset with n samples
+        will have a subsampled size of n / n_neighbors.
+    """
+
+    def __init__(self, n_hops: int = 1, n_neighbors: Optional[int] = None):
+        from .... import settings, use_setting
+
+        Subsampling.__init__(self, str_identifier="VERTEX_COVER")
+        self.n_hops = n_hops
+        self.n_neighbors = use_setting(n_neighbors, settings.vertexcover_n_neighbors)
+
+    def subsample(
+        self,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+    ) -> List[_TypeSubsampling]:
+        """
+        Simply retrieves neighbor graphs, and uses it to compute vertex covers.
+        """
+        results = []
+        for adata in datasets:
+            Adj = nearest_neighbors(adata, "edges", n_neighbors=self.n_neighbors)
+            references = sccover.vertex_cover_base(Adj)
+            anchors = np.array(
+                [int(ref == i) for i, ref in enumerate(references)], dtype=bool
+            )
+            results.append((anchors, references))
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/subsampling/subsampling.py` & `transmorph-0.2.7/src/transmorph/engine/subsampling/subsampling.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-import anndata as ad
-import numpy as np
-
-from abc import ABC, abstractmethod
-from typing import List
-
-from ..traits import CanLog
-
-_TypeSubsampling = np.ndarray
-
-
-class Subsampling(ABC, CanLog):
-    """
-    A subsampling scheme choses a subset of representers from a large collection
-    of points. These representers are then used during heavy computational parts
-    of the pipeline to speed up computations. SubsamplingABC is the abstraction
-    that allows other parts of Transmorph to manipulate subsampling schemes.
-
-    Parameters
-    ----------
-    str_type: str
-        String representation of the matching algorithm. Will
-        typically be the matching algorithm name.
-    """
-
-    def __init__(self, str_identifier: str = "DEFAULT"):
-        CanLog.__init__(self, str_identifier=f"SUBSAMPLING_{str_identifier}")
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Takes a list of np.ndarray representing datasets to subsample,
-        and verifies their validity. Should raise warnings or
-        errors in case of unexpected input. Will be called before
-        carrying out the matching task. Can be overrode by child
-        classes.
-        """
-        pass
-
-    @abstractmethod
-    def subsample(
-        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
-    ) -> List[_TypeSubsampling]:
-        """
-        Applies a subsampling algorithm to a list of matrices
-        representing datasets. Returns results in the following
-        shape,
-        List[
-            (anchors_1, references_1),
-            ...
-            (anchors_N, references_N),
-        ]
-
-        Parameters
-        ----------
-        datasets: List[np.ndarray]
-            Matrix representation of datasets to subsample.
-        """
-        pass
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+import anndata as ad
+import numpy as np
+
+from abc import ABC, abstractmethod
+from typing import List
+
+from ..traits import CanLog
+
+_TypeSubsampling = np.ndarray
+
+
+class Subsampling(ABC, CanLog):
+    """
+    A subsampling scheme choses a subset of representers from a large collection
+    of points. These representers are then used during heavy computational parts
+    of the pipeline to speed up computations. SubsamplingABC is the abstraction
+    that allows other parts of Transmorph to manipulate subsampling schemes.
+
+    Parameters
+    ----------
+    str_type: str
+        String representation of the matching algorithm. Will
+        typically be the matching algorithm name.
+    """
+
+    def __init__(self, str_identifier: str = "DEFAULT"):
+        CanLog.__init__(self, str_identifier=f"SUBSAMPLING_{str_identifier}")
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Takes a list of np.ndarray representing datasets to subsample,
+        and verifies their validity. Should raise warnings or
+        errors in case of unexpected input. Will be called before
+        carrying out the matching task. Can be overrode by child
+        classes.
+        """
+        pass
+
+    @abstractmethod
+    def subsample(
+        self, datasets: List[ad.AnnData], embeddings: List[np.ndarray]
+    ) -> List[_TypeSubsampling]:
+        """
+        Applies a subsampling algorithm to a list of matrices
+        representing datasets. Returns results in the following
+        shape,
+        List[
+            (anchors_1, references_1),
+            ...
+            (anchors_N, references_N),
+        ]
+
+        Parameters
+        ----------
+        datasets: List[np.ndarray]
+            Matrix representation of datasets to subsample.
+        """
+        pass
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/__init__.py` & `transmorph-0.2.7/src/transmorph/engine/traits/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#!/usr/bin/env python3
-
-# A trait is a small module of features that can be added
-# to a class using inheritance. It allows code factorization,
-# and easier compatibility checking. The base trait does nothing
-# but checking if an object is endowed with it.
-
-from .cancatchchecking import CanCatchChecking
-from .canlog import CanLog
-from .containstransformations import ContainsTransformations
-from .hasmetadata import HasMetadata
-from .isprofilable import IsProfilable, profile_method
-from .isrepresentable import IsRepresentable
-from .issubsamplable import UsesSubsampling
-from .usescommonfeatures import UsesCommonFeatures
-from .usesmatching import UsesMatching, _TypeMatchingModes
-from .usesmetric import UsesMetric
-from .usesreference import UsesReference
-from .usessamplelabels import UsesSampleLabels
-from .utils import assert_trait
-
-__all__ = [
-    "CanCatchChecking",
-    "CanLog",
-    "ContainsTransformations",
-    "HasMetadata",
-    "IsProfilable",
-    "profile_method",
-    "IsRepresentable",
-    "UsesSubsampling",
-    "UsesCommonFeatures",
-    "UsesMatching",
-    "_TypeMatchingModes",
-    "UsesMetric",
-    "UsesReference",
-    "UsesSampleLabels",
-    "assert_trait",
-]
+#!/usr/bin/env python3
+
+# A trait is a small module of features that can be added
+# to a class using inheritance. It allows code factorization,
+# and easier compatibility checking. The base trait does nothing
+# but checking if an object is endowed with it.
+
+from .cancatchchecking import CanCatchChecking
+from .canlog import CanLog
+from .containstransformations import ContainsTransformations
+from .hasmetadata import HasMetadata
+from .isprofilable import IsProfilable, profile_method
+from .isrepresentable import IsRepresentable
+from .issubsamplable import UsesSubsampling
+from .usescommonfeatures import UsesCommonFeatures
+from .usesmatching import UsesMatching, _TypeMatchingModes
+from .usesmetric import UsesMetric
+from .usesreference import UsesReference
+from .usessamplelabels import UsesSampleLabels
+from .utils import assert_trait
+
+__all__ = [
+    "CanCatchChecking",
+    "CanLog",
+    "ContainsTransformations",
+    "HasMetadata",
+    "IsProfilable",
+    "profile_method",
+    "IsRepresentable",
+    "UsesSubsampling",
+    "UsesCommonFeatures",
+    "UsesMatching",
+    "_TypeMatchingModes",
+    "UsesMetric",
+    "UsesReference",
+    "UsesSampleLabels",
+    "assert_trait",
+]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/cancatchchecking.py` & `transmorph-0.2.7/src/transmorph/engine/traits/cancatchchecking.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-from typing import Optional, TYPE_CHECKING
-
-from .isrepresentable import IsRepresentable
-
-if TYPE_CHECKING:
-    from ..layers import LayerChecking
-
-
-class CanCatchChecking:
-    """
-    A layer equipped with CanCatchChcking trait can be set as
-    the rejected layer of a LayerChecking. It provides it a set
-    of attributes and methods that allow their embedding reference
-    to be safely manipulated to be temporarily set to the
-    checking layer responsible for the rejection.
-
-    Attributes
-    ----------
-    base_reference: IsRepresentable
-        Initial embedding reference of the layer.
-
-    check_reference: IsRepresentable
-        Embedding reference of the checking layer, to use in case
-        of rejection as an embedding reference.
-
-    called_by_checking: boolean property
-        Setting this attribute will switch representation
-        accordingly between true embedding reference and checking
-        reference.
-    """
-
-    def __init__(self):
-        self.base_reference: Optional[IsRepresentable] = None
-        self.check_reference: Optional[IsRepresentable] = None
-        self._called_by_checking = False
-
-    @property
-    def called_by_checking(self) -> bool:
-        return self._called_by_checking
-
-    @called_by_checking.setter
-    def called_by_checking(self, state: bool) -> None:
-        """
-        Toggles embedding layer to use.
-        """
-        self._called_by_checking = state
-        if state:
-            self._embedding_reference = self.check_reference
-        else:
-            self._embedding_reference = self.base_reference
-
-    def catch_checking_rejected(self, layer: LayerChecking) -> None:
-        """
-        Registers a LayerChecking to be the one which can provide
-        an alternate embedding representation.
-        """
-        assert isinstance(layer, IsRepresentable)
-        self.base_reference = self._embedding_reference
-        self.check_reference = layer
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+from typing import Optional, TYPE_CHECKING
+
+from .isrepresentable import IsRepresentable
+
+if TYPE_CHECKING:
+    from ..layers import LayerChecking
+
+
+class CanCatchChecking:
+    """
+    A layer equipped with CanCatchChcking trait can be set as
+    the rejected layer of a LayerChecking. It provides it a set
+    of attributes and methods that allow their embedding reference
+    to be safely manipulated to be temporarily set to the
+    checking layer responsible for the rejection.
+
+    Attributes
+    ----------
+    base_reference: IsRepresentable
+        Initial embedding reference of the layer.
+
+    check_reference: IsRepresentable
+        Embedding reference of the checking layer, to use in case
+        of rejection as an embedding reference.
+
+    called_by_checking: boolean property
+        Setting this attribute will switch representation
+        accordingly between true embedding reference and checking
+        reference.
+    """
+
+    def __init__(self):
+        self.base_reference: Optional[IsRepresentable] = None
+        self.check_reference: Optional[IsRepresentable] = None
+        self._called_by_checking = False
+
+    @property
+    def called_by_checking(self) -> bool:
+        return self._called_by_checking
+
+    @called_by_checking.setter
+    def called_by_checking(self, state: bool) -> None:
+        """
+        Toggles embedding layer to use.
+        """
+        self._called_by_checking = state
+        if state:
+            self._embedding_reference = self.check_reference
+        else:
+            self._embedding_reference = self.base_reference
+
+    def catch_checking_rejected(self, layer: LayerChecking) -> None:
+        """
+        Registers a LayerChecking to be the one which can provide
+        an alternate embedding representation.
+        """
+        assert isinstance(layer, IsRepresentable)
+        self.base_reference = self._embedding_reference
+        self.check_reference = layer
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/canlog.py` & `transmorph-0.2.7/src/transmorph/engine/traits/canlog.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-#!/usr/bin/env python3
-
-import logging
-import warnings
-
-from typing import Type
-
-from ..._logging import logger
-
-
-class CanLog:
-    """
-    This trait allows a class to send messages to the logging system,
-    and attributes it a name. It gives access to a set of logging
-    methods that can then be used at any moment by the objects.
-
-    Parameters
-    ----------
-    str_identifier: str
-        String identifier of the object to use duing logging.
-    """
-
-    def __init__(self, str_identifier: str):
-        self.str_identifier = str_identifier
-
-    def log(self, msg: str, level: int = logging.DEBUG) -> None:
-        """
-        Transmits a message to the logging module.
-
-        Parameters
-        ----------
-        msg: str
-            Message to print
-
-        leve: int, default = logging.DEBUG
-            Message priority. Set it higher to make it pass filters.
-        """
-        logger.log(level, f"{self.str_identifier} > {msg}")
-
-    def info(self, msg: str) -> None:
-        """
-        Transmits a message to the logging module with INFO priority.
-
-        Parameters
-        ----------
-        msg: str
-            Message to print
-        """
-        self.log(msg, level=logging.INFO)
-
-    def warn(self, msg: str) -> None:
-        """
-        Emits a warning message that will both reach the logger and the warning
-        console stream.
-
-        Parameters
-        ----------
-        msg: str
-            Message to print
-        """
-        from ..._settings import settings
-
-        if settings.logging_level_console < logging.ERROR:
-            warnings.warn(msg)
-        self.log(msg)
-
-    def raise_error(self, error_type: Type, msg: str = "") -> None:
-        """
-        Raises an error of the specified type, and prints the message both in
-        the console and in the logging stream.
-        """
-        self.log(f"{error_type.__name__} -- {msg}")
-        raise error_type(msg)
-
-    def __str__(self) -> str:
-        return self.str_identifier
+#!/usr/bin/env python3
+
+import logging
+import warnings
+
+from typing import Type
+
+from ..._logging import logger
+
+
+class CanLog:
+    """
+    This trait allows a class to send messages to the logging system,
+    and attributes it a name. It gives access to a set of logging
+    methods that can then be used at any moment by the objects.
+
+    Parameters
+    ----------
+    str_identifier: str
+        String identifier of the object to use duing logging.
+    """
+
+    def __init__(self, str_identifier: str):
+        self.str_identifier = str_identifier
+
+    def log(self, msg: str, level: int = logging.DEBUG) -> None:
+        """
+        Transmits a message to the logging module.
+
+        Parameters
+        ----------
+        msg: str
+            Message to print
+
+        leve: int, default = logging.DEBUG
+            Message priority. Set it higher to make it pass filters.
+        """
+        logger.log(level, f"{self.str_identifier} > {msg}")
+
+    def info(self, msg: str) -> None:
+        """
+        Transmits a message to the logging module with INFO priority.
+
+        Parameters
+        ----------
+        msg: str
+            Message to print
+        """
+        self.log(msg, level=logging.INFO)
+
+    def warn(self, msg: str) -> None:
+        """
+        Emits a warning message that will both reach the logger and the warning
+        console stream.
+
+        Parameters
+        ----------
+        msg: str
+            Message to print
+        """
+        from ..._settings import settings
+
+        if settings.logging_level_console < logging.ERROR:
+            warnings.warn(msg)
+        self.log(msg)
+
+    def raise_error(self, error_type: Type, msg: str = "") -> None:
+        """
+        Raises an error of the specified type, and prints the message both in
+        the console and in the logging stream.
+        """
+        self.log(f"{error_type.__name__} -- {msg}")
+        raise error_type(msg)
+
+    def __str__(self) -> str:
+        return self.str_identifier
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/containstransformations.py` & `transmorph-0.2.7/src/transmorph/engine/traits/containstransformations.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from anndata import AnnData
-from typing import Callable, List, Optional
-
-from .utils import assert_trait
-from .isrepresentable import IsRepresentable
-from ..transforming.transformation import Transformation
-from ..traits.utils import preprocess_traits
-from ...utils.misc import assert_type
-
-
-class ContainsTransformations:
-    """
-    A class inheriting this trait can contain and run
-    Transformation objects.
-
-    Attributes
-    ----------
-    transformations: List[Transformation]
-        A list of transformation objects, expected to be already
-        parametrized, and equiped with a transform() method.
-    """
-
-    def __init__(self) -> None:
-        self.transformations: List[Transformation] = []
-
-    @property
-    def has_transformations(self) -> bool:
-        return len(self.transformations) > 0
-
-    @property
-    def preserves_space(self) -> bool:
-        return all(tr.preserves_space for tr in self.transformations)
-
-    def add_transformation(self, transformation: Transformation) -> None:
-        """
-        Adds a transformation step to the layer, that will be applied
-        before running the internal algorithm. Transformations will be
-        applied in the order of addition.
-
-        Parameters
-        ----------
-        transformation: Transformation
-            Transformation object to append, already parametrized.
-        """
-        assert_type(transformation, Transformation)
-        assert (
-            transformation not in self.transformations
-        ), "Transformation already exists."
-        self.transformations.append(transformation)
-
-    def transform(
-        self,
-        datasets: List[AnnData],
-        representer: IsRepresentable,
-        log_callback: Optional[Callable] = None,
-    ) -> List[np.ndarray]:
-        """
-        Runs all transformations in the order of addition via add_transformation,
-        then returns the final result.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of datasets represented as AnnData objects.
-
-        representer: IsRepresentable
-            Layer providing the embedding reference for these AnnData objects.
-
-        log_callback: Optional[Callable]
-            Logging function to use if necessary. If left None, won't log anything.
-        """
-        is_feature_space = representer.is_feature_space
-        assert is_feature_space is not None
-        if log_callback is not None:
-            log_callback(
-                f"Beginning of transform(). Is feature space: {is_feature_space}"
-            )
-        assert_trait(representer, IsRepresentable)
-        Xs = [representer.get_representation(adata) for adata in datasets]
-        for transformation in self.transformations:
-            # If necessary, we let transformation retrieve
-            # additional information
-            if log_callback is not None:
-                log_callback(f"Running transformation {transformation}")
-            preprocess_traits(transformation, datasets, is_feature_space)
-            transformation.check_input(Xs)
-            if log_callback is not None:
-                init_dimension = f"[{', '.join([str(X.shape) for X in Xs])}]"
-                log_callback(f"Initial spaces dimension: {init_dimension}")
-            Xs = transformation.transform(datasets, Xs)
-            is_feature_space = is_feature_space and transformation.preserves_space
-            if log_callback is not None:
-                final_dimension = f"[{', '.join([str(X.shape) for X in Xs])}]"
-                log_callback(f"Final spaces dimension: {final_dimension}")
-                log_callback(f"Is feature space: {is_feature_space}")
-        return Xs
+#!/usr/bin/env python3
+
+import numpy as np
+
+from anndata import AnnData
+from typing import Callable, List, Optional
+
+from .utils import assert_trait
+from .isrepresentable import IsRepresentable
+from ..transforming.transformation import Transformation
+from ..traits.utils import preprocess_traits
+from ...utils.misc import assert_type
+
+
+class ContainsTransformations:
+    """
+    A class inheriting this trait can contain and run
+    Transformation objects.
+
+    Attributes
+    ----------
+    transformations: List[Transformation]
+        A list of transformation objects, expected to be already
+        parametrized, and equiped with a transform() method.
+    """
+
+    def __init__(self) -> None:
+        self.transformations: List[Transformation] = []
+
+    @property
+    def has_transformations(self) -> bool:
+        return len(self.transformations) > 0
+
+    @property
+    def preserves_space(self) -> bool:
+        return all(tr.preserves_space for tr in self.transformations)
+
+    def add_transformation(self, transformation: Transformation) -> None:
+        """
+        Adds a transformation step to the layer, that will be applied
+        before running the internal algorithm. Transformations will be
+        applied in the order of addition.
+
+        Parameters
+        ----------
+        transformation: Transformation
+            Transformation object to append, already parametrized.
+        """
+        assert_type(transformation, Transformation)
+        assert (
+            transformation not in self.transformations
+        ), "Transformation already exists."
+        self.transformations.append(transformation)
+
+    def transform(
+        self,
+        datasets: List[AnnData],
+        representer: IsRepresentable,
+        log_callback: Optional[Callable] = None,
+    ) -> List[np.ndarray]:
+        """
+        Runs all transformations in the order of addition via add_transformation,
+        then returns the final result.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of datasets represented as AnnData objects.
+
+        representer: IsRepresentable
+            Layer providing the embedding reference for these AnnData objects.
+
+        log_callback: Optional[Callable]
+            Logging function to use if necessary. If left None, won't log anything.
+        """
+        is_feature_space = representer.is_feature_space
+        assert is_feature_space is not None
+        if log_callback is not None:
+            log_callback(
+                f"Beginning of transform(). Is feature space: {is_feature_space}"
+            )
+        assert_trait(representer, IsRepresentable)
+        Xs = [representer.get_representation(adata) for adata in datasets]
+        for transformation in self.transformations:
+            # If necessary, we let transformation retrieve
+            # additional information
+            if log_callback is not None:
+                log_callback(f"Running transformation {transformation}")
+            preprocess_traits(transformation, datasets, is_feature_space)
+            transformation.check_input(Xs)
+            if log_callback is not None:
+                init_dimension = f"[{', '.join([str(X.shape) for X in Xs])}]"
+                log_callback(f"Initial spaces dimension: {init_dimension}")
+            Xs = transformation.transform(datasets, Xs)
+            is_feature_space = is_feature_space and transformation.preserves_space
+            if log_callback is not None:
+                final_dimension = f"[{', '.join([str(X.shape) for X in Xs])}]"
+                log_callback(f"Final spaces dimension: {final_dimension}")
+                log_callback(f"Is feature space: {is_feature_space}")
+        return Xs
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/hasmetadata.py` & `transmorph-0.2.7/src/transmorph/engine/traits/hasmetadata.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Any, Dict, List
-
-_TypeMetadata = Dict[str, Any]
-
-
-class HasMetadata:
-    """
-    This trait allows a module to retrieve and store metadata
-    from an AnnData object, in a safe manner. In transmorphh, metadata
-    has to be understood as "general information about a dataset" and
-    must not be confused with for instance sample labels, which have
-    its own trait. This trait is useful to retrieve information in
-    AnnData objects for classes that are not allowed to handle these
-    objects in their processing method.
-
-    Metadata is handled in a way as safe as possible. When a class
-    inherits from HasMetadata, it must explicitly provide all metadata
-    keys that will be used, and provide a default value for each of
-    those in case it is missing in the AnnData object. Any metadata
-    key that would be set without having been declared will raise
-    a runtime error.
-
-    All classes inheriting from HasMetadata are expected to implement
-    their own retrieve_metadata method, which returns gathered metadata
-    as a dictionary.
-
-    Parameters
-    ----------
-    default_values: Dict[str, Any]
-        Dictionary used to declare metadata keys and set their default
-        values. Declared metadata keys are exactly keys of this
-        dictionary, and their default values are the corresponding
-        values in the dictionary.
-
-    Attributes
-    ----------
-    metadata: List[Dict[str, Any]]
-        For each dataset passed to retrieve_all_metadata, its metadata
-        is stored in this list of dictionaries at the corresponding
-        index.
-    """
-
-    def __init__(self, default_values: _TypeMetadata):
-        self.metadata_default = default_values.copy()
-        self.metadata: List[_TypeMetadata] = []
-
-    def retrieve_all_metadata(self, datasets: List[AnnData]) -> None:
-        """
-        Retrieves necessary information from a list of AnnData objects.
-        Completes with default values provided. This method must NOT
-        be overwrittent by child classes, see retrieve_metadata instead.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            AnnData objects to retrieve metadata from.
-        """
-        for adata in datasets:
-            metadata_qry = self.retrieve_metadatata(adata)
-            metadata_to_save = self.metadata_default.copy()
-            for key in metadata_qry:
-                if key not in metadata_to_save:
-                    raise ValueError(
-                        f"Unexpected key {key}. Allowed keys are "
-                        f"{','.join(self.metadata_default.keys())}."
-                    )
-                metadata_to_save[key] = metadata_qry[key]
-            self.metadata.append(metadata_to_save)
-
-    def retrieve_metadatata(self, adata: AnnData) -> _TypeMetadata:
-        """
-        Given an AnnData objects, extracts relevant metadata and
-        store them in a dictionary with the appropriate acces keys.
-        These metadata can then be accessed in any other method
-        using get_metadata(index, key). This method must be overwritten
-        by child classes.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to retrieve anndata from.
-        """
-        raise NotImplementedError
-
-    def get_metadata(self, index: int, key: str) -> Any:
-        """
-        Returns stored metadata at a given index and key using
-        cached information.
-
-        Parameters
-        ----------
-        index: int
-            Dataset index, must coincidate with the one passed in
-            retrieve_all_metadata.
-
-        key: str
-            Metadata key to retrieve, must have been declared in
-            the initialization.
-        """
-        assert key in self.metadata_default
-        print(self.metadata)
-        return self.metadata[index][key]
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Any, Dict, List
+
+_TypeMetadata = Dict[str, Any]
+
+
+class HasMetadata:
+    """
+    This trait allows a module to retrieve and store metadata
+    from an AnnData object, in a safe manner. In transmorphh, metadata
+    has to be understood as "general information about a dataset" and
+    must not be confused with for instance sample labels, which have
+    its own trait. This trait is useful to retrieve information in
+    AnnData objects for classes that are not allowed to handle these
+    objects in their processing method.
+
+    Metadata is handled in a way as safe as possible. When a class
+    inherits from HasMetadata, it must explicitly provide all metadata
+    keys that will be used, and provide a default value for each of
+    those in case it is missing in the AnnData object. Any metadata
+    key that would be set without having been declared will raise
+    a runtime error.
+
+    All classes inheriting from HasMetadata are expected to implement
+    their own retrieve_metadata method, which returns gathered metadata
+    as a dictionary.
+
+    Parameters
+    ----------
+    default_values: Dict[str, Any]
+        Dictionary used to declare metadata keys and set their default
+        values. Declared metadata keys are exactly keys of this
+        dictionary, and their default values are the corresponding
+        values in the dictionary.
+
+    Attributes
+    ----------
+    metadata: List[Dict[str, Any]]
+        For each dataset passed to retrieve_all_metadata, its metadata
+        is stored in this list of dictionaries at the corresponding
+        index.
+    """
+
+    def __init__(self, default_values: _TypeMetadata):
+        self.metadata_default = default_values.copy()
+        self.metadata: List[_TypeMetadata] = []
+
+    def retrieve_all_metadata(self, datasets: List[AnnData]) -> None:
+        """
+        Retrieves necessary information from a list of AnnData objects.
+        Completes with default values provided. This method must NOT
+        be overwrittent by child classes, see retrieve_metadata instead.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            AnnData objects to retrieve metadata from.
+        """
+        for adata in datasets:
+            metadata_qry = self.retrieve_metadatata(adata)
+            metadata_to_save = self.metadata_default.copy()
+            for key in metadata_qry:
+                if key not in metadata_to_save:
+                    raise ValueError(
+                        f"Unexpected key {key}. Allowed keys are "
+                        f"{','.join(self.metadata_default.keys())}."
+                    )
+                metadata_to_save[key] = metadata_qry[key]
+            self.metadata.append(metadata_to_save)
+
+    def retrieve_metadatata(self, adata: AnnData) -> _TypeMetadata:
+        """
+        Given an AnnData objects, extracts relevant metadata and
+        store them in a dictionary with the appropriate acces keys.
+        These metadata can then be accessed in any other method
+        using get_metadata(index, key). This method must be overwritten
+        by child classes.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to retrieve anndata from.
+        """
+        raise NotImplementedError
+
+    def get_metadata(self, index: int, key: str) -> Any:
+        """
+        Returns stored metadata at a given index and key using
+        cached information.
+
+        Parameters
+        ----------
+        index: int
+            Dataset index, must coincidate with the one passed in
+            retrieve_all_metadata.
+
+        key: str
+            Metadata key to retrieve, must have been declared in
+            the initialization.
+        """
+        assert key in self.metadata_default
+        print(self.metadata)
+        return self.metadata[index][key]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/isprofilable.py` & `transmorph-0.2.7/src/transmorph/engine/traits/isprofilable.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-from typing import Dict
-
-from .utils import assert_trait
-from ..._profiling import profiler
-
-
-def profile_method(method):
-    # Profiling decorator for class methods that
-    # allows to measure time elapsed in a profilable
-    # object.
-    def wrapper(*args):
-        self = args[0]
-        assert self is not None
-        assert_trait(self, IsProfilable)
-        tstr = f"{str(self)}.{method.__name__}"
-        tid = profiler.task_start(tstr)
-        result = method(*args)
-        elapsed = profiler.task_end(tid)
-        self.time_elapsed[tstr] = elapsed
-        return result
-
-    return wrapper
-
-
-class IsProfilable:
-    """
-    A profilable object can be monitored by the Profiler. Methods
-    to profile must be decorated by @profile_method.
-    TODO: add a self.set_stop() allowing to monitor particular
-    function parts
-
-    Attributes
-    ----------
-    time_elapsed: Dict[str, float]
-        Dictionary containing for each profiled method the latest time recorded.
-    """
-
-    def __init__(self):
-        self.time_elapsed: Dict[str, float] = {}
-
-    def get_time_spent(self) -> float:
-        """
-        Returns the total time of all tasks profiled.
-        """
-        return sum(self.time_elapsed.values())
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+from typing import Dict
+
+from .utils import assert_trait
+from ..._profiling import profiler
+
+
+def profile_method(method):
+    # Profiling decorator for class methods that
+    # allows to measure time elapsed in a profilable
+    # object.
+    def wrapper(*args):
+        self = args[0]
+        assert self is not None
+        assert_trait(self, IsProfilable)
+        tstr = f"{str(self)}.{method.__name__}"
+        tid = profiler.task_start(tstr)
+        result = method(*args)
+        elapsed = profiler.task_end(tid)
+        self.time_elapsed[tstr] = elapsed
+        return result
+
+    return wrapper
+
+
+class IsProfilable:
+    """
+    A profilable object can be monitored by the Profiler. Methods
+    to profile must be decorated by @profile_method.
+    TODO: add a self.set_stop() allowing to monitor particular
+    function parts
+
+    Attributes
+    ----------
+    time_elapsed: Dict[str, float]
+        Dictionary containing for each profiled method the latest time recorded.
+    """
+
+    def __init__(self):
+        self.time_elapsed: Dict[str, float] = {}
+
+    def get_time_spent(self) -> float:
+        """
+        Returns the total time of all tasks profiled.
+        """
+        return sum(self.time_elapsed.values())
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/isrepresentable.py` & `transmorph-0.2.7/src/transmorph/engine/traits/isrepresentable.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-import numpy as np
-
-from anndata import AnnData
-from scipy.sparse import csr_matrix
-from typing import List, Union
-
-from ...utils.anndata_manager import (
-    anndata_manager as adm,
-    AnnDataKeyIdentifiers,
-    _TypePersistLevels,
-)
-
-
-class IsRepresentable:
-    """
-    A representable object is able to provide a matrix
-    representation of an AnnData object, and knows if this
-    representation is in the same space and basis as the
-    original features space.
-
-    Prameters
-    ---------
-    repr_key: Union[str, AnnDataKeyIdentifiers]
-        String representation that will be used to save
-        the matrix representation in AnnData objects.
-        IsRepresentable will ensure this representation is unique,
-        by appending a suffix if necessary.
-
-    Attributes
-    ----------
-    is_feature_space: bool
-        Whether the matrix representation is in the same features
-        space than initial datasets, with the same basis.
-    """
-
-    def __init__(self, repr_key: Union[str, AnnDataKeyIdentifiers]):
-        # Finds a suffix so that representation is unique
-        self.repr_key = repr_key
-        self.is_feature_space: bool = True
-
-    def write_representation(
-        self,
-        adata: AnnData,
-        X: Union[np.ndarray, csr_matrix],
-        is_feature_space: bool,
-        persist: _TypePersistLevels = "pipeline",
-    ) -> None:
-        """
-        Inserts a new representation of a dataset in the .obsm
-        field of an AnnData object.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to write in
-
-        X: Union[np.ndarray, csr_matrix]
-            Representation matrix to write in adata
-
-        is_feature_space: bool
-            Matrix representation is expressed in the initial features
-            space, with the initial basis.
-
-        persist: Literal["output", "pipeline", "layer"]
-            Life duration of the matrix. If "output", won't be erased. If
-            "pipeline", will be erased at the end of a Model. If "layer",
-            will be erased at the end of the next layer fit().
-        """
-        self.is_feature_space = is_feature_space
-        adm.set_value(
-            adata=adata,
-            key=self.repr_key,
-            field="obsm",
-            value=X,
-            persist=persist,
-        )
-
-    def get_representation(self, adata: AnnData) -> np.ndarray:
-        """
-        Retrieves matrix representation of an AnnData object that
-        has already been written.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to retrieve representation from.
-        """
-        X = adm.get_value(adata=adata, key=self.repr_key)
-        assert X is not None, "Representation has not been computed."
-        if isinstance(X, csr_matrix):
-            X = X.toarray()
-        return X
-
-    @staticmethod
-    def assert_representation_equals(
-        representers: List[IsRepresentable],
-        datasets: List[AnnData],
-    ) -> None:
-        """
-        For testing purposes. Tests if a list of IsRepresentable objects
-        have similar representations of a set of AnnData datasets.
-        """
-        if len(representers) == 0:
-            return
-        for adata in datasets:
-            X_ref = representers[0].get_representation(adata)
-            for rpr in representers[1:]:
-                np.testing.assert_array_almost_equal(
-                    X_ref, rpr.get_representation(adata)
-                )
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+import numpy as np
+
+from anndata import AnnData
+from scipy.sparse import csr_matrix
+from typing import List, Union
+
+from ...utils.anndata_manager import (
+    anndata_manager as adm,
+    AnnDataKeyIdentifiers,
+    _TypePersistLevels,
+)
+
+
+class IsRepresentable:
+    """
+    A representable object is able to provide a matrix
+    representation of an AnnData object, and knows if this
+    representation is in the same space and basis as the
+    original features space.
+
+    Prameters
+    ---------
+    repr_key: Union[str, AnnDataKeyIdentifiers]
+        String representation that will be used to save
+        the matrix representation in AnnData objects.
+        IsRepresentable will ensure this representation is unique,
+        by appending a suffix if necessary.
+
+    Attributes
+    ----------
+    is_feature_space: bool
+        Whether the matrix representation is in the same features
+        space than initial datasets, with the same basis.
+    """
+
+    def __init__(self, repr_key: Union[str, AnnDataKeyIdentifiers]):
+        # Finds a suffix so that representation is unique
+        self.repr_key = repr_key
+        self.is_feature_space: bool = True
+
+    def write_representation(
+        self,
+        adata: AnnData,
+        X: Union[np.ndarray, csr_matrix],
+        is_feature_space: bool,
+        persist: _TypePersistLevels = "pipeline",
+    ) -> None:
+        """
+        Inserts a new representation of a dataset in the .obsm
+        field of an AnnData object.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to write in
+
+        X: Union[np.ndarray, csr_matrix]
+            Representation matrix to write in adata
+
+        is_feature_space: bool
+            Matrix representation is expressed in the initial features
+            space, with the initial basis.
+
+        persist: Literal["output", "pipeline", "layer"]
+            Life duration of the matrix. If "output", won't be erased. If
+            "pipeline", will be erased at the end of a Model. If "layer",
+            will be erased at the end of the next layer fit().
+        """
+        self.is_feature_space = is_feature_space
+        adm.set_value(
+            adata=adata,
+            key=self.repr_key,
+            field="obsm",
+            value=X,
+            persist=persist,
+        )
+
+    def get_representation(self, adata: AnnData) -> np.ndarray:
+        """
+        Retrieves matrix representation of an AnnData object that
+        has already been written.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to retrieve representation from.
+        """
+        X = adm.get_value(adata=adata, key=self.repr_key)
+        assert X is not None, "Representation has not been computed."
+        if isinstance(X, csr_matrix):
+            X = X.toarray()
+        return X
+
+    @staticmethod
+    def assert_representation_equals(
+        representers: List[IsRepresentable],
+        datasets: List[AnnData],
+    ) -> None:
+        """
+        For testing purposes. Tests if a list of IsRepresentable objects
+        have similar representations of a set of AnnData datasets.
+        """
+        if len(representers) == 0:
+            return
+        for adata in datasets:
+            X_ref = representers[0].get_representation(adata)
+            for rpr in representers[1:]:
+                np.testing.assert_array_almost_equal(
+                    X_ref, rpr.get_representation(adata)
+                )
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/issubsamplable.py` & `transmorph-0.2.7/src/transmorph/engine/traits/issubsamplable.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-#!/usr/bin/env python3
-
-import numba
-import numpy as np
-import sccover
-
-from anndata import AnnData
-from scipy.sparse import csr_matrix
-from typing import Callable, List, Optional, Union
-
-from ..subsampling import Subsampling, KeepAll
-from ..traits.utils import preprocess_traits
-from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
-
-
-@numba.njit
-def _get_cell_anchor_matrix_njit(nx, na, anchors, connectivities):
-    T = np.zeros((nx, na))
-    for i in range(nx):
-        for anchor_ind in range(na):
-            T[i, anchor_ind] = connectivities[i, anchors[anchor_ind]]
-    return T
-
-
-def get_cell_anchor_matrix(adata):
-    subsampling_set_key = adm.gen_keystring(AnnDataKeyIdentifiers.SubsamplingAnchors)
-    sccover.get_closest_anchor(adata, key_set=subsampling_set_key)
-    nx = adata.n_obs
-    anchors = np.arange(nx)[adata.obs[subsampling_set_key].astype(bool)]
-    na = anchors.shape[0]
-    T = _get_cell_anchor_matrix_njit(
-        nx, na, anchors, adata.obsp["connectivities"].toarray()
-    )
-    T_norm = T.sum(axis=1)
-    T_norm[T_norm == 0.0] = 1.0
-    return T / T_norm[:, None]
-
-
-class UsesSubsampling:
-    """
-    This trait allows a class to host a subsampling algorithm, and manipulate
-    subsampled matrices. This is a key trait for performance-hungry components.
-    """
-
-    def __init__(
-        self,
-        subsampling: Optional[Subsampling] = None,
-    ) -> None:
-        if subsampling is None:
-            subsampling = KeepAll()
-        self.is_subsampled = not isinstance(subsampling, KeepAll)
-        self.subsampling = subsampling
-        self.references: List[np.ndarray] = []
-
-    @property
-    def has_subsampling(self) -> bool:
-        return not isinstance(self.subsampling, KeepAll)
-
-    def compute_subsampling(
-        self,
-        datasets: List[AnnData],
-        matrices: List[np.ndarray],
-        is_feature_space: bool,
-        log_callback: Optional[Callable] = None,
-    ) -> None:
-        """
-        Runs the subsampling on a list of datasets, and
-        stores the result in AnnData objects. If subsampling results
-        are already found, skips the dataset.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            AnnData objects containing datasets to subsample.
-
-        matrices: List[np.ndarray]
-            Matrix representation of datasets to subsample.
-        """
-        if self.has_subsampling is False:
-            return
-        if log_callback is not None:
-            log_callback(f"Applying subsampling {self.subsampling}.")
-        preprocess_traits(self.subsampling, datasets, is_feature_space)
-        ndatasets = len(datasets)
-        assert len(matrices) == ndatasets, "Inconsistent number of matrices/annadatas."
-        to_compute = []
-        self.anchors = [None] * ndatasets
-        self.references = [None] * ndatasets
-        for i, adata in enumerate(datasets):
-            anchors = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingAnchors)
-            references = adm.get_value(
-                adata, AnnDataKeyIdentifiers.SubsamplingReferences
-            )
-            if anchors is None or references is None:
-                # Needs to be computed
-                to_compute.append((i, matrices[i]))
-            else:
-                self.anchors[i] = anchors
-                self.references[i] = references
-
-        # Computes missing subsamplings
-        subsampling_results = self.subsampling.subsample(
-            datasets, [mtx for _, mtx in to_compute]
-        )
-        # We store results in AnnData objects
-        for (i, _), (anchors, references) in zip(to_compute, subsampling_results):
-            adm.set_value(
-                adata=datasets[i],
-                key=AnnDataKeyIdentifiers.SubsamplingAnchors,
-                field="obs",
-                value=anchors,
-                persist="output",
-            )
-            adm.set_value(
-                adata=datasets[i],
-                key=AnnDataKeyIdentifiers.SubsamplingReferences,
-                field="obs",
-                value=references,
-                persist="output",
-            )
-            self.anchors[i] = anchors
-            self.references[i] = references
-
-        if log_callback is not None:
-            for i, anchors in enumerate(self.anchors):
-                log_callback(
-                    f"Dataset {i} subsampled from {anchors.shape[0]} to "
-                    f"{anchors.sum()} samples."
-                )
-
-    @staticmethod
-    def get_anchors(adata: AnnData) -> np.ndarray:
-        """
-        Returns the chosen subsample as a boolean numpy array.
-        """
-        anchors = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingAnchors)
-        if anchors is None:
-            raise KeyError(f"No anchors found for the AnnData {adata}.")
-        return anchors
-
-    @staticmethod
-    def get_references(adata: AnnData) -> np.ndarray:
-        """
-        Returns the chosen subsample as a boolean numpy array.
-        """
-        references = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingReferences)
-        if references is None:
-            raise KeyError(f"No references found for the AnnData {adata}.")
-        return references
-
-    def subsample_matrix(
-        self,
-        matrix: Union[np.ndarray, csr_matrix],
-        idx: int,
-        idx_2: Optional[int] = None,
-        pairwise: bool = False,
-    ) -> Union[np.ndarray, csr_matrix]:
-        """
-        Returns row-sliced matrix with respect to computed subsample.
-
-        Parameters
-        ----------
-        matrix: np.ndarray
-            Array to slice.
-
-        index: int
-            Matrix index used in compute_subsampling
-
-        pairwise: bool, default = False
-            Also column-slice the matrix, matrix must be squared.
-        """
-        if self.has_subsampling is False:
-            return matrix
-        assert idx < len(
-            self.anchors
-        ), "Ensure compute_subsampling has been called first."
-        assert not (idx_2 is not None and pairwise), "Incompatible pairwise non-square."
-        anchors = self.anchors[idx]
-        X = matrix[anchors]
-        if pairwise:
-            X = X[:, anchors]
-        if idx_2 is not None:
-            X = X[:, self.anchors[idx_2]]
-        return X
-
-    def subsample_matrices(
-        self,
-        matrices: List[Union[np.ndarray, csr_matrix]],
-        pairwise: bool = False,
-    ) -> List[Union[np.ndarray, csr_matrix]]:
-        """
-        Returns row-sliced views of input matrices according to
-        the subsampling computed.
-
-        Parameters
-        ----------
-        matrices: List[np.ndarray]
-            Arrays to slice in a list.
-
-        pairwise: bool, default = False
-            Also column-slice the matrix, matrix must be squared.
-        """
-        result = []
-        for i, X in enumerate(matrices):
-            result.append(self.subsample_matrix(X, i, pairwise=pairwise))
-        return result
-
-    def unsubsample_matrix_exact(
-        self,
-        matrix: Union[csr_matrix, np.ndarray],
-        idx: int,
-        idx_2: Optional[int] = None,
-    ) -> Union[csr_matrix, np.ndarray]:
-        """
-        Restores initial structure of a subsampled matrix, possibly
-        pairwise. Useful to reverse subsampling of a distance matrix for
-        instance.
-
-        Parameters
-        ----------
-        matrix: Union[csr_matrix, np.ndarray]
-            Subsampled matrix to turn back to full size.
-
-        idx: int
-            Index of the subsampling to use.
-
-        idx_2: Optional[int]
-            In case of pairwise matrix between different datasets, subsampling
-            index of the second dataset.
-        """
-        # Sanity check
-        if self.has_subsampling is False:
-            return matrix
-        assert isinstance(
-            matrix, (csr_matrix, np.ndarray)
-        ), f"Unknown type: {type(matrix)}"
-
-        # Inverting subsampling indices
-        n_samples = self.anchors[idx].shape[0]
-        n_features = n_samples
-        s_to_S1 = np.arange(n_samples)[self.anchors[idx].astype(bool)]
-        s_to_S2 = s_to_S1
-        if idx_2 is not None:
-            anchors_2 = self.anchors[idx_2]
-            n_features = anchors_2.shape[0]
-            s_to_S2 = np.arange(n_features)[anchors_2.astype(bool)]
-
-        # Reversing subsampling
-        if isinstance(matrix, csr_matrix):
-            X_coo = matrix.tocoo()
-            srow, scol, sdata = X_coo.row, X_coo.col, X_coo.data
-            Srow = s_to_S1[srow]
-            if idx_2 is None:
-                Scol = scol
-            else:
-                Scol = s_to_S2[scol]
-            return csr_matrix(
-                (sdata, (Srow, Scol)),
-                shape=(n_samples, n_features),
-            )
-        else:  # np.ndarray
-            X = np.zeros((n_samples, n_features), dtype=matrix.dtype)
-            for idx_i, coord_i in enumerate(s_to_S1):
-                for idx_j, coord_j in enumerate(s_to_S2):
-                    X[coord_i, coord_j] = matrix[idx_i, idx_j]
-            return X
-
-    def unsubsample_matrix_transitive(
-        self,
-        matrix: csr_matrix,
-        adata_src: AnnData,
-        adata_ref: AnnData,
-    ) -> csr_matrix:
-        """
-        TODO
-        """
-        Tx = get_cell_anchor_matrix(adata_src)
-        Ty = get_cell_anchor_matrix(adata_ref)
-        T_tot = Tx @ matrix @ Ty.T
-        T_tot_norm = T_tot.sum(axis=1)
-        T_tot_norm[T_tot_norm == 0.0] = 1.0
-        return csr_matrix(T_tot / T_tot_norm[:, None])
+#!/usr/bin/env python3
+
+import numba
+import numpy as np
+import sccover
+
+from anndata import AnnData
+from scipy.sparse import csr_matrix
+from typing import Callable, List, Optional, Union
+
+from ..subsampling import Subsampling, KeepAll
+from ..traits.utils import preprocess_traits
+from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
+
+
+@numba.njit
+def _get_cell_anchor_matrix_njit(nx, na, anchors, connectivities):
+    T = np.zeros((nx, na))
+    for i in range(nx):
+        for anchor_ind in range(na):
+            T[i, anchor_ind] = connectivities[i, anchors[anchor_ind]]
+    return T
+
+
+def get_cell_anchor_matrix(adata):
+    subsampling_set_key = adm.gen_keystring(AnnDataKeyIdentifiers.SubsamplingAnchors)
+    sccover.get_closest_anchor(adata, key_set=subsampling_set_key)
+    nx = adata.n_obs
+    anchors = np.arange(nx)[adata.obs[subsampling_set_key].astype(bool)]
+    na = anchors.shape[0]
+    T = _get_cell_anchor_matrix_njit(
+        nx, na, anchors, adata.obsp["connectivities"].toarray()
+    )
+    T_norm = T.sum(axis=1)
+    T_norm[T_norm == 0.0] = 1.0
+    return T / T_norm[:, None]
+
+
+class UsesSubsampling:
+    """
+    This trait allows a class to host a subsampling algorithm, and manipulate
+    subsampled matrices. This is a key trait for performance-hungry components.
+    """
+
+    def __init__(
+        self,
+        subsampling: Optional[Subsampling] = None,
+    ) -> None:
+        if subsampling is None:
+            subsampling = KeepAll()
+        self.is_subsampled = not isinstance(subsampling, KeepAll)
+        self.subsampling = subsampling
+        self.references: List[np.ndarray] = []
+
+    @property
+    def has_subsampling(self) -> bool:
+        return not isinstance(self.subsampling, KeepAll)
+
+    def compute_subsampling(
+        self,
+        datasets: List[AnnData],
+        matrices: List[np.ndarray],
+        is_feature_space: bool,
+        log_callback: Optional[Callable] = None,
+    ) -> None:
+        """
+        Runs the subsampling on a list of datasets, and
+        stores the result in AnnData objects. If subsampling results
+        are already found, skips the dataset.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            AnnData objects containing datasets to subsample.
+
+        matrices: List[np.ndarray]
+            Matrix representation of datasets to subsample.
+        """
+        if self.has_subsampling is False:
+            return
+        if log_callback is not None:
+            log_callback(f"Applying subsampling {self.subsampling}.")
+        preprocess_traits(self.subsampling, datasets, is_feature_space)
+        ndatasets = len(datasets)
+        assert len(matrices) == ndatasets, "Inconsistent number of matrices/annadatas."
+        to_compute = []
+        self.anchors = [None] * ndatasets
+        self.references = [None] * ndatasets
+        for i, adata in enumerate(datasets):
+            anchors = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingAnchors)
+            references = adm.get_value(
+                adata, AnnDataKeyIdentifiers.SubsamplingReferences
+            )
+            if anchors is None or references is None:
+                # Needs to be computed
+                to_compute.append((i, matrices[i]))
+            else:
+                self.anchors[i] = anchors
+                self.references[i] = references
+
+        # Computes missing subsamplings
+        subsampling_results = self.subsampling.subsample(
+            datasets, [mtx for _, mtx in to_compute]
+        )
+        # We store results in AnnData objects
+        for (i, _), (anchors, references) in zip(to_compute, subsampling_results):
+            adm.set_value(
+                adata=datasets[i],
+                key=AnnDataKeyIdentifiers.SubsamplingAnchors,
+                field="obs",
+                value=anchors,
+                persist="output",
+            )
+            adm.set_value(
+                adata=datasets[i],
+                key=AnnDataKeyIdentifiers.SubsamplingReferences,
+                field="obs",
+                value=references,
+                persist="output",
+            )
+            self.anchors[i] = anchors
+            self.references[i] = references
+
+        if log_callback is not None:
+            for i, anchors in enumerate(self.anchors):
+                log_callback(
+                    f"Dataset {i} subsampled from {anchors.shape[0]} to "
+                    f"{anchors.sum()} samples."
+                )
+
+    @staticmethod
+    def get_anchors(adata: AnnData) -> np.ndarray:
+        """
+        Returns the chosen subsample as a boolean numpy array.
+        """
+        anchors = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingAnchors)
+        if anchors is None:
+            raise KeyError(f"No anchors found for the AnnData {adata}.")
+        return anchors
+
+    @staticmethod
+    def get_references(adata: AnnData) -> np.ndarray:
+        """
+        Returns the chosen subsample as a boolean numpy array.
+        """
+        references = adm.get_value(adata, AnnDataKeyIdentifiers.SubsamplingReferences)
+        if references is None:
+            raise KeyError(f"No references found for the AnnData {adata}.")
+        return references
+
+    def subsample_matrix(
+        self,
+        matrix: Union[np.ndarray, csr_matrix],
+        idx: int,
+        idx_2: Optional[int] = None,
+        pairwise: bool = False,
+    ) -> Union[np.ndarray, csr_matrix]:
+        """
+        Returns row-sliced matrix with respect to computed subsample.
+
+        Parameters
+        ----------
+        matrix: np.ndarray
+            Array to slice.
+
+        index: int
+            Matrix index used in compute_subsampling
+
+        pairwise: bool, default = False
+            Also column-slice the matrix, matrix must be squared.
+        """
+        if self.has_subsampling is False:
+            return matrix
+        assert idx < len(
+            self.anchors
+        ), "Ensure compute_subsampling has been called first."
+        assert not (idx_2 is not None and pairwise), "Incompatible pairwise non-square."
+        anchors = self.anchors[idx]
+        X = matrix[anchors]
+        if pairwise:
+            X = X[:, anchors]
+        if idx_2 is not None:
+            X = X[:, self.anchors[idx_2]]
+        return X
+
+    def subsample_matrices(
+        self,
+        matrices: List[Union[np.ndarray, csr_matrix]],
+        pairwise: bool = False,
+    ) -> List[Union[np.ndarray, csr_matrix]]:
+        """
+        Returns row-sliced views of input matrices according to
+        the subsampling computed.
+
+        Parameters
+        ----------
+        matrices: List[np.ndarray]
+            Arrays to slice in a list.
+
+        pairwise: bool, default = False
+            Also column-slice the matrix, matrix must be squared.
+        """
+        result = []
+        for i, X in enumerate(matrices):
+            result.append(self.subsample_matrix(X, i, pairwise=pairwise))
+        return result
+
+    def unsubsample_matrix_exact(
+        self,
+        matrix: Union[csr_matrix, np.ndarray],
+        idx: int,
+        idx_2: Optional[int] = None,
+    ) -> Union[csr_matrix, np.ndarray]:
+        """
+        Restores initial structure of a subsampled matrix, possibly
+        pairwise. Useful to reverse subsampling of a distance matrix for
+        instance.
+
+        Parameters
+        ----------
+        matrix: Union[csr_matrix, np.ndarray]
+            Subsampled matrix to turn back to full size.
+
+        idx: int
+            Index of the subsampling to use.
+
+        idx_2: Optional[int]
+            In case of pairwise matrix between different datasets, subsampling
+            index of the second dataset.
+        """
+        # Sanity check
+        if self.has_subsampling is False:
+            return matrix
+        assert isinstance(
+            matrix, (csr_matrix, np.ndarray)
+        ), f"Unknown type: {type(matrix)}"
+
+        # Inverting subsampling indices
+        n_samples = self.anchors[idx].shape[0]
+        n_features = n_samples
+        s_to_S1 = np.arange(n_samples)[self.anchors[idx].astype(bool)]
+        s_to_S2 = s_to_S1
+        if idx_2 is not None:
+            anchors_2 = self.anchors[idx_2]
+            n_features = anchors_2.shape[0]
+            s_to_S2 = np.arange(n_features)[anchors_2.astype(bool)]
+
+        # Reversing subsampling
+        if isinstance(matrix, csr_matrix):
+            X_coo = matrix.tocoo()
+            srow, scol, sdata = X_coo.row, X_coo.col, X_coo.data
+            Srow = s_to_S1[srow]
+            if idx_2 is None:
+                Scol = scol
+            else:
+                Scol = s_to_S2[scol]
+            return csr_matrix(
+                (sdata, (Srow, Scol)),
+                shape=(n_samples, n_features),
+            )
+        else:  # np.ndarray
+            X = np.zeros((n_samples, n_features), dtype=matrix.dtype)
+            for idx_i, coord_i in enumerate(s_to_S1):
+                for idx_j, coord_j in enumerate(s_to_S2):
+                    X[coord_i, coord_j] = matrix[idx_i, idx_j]
+            return X
+
+    def unsubsample_matrix_transitive(
+        self,
+        matrix: csr_matrix,
+        adata_src: AnnData,
+        adata_ref: AnnData,
+    ) -> csr_matrix:
+        """
+        TODO
+        """
+        Tx = get_cell_anchor_matrix(adata_src)
+        Ty = get_cell_anchor_matrix(adata_ref)
+        T_tot = Tx @ matrix @ Ty.T
+        T_tot_norm = T_tot.sum(axis=1)
+        T_tot_norm[T_tot_norm == 0.0] = 1.0
+        return csr_matrix(T_tot / T_tot_norm[:, None])
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/usescommonfeatures.py` & `transmorph-0.2.7/src/transmorph/engine/traits/usescommonfeatures.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from anndata import AnnData
-from typing import List, Literal, Optional, Tuple, Union
-
-from ...utils.anndata_manager import (
-    _TypePairwiseSlice,
-    _TypeTotalSlice,
-    get_pairwise_feature_slices,
-    get_total_feature_slices,
-)
-
-_TypeAnnDataCommonModes = Literal["pairwise", "total", "ignore"]
-
-
-class UsesCommonFeatures:
-    """
-    This trait will allow an object to retrieve feature names from an AnnData
-    object. They will then be used to slice count matrices in order to select
-    pairwise or total common genes intersection.
-    """
-
-    def __init__(self, mode: _TypeAnnDataCommonModes):
-        assert mode in ("pairwise", "total", "ignore")
-        self.mode = mode
-        # TFS is used for mode "total", PFS for mode "pairwise"
-        self.total_feature_slices: _TypeTotalSlice = []
-        self.pairwise_feature_slices: _TypePairwiseSlice = {}
-        self.fitted = False
-        self.is_feature_space = False
-
-    def retrieve_common_features(
-        self, datasets: List[AnnData], is_feature_space: bool
-    ) -> None:
-        """
-        Stores gene names for later use.
-        """
-        self.is_feature_space = is_feature_space
-        if not is_feature_space or self.mode == "ignore":
-            return
-        if self.mode == "pairwise":
-            self.pairwise_feature_slices = get_pairwise_feature_slices(datasets)
-        elif self.mode == "total":
-            self.total_feature_slices = get_total_feature_slices(datasets)
-        else:
-            raise ValueError(f"Unknown mode {self.mode}.")
-        self.fitted = True
-
-    def get_common_features(
-        self, idx_1: int, idx_2: int
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Returns a tuple containing feature slices to use between two datasets
-        identified as their index. Raises a ValueError if idx_1, idx_2 is unknown.
-        """
-        assert self.fitted, "UsesCommonFeatures trait has not retrieved features."
-        if self.mode == "pairwise":
-            slices = self.pairwise_feature_slices.get((idx_1, idx_2), None)
-            if slices is None:
-                raise ValueError(f"No feature slice found for {idx_1}, {idx_2}.")
-        elif self.mode == "total":
-            assert idx_1 < len(self.total_feature_slices), f"{idx_1} out of bounds."
-            assert idx_2 < len(self.total_feature_slices), f"{idx_2} out of bounds."
-            slices = self.total_feature_slices[idx_1], self.total_feature_slices[idx_2]
-        else:
-            raise ValueError(f"Unknown mode {self.mode}.")
-        return slices
-
-    def slice_features(
-        self,
-        X1: np.ndarray,
-        idx_1: int,
-        X2: Optional[np.ndarray] = None,
-        idx_2: Optional[int] = None,
-    ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
-        """
-        Returns a sliced view of datasets X1 and X2, indexed by idx_1 and idx_2. Raises
-        a ValueError if indices are not found, or if slice size does not coincidate.
-        """
-        assert not ((X2 is None) ^ (idx_2 is None))
-        # If we are not in feature space, we must skip the processing.
-        if not self.is_feature_space or not self.fitted or self.mode == "ignore":
-            if X2 is None:
-                return X1
-            return X1, X2
-        if X2 is None:
-            assert (
-                self.mode == "total"
-            ), "Calling slice_features with one dataset is only"
-            " valid for mode == 'total'."
-            return X1[:, self.total_feature_slices[idx_1]].copy()
-        s1, s2 = self.get_common_features(idx_1, idx_2)
-        return X1[:, s1].copy(), X2[:, s2].copy()
-
-    def assert_common_features(self, datasets: List[AnnData]) -> None:
-        """
-        For testing purposes, asserts a list of AnnData objects is correctly
-        sliced in a common features space.
-        """
-        if self.mode == "total":
-            com_features: Optional[np.ndarray] = None
-            for adata, fslice in zip(datasets, self.total_feature_slices):
-                if com_features is None:
-                    com_features = adata.var_names[fslice].to_numpy()
-                else:
-                    np.testing.assert_array_equal(
-                        com_features,
-                        adata.var_names[fslice].to_numpy(),
-                    )
-        elif self.mode == "pairwise":
-            for i, adata_i in enumerate(datasets):
-                for j, adata_j in enumerate(datasets):
-                    slice_i, slice_j = self.pairwise_feature_slices[i, j]
-                    np.testing.assert_array_equal(
-                        adata_i.var_names[slice_i].to_numpy(),
-                        adata_j.var_names[slice_j].to_numpy(),
-                    )
-        else:
-            raise ValueError(f"Unrecognized mode: {self.mode}.")
+#!/usr/bin/env python3
+
+import numpy as np
+
+from anndata import AnnData
+from typing import List, Literal, Optional, Tuple, Union
+
+from ...utils.anndata_manager import (
+    _TypePairwiseSlice,
+    _TypeTotalSlice,
+    get_pairwise_feature_slices,
+    get_total_feature_slices,
+)
+
+_TypeAnnDataCommonModes = Literal["pairwise", "total", "ignore"]
+
+
+class UsesCommonFeatures:
+    """
+    This trait will allow an object to retrieve feature names from an AnnData
+    object. They will then be used to slice count matrices in order to select
+    pairwise or total common genes intersection.
+    """
+
+    def __init__(self, mode: _TypeAnnDataCommonModes):
+        assert mode in ("pairwise", "total", "ignore")
+        self.mode = mode
+        # TFS is used for mode "total", PFS for mode "pairwise"
+        self.total_feature_slices: _TypeTotalSlice = []
+        self.pairwise_feature_slices: _TypePairwiseSlice = {}
+        self.fitted = False
+        self.is_feature_space = False
+
+    def retrieve_common_features(
+        self, datasets: List[AnnData], is_feature_space: bool
+    ) -> None:
+        """
+        Stores gene names for later use.
+        """
+        self.is_feature_space = is_feature_space
+        if not is_feature_space or self.mode == "ignore":
+            return
+        if self.mode == "pairwise":
+            self.pairwise_feature_slices = get_pairwise_feature_slices(datasets)
+        elif self.mode == "total":
+            self.total_feature_slices = get_total_feature_slices(datasets)
+        else:
+            raise ValueError(f"Unknown mode {self.mode}.")
+        self.fitted = True
+
+    def get_common_features(
+        self, idx_1: int, idx_2: int
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Returns a tuple containing feature slices to use between two datasets
+        identified as their index. Raises a ValueError if idx_1, idx_2 is unknown.
+        """
+        assert self.fitted, "UsesCommonFeatures trait has not retrieved features."
+        if self.mode == "pairwise":
+            slices = self.pairwise_feature_slices.get((idx_1, idx_2), None)
+            if slices is None:
+                raise ValueError(f"No feature slice found for {idx_1}, {idx_2}.")
+        elif self.mode == "total":
+            assert idx_1 < len(self.total_feature_slices), f"{idx_1} out of bounds."
+            assert idx_2 < len(self.total_feature_slices), f"{idx_2} out of bounds."
+            slices = self.total_feature_slices[idx_1], self.total_feature_slices[idx_2]
+        else:
+            raise ValueError(f"Unknown mode {self.mode}.")
+        return slices
+
+    def slice_features(
+        self,
+        X1: np.ndarray,
+        idx_1: int,
+        X2: Optional[np.ndarray] = None,
+        idx_2: Optional[int] = None,
+    ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
+        """
+        Returns a sliced view of datasets X1 and X2, indexed by idx_1 and idx_2. Raises
+        a ValueError if indices are not found, or if slice size does not coincidate.
+        """
+        assert not ((X2 is None) ^ (idx_2 is None))
+        # If we are not in feature space, we must skip the processing.
+        if not self.is_feature_space or not self.fitted or self.mode == "ignore":
+            if X2 is None:
+                return X1
+            return X1, X2
+        if X2 is None:
+            assert (
+                self.mode == "total"
+            ), "Calling slice_features with one dataset is only"
+            " valid for mode == 'total'."
+            return X1[:, self.total_feature_slices[idx_1]].copy()
+        s1, s2 = self.get_common_features(idx_1, idx_2)
+        return X1[:, s1].copy(), X2[:, s2].copy()
+
+    def assert_common_features(self, datasets: List[AnnData]) -> None:
+        """
+        For testing purposes, asserts a list of AnnData objects is correctly
+        sliced in a common features space.
+        """
+        if self.mode == "total":
+            com_features: Optional[np.ndarray] = None
+            for adata, fslice in zip(datasets, self.total_feature_slices):
+                if com_features is None:
+                    com_features = adata.var_names[fslice].to_numpy()
+                else:
+                    np.testing.assert_array_equal(
+                        com_features,
+                        adata.var_names[fslice].to_numpy(),
+                    )
+        elif self.mode == "pairwise":
+            for i, adata_i in enumerate(datasets):
+                for j, adata_j in enumerate(datasets):
+                    slice_i, slice_j = self.pairwise_feature_slices[i, j]
+                    np.testing.assert_array_equal(
+                        adata_i.var_names[slice_i].to_numpy(),
+                        adata_j.var_names[slice_j].to_numpy(),
+                    )
+        else:
+            raise ValueError(f"Unrecognized mode: {self.mode}.")
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/usesmatching.py` & `transmorph-0.2.7/src/transmorph/engine/traits/usesmatching.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from scipy.sparse import csr_matrix, diags
-from typing import Dict, Literal, Optional
-
-from ..matching import _TypeMatchingSet
-
-_TypeMatchingModes = Literal["raw", "bool", "normalized"]
-
-
-class UsesMatching:
-    """
-    Allows an object to use matching matrices between datasets.
-    """
-
-    def __init__(self, mode: _TypeMatchingModes = "raw"):
-        # Read-only
-        self.matchings: Optional[_TypeMatchingSet] = None
-        assert mode in ("raw", "bool", "normalized")
-        self.mode = mode
-
-    def set_matchings(self, matchings: _TypeMatchingSet) -> None:
-        """
-        Loads the object with a read-only dictionary of matching matrices,
-        coming from a LayerMatching.
-        """
-        assert isinstance(matchings, Dict)
-        self.matchings = matchings
-
-    def get_matching(self, idx1: int, idx2: int) -> csr_matrix:
-        """
-        Returns matching between datasets idx1 and idx2. Raises an exception
-        if matching has not been found.
-        """
-        assert self.matchings is not None, "No matching provided."
-        result = self.matchings.get((idx1, idx2), None)
-        if result is None:
-            result = self.matchings.get((idx2, idx2), None)
-            assert result is not None, f"{idx1}, {idx2} not found in matching."
-            result = csr_matrix(result.T)
-        if self.mode == "raw":
-            return result
-        if self.mode == "bool":
-            return result.astype(bool)
-        if self.mode == "normalized":
-            norm = np.array(result.sum(axis=1)).reshape(-1)
-            norm[norm == 0.0] = 1.0
-            return diags(1.0 / norm) @ result
-        raise ValueError(f"Unknown mode {self.mode}")
+#!/usr/bin/env python3
+
+import numpy as np
+
+from scipy.sparse import csr_matrix, diags
+from typing import Dict, Literal, Optional
+
+from ..matching import _TypeMatchingSet
+
+_TypeMatchingModes = Literal["raw", "bool", "normalized"]
+
+
+class UsesMatching:
+    """
+    Allows an object to use matching matrices between datasets.
+    """
+
+    def __init__(self, mode: _TypeMatchingModes = "raw"):
+        # Read-only
+        self.matchings: Optional[_TypeMatchingSet] = None
+        assert mode in ("raw", "bool", "normalized")
+        self.mode = mode
+
+    def set_matchings(self, matchings: _TypeMatchingSet) -> None:
+        """
+        Loads the object with a read-only dictionary of matching matrices,
+        coming from a LayerMatching.
+        """
+        assert isinstance(matchings, Dict)
+        self.matchings = matchings
+
+    def get_matching(self, idx1: int, idx2: int) -> csr_matrix:
+        """
+        Returns matching between datasets idx1 and idx2. Raises an exception
+        if matching has not been found.
+        """
+        assert self.matchings is not None, "No matching provided."
+        result = self.matchings.get((idx1, idx2), None)
+        if result is None:
+            result = self.matchings.get((idx2, idx2), None)
+            assert result is not None, f"{idx1}, {idx2} not found in matching."
+            result = csr_matrix(result.T)
+        if self.mode == "raw":
+            return result
+        if self.mode == "bool":
+            return result.astype(bool)
+        if self.mode == "normalized":
+            norm = np.array(result.sum(axis=1)).reshape(-1)
+            norm[norm == 0.0] = 1.0
+            return diags(1.0 / norm) @ result
+        raise ValueError(f"Unknown mode {self.mode}")
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/usesmetric.py` & `transmorph-0.2.7/src/transmorph/engine/traits/usesmetric.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Dict, List, Optional, Tuple
-
-from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
-
-_TypeMetric = Tuple[str, Dict]
-
-
-class UsesMetric:
-    """
-    Objects with this trait can set and get internal metrics of
-    AnnData objects.
-
-    Parameters
-    ----------
-    default_metric: str, default = "sqeuclidean"
-        Scipy-compatible metric to use if no metric is found in an AnnData object.
-
-    default_kwargs: Dict, default = {}
-        Additional parameters to provide to metric
-
-    Attributes
-    ----------
-    _stored_metrics: List[Tuple[str, Dict]]
-        List of cached metrics to use in methods that do not have direct access
-        to AnnData objects.
-    """
-
-    def __init__(self, default_metric: str, default_kwargs: Optional[Dict] = None):
-        self._default_metric = default_metric
-        if default_kwargs is None:
-            default_kwargs = {}
-        self._default_metric_kwargs = default_kwargs
-        self._stored_metrics: List[_TypeMetric] = []
-
-    @staticmethod
-    def set_adata_metric(
-        adata: AnnData,
-        metric: str,
-        metric_kwargs: Optional[Dict] = None,
-    ) -> None:
-        """
-        Sets AnnData internal metric inside a AnnData object. Modules which use
-        internal metric will use this one in priority.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to write metric in.
-
-        metric: str
-            Scipy-compatible metric name.
-
-        metric_kwargs: Optional[Dict]
-            Optional additional parameters to provide to cdist() function.
-        """
-        if metric_kwargs is None:
-            metric_kwargs = {}
-        adm.set_value(
-            adata=adata,
-            key=AnnDataKeyIdentifiers.Metric,
-            field="uns",
-            value=metric,
-            persist="output",
-        )
-        adm.set_value(
-            adata=adata,
-            key=AnnDataKeyIdentifiers.MetricKwargs,
-            field="uns",
-            value=metric_kwargs,
-            persist="output",
-        )
-
-    @staticmethod
-    def get_adata_metric(adata: AnnData) -> Optional[_TypeMetric]:
-        """
-        Returns AnnData internal metric if set, None otherwise.
-
-        Parameters
-        ----------
-            adata: AnnData to retrieve metric from.
-        """
-        metric = adm.get_value(adata, AnnDataKeyIdentifiers.Metric)
-        if metric is None:
-            return None
-        kwargs = adm.get_value(adata, AnnDataKeyIdentifiers.MetricKwargs)
-        if kwargs is None:
-            kwargs = {}
-        return metric, kwargs
-
-    def retrieve_all_metrics(self, datasets: List[AnnData]) -> None:
-        """
-        Retrieves metrics from a list of AnnData datasets and saves them
-        in objsct cache. If information is missing, fills with default value.
-
-        Parameters
-        ----------
-        datasets: AnnData
-            AnnData objects to extract metric information from.
-        """
-        for adata in datasets:
-            adata_metric = UsesMetric.get_adata_metric(adata)
-            if adata_metric is None:
-                metric, kwargs = self._default_metric, self._default_metric_kwargs
-            else:
-                metric, kwargs = adata_metric
-            self._stored_metrics.append((metric, kwargs))
-
-    def get_metric(self, index: int) -> _TypeMetric:
-        """
-        Returns metric and metric kwargs contained in anndata, or default ones
-        if information is missing.
-
-        Parameters
-        ----------
-        index: int
-            Dataset index corresponding to the list order passed to
-            retrieve_all_metrics
-        """
-        assert index < len(
-            self._stored_metrics
-        ), f"{index} out of range, make sure retrieve_all_metrics have been called."
-        return self._stored_metrics[index]
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Dict, List, Optional, Tuple
+
+from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
+
+_TypeMetric = Tuple[str, Dict]
+
+
+class UsesMetric:
+    """
+    Objects with this trait can set and get internal metrics of
+    AnnData objects.
+
+    Parameters
+    ----------
+    default_metric: str, default = "sqeuclidean"
+        Scipy-compatible metric to use if no metric is found in an AnnData object.
+
+    default_kwargs: Dict, default = {}
+        Additional parameters to provide to metric
+
+    Attributes
+    ----------
+    _stored_metrics: List[Tuple[str, Dict]]
+        List of cached metrics to use in methods that do not have direct access
+        to AnnData objects.
+    """
+
+    def __init__(self, default_metric: str, default_kwargs: Optional[Dict] = None):
+        self._default_metric = default_metric
+        if default_kwargs is None:
+            default_kwargs = {}
+        self._default_metric_kwargs = default_kwargs
+        self._stored_metrics: List[_TypeMetric] = []
+
+    @staticmethod
+    def set_adata_metric(
+        adata: AnnData,
+        metric: str,
+        metric_kwargs: Optional[Dict] = None,
+    ) -> None:
+        """
+        Sets AnnData internal metric inside a AnnData object. Modules which use
+        internal metric will use this one in priority.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to write metric in.
+
+        metric: str
+            Scipy-compatible metric name.
+
+        metric_kwargs: Optional[Dict]
+            Optional additional parameters to provide to cdist() function.
+        """
+        if metric_kwargs is None:
+            metric_kwargs = {}
+        adm.set_value(
+            adata=adata,
+            key=AnnDataKeyIdentifiers.Metric,
+            field="uns",
+            value=metric,
+            persist="output",
+        )
+        adm.set_value(
+            adata=adata,
+            key=AnnDataKeyIdentifiers.MetricKwargs,
+            field="uns",
+            value=metric_kwargs,
+            persist="output",
+        )
+
+    @staticmethod
+    def get_adata_metric(adata: AnnData) -> Optional[_TypeMetric]:
+        """
+        Returns AnnData internal metric if set, None otherwise.
+
+        Parameters
+        ----------
+            adata: AnnData to retrieve metric from.
+        """
+        metric = adm.get_value(adata, AnnDataKeyIdentifiers.Metric)
+        if metric is None:
+            return None
+        kwargs = adm.get_value(adata, AnnDataKeyIdentifiers.MetricKwargs)
+        if kwargs is None:
+            kwargs = {}
+        return metric, kwargs
+
+    def retrieve_all_metrics(self, datasets: List[AnnData]) -> None:
+        """
+        Retrieves metrics from a list of AnnData datasets and saves them
+        in objsct cache. If information is missing, fills with default value.
+
+        Parameters
+        ----------
+        datasets: AnnData
+            AnnData objects to extract metric information from.
+        """
+        for adata in datasets:
+            adata_metric = UsesMetric.get_adata_metric(adata)
+            if adata_metric is None:
+                metric, kwargs = self._default_metric, self._default_metric_kwargs
+            else:
+                metric, kwargs = adata_metric
+            self._stored_metrics.append((metric, kwargs))
+
+    def get_metric(self, index: int) -> _TypeMetric:
+        """
+        Returns metric and metric kwargs contained in anndata, or default ones
+        if information is missing.
+
+        Parameters
+        ----------
+        index: int
+            Dataset index corresponding to the list order passed to
+            retrieve_all_metrics
+        """
+        assert index < len(
+            self._stored_metrics
+        ), f"{index} out of range, make sure retrieve_all_metrics have been called."
+        return self._stored_metrics[index]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/usesreference.py` & `transmorph-0.2.7/src/transmorph/engine/layers/layeroutput.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,48 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import List, Optional, TypeVar
-from ...utils.anndata_manager import anndata_manager as adm, AnnDataKeyIdentifiers
-
-T = TypeVar("T")
-
-
-class UsesReference:
-    """
-    This trait is shared by objects that must use a reference
-    dataset.
-    """
-
-    def __init__(self):
-        self.reference_index: Optional[int] = None
-
-    @staticmethod
-    def write_is_reference(adata: AnnData) -> None:
-        """
-        Sets an anndata to be considered as reference. Should not be used on
-        more than one anndata object.
-        """
-        adm.set_value(
-            adata=adata,
-            key=AnnDataKeyIdentifiers.IsReference,
-            field="uns",
-            value=True,
-            persist="pipeline",
-        )
-
-    def retrieve_reference_index(self, datasets: List[AnnData]) -> None:
-        """
-        Returns index of AnnData that has been chosen as a reference. If
-        found none or several, returns -1.
-        """
-        ref_id = -1
-        for k, adata in enumerate(datasets):
-            is_ref = adm.get_value(adata, AnnDataKeyIdentifiers.IsReference)
-            if is_ref is not None:
-                if ref_id != -1:
-                    raise AttributeError("More than one reference.")
-                ref_id = k
-        if ref_id == -1:
-            return
-        self.reference_index = ref_id
-
-    def get_reference_item(self, datasets: List[T]) -> Optional[T]:
-        """
-        Returns object that has been chosen as a reference from a list. If
-        found none or several, returns None.
-        """
-        ref_id = self.reference_index
-        if ref_id is None:
-            return None
-        return datasets[ref_id]
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import List
+
+from . import Layer
+from ..traits import CanCatchChecking, IsRepresentable
+from ...utils.anndata_manager import AnnDataKeyIdentifiers
+
+
+class LayerOutput(Layer, CanCatchChecking, IsRepresentable):
+    """
+    A LayerOutput is the final step of any model. Its only role
+    is to retrieve last computed representation, and write it
+    durably in AnnDatas under the entry .obsm['X_transmorph'].
+    """
+
+    def __init__(self) -> None:
+        Layer.__init__(
+            self,
+            compatible_inputs=[IsRepresentable],
+            str_identifier="OUTPUT",
+        )
+        IsRepresentable.__init__(
+            self,
+            repr_key=AnnDataKeyIdentifiers.TransmorphRepresentation,
+        )
+        CanCatchChecking.__init__(self)
+
+    def fit(self, datasets: List[AnnData]) -> List[Layer]:
+        """
+        Simply retrieves last computed representation,
+        and write it in AnnData objects.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            Datasets to write results in.
+        """
+        self.log(f"Retrieving data from {self.embedding_reference.repr_key}.")
+        for adata in datasets:
+            self.write_representation(
+                adata,
+                self.embedding_reference.get_representation(adata),
+                self.embedding_reference.is_feature_space,
+                persist="output",
+            )
+        return []
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/usessamplelabels.py` & `transmorph-0.2.7/src/transmorph/engine/traits/usessamplelabels.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-from anndata import AnnData
-from scipy.sparse import csr_matrix
-from typing import List, Optional
-
-
-class UsesSampleLabels:
-    """
-    Allows a class to extract sample labels.
-
-    Parameters
-    ----------
-    label_obs: str
-        AnnData obs key to extract label from. If left None,
-        this trait is ignored.
-    """
-
-    def __init__(self, label_obs: Optional[str] = None) -> None:
-        self.label_obs = label_obs
-        self.labels: List[np.ndarray] = []
-        self.fitted = False
-
-    def _check_index(self, idx: int) -> None:
-        """
-        Raises an exception if self.labels[$idx] is not accessable.
-        """
-        if self.label_obs is None:
-            raise RuntimeError("Label obs was not specified.")
-        if not self.fitted:
-            raise RuntimeError("self.retrieve_all_labels not called.")
-        if idx >= len(self.labels):
-            raise IndexError(
-                f"Index {idx} out of range for list " f"of size {len(self.labels)}."
-            )
-
-    def retrieve_all_labels(self, datasets: List[AnnData]) -> None:
-        """
-        Retrieves and stores labels from AnnData objects.
-        """
-        if self.label_obs is None:
-            return
-        assert all(self.label_obs in adata.obs for adata in datasets), (
-            f"Key '{self.label_obs}' missing in some datasets. Available label "
-            f"keys in this dataset are: {', '.join(sorted(datasets[0].obs))}"
-        )
-        for adata in datasets:
-            self.labels.append(adata.obs[self.label_obs].to_numpy())
-        self.fitted = True
-
-    def get_dataset_labels(self, idx: int) -> np.ndarray:
-        """
-        Returns labels of dataset #idx.
-        """
-        self._check_index(idx)
-        return self.labels[idx]
-
-    def get_matching_matrix(self, idx_1: int, idx_2: int) -> csr_matrix:
-        """
-        Returns a n1 x n2 matrix where M[i, j] = yi == yj, to the
-        CSR sparse format.
-        """
-        labels_1 = self.get_dataset_labels(idx_1)
-        labels_2 = self.get_dataset_labels(idx_2)
-        return csr_matrix(labels_1[:, None] == labels_2)
+#!/usr/bin/env python3
+
+import numpy as np
+
+from anndata import AnnData
+from scipy.sparse import csr_matrix
+from typing import List, Optional
+
+
+class UsesSampleLabels:
+    """
+    Allows a class to extract sample labels.
+
+    Parameters
+    ----------
+    label_obs: str
+        AnnData obs key to extract label from. If left None,
+        this trait is ignored.
+    """
+
+    def __init__(self, label_obs: Optional[str] = None) -> None:
+        self.label_obs = label_obs
+        self.labels: List[np.ndarray] = []
+        self.fitted = False
+
+    def _check_index(self, idx: int) -> None:
+        """
+        Raises an exception if self.labels[$idx] is not accessable.
+        """
+        if self.label_obs is None:
+            raise RuntimeError("Label obs was not specified.")
+        if not self.fitted:
+            raise RuntimeError("self.retrieve_all_labels not called.")
+        if idx >= len(self.labels):
+            raise IndexError(
+                f"Index {idx} out of range for list " f"of size {len(self.labels)}."
+            )
+
+    def retrieve_all_labels(self, datasets: List[AnnData]) -> None:
+        """
+        Retrieves and stores labels from AnnData objects.
+        """
+        if self.label_obs is None:
+            return
+        assert all(self.label_obs in adata.obs for adata in datasets), (
+            f"Key '{self.label_obs}' missing in some datasets. Available label "
+            f"keys in this dataset are: {', '.join(sorted(datasets[0].obs))}"
+        )
+        for adata in datasets:
+            self.labels.append(adata.obs[self.label_obs].to_numpy())
+        self.fitted = True
+
+    def get_dataset_labels(self, idx: int) -> np.ndarray:
+        """
+        Returns labels of dataset #idx.
+        """
+        self._check_index(idx)
+        return self.labels[idx]
+
+    def get_matching_matrix(self, idx_1: int, idx_2: int) -> csr_matrix:
+        """
+        Returns a n1 x n2 matrix where M[i, j] = yi == yj, to the
+        CSR sparse format.
+        """
+        labels_1 = self.get_dataset_labels(idx_1)
+        labels_2 = self.get_dataset_labels(idx_2)
+        return csr_matrix(labels_1[:, None] == labels_2)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/traits/utils.py` & `transmorph-0.2.7/src/transmorph/engine/traits/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Any, List, Tuple, Type, Union
-
-
-from .hasmetadata import HasMetadata
-from .usescommonfeatures import UsesCommonFeatures
-from .usesmetric import UsesMetric
-from .usesreference import UsesReference
-from .usessamplelabels import UsesSampleLabels
-
-
-def assert_trait(obj: Any, traits: Union[Type, Tuple[Type, ...]]):
-    """
-    Raises an exception if $obj is not endowed with the
-    trait $trait.
-    """
-    if isinstance(obj, traits):
-        return
-    if isinstance(traits, Type):
-        all_traits: str = traits.__name__
-    else:
-        all_traits: str = ", ".join([trait.__name__ for trait in traits])
-    raise TypeError(
-        f"Object {obj} of type {type(obj)} is not endowed"
-        f" with trait(s) {all_traits}."
-    )
-
-
-def preprocess_traits(
-    obj: Any,
-    datasets: List[AnnData],
-    is_feature_space: bool,
-) -> None:
-    """
-    Helper function to ensure all traits are preprocessed.
-    """
-    if isinstance(obj, HasMetadata):
-        obj.retrieve_all_metadata(datasets)
-    if isinstance(obj, UsesCommonFeatures):
-        obj.retrieve_common_features(datasets, is_feature_space)
-    if isinstance(obj, UsesMetric):
-        obj.retrieve_all_metrics(datasets)
-    if isinstance(obj, UsesReference):
-        obj.retrieve_reference_index(datasets)
-    if isinstance(obj, UsesSampleLabels):
-        obj.retrieve_all_labels(datasets)
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Any, List, Tuple, Type, Union
+
+
+from .hasmetadata import HasMetadata
+from .usescommonfeatures import UsesCommonFeatures
+from .usesmetric import UsesMetric
+from .usesreference import UsesReference
+from .usessamplelabels import UsesSampleLabels
+
+
+def assert_trait(obj: Any, traits: Union[Type, Tuple[Type, ...]]):
+    """
+    Raises an exception if $obj is not endowed with the
+    trait $trait.
+    """
+    if isinstance(obj, traits):
+        return
+    if isinstance(traits, Type):
+        all_traits: str = traits.__name__
+    else:
+        all_traits: str = ", ".join([trait.__name__ for trait in traits])
+    raise TypeError(
+        f"Object {obj} of type {type(obj)} is not endowed"
+        f" with trait(s) {all_traits}."
+    )
+
+
+def preprocess_traits(
+    obj: Any,
+    datasets: List[AnnData],
+    is_feature_space: bool,
+) -> None:
+    """
+    Helper function to ensure all traits are preprocessed.
+    """
+    if isinstance(obj, HasMetadata):
+        obj.retrieve_all_metadata(datasets)
+    if isinstance(obj, UsesCommonFeatures):
+        obj.retrieve_common_features(datasets, is_feature_space)
+    if isinstance(obj, UsesMetric):
+        obj.retrieve_all_metrics(datasets)
+    if isinstance(obj, UsesReference):
+        obj.retrieve_reference_index(datasets)
+    if isinstance(obj, UsesSampleLabels):
+        obj.retrieve_all_labels(datasets)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/ica.py` & `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/ica.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-import anndata as ad
-from typing import List
-
-from ..transformation import Transformation
-from ...traits.usescommonfeatures import UsesCommonFeatures
-from ....utils.dimred import ica
-from ....utils.matrix import extract_chunks
-
-
-class ICA(Transformation, UsesCommonFeatures):
-    """
-    Embeds a set of datasets in a common independent component (IC) space,
-    using StabilizedICA package. This is typically slower than PCA, but
-    features better tend to represent relevant and interpretable signals.
-
-    Parameters
-    ----------
-    n_components: int, default = 30
-        Number of PCs to use.
-
-    max_iter: int, default = 1000
-        Number of iterations in the optimization procedure.
-
-    n_runs: int, default = 10
-        Number of runs to carry out, more runs will yield a more
-        stable result.
-    """
-
-    def __init__(
-        self,
-        n_components: int = 30,
-        max_iter: int = 1000,
-        n_runs: int = 10,
-    ):
-        Transformation.__init__(self, str_identifier="PCA", preserves_space=False)
-        UsesCommonFeatures.__init__(self, mode="total")
-        self.n_components = n_components
-        self.max_iter = max_iter
-        self.n_runs = n_runs
-
-    def transform(
-        self,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-    ) -> List[np.ndarray]:
-        """
-        Slices datasets in the same space if necessary, then carries out the
-        information.
-        """
-        to_reduce = []
-        for i, X in enumerate(embeddings):
-            to_reduce.append(self.slice_features(X1=X, idx_1=i))
-        X_ica = ica(
-            np.concatenate(to_reduce, axis=0),
-            n_components=self.n_components,
-            max_iter=self.max_iter,
-            n_runs=self.n_runs,
-        )
-        return extract_chunks(X_ica, [X.shape[0] for X in datasets])
+#!/usr/bin/env python3
+
+import numpy as np
+
+import anndata as ad
+from typing import List
+
+from ..transformation import Transformation
+from ...traits.usescommonfeatures import UsesCommonFeatures
+from ....utils.dimred import ica
+from ....utils.matrix import extract_chunks
+
+
+class ICA(Transformation, UsesCommonFeatures):
+    """
+    Embeds a set of datasets in a common independent component (IC) space,
+    using StabilizedICA package. This is typically slower than PCA, but
+    features better tend to represent relevant and interpretable signals.
+
+    Parameters
+    ----------
+    n_components: int, default = 30
+        Number of PCs to use.
+
+    max_iter: int, default = 1000
+        Number of iterations in the optimization procedure.
+
+    n_runs: int, default = 10
+        Number of runs to carry out, more runs will yield a more
+        stable result.
+    """
+
+    def __init__(
+        self,
+        n_components: int = 30,
+        max_iter: int = 1000,
+        n_runs: int = 10,
+    ):
+        Transformation.__init__(self, str_identifier="PCA", preserves_space=False)
+        UsesCommonFeatures.__init__(self, mode="total")
+        self.n_components = n_components
+        self.max_iter = max_iter
+        self.n_runs = n_runs
+
+    def transform(
+        self,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+    ) -> List[np.ndarray]:
+        """
+        Slices datasets in the same space if necessary, then carries out the
+        information.
+        """
+        to_reduce = []
+        for i, X in enumerate(embeddings):
+            to_reduce.append(self.slice_features(X1=X, idx_1=i))
+        X_ica = ica(
+            np.concatenate(to_reduce, axis=0),
+            n_components=self.n_components,
+            max_iter=self.max_iter,
+            n_runs=self.n_runs,
+        )
+        return extract_chunks(X_ica, [X.shape[0] for X in datasets])
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/pooling.py` & `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/pooling.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-
-from typing import List
-
-from ..transformation import Transformation
-from ....utils.matrix import pooling, extract_chunks, sort_sparse_matrix, perturbate
-from ....utils.graph import nearest_neighbors, nearest_neighbors_custom
-
-
-class Pooling(Transformation):
-    """
-    Replaces each sample by the average of its neighbors. This
-    is a useful to smooth data manifolds, and reduce the impact
-    of outliers or artifacts. It can also be used after a merging
-    to smooth the result, by toggling per_dataset parameter.
-
-    Parameters
-    ----------
-    n_neighbors: int, default = 5
-        Number of neighhbors to use for the pooling. The higher,
-        the smoother data is.
-
-    jitter_std: float, default = 0.01
-        If > 0, applies a small perturbation at the end of pooling of
-        standard deviation $jitter_std to unstick samples.
-
-    per_dataset: bool, default = True
-        Performs the pooling for each dataset independently. If false,
-        all datasets are concatenated (they are then expected to be
-        embedded in the same features space).
-    """
-
-    def __init__(
-        self,
-        n_neighbors: int = 5,
-        transformation_rate: float = 1.0,
-        jitter_std: float = 0.01,
-        per_dataset: bool = True,
-    ):
-        Transformation.__init__(self, "POOLING", True, transformation_rate)
-        self.n_neighbors = n_neighbors
-        self.jitter_std = jitter_std
-        self.per_dataset = per_dataset
-
-    def transform(
-        self,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-    ) -> List[np.ndarray]:
-        """
-        Applies pooling, potentially partial.
-        """
-        if self.per_dataset:
-            result = []
-            for adata, X in zip(datasets, embeddings):
-                neighbors = nearest_neighbors(
-                    adata,
-                    mode="edges",
-                    n_neighbors=self.n_neighbors,
-                )
-                indices, _ = sort_sparse_matrix(neighbors)
-                X_pooled = pooling(X, indices)
-                if self.transformation_rate <= 1.0:
-                    X_pooled *= self.transformation_rate
-                    X_pooled += X * (1.0 - self.transformation_rate)
-                result.append(X_pooled)
-        else:
-            X_all = np.concatenate(datasets, axis=0)
-            nn_matrix = nearest_neighbors_custom(
-                X_all,
-                "edges",
-                n_neighbors=self.n_neighbors,
-            )
-            indices, _ = sort_sparse_matrix(nn_matrix, fill_empty=True)
-            X_pooled = pooling(X_all, indices)
-            if self.transformation_rate <= 1.0:
-                X_pooled *= self.transformation_rate
-                X_pooled += X_all * (1.0 - self.transformation_rate)
-            result = extract_chunks(X_pooled, [X.shape[0] for X in datasets])
-
-        if self.jitter_std > 0:
-            for X in result:
-                X = perturbate(X, std=self.jitter_std)
-
-        return result
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+
+from typing import List
+
+from ..transformation import Transformation
+from ....utils.matrix import pooling, extract_chunks, sort_sparse_matrix, perturbate
+from ....utils.graph import nearest_neighbors, nearest_neighbors_custom
+
+
+class Pooling(Transformation):
+    """
+    Replaces each sample by the average of its neighbors. This
+    is a useful to smooth data manifolds, and reduce the impact
+    of outliers or artifacts. It can also be used after a merging
+    to smooth the result, by toggling per_dataset parameter.
+
+    Parameters
+    ----------
+    n_neighbors: int, default = 5
+        Number of neighhbors to use for the pooling. The higher,
+        the smoother data is.
+
+    jitter_std: float, default = 0.01
+        If > 0, applies a small perturbation at the end of pooling of
+        standard deviation $jitter_std to unstick samples.
+
+    per_dataset: bool, default = True
+        Performs the pooling for each dataset independently. If false,
+        all datasets are concatenated (they are then expected to be
+        embedded in the same features space).
+    """
+
+    def __init__(
+        self,
+        n_neighbors: int = 5,
+        transformation_rate: float = 1.0,
+        jitter_std: float = 0.01,
+        per_dataset: bool = True,
+    ):
+        Transformation.__init__(self, "POOLING", True, transformation_rate)
+        self.n_neighbors = n_neighbors
+        self.jitter_std = jitter_std
+        self.per_dataset = per_dataset
+
+    def transform(
+        self,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+    ) -> List[np.ndarray]:
+        """
+        Applies pooling, potentially partial.
+        """
+        if self.per_dataset:
+            result = []
+            for adata, X in zip(datasets, embeddings):
+                neighbors = nearest_neighbors(
+                    adata,
+                    mode="edges",
+                    n_neighbors=self.n_neighbors,
+                )
+                indices, _ = sort_sparse_matrix(neighbors)
+                X_pooled = pooling(X, indices)
+                if self.transformation_rate <= 1.0:
+                    X_pooled *= self.transformation_rate
+                    X_pooled += X * (1.0 - self.transformation_rate)
+                result.append(X_pooled)
+        else:
+            X_all = np.concatenate(datasets, axis=0)
+            nn_matrix = nearest_neighbors_custom(
+                X_all,
+                "edges",
+                n_neighbors=self.n_neighbors,
+            )
+            indices, _ = sort_sparse_matrix(nn_matrix, fill_empty=True)
+            X_pooled = pooling(X_all, indices)
+            if self.transformation_rate <= 1.0:
+                X_pooled *= self.transformation_rate
+                X_pooled += X_all * (1.0 - self.transformation_rate)
+            result = extract_chunks(X_pooled, [X.shape[0] for X in datasets])
+
+        if self.jitter_std > 0:
+            for X in result:
+                X = perturbate(X, std=self.jitter_std)
+
+        return result
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/transforming/algorithms/standardize.py` & `transmorph-0.2.7/src/transmorph/engine/transforming/algorithms/standardize.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import numpy as np
-
-from typing import List
-
-from ..transformation import Transformation
-from ....utils.matrix import center_matrix, scale_matrix
-
-
-class Standardize(Transformation):
-    """
-    Centers (substracts mean) and scales (divides by STD) datasets.
-
-    Parameters
-    ----------
-    center: bool, default = True
-        Applies the centering.
-
-    scale: bool, default = True
-        Applies the scaling.
-    """
-
-    def __init__(self, center: bool = True, scale: bool = True):
-        Transformation.__init__(
-            self, str_identifier="STANDARDIZE", preserves_space=True
-        )
-        self.center = center
-        self.scale = scale
-
-    def transform(
-        self,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-    ) -> List[np.ndarray]:
-        results = []
-        for X in embeddings:
-            X = X.copy()
-            if self.center:
-                X = center_matrix(X, axis=0)
-            if self.scale:
-                X = scale_matrix(X, axis=0)
-            results.append(X)
-        return results
+#!/usr/bin/env python3
+
+import anndata as ad
+import numpy as np
+
+from typing import List
+
+from ..transformation import Transformation
+from ....utils.matrix import center_matrix, scale_matrix
+
+
+class Standardize(Transformation):
+    """
+    Centers (substracts mean) and scales (divides by STD) datasets.
+
+    Parameters
+    ----------
+    center: bool, default = True
+        Applies the centering.
+
+    scale: bool, default = True
+        Applies the scaling.
+    """
+
+    def __init__(self, center: bool = True, scale: bool = True):
+        Transformation.__init__(
+            self, str_identifier="STANDARDIZE", preserves_space=True
+        )
+        self.center = center
+        self.scale = scale
+
+    def transform(
+        self,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+    ) -> List[np.ndarray]:
+        results = []
+        for X in embeddings:
+            X = X.copy()
+            if self.center:
+                X = center_matrix(X, axis=0)
+            if self.scale:
+                X = scale_matrix(X, axis=0)
+            results.append(X)
+        return results
```

### Comparing `transmorph-0.2.6b0/src/transmorph/engine/transforming/transformation.py` & `transmorph-0.2.7/src/transmorph/engine/transforming/transformation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-import anndata as ad
-import numpy as np
-
-from abc import ABC, abstractmethod
-from numpy import testing
-from typing import List
-
-from ..traits.canlog import CanLog
-from ..traits.isprofilable import IsProfilable
-from ...utils.misc import assert_type
-
-
-class Transformation(ABC, CanLog, IsProfilable):
-    """
-    Abstract class for Preprocessing objects. Implements a method
-    transform(List[np.ndarray]) that computes the preprocessing.
-    Child classes can be enriched by traits.
-    """
-
-    def __init__(
-        self,
-        str_identifier: str = "DEFAULT",
-        preserves_space: bool = False,
-        transformation_rate: float = 1.0,
-    ):
-        CanLog.__init__(self, str_identifier=f"TRANSFORMATION_{str_identifier}")
-        self.preserves_space = preserves_space
-        if transformation_rate != 1.0:
-            assert self.preserves_space, (
-                "Partial transformations are only allowed for "
-                "space-preserving transformations."
-            )
-        assert (
-            0.0 <= transformation_rate <= 1.0
-        ), f"Partial rate must be between 0.0 and 1.0, found {transformation_rate}."
-        self.transformation_rate = transformation_rate
-
-    def check_input(self, datasets: List[np.ndarray]) -> None:
-        """
-        Can be implemented to perform checks on datasets, and raise warnings
-        or exceptions in case of issues.
-        """
-        pass
-
-    @abstractmethod
-    def transform(
-        self,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-    ) -> List[np.ndarray]:
-        """
-        Takes a list of representations as input, and returns a list of
-        representations as output in the same order. Retrieved metadata
-        can be used in this step.
-        """
-        pass
-
-    @staticmethod
-    def assert_transform_equals(
-        transformation: Transformation,
-        datasets: List[ad.AnnData],
-        embeddings: List[np.ndarray],
-        targets: List[np.ndarray],
-        decimal: float = 6.0,
-        print_debug: bool = False,
-    ) -> None:
-        """
-        For testing purposes, checks if a Transformation works as
-        expected.
-
-        Parameters
-        ----------
-        transformation: Transformation
-            Transformation to test.
-
-        datasets: List[np.ndrray]
-            List of testing matrices
-
-        targets: List[np.ndarray]
-            List of expected values
-
-        decimal: float, default = 6
-            Number of decimals to use for assert_array_almost_equal
-
-        print_debug: bool, default = False
-            Prints additional debug information in console.
-        """
-        if print_debug:
-            print(f"> transformation: {transformation}")
-            print(f"> n_datasets: {len(datasets)}")
-            print(f"> n_targets: {len(targets)}")
-            print(f"> decimal: {decimal}")
-        assert_type(transformation, Transformation)
-        # To ensure transform does not change initial matrices
-        initial_Xs = [X.copy() for X in embeddings]
-        transformed_Xs = transformation.transform(
-            datasets=datasets,
-            embeddings=initial_Xs,
-        )
-        for X_tra, X_tar in zip(transformed_Xs, targets):
-            # Transformed are correct
-            if print_debug:
-                print(f"> X transform: {type(X_tra)}, {X_tra.shape}, {X_tra.dtype}")
-                print(f"> X target: {type(X_tar)}, {X_tar.shape}, {X_tar.dtype}")
-            testing.assert_array_almost_equal(X_tra, X_tar, decimal=decimal)
-        for X_ini, X_dat in zip(initial_Xs, embeddings):
-            # Initial datasets unchanged
-            testing.assert_array_equal(X_ini, X_dat)
-            if print_debug:
-                print(f"> X initial: {type(X_ini)}, {X_ini.shape}, {X_ini.dtype}")
-                print(f"> X final: {type(X_dat)}, {X_dat.shape}, {X_dat.dtype}")
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+import anndata as ad
+import numpy as np
+
+from abc import ABC, abstractmethod
+from numpy import testing
+from typing import List
+
+from ..traits.canlog import CanLog
+from ..traits.isprofilable import IsProfilable
+from ...utils.misc import assert_type
+
+
+class Transformation(ABC, CanLog, IsProfilable):
+    """
+    Abstract class for Preprocessing objects. Implements a method
+    transform(List[np.ndarray]) that computes the preprocessing.
+    Child classes can be enriched by traits.
+    """
+
+    def __init__(
+        self,
+        str_identifier: str = "DEFAULT",
+        preserves_space: bool = False,
+        transformation_rate: float = 1.0,
+    ):
+        CanLog.__init__(self, str_identifier=f"TRANSFORMATION_{str_identifier}")
+        self.preserves_space = preserves_space
+        if transformation_rate != 1.0:
+            assert self.preserves_space, (
+                "Partial transformations are only allowed for "
+                "space-preserving transformations."
+            )
+        assert (
+            0.0 <= transformation_rate <= 1.0
+        ), f"Partial rate must be between 0.0 and 1.0, found {transformation_rate}."
+        self.transformation_rate = transformation_rate
+
+    def check_input(self, datasets: List[np.ndarray]) -> None:
+        """
+        Can be implemented to perform checks on datasets, and raise warnings
+        or exceptions in case of issues.
+        """
+        pass
+
+    @abstractmethod
+    def transform(
+        self,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+    ) -> List[np.ndarray]:
+        """
+        Takes a list of representations as input, and returns a list of
+        representations as output in the same order. Retrieved metadata
+        can be used in this step.
+        """
+        pass
+
+    @staticmethod
+    def assert_transform_equals(
+        transformation: Transformation,
+        datasets: List[ad.AnnData],
+        embeddings: List[np.ndarray],
+        targets: List[np.ndarray],
+        decimal: float = 6.0,
+        print_debug: bool = False,
+    ) -> None:
+        """
+        For testing purposes, checks if a Transformation works as
+        expected.
+
+        Parameters
+        ----------
+        transformation: Transformation
+            Transformation to test.
+
+        datasets: List[np.ndrray]
+            List of testing matrices
+
+        targets: List[np.ndarray]
+            List of expected values
+
+        decimal: float, default = 6
+            Number of decimals to use for assert_array_almost_equal
+
+        print_debug: bool, default = False
+            Prints additional debug information in console.
+        """
+        if print_debug:
+            print(f"> transformation: {transformation}")
+            print(f"> n_datasets: {len(datasets)}")
+            print(f"> n_targets: {len(targets)}")
+            print(f"> decimal: {decimal}")
+        assert_type(transformation, Transformation)
+        # To ensure transform does not change initial matrices
+        initial_Xs = [X.copy() for X in embeddings]
+        transformed_Xs = transformation.transform(
+            datasets=datasets,
+            embeddings=initial_Xs,
+        )
+        for X_tra, X_tar in zip(transformed_Xs, targets):
+            # Transformed are correct
+            if print_debug:
+                print(f"> X transform: {type(X_tra)}, {X_tra.shape}, {X_tra.dtype}")
+                print(f"> X target: {type(X_tar)}, {X_tar.shape}, {X_tar.dtype}")
+            testing.assert_array_almost_equal(X_tra, X_tar, decimal=decimal)
+        for X_ini, X_dat in zip(initial_Xs, embeddings):
+            # Initial datasets unchanged
+            testing.assert_array_equal(X_ini, X_dat)
+            if print_debug:
+                print(f"> X initial: {type(X_ini)}, {X_ini.shape}, {X_ini.dtype}")
+                print(f"> X final: {type(X_dat)}, {X_dat.shape}, {X_dat.dtype}")
```

### Comparing `transmorph-0.2.6b0/src/transmorph/models/embedmnn.py` & `transmorph-0.2.7/src/transmorph/models/embedmnn.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Dict, List, Literal, Optional
-
-from transmorph.engine import Model
-from transmorph.engine.layers import (
-    LayerInput,
-    LayerTransformation,
-    LayerMatching,
-    LayerMerging,
-    LayerOutput,
-)
-from transmorph.engine.matching import BKNN, MNN
-from transmorph.engine.merging import GraphEmbedding
-from transmorph.engine.transforming import CommonFeatures, PCA
-
-
-class EmbedMNN(Model):
-    """
-    This model performs preprocessing steps, then carries out mutual nearest
-    neighbors (MNN) between pairs of datasets. It eventually embeds a combination
-    of datasets kNN graphs and pairwise MNN graphs into a low dimensional space,
-    in which further analyzes such as clustering can be carried out.
-
-    Parameters
-    ----------
-    matching: Literal["mnn", "bknn"], default = "bknn"
-        Nearest neighbors matching to use, either Mutual Nearest Neighbors
-        (MNN) or Batch k-Nearest Neighbors (BKNN). For a given number of
-        neighbors $k$, here is the subtlety between both algorithms.
-
-        - In MNN, points $x_i$ from batch $X$ and $y_j$ from batch $Y$ are
-          matched if $x_i$ belongs to the $k$ nearest neighbors of $y_j$ in
-          $X$, and vice-versa.
-        - In BKNN, point $x_i$ is matched with point $y_j$ if $y_j$ belongs
-          to the $k$ nearest neighbors of $x_i$ in $Y$.
-
-    matching_n_neighbors: int, default = None
-        Number of neighbors to use for the mutual nearest neighbors step. If
-        None is provided, it is determined automatically.
-
-    matching_metric: str, default = "sqeuclidean"
-        Metric to use to determine nearest neighbors.
-
-    matching_metric_kwargs: Optional[Dict], default = None
-        Additional metric parameters.
-
-    obs_class: Optional[str], default = None
-        Provides the AnnData.obs key where sample type is stored. If
-        specified, matching edges between samples of different class
-        are discarded.
-
-    embedding_optimizer: Literal["umap", "mde"], default = "umap"
-        Graph embedding algorithm to use.
-
-    embedding_n_neighbors: int, default = 10
-        Target number of edges per point in the graph to embed. Only
-        this number of most significant edges are conserved. Try to
-        keep this number greater than dataset number.
-
-    embedding_dimension: int, default = 2
-        Number of dimensions in the final embedding.
-
-    pca_n_components: int, default = 30
-        Number of principal components to use if data dimensionality is
-        greater.
-
-    verbose: bool, default = True
-        Logs information in console.
-
-    Example
-    -------
-    >>> from transmorph.datasets import load_zhou_10x
-    >>> from transmorph.models import EmbedMNN
-    >>> model = EmbedMNN()
-    >>> dataset = load_zhou_10x()
-    >>> model.fit(datasets)
-    """
-
-    def __init__(
-        self,
-        matching: Literal["mnn", "bknn"] = "bknn",
-        matching_n_neighbors: Optional[int] = None,
-        matching_metric: str = "sqeuclidean",
-        matching_metric_kwargs: Optional[Dict] = None,
-        obs_class: Optional[str] = None,
-        embedding_n_neighbors: int = 10,
-        embedding_optimizer: Literal["umap", "mde"] = "umap",
-        pca_n_components: int = 30,
-        embedding_dimension: int = 2,
-        verbose: bool = True,
-    ):
-        from .. import settings
-
-        if verbose:
-            settings.verbose = "INFO"
-        else:
-            settings.verbose = "WARNING"
-
-        # Loading algorithms
-        preprocessings = [
-            CommonFeatures(),
-            PCA(n_components=pca_n_components, strategy="concatenate"),
-        ]
-
-        if matching == "mnn":
-            if matching_n_neighbors is None:
-                matching_n_neighbors = 30
-            matching_alg = MNN(
-                metric=matching_metric,
-                metric_kwargs=matching_metric_kwargs,
-                n_neighbors=matching_n_neighbors,
-                common_features_mode="total",
-                solver="auto",
-            )
-        elif matching == "bknn":
-            if matching_n_neighbors is None:
-                matching_n_neighbors = 10
-            matching_alg = BKNN(
-                metric=matching_metric,
-                metric_kwargs=matching_metric_kwargs,
-                n_neighbors=matching_n_neighbors,
-                common_features_mode="total",
-            )
-        else:
-            raise ValueError(
-                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
-            )
-
-        merging = GraphEmbedding(
-            optimizer=embedding_optimizer,
-            n_neighbors=embedding_n_neighbors,
-            embedding_dimension=embedding_dimension,
-            symmetrize_edges=True,
-        )
-
-        # Building model
-        linput = LayerInput()
-        ltransform = LayerTransformation()
-        for transformation in preprocessings:
-            ltransform.add_transformation(transformation=transformation)
-        lmatching = LayerMatching(
-            matching=matching_alg,
-            obs_class=obs_class,
-        )
-        lmerging = LayerMerging(merging=merging)
-        loutput = LayerOutput()
-        linput.connect(ltransform)
-        ltransform.connect(lmatching)
-        lmatching.connect(lmerging)
-        lmerging.connect(loutput)
-
-        Model.__init__(self, input_layer=linput, str_identifier="EMBED_MNN")
-
-    def transform(
-        self,
-        datasets: List[AnnData],
-        use_representation: Optional[str] = None,
-        output_representation: Optional[str] = None,
-    ) -> None:
-        """
-        Carries out the model on a list of AnnData objects. Writes the result in
-        .obsm fields.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of anndata objects, must have at least one common feature.
-
-        use_representation: Optional[str]
-            .obsm to use as input.
-
-        output_representation: str
-            .obsm destination key, "transmorph" by default.
-        """
-        self.fit(
-            datasets=datasets,
-            reference=None,
-            use_representation=use_representation,
-            output_representation=output_representation,
-        )
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Dict, List, Literal, Optional
+
+from transmorph.engine import Model
+from transmorph.engine.layers import (
+    LayerInput,
+    LayerTransformation,
+    LayerMatching,
+    LayerMerging,
+    LayerOutput,
+)
+from transmorph.engine.matching import BKNN, MNN
+from transmorph.engine.merging import GraphEmbedding
+from transmorph.engine.transforming import CommonFeatures, PCA
+
+
+class EmbedMNN(Model):
+    """
+    This model performs preprocessing steps, then carries out mutual nearest
+    neighbors (MNN) between pairs of datasets. It eventually embeds a combination
+    of datasets kNN graphs and pairwise MNN graphs into a low dimensional space,
+    in which further analyzes such as clustering can be carried out.
+
+    Parameters
+    ----------
+    matching: Literal["mnn", "bknn"], default = "bknn"
+        Nearest neighbors matching to use, either Mutual Nearest Neighbors
+        (MNN) or Batch k-Nearest Neighbors (BKNN). For a given number of
+        neighbors $k$, here is the subtlety between both algorithms.
+
+        - In MNN, points $x_i$ from batch $X$ and $y_j$ from batch $Y$ are
+          matched if $x_i$ belongs to the $k$ nearest neighbors of $y_j$ in
+          $X$, and vice-versa.
+        - In BKNN, point $x_i$ is matched with point $y_j$ if $y_j$ belongs
+          to the $k$ nearest neighbors of $x_i$ in $Y$.
+
+    matching_n_neighbors: int, default = None
+        Number of neighbors to use for the mutual nearest neighbors step. If
+        None is provided, it is determined automatically.
+
+    matching_metric: str, default = "sqeuclidean"
+        Metric to use to determine nearest neighbors.
+
+    matching_metric_kwargs: Optional[Dict], default = None
+        Additional metric parameters.
+
+    obs_class: Optional[str], default = None
+        Provides the AnnData.obs key where sample type is stored. If
+        specified, matching edges between samples of different class
+        are discarded.
+
+    embedding_optimizer: Literal["umap", "mde"], default = "umap"
+        Graph embedding algorithm to use.
+
+    embedding_n_neighbors: int, default = 10
+        Target number of edges per point in the graph to embed. Only
+        this number of most significant edges are conserved. Try to
+        keep this number greater than dataset number.
+
+    embedding_dimension: int, default = 2
+        Number of dimensions in the final embedding.
+
+    pca_n_components: int, default = 30
+        Number of principal components to use if data dimensionality is
+        greater.
+
+    verbose: bool, default = True
+        Logs information in console.
+
+    Example
+    -------
+    >>> from transmorph.datasets import load_zhou_10x
+    >>> from transmorph.models import EmbedMNN
+    >>> model = EmbedMNN()
+    >>> dataset = load_zhou_10x()
+    >>> model.fit(datasets)
+    """
+
+    def __init__(
+        self,
+        matching: Literal["mnn", "bknn"] = "bknn",
+        matching_n_neighbors: Optional[int] = None,
+        matching_metric: str = "sqeuclidean",
+        matching_metric_kwargs: Optional[Dict] = None,
+        obs_class: Optional[str] = None,
+        embedding_n_neighbors: int = 10,
+        embedding_optimizer: Literal["umap", "mde"] = "umap",
+        pca_n_components: int = 30,
+        embedding_dimension: int = 2,
+        verbose: bool = True,
+    ):
+        from .. import settings
+
+        if verbose:
+            settings.verbose = "INFO"
+        else:
+            settings.verbose = "WARNING"
+
+        # Loading algorithms
+        preprocessings = [
+            CommonFeatures(),
+            PCA(n_components=pca_n_components, strategy="concatenate"),
+        ]
+
+        if matching == "mnn":
+            if matching_n_neighbors is None:
+                matching_n_neighbors = 30
+            matching_alg = MNN(
+                metric=matching_metric,
+                metric_kwargs=matching_metric_kwargs,
+                n_neighbors=matching_n_neighbors,
+                common_features_mode="total",
+                solver="auto",
+            )
+        elif matching == "bknn":
+            if matching_n_neighbors is None:
+                matching_n_neighbors = 10
+            matching_alg = BKNN(
+                metric=matching_metric,
+                metric_kwargs=matching_metric_kwargs,
+                n_neighbors=matching_n_neighbors,
+                common_features_mode="total",
+            )
+        else:
+            raise ValueError(
+                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
+            )
+
+        merging = GraphEmbedding(
+            optimizer=embedding_optimizer,
+            n_neighbors=embedding_n_neighbors,
+            embedding_dimension=embedding_dimension,
+            symmetrize_edges=True,
+        )
+
+        # Building model
+        linput = LayerInput()
+        ltransform = LayerTransformation()
+        for transformation in preprocessings:
+            ltransform.add_transformation(transformation=transformation)
+        lmatching = LayerMatching(
+            matching=matching_alg,
+            obs_class=obs_class,
+        )
+        lmerging = LayerMerging(merging=merging)
+        loutput = LayerOutput()
+        linput.connect(ltransform)
+        ltransform.connect(lmatching)
+        lmatching.connect(lmerging)
+        lmerging.connect(loutput)
+
+        Model.__init__(self, input_layer=linput, str_identifier="EMBED_MNN")
+
+    def transform(
+        self,
+        datasets: List[AnnData],
+        use_representation: Optional[str] = None,
+        output_representation: Optional[str] = None,
+    ) -> None:
+        """
+        Carries out the model on a list of AnnData objects. Writes the result in
+        .obsm fields.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of anndata objects, must have at least one common feature.
+
+        use_representation: Optional[str]
+            .obsm to use as input.
+
+        output_representation: str
+            .obsm destination key, "transmorph" by default.
+        """
+        self.fit(
+            datasets=datasets,
+            reference=None,
+            use_representation=use_representation,
+            output_representation=output_representation,
+        )
```

### Comparing `transmorph-0.2.6b0/src/transmorph/models/mnncorrection.py` & `transmorph-0.2.7/src/transmorph/models/mnncorrection.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Dict, List, Literal, Optional
-
-from transmorph.engine import Model
-from transmorph.engine.layers import (
-    LayerInput,
-    LayerTransformation,
-    LayerMatching,
-    LayerMerging,
-    LayerOutput,
-)
-from transmorph.engine.matching import BKNN, MNN
-from transmorph.engine.merging import LinearCorrection
-from transmorph.engine.transforming import CommonFeatures, PCA
-from transmorph.utils.anndata_manager import get_total_feature_slices
-
-
-class MNNCorrection(Model):
-    """
-    This model performs preprocessing steps, then carries out mutual nearest
-    neighbors (MNN) between pairs of datasets. It then corrects every dataset
-    with respect to a reference dataset chosen by the user.
-
-    Parameters
-    ----------
-    matching: Literal["mnn", "bknn"], default = "bknn"
-        Nearest neighbors matching to use, either Mutual Nearest Neighbors
-        (MNN) or Batch k-Nearest Neighbors (BKNN). For a given number of
-        neighbors $k$, here is the subtlety between both algorithms.
-
-        - In MNN, points $x_i$ from batch $X$ and $y_j$ from batch $Y$ are
-          matched if $x_i$ belongs to the $k$ nearest neighbors of $y_j$ in
-          $X$, and vice-versa.
-        - In BKNN, point $x_i$ is matched with point $y_j$ if $y_j$ belongs
-          to the $k$ nearest neighbors of $x_i$ in $Y$.
-
-    matching_n_neighbors: int, default = None
-        Number of neighbors to use for the mutual nearest neighbors step. If
-        None is provided, it is determined automatically.
-
-    matching_metric: str, default = "sqeuclidean"
-        Metric to use to determine nearest neighbors.
-
-    matching_metric_kwargs: Optional[Dict], default = None
-        Additional metric parameters.
-
-    obs_class: Optional[str], default = None
-        Provides the AnnData.obs key where sample type is stored. If
-        specified, matching edges between samples of different class
-        are discarded.
-
-    n_components: int, default = 30
-        Number of principal components to use if data dimensionality is
-        greater.
-
-    lc_n_neighbors: int, default = 10
-        Number of neighbors to use for linear correction neighbors graph.
-
-    use_feature_space: bool, default = True
-        Performs correction in datasets feature space rather than in PC space.
-
-    verbose: bool, default = True
-        Logs information in console.
-
-    Example
-    -------
-    >>> from transmorph.datasets import load_chen_10x
-    >>> from transmorph.models import MNNCorrection
-    >>> model = MNNCorrection()
-    >>> dataset = load_chen_10x()
-    >>> model.fit(datasets, reference=dataset['P01'])
-    """
-
-    def __init__(
-        self,
-        matching: Literal["mnn", "bknn"] = "bknn",
-        matching_n_neighbors: Optional[int] = None,
-        matching_metric: str = "sqeuclidean",
-        matching_metric_kwargs: Optional[Dict] = None,
-        obs_class: Optional[str] = None,
-        n_components: int = 30,
-        lc_n_neighbors: int = 10,
-        use_feature_space: bool = True,
-        verbose: bool = True,
-    ) -> None:
-        from .. import settings
-
-        if verbose:
-            settings.verbose = "INFO"
-        else:
-            settings.verbose = "WARNING"
-
-        # Loading algorithms
-        if matching == "mnn":
-            if matching_n_neighbors is None:
-                matching_n_neighbors = 30
-            matching_alg = MNN(
-                metric=matching_metric,
-                metric_kwargs=matching_metric_kwargs,
-                n_neighbors=matching_n_neighbors,
-                common_features_mode="total",
-            )
-        elif matching == "bknn":
-            if matching_n_neighbors is None:
-                matching_n_neighbors = 10
-            matching_alg = BKNN(
-                metric=matching_metric,
-                metric_kwargs=matching_metric_kwargs,
-                n_neighbors=matching_n_neighbors,
-                common_features_mode="total",
-            )
-        else:
-            raise ValueError(
-                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
-            )
-        merging = LinearCorrection(n_neighbors=lc_n_neighbors)
-
-        # Initializing layers
-        linput = LayerInput()
-
-        ltransform_features = LayerTransformation()
-        ltransform_features.add_transformation(CommonFeatures())
-
-        ltransform_dimred = LayerTransformation()
-        ltransform_dimred.add_transformation(PCA(n_components=n_components))
-
-        lmatching = LayerMatching(matching=matching_alg, obs_class=obs_class)
-
-        lmerging = LayerMerging(merging=merging)
-
-        loutput = LayerOutput()
-
-        # Building model
-        linput.connect(ltransform_features)
-        ltransform_features.connect(ltransform_dimred)
-        ltransform_dimred.connect(lmatching)
-        lmatching.connect(lmerging)
-
-        lmerging.connect(loutput)
-
-        self.use_feature_space = use_feature_space
-        if use_feature_space:
-            lmerging.embedding_reference = ltransform_features
-        else:
-            lmerging.embedding_reference = ltransform_dimred
-
-        Model.__init__(self, input_layer=linput, str_identifier="MNN_CORRECTION")
-
-    def transform(
-        self,
-        datasets: List[AnnData],
-        reference: AnnData,
-        use_representation: Optional[str] = None,
-        output_representation: Optional[str] = None,
-    ) -> None:
-        """
-        Carries out the model on a list of AnnData objects. Writes the result in
-        .obsm fields.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of anndata objects, must have at least one common feature.
-
-        reference: AnnData
-            Reference dataset for the correction.
-
-        use_representation: Optional[str]
-            .obsm to use as input.
-
-        output_representation: str
-            .obsm destination key, "transmorph" by default.
-        """
-        if isinstance(datasets, Dict):
-            datasets = list(datasets.values())
-        self.fit(
-            datasets,
-            reference=reference,
-            use_representation=use_representation,
-            output_representation=output_representation,
-        )
-        if self.use_feature_space:
-            self.embedding_features = datasets[0].var_names[
-                get_total_feature_slices(datasets)[0]
-            ]
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Dict, List, Literal, Optional
+
+from transmorph.engine import Model
+from transmorph.engine.layers import (
+    LayerInput,
+    LayerTransformation,
+    LayerMatching,
+    LayerMerging,
+    LayerOutput,
+)
+from transmorph.engine.matching import BKNN, MNN
+from transmorph.engine.merging import LinearCorrection
+from transmorph.engine.transforming import CommonFeatures, PCA
+from transmorph.utils.anndata_manager import get_total_feature_slices
+
+
+class MNNCorrection(Model):
+    """
+    This model performs preprocessing steps, then carries out mutual nearest
+    neighbors (MNN) between pairs of datasets. It then corrects every dataset
+    with respect to a reference dataset chosen by the user.
+
+    Parameters
+    ----------
+    matching: Literal["mnn", "bknn"], default = "bknn"
+        Nearest neighbors matching to use, either Mutual Nearest Neighbors
+        (MNN) or Batch k-Nearest Neighbors (BKNN). For a given number of
+        neighbors $k$, here is the subtlety between both algorithms.
+
+        - In MNN, points $x_i$ from batch $X$ and $y_j$ from batch $Y$ are
+          matched if $x_i$ belongs to the $k$ nearest neighbors of $y_j$ in
+          $X$, and vice-versa.
+        - In BKNN, point $x_i$ is matched with point $y_j$ if $y_j$ belongs
+          to the $k$ nearest neighbors of $x_i$ in $Y$.
+
+    matching_n_neighbors: int, default = None
+        Number of neighbors to use for the mutual nearest neighbors step. If
+        None is provided, it is determined automatically.
+
+    matching_metric: str, default = "sqeuclidean"
+        Metric to use to determine nearest neighbors.
+
+    matching_metric_kwargs: Optional[Dict], default = None
+        Additional metric parameters.
+
+    obs_class: Optional[str], default = None
+        Provides the AnnData.obs key where sample type is stored. If
+        specified, matching edges between samples of different class
+        are discarded.
+
+    n_components: int, default = 30
+        Number of principal components to use if data dimensionality is
+        greater.
+
+    lc_n_neighbors: int, default = 10
+        Number of neighbors to use for linear correction neighbors graph.
+
+    use_feature_space: bool, default = True
+        Performs correction in datasets feature space rather than in PC space.
+
+    verbose: bool, default = True
+        Logs information in console.
+
+    Example
+    -------
+    >>> from transmorph.datasets import load_chen_10x
+    >>> from transmorph.models import MNNCorrection
+    >>> model = MNNCorrection()
+    >>> dataset = load_chen_10x()
+    >>> model.fit(datasets, reference=dataset['P01'])
+    """
+
+    def __init__(
+        self,
+        matching: Literal["mnn", "bknn"] = "bknn",
+        matching_n_neighbors: Optional[int] = None,
+        matching_metric: str = "sqeuclidean",
+        matching_metric_kwargs: Optional[Dict] = None,
+        obs_class: Optional[str] = None,
+        n_components: int = 30,
+        lc_n_neighbors: int = 10,
+        use_feature_space: bool = True,
+        verbose: bool = True,
+    ) -> None:
+        from .. import settings
+
+        if verbose:
+            settings.verbose = "INFO"
+        else:
+            settings.verbose = "WARNING"
+
+        # Loading algorithms
+        if matching == "mnn":
+            if matching_n_neighbors is None:
+                matching_n_neighbors = 30
+            matching_alg = MNN(
+                metric=matching_metric,
+                metric_kwargs=matching_metric_kwargs,
+                n_neighbors=matching_n_neighbors,
+                common_features_mode="total",
+            )
+        elif matching == "bknn":
+            if matching_n_neighbors is None:
+                matching_n_neighbors = 10
+            matching_alg = BKNN(
+                metric=matching_metric,
+                metric_kwargs=matching_metric_kwargs,
+                n_neighbors=matching_n_neighbors,
+                common_features_mode="total",
+            )
+        else:
+            raise ValueError(
+                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
+            )
+        merging = LinearCorrection(n_neighbors=lc_n_neighbors)
+
+        # Initializing layers
+        linput = LayerInput()
+
+        ltransform_features = LayerTransformation()
+        ltransform_features.add_transformation(CommonFeatures())
+
+        ltransform_dimred = LayerTransformation()
+        ltransform_dimred.add_transformation(PCA(n_components=n_components))
+
+        lmatching = LayerMatching(matching=matching_alg, obs_class=obs_class)
+
+        lmerging = LayerMerging(merging=merging)
+
+        loutput = LayerOutput()
+
+        # Building model
+        linput.connect(ltransform_features)
+        ltransform_features.connect(ltransform_dimred)
+        ltransform_dimred.connect(lmatching)
+        lmatching.connect(lmerging)
+
+        lmerging.connect(loutput)
+
+        self.use_feature_space = use_feature_space
+        if use_feature_space:
+            lmerging.embedding_reference = ltransform_features
+        else:
+            lmerging.embedding_reference = ltransform_dimred
+
+        Model.__init__(self, input_layer=linput, str_identifier="MNN_CORRECTION")
+
+    def transform(
+        self,
+        datasets: List[AnnData],
+        reference: AnnData,
+        use_representation: Optional[str] = None,
+        output_representation: Optional[str] = None,
+    ) -> None:
+        """
+        Carries out the model on a list of AnnData objects. Writes the result in
+        .obsm fields.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of anndata objects, must have at least one common feature.
+
+        reference: AnnData
+            Reference dataset for the correction.
+
+        use_representation: Optional[str]
+            .obsm to use as input.
+
+        output_representation: str
+            .obsm destination key, "transmorph" by default.
+        """
+        if isinstance(datasets, Dict):
+            datasets = list(datasets.values())
+        self.fit(
+            datasets,
+            reference=reference,
+            use_representation=use_representation,
+            output_representation=output_representation,
+        )
+        if self.use_feature_space:
+            self.embedding_features = datasets[0].var_names[
+                get_total_feature_slices(datasets)[0]
+            ]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/models/transportcorrection.py` & `transmorph-0.2.7/src/transmorph/models/transportcorrection.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-#!/usr/bin/env python3
-
-from anndata import AnnData
-from typing import Dict, List, Literal, Optional
-
-from transmorph.engine import Model
-from transmorph.engine.layers import (
-    LayerInput,
-    LayerTransformation,
-    LayerMatching,
-    LayerMerging,
-    LayerOutput,
-)
-from transmorph.engine.matching import OT, GW
-from transmorph.engine.merging import Barycenter
-from transmorph.engine.transforming import CommonFeatures, PCA
-from transmorph.utils.anndata_manager import get_total_feature_slices
-
-
-class TransportCorrection(Model):
-    """
-    This model performs preprocessing steps, then carries out optimal transport
-    between pairs of datasets. It then correctes every dataset with respect to
-    a reference dataset chosen by the user using barycentric embedding.
-
-    Parameters
-    ----------
-    matching: Literal["ot", "gromov"], default = "ot"
-        Transportation framework to use, either Optimal Transport (OT) or
-        Gromov-Wasserstein (GW). Optimal transport requires batches to be
-        embedded in the same space, while Gromov-Wasserstein can work with
-        batches embedded in different space at the cost of weaker constraints.
-
-    solver: Literal["exact", "entropic", "unbalanced"], default = "exact"
-        Optimization problem formulation.
-
-        - "exact" is available for both OT and Gromov-Wasserstein, and attempts
-          to solve exactly the optimization problem. It can scale poorly to large
-          datasets (with several tens of thousands of points).
-        - "entropic" is available for both OT and Gromov-Wasserstein, and uses
-          en entropic regularizer term to be able to use a convex solver. The solution
-          is approximate.
-        - "unbalanced" is available for OT only, and uses the unbalanced OT formulation
-          to deal with datasets with unbalanced class proportions.
-
-    entropy_epsilon: Optional[float], default = None
-        If solver is "entropy", allows to tweak the entropy term strength.
-
-    unbalanced_reg: Optional[float]
-        Mass conservation regularizer to use in the unbalanced optimal
-        transport formulation. The higher, the closer result is from
-        constrained optimal transport. The lower, the better the matching
-        will be dealing with unbalanced datasets, but convergence will be
-        harder. Will be set to 1e-1 by default.
-
-    matching_metric: str, default = "sqeuclidean"
-        Metric to use to determine nearest neighbors.
-
-    matching_metric_kwargs: Optional[Dict], default = None
-        Additional metric parameters.
-
-    obs_class: Optional[str], default = None
-        Provides the AnnData.obs key where sample type is stored. If
-        specified, matching edges between samples of different class
-        are discarded.
-
-    n_components: int, default = 30
-        Number of principal components to use if data dimensionality is
-        greater.
-
-    use_feature_space: bool, default = True
-        Performs correction in datasets feature space rather than in PC space.
-
-    verbose: bool, default = True
-        Logs information in console.
-
-    Example
-    -------
-    >>> from transmorph.datasets import load_chen_10x
-    >>> from transmorph.models import TransportCorrection
-    >>> model = TransportCorrection()
-    >>> dataset = load_chen_10x()
-    >>> model.fit(datasets, reference=dataset['P01'])
-    """
-
-    def __init__(
-        self,
-        matching: Literal["ot", "gromov"] = "ot",
-        solver: Literal["exact", "entropic", "partial", "unbalanced"] = "exact",
-        entropy_epsilon: Optional[float] = None,
-        unbalanced_reg: Optional[float] = None,
-        matching_metric: str = "sqeuclidean",
-        matching_metric_kwargs: Optional[Dict] = None,
-        obs_class: Optional[str] = None,
-        n_components: int = 30,
-        use_feature_space: bool = False,
-        verbose: bool = True,
-    ) -> None:
-        from .. import settings
-
-        if verbose:
-            settings.verbose = "INFO"
-        else:
-            settings.verbose = "WARNING"
-
-        # Loading algorithms
-        if matching == "ot":
-            if solver == "exact":
-                solver_ot = "emd"
-            elif solver == "entropic":
-                solver_ot = "sinkhorn"
-            else:
-                solver_ot = "unbalanced"
-            matching_alg = OT(
-                solver=solver_ot,
-                metric=matching_metric,
-                metric_kwargs=matching_metric_kwargs,
-                common_features_mode="total",
-                sinkhorn_reg=entropy_epsilon,
-                unbalanced_reg=unbalanced_reg,
-            )
-        elif matching == "gromov":
-            if solver == "exact":
-                solver_gw = "gw"
-            elif solver == "entropic":
-                solver_gw = "entropic_gw"
-            else:
-                raise ValueError(f"Solver {solver} not found for GW matching.")
-            matching_alg = GW(
-                optimizer=solver_gw,
-                default_metric=matching_metric,
-                default_metric_kwargs=matching_metric_kwargs,
-                GW_loss="square_loss",
-                entropy_epsilon=entropy_epsilon,
-            )
-        else:
-            raise ValueError(
-                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
-            )
-        merging = Barycenter()
-
-        # Initializing layers
-        linput = LayerInput()
-
-        ltransform_features = LayerTransformation()
-        if matching == "ot":
-            ltransform_features.add_transformation(CommonFeatures())
-
-        ltransform_dimred = LayerTransformation()
-        ltransform_dimred.add_transformation(PCA(n_components=n_components))
-
-        lmatching = LayerMatching(matching=matching_alg, obs_class=obs_class)
-
-        lmerging = LayerMerging(merging=merging)
-
-        loutput = LayerOutput()
-
-        # Building model
-        linput.connect(ltransform_features)
-        ltransform_features.connect(ltransform_dimred)
-        ltransform_dimred.connect(lmatching)
-        lmatching.connect(lmerging)
-
-        lmerging.connect(loutput)
-
-        self.use_feature_space = use_feature_space
-        if use_feature_space:
-            lmerging.embedding_reference = ltransform_features
-        else:
-            lmerging.embedding_reference = ltransform_dimred
-
-        Model.__init__(self, input_layer=linput, str_identifier="MNN_CORRECTION")
-
-    def transform(
-        self,
-        datasets: List[AnnData],
-        reference: AnnData,
-        use_representation: Optional[str] = None,
-        output_representation: Optional[str] = None,
-    ) -> None:
-        """
-        Carries out the model on a list of AnnData objects. Writes the result in
-        .obsm fields.
-
-        Parameters
-        ----------
-        datasets: List[AnnData]
-            List of anndata objects, must have at least one common feature.
-
-        reference: AnnData
-            Reference dataset for the correction.
-
-        use_representation: Optional[str]
-            .obsm to use as input.
-
-        output_representation: str
-            .obsm destination key, "transmorph" by default.
-        """
-        if isinstance(datasets, Dict):
-            datasets = list(datasets.values())
-        self.fit(
-            datasets,
-            reference=reference,
-            use_representation=use_representation,
-            output_representation=output_representation,
-        )
-        if self.use_feature_space:
-            self.embedding_features = datasets[0].var_names[
-                get_total_feature_slices(datasets)[0]
-            ]
+#!/usr/bin/env python3
+
+from anndata import AnnData
+from typing import Dict, List, Literal, Optional
+
+from transmorph.engine import Model
+from transmorph.engine.layers import (
+    LayerInput,
+    LayerTransformation,
+    LayerMatching,
+    LayerMerging,
+    LayerOutput,
+)
+from transmorph.engine.matching import OT, GW
+from transmorph.engine.merging import Barycenter
+from transmorph.engine.transforming import CommonFeatures, PCA
+from transmorph.utils.anndata_manager import get_total_feature_slices
+
+
+class TransportCorrection(Model):
+    """
+    This model performs preprocessing steps, then carries out optimal transport
+    between pairs of datasets. It then correctes every dataset with respect to
+    a reference dataset chosen by the user using barycentric embedding.
+
+    Parameters
+    ----------
+    matching: Literal["ot", "gromov"], default = "ot"
+        Transportation framework to use, either Optimal Transport (OT) or
+        Gromov-Wasserstein (GW). Optimal transport requires batches to be
+        embedded in the same space, while Gromov-Wasserstein can work with
+        batches embedded in different space at the cost of weaker constraints.
+
+    solver: Literal["exact", "entropic", "unbalanced"], default = "exact"
+        Optimization problem formulation.
+
+        - "exact" is available for both OT and Gromov-Wasserstein, and attempts
+          to solve exactly the optimization problem. It can scale poorly to large
+          datasets (with several tens of thousands of points).
+        - "entropic" is available for both OT and Gromov-Wasserstein, and uses
+          en entropic regularizer term to be able to use a convex solver. The solution
+          is approximate.
+        - "unbalanced" is available for OT only, and uses the unbalanced OT formulation
+          to deal with datasets with unbalanced class proportions.
+
+    entropy_epsilon: Optional[float], default = None
+        If solver is "entropy", allows to tweak the entropy term strength.
+
+    unbalanced_reg: Optional[float]
+        Mass conservation regularizer to use in the unbalanced optimal
+        transport formulation. The higher, the closer result is from
+        constrained optimal transport. The lower, the better the matching
+        will be dealing with unbalanced datasets, but convergence will be
+        harder. Will be set to 1e-1 by default.
+
+    matching_metric: str, default = "sqeuclidean"
+        Metric to use to determine nearest neighbors.
+
+    matching_metric_kwargs: Optional[Dict], default = None
+        Additional metric parameters.
+
+    obs_class: Optional[str], default = None
+        Provides the AnnData.obs key where sample type is stored. If
+        specified, matching edges between samples of different class
+        are discarded.
+
+    n_components: int, default = 30
+        Number of principal components to use if data dimensionality is
+        greater.
+
+    use_feature_space: bool, default = True
+        Performs correction in datasets feature space rather than in PC space.
+
+    verbose: bool, default = True
+        Logs information in console.
+
+    Example
+    -------
+    >>> from transmorph.datasets import load_chen_10x
+    >>> from transmorph.models import TransportCorrection
+    >>> model = TransportCorrection()
+    >>> dataset = load_chen_10x()
+    >>> model.fit(datasets, reference=dataset['P01'])
+    """
+
+    def __init__(
+        self,
+        matching: Literal["ot", "gromov"] = "ot",
+        solver: Literal["exact", "entropic", "partial", "unbalanced"] = "exact",
+        entropy_epsilon: Optional[float] = None,
+        unbalanced_reg: Optional[float] = None,
+        matching_metric: str = "sqeuclidean",
+        matching_metric_kwargs: Optional[Dict] = None,
+        obs_class: Optional[str] = None,
+        n_components: int = 30,
+        use_feature_space: bool = False,
+        verbose: bool = True,
+    ) -> None:
+        from .. import settings
+
+        if verbose:
+            settings.verbose = "INFO"
+        else:
+            settings.verbose = "WARNING"
+
+        # Loading algorithms
+        if matching == "ot":
+            if solver == "exact":
+                solver_ot = "emd"
+            elif solver == "entropic":
+                solver_ot = "sinkhorn"
+            else:
+                solver_ot = "unbalanced"
+            matching_alg = OT(
+                solver=solver_ot,
+                metric=matching_metric,
+                metric_kwargs=matching_metric_kwargs,
+                common_features_mode="total",
+                sinkhorn_reg=entropy_epsilon,
+                unbalanced_reg=unbalanced_reg,
+            )
+        elif matching == "gromov":
+            if solver == "exact":
+                solver_gw = "gw"
+            elif solver == "entropic":
+                solver_gw = "entropic_gw"
+            else:
+                raise ValueError(f"Solver {solver} not found for GW matching.")
+            matching_alg = GW(
+                optimizer=solver_gw,
+                default_metric=matching_metric,
+                default_metric_kwargs=matching_metric_kwargs,
+                GW_loss="square_loss",
+                entropy_epsilon=entropy_epsilon,
+            )
+        else:
+            raise ValueError(
+                f"Unrecognized matching: {matching}. Expected 'mnn' or 'bknn'."
+            )
+        merging = Barycenter()
+
+        # Initializing layers
+        linput = LayerInput()
+
+        ltransform_features = LayerTransformation()
+        if matching == "ot":
+            ltransform_features.add_transformation(CommonFeatures())
+
+        ltransform_dimred = LayerTransformation()
+        ltransform_dimred.add_transformation(PCA(n_components=n_components))
+
+        lmatching = LayerMatching(matching=matching_alg, obs_class=obs_class)
+
+        lmerging = LayerMerging(merging=merging)
+
+        loutput = LayerOutput()
+
+        # Building model
+        linput.connect(ltransform_features)
+        ltransform_features.connect(ltransform_dimred)
+        ltransform_dimred.connect(lmatching)
+        lmatching.connect(lmerging)
+
+        lmerging.connect(loutput)
+
+        self.use_feature_space = use_feature_space
+        if use_feature_space:
+            lmerging.embedding_reference = ltransform_features
+        else:
+            lmerging.embedding_reference = ltransform_dimred
+
+        Model.__init__(self, input_layer=linput, str_identifier="MNN_CORRECTION")
+
+    def transform(
+        self,
+        datasets: List[AnnData],
+        reference: AnnData,
+        use_representation: Optional[str] = None,
+        output_representation: Optional[str] = None,
+    ) -> None:
+        """
+        Carries out the model on a list of AnnData objects. Writes the result in
+        .obsm fields.
+
+        Parameters
+        ----------
+        datasets: List[AnnData]
+            List of anndata objects, must have at least one common feature.
+
+        reference: AnnData
+            Reference dataset for the correction.
+
+        use_representation: Optional[str]
+            .obsm to use as input.
+
+        output_representation: str
+            .obsm destination key, "transmorph" by default.
+        """
+        if isinstance(datasets, Dict):
+            datasets = list(datasets.values())
+        self.fit(
+            datasets,
+            reference=reference,
+            use_representation=use_representation,
+            output_representation=output_representation,
+        )
+        if self.use_feature_space:
+            self.embedding_features = datasets[0].var_names[
+                get_total_feature_slices(datasets)[0]
+            ]
```

### Comparing `transmorph-0.2.6b0/src/transmorph/stats/entropy.py` & `transmorph-0.2.7/src/transmorph/stats/entropy.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python3
-
-import numba
-import numpy as np
-
-from math import log
-from scipy.sparse import diags
-
-from ..utils.graph import nearest_neighbors_custom
-from ..utils.matrix import sort_sparse_matrix
-
-
-@numba.njit(fastmath=True)
-def _label_entropy_njit(sample_labels: np.ndarray, labels: np.ndarray) -> np.ndarray:
-    """
-    Computes entropy of a discrete label distribution. Numba-accelerated.
-
-    Parameters
-    ----------
-    sample_labels: np.ndarray
-        Matrix of shape (n_samples, k) where M[i, j] is the label of
-        point $j in sample $i.
-
-    labels: np.ndarray
-        Vector of shape (n_labels,) containing all possible labels
-
-    Returns
-    -------
-    A np.ndarray of shape (n_samples,) that contains for each sample its
-    label entropy.
-    """
-    (npoints, k), nlabels = sample_labels.shape, labels.shape[0]
-    entropies = np.zeros(npoints)
-    if nlabels <= 1:  # No label diversity
-        return entropies
-    # M[i, l] is the frequency of label $l in sample $i
-    probs = np.zeros((npoints, nlabels))
-    for i, lb in enumerate(labels):
-        probs[:, i] = np.sum(sample_labels == lb, axis=1)
-    probs /= k
-    for i in range(npoints):
-        n_classes = np.count_nonzero(probs[i])
-        if n_classes <= 1:
-            continue
-        for p in probs[i]:
-            if p == 0.0:
-                continue
-            entropies[i] -= p * log(p)
-    return entropies
-
-
-def label_entropy(X: np.ndarray, labels: np.ndarray, n_neighbors: int) -> float:
-    """
-    Computes label entropy from a nearest neighbors matrix.
-    """
-    N = X.shape[0]
-
-    # We build a kNN matrix where values are initial labels.
-    T_all = nearest_neighbors_custom(X, mode="edges", n_neighbors=n_neighbors)
-    T_all = T_all @ diags(labels)
-
-    _, origins = sort_sparse_matrix(T_all)
-    labels_set = list(set(origins.flatten()))
-    entropies = _label_entropy_njit(origins, np.array(labels_set).astype(int))
-
-    return entropies.sum() / N
+#!/usr/bin/env python3
+
+import numba
+import numpy as np
+
+from math import log
+from scipy.sparse import diags
+
+from ..utils.graph import nearest_neighbors_custom
+from ..utils.matrix import sort_sparse_matrix
+
+
+@numba.njit(fastmath=True)
+def _label_entropy_njit(sample_labels: np.ndarray, labels: np.ndarray) -> np.ndarray:
+    """
+    Computes entropy of a discrete label distribution. Numba-accelerated.
+
+    Parameters
+    ----------
+    sample_labels: np.ndarray
+        Matrix of shape (n_samples, k) where M[i, j] is the label of
+        point $j in sample $i.
+
+    labels: np.ndarray
+        Vector of shape (n_labels,) containing all possible labels
+
+    Returns
+    -------
+    A np.ndarray of shape (n_samples,) that contains for each sample its
+    label entropy.
+    """
+    (npoints, k), nlabels = sample_labels.shape, labels.shape[0]
+    entropies = np.zeros(npoints)
+    if nlabels <= 1:  # No label diversity
+        return entropies
+    # M[i, l] is the frequency of label $l in sample $i
+    probs = np.zeros((npoints, nlabels))
+    for i, lb in enumerate(labels):
+        probs[:, i] = np.sum(sample_labels == lb, axis=1)
+    probs /= k
+    for i in range(npoints):
+        n_classes = np.count_nonzero(probs[i])
+        if n_classes <= 1:
+            continue
+        for p in probs[i]:
+            if p == 0.0:
+                continue
+            entropies[i] -= p * log(p)
+    return entropies
+
+
+def label_entropy(X: np.ndarray, labels: np.ndarray, n_neighbors: int) -> float:
+    """
+    Computes label entropy from a nearest neighbors matrix.
+    """
+    N = X.shape[0]
+
+    # We build a kNN matrix where values are initial labels.
+    T_all = nearest_neighbors_custom(X, mode="edges", n_neighbors=n_neighbors)
+    T_all = T_all @ diags(labels)
+
+    _, origins = sort_sparse_matrix(T_all)
+    labels_set = list(set(origins.flatten()))
+    entropies = _label_entropy_njit(origins, np.array(labels_set).astype(int))
+
+    return entropies.sum() / N
```

### Comparing `transmorph-0.2.6b0/src/transmorph/stats/integration.py` & `transmorph-0.2.7/src/transmorph/stats/integration.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-#!/usr/bin/env python3
-
-import numpy as np
-from typing import Dict, Optional, Union
-
-from ot.lp import emd
-from scipy.sparse import csr_matrix
-from scipy.spatial.distance import cdist
-
-from ..utils.geometry import sparse_cdist
-
-# TODO: update to better compare between datasets
-
-
-def matching_divergence(
-    X1: np.ndarray,
-    X2: np.ndarray,
-    matching: csr_matrix,
-    metric: str = "sqeuclidean",
-    metric_kwargs: Optional[Dict] = None,
-    per_point: bool = False,
-    accelerated: bool = False,
-) -> Union[float, np.ndarray]:
-    """
-    Computes the distorsion of an embedding between two datasets
-    with known ground truth matching between samples.
-    Given a boolean matching where M[i, j] = 1 if xi <-> yj,
-    matching_divergence(X, Y, M) =
-
-        1 / sum_ij (M[i, j]) * sum_ij M[i, j]*d(xi, yj)
-
-    This is a basic measure of quadratic divergence (see MDE for instance).
-
-    Parameters
-    ----------
-    X1: np.ndarray (n, d)
-        First dataset embedded in a d-dimensional vector space
-
-    X2: np.ndarray (m, d)
-        Second dataset embedded in a d-dimensional vector space
-
-    matching: scipy.sparse.csr_matrix (n, m)
-        Boolean matching matrix between X1 and X2.
-
-    metric: str, default = "sqeuclidean"
-        Metric string to use for the distorsion.
-
-    metric_kwargs: dict, default = {}
-        Additional metric parameters
-
-    accelerated: bool, default = False
-        Use a sparse implementation instead of scipy.cdist for much higher
-        speed. If so, metric can only be those supported by sparse_cdist
-        from Transmorph.utils.geometry.
-    """
-    metric_kwargs = {} if metric_kwargs is None else metric_kwargs
-    if accelerated:
-        matched_distances = sparse_cdist(X1, X2=X2, T=matching, metric=metric)
-    else:
-        matched_distances = matching.multiply(
-            cdist(X1, X2, metric=metric, **metric_kwargs)
-        )
-    matched_distances /= matching.count_nonzero()
-    if per_point:
-        return np.asarray(matched_distances.sum(axis=1)).reshape(
-            -1,
-        )
-    return matched_distances.sum()
-
-
-def earth_movers_distance(
-    X1: np.ndarray,
-    X2: np.ndarray,
-    C: Optional[np.ndarray] = None,
-    metric: str = "sqeuclidean",
-    metric_kwargs: Optional[Dict] = None,
-    per_point: bool = False,
-    max_iter: int = 1000000,
-):
-    """
-    Earth movers distance (EMD) between X1 and X2 measures how well both
-    embeddings overlap each other. We use a POT backend here to compute
-    this measure. The higher EMD is, the more expansive it is to make
-    both datasets overlap (and then, the poorer the overlap is).
-
-    Parameters
-    ----------
-    X1: np.ndarray
-        Source dataset after integration
-
-    X2: np.ndarray
-        Reference dataset
-
-    C: np.ndarray, optional
-        Cost matrix between X1 and X2, if None then C is set to be
-        the distance matrix between X1 and X2.
-
-    metric: str = "squeuclidean"
-        Metric to use if a distance matrix needs to be computed. It
-        is passed as an argument to scipy.spatial.distance.cdist.
-
-    metric_kwargs: dict, default = {}
-        Additional metric parameters for cdist.
-
-    per_point: bool, default = False
-        If true, EMD per point is returned. Otherwise, the full cost
-        is returned.
-
-    max_iter: int, default = 1000000
-        Number of iterations maximum for ot.lp.emd. Increase this
-        number in case of convergence issues.
-    """
-    assert (
-        C is not None or X1.shape[1] == X2.shape[1]
-    ), "Explicit cost matrix needed if datasets are not in the same space."
-    metric_kwargs = {} if metric_kwargs is None else metric_kwargs
-    if C is None:
-        C = cdist(X1, X2, metric=metric, **metric_kwargs)
-    C /= C.max()
-    w1, w2 = (np.ones(X1.shape[0]) / X1.shape[0], np.ones(X2.shape[0]) / X2.shape[0])
-    T = emd(w1, w2, C, numItermax=max_iter)
-    if per_point:
-        return (T * C).sum(axis=1) * X1.shape[0]
-    return (T * C).sum() * (X1.shape[0] * X1.shape[1])
+#!/usr/bin/env python3
+
+import numpy as np
+from typing import Dict, Optional, Union
+
+from ot.lp import emd
+from scipy.sparse import csr_matrix
+from scipy.spatial.distance import cdist
+
+from ..utils.geometry import sparse_cdist
+
+# TODO: update to better compare between datasets
+
+
+def matching_divergence(
+    X1: np.ndarray,
+    X2: np.ndarray,
+    matching: csr_matrix,
+    metric: str = "sqeuclidean",
+    metric_kwargs: Optional[Dict] = None,
+    per_point: bool = False,
+    accelerated: bool = False,
+) -> Union[float, np.ndarray]:
+    """
+    Computes the distorsion of an embedding between two datasets
+    with known ground truth matching between samples.
+    Given a boolean matching where M[i, j] = 1 if xi <-> yj,
+    matching_divergence(X, Y, M) =
+
+        1 / sum_ij (M[i, j]) * sum_ij M[i, j]*d(xi, yj)
+
+    This is a basic measure of quadratic divergence (see MDE for instance).
+
+    Parameters
+    ----------
+    X1: np.ndarray (n, d)
+        First dataset embedded in a d-dimensional vector space
+
+    X2: np.ndarray (m, d)
+        Second dataset embedded in a d-dimensional vector space
+
+    matching: scipy.sparse.csr_matrix (n, m)
+        Boolean matching matrix between X1 and X2.
+
+    metric: str, default = "sqeuclidean"
+        Metric string to use for the distorsion.
+
+    metric_kwargs: dict, default = {}
+        Additional metric parameters
+
+    accelerated: bool, default = False
+        Use a sparse implementation instead of scipy.cdist for much higher
+        speed. If so, metric can only be those supported by sparse_cdist
+        from Transmorph.utils.geometry.
+    """
+    metric_kwargs = {} if metric_kwargs is None else metric_kwargs
+    if accelerated:
+        matched_distances = sparse_cdist(X1, X2=X2, T=matching, metric=metric)
+    else:
+        matched_distances = matching.multiply(
+            cdist(X1, X2, metric=metric, **metric_kwargs)
+        )
+    matched_distances /= matching.count_nonzero()
+    if per_point:
+        return np.asarray(matched_distances.sum(axis=1)).reshape(
+            -1,
+        )
+    return matched_distances.sum()
+
+
+def earth_movers_distance(
+    X1: np.ndarray,
+    X2: np.ndarray,
+    C: Optional[np.ndarray] = None,
+    metric: str = "sqeuclidean",
+    metric_kwargs: Optional[Dict] = None,
+    per_point: bool = False,
+    max_iter: int = 1000000,
+):
+    """
+    Earth movers distance (EMD) between X1 and X2 measures how well both
+    embeddings overlap each other. We use a POT backend here to compute
+    this measure. The higher EMD is, the more expansive it is to make
+    both datasets overlap (and then, the poorer the overlap is).
+
+    Parameters
+    ----------
+    X1: np.ndarray
+        Source dataset after integration
+
+    X2: np.ndarray
+        Reference dataset
+
+    C: np.ndarray, optional
+        Cost matrix between X1 and X2, if None then C is set to be
+        the distance matrix between X1 and X2.
+
+    metric: str = "squeuclidean"
+        Metric to use if a distance matrix needs to be computed. It
+        is passed as an argument to scipy.spatial.distance.cdist.
+
+    metric_kwargs: dict, default = {}
+        Additional metric parameters for cdist.
+
+    per_point: bool, default = False
+        If true, EMD per point is returned. Otherwise, the full cost
+        is returned.
+
+    max_iter: int, default = 1000000
+        Number of iterations maximum for ot.lp.emd. Increase this
+        number in case of convergence issues.
+    """
+    assert (
+        C is not None or X1.shape[1] == X2.shape[1]
+    ), "Explicit cost matrix needed if datasets are not in the same space."
+    metric_kwargs = {} if metric_kwargs is None else metric_kwargs
+    if C is None:
+        C = cdist(X1, X2, metric=metric, **metric_kwargs)
+    C /= C.max()
+    w1, w2 = (np.ones(X1.shape[0]) / X1.shape[0], np.ones(X2.shape[0]) / X2.shape[0])
+    T = emd(w1, w2, C, numItermax=max_iter)
+    if per_point:
+        return (T * C).sum(axis=1) * X1.shape[0]
+    return (T * C).sum() * (X1.shape[0] * X1.shape[1])
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/anndata_manager.py` & `transmorph-0.2.7/src/transmorph/utils/anndata_manager.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,407 +1,407 @@
-#!/usr/bin/env python3
-
-import logging
-import numpy as np
-import pandas as pd
-
-from anndata import AnnData
-from collections import namedtuple
-from enum import Enum
-from scipy.sparse import csr_matrix
-from typing import Any, Dict, List, Literal, Optional, Tuple, Union
-
-from .._logging import logger
-
-_TypeAnnDataFields = Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
-_TypePairwiseSlice = Dict[Tuple[int, int], Tuple[np.ndarray, np.ndarray]]
-_TypeTotalSlice = List[np.ndarray]
-_TypePersistLevels = Literal["layer", "pipeline", "output"]
-
-
-def generate_features_slice(features: np.ndarray, selected: np.ndarray) -> np.ndarray:
-    """
-    Returns an integer selector to slice {features} to {selected}
-    """
-    assert (
-        np.unique(features).shape[0] == features.shape[0]
-    ), "Duplicated features detected. Please fix this ambiguity."
-    assert (
-        np.unique(selected).shape[0] == selected.shape[0]
-    ), "Duplicated selected features detected. Please report this issue."
-    fslice = np.zeros(selected.shape).astype(int)
-    for i, fname in enumerate(selected):
-        feature_idx = np.where(features == fname)[0]
-        assert feature_idx.shape[0] == 1, f"Missing features: {fname}."
-        fslice[i] = np.where(features == fname)[0]  # Yuk, could be done better
-    return fslice
-
-
-def get_pairwise_feature_slices(datasets: List[AnnData]) -> _TypePairwiseSlice:
-    """
-    Returns a dictionary where index (i, j) corresponds to integer
-    slices to use to put datasets i and j to the same feature space.
-    """
-    result: _TypePairwiseSlice = {}
-    for i, adata_i in enumerate(datasets):
-        features_i = adata_i.var_names.to_numpy()
-        slice_ii = generate_features_slice(
-            features=adata_i.var_names.to_numpy(),
-            selected=np.sort(adata_i.var_names.to_numpy()),
-        )
-        result[i, i] = (slice_ii, slice_ii)
-        for j, adata_j in enumerate(datasets):
-            if j <= i:
-                continue
-            features_j = adata_j.var_names.to_numpy()
-            common_features = np.intersect1d(features_i, features_j)
-            common_features = np.sort(common_features)
-            slice_i = generate_features_slice(
-                features=features_i,
-                selected=common_features,
-            )
-            slice_j = generate_features_slice(
-                features=features_j,
-                selected=common_features,
-            )
-            result[i, j] = (slice_i, slice_j)
-            result[j, i] = (slice_j, slice_i)
-    return result
-
-
-def get_total_feature_slices(datasets: List[AnnData]) -> _TypeTotalSlice:
-    """
-    Returns a list where array at index i corresponds to boolean
-    slice to use to slice dataset i in a common feature space.
-    """
-    result: _TypeTotalSlice = []
-    if len(datasets) == 0:
-        return []
-    common_features = datasets[0].var_names.to_numpy()
-    for adata in datasets[1:]:
-        common_features = np.intersect1d(
-            common_features,
-            adata.var_names.to_numpy(),
-        )
-    common_features = np.sort(common_features)
-    for adata in datasets:
-        result.append(
-            generate_features_slice(adata.var_names.to_numpy(), common_features)
-        )
-    return result
-
-
-def slice_common_features(datasets: List[AnnData]) -> List[np.ndarray]:
-    """
-    Returns a list of AnnData objects in a common features space.
-    """
-    slices = get_total_feature_slices(datasets)
-    return [adata.X[:, sl] for adata, sl in zip(datasets, slices)]
-
-
-# FIXME: this will cause issues in the future.
-# It was bad design
-class AnnDataKeyIdentifiers(Enum):
-    """
-    String constants to pass to AnnDataManager to easily manage
-    data storing in AnnData objects.
-
-    tr_... suggests the key is internal to the engine, and
-    helps avoiding key collisions with other packages.
-    """
-
-    # Default representation keys
-    BaseRepresentation = "tr_base_representation"
-    TransmorphRepresentation = "X_transmorph"
-
-    # AnnData metadata
-    AnnDataId = "tr_adata_id"
-    IsReference = "tr_is_reference"
-    Metric = "tr_default_metric"
-    MetricKwargs = "tr_default_metric_kwargs"
-
-    # Structural keys
-    DistanceMatrix = "tr_distance_matrix"
-    SimilarityMatrix = "tr_similarity_matrix"
-    SubsamplingAnchors = "tr_ssp_anchors"
-    SubsamplingReferences = "tr_ssp_references"
-
-    # Plotting keys
-    PlotRepresentation = "tr_plot_representation"
-
-
-AnnDataKey = namedtuple("AnnDataKey", ["identifier", "field", "persist"])
-
-
-class AnnDataManager:
-    """
-    This class allows to safely handle AnnData objects, either through
-    its static methods or using the global anndata manager object.
-    """
-
-    def __init__(self):
-        adataid_str = AnnDataKeyIdentifiers.AnnDataId.value
-        self.keys: Dict[str, AnnDataKey] = {
-            adataid_str: AnnDataKey(adataid_str, "uns", "pipeline")
-        }
-        self.current_id = 0
-
-    @staticmethod
-    def log(msg: str, level: int = logging.DEBUG) -> None:
-        logger.log(level, f"ADManager > {msg}")
-
-    @staticmethod
-    def gen_keystring(key: Union[str, AnnDataKeyIdentifiers]) -> str:
-        """
-        Adds a prefix to a given key to decrease collision cases
-        with other packages.
-        """
-        if isinstance(key, AnnDataKeyIdentifiers):
-            return key.value
-        return key
-
-    @staticmethod
-    def to_delete(query: _TypePersistLevels, target: _TypePersistLevels) -> bool:
-        """
-        Returns true if query level <= target level.
-        """
-        levels = ["layer", "pipeline", "output"]
-        assert query in levels, f"Unknown query level: {query}"
-        assert target in levels, f"Unknown target level: {target}"
-        if target == "output":
-            return True
-        if target == "pipeline":
-            return query != "output"
-        if target == "layer":
-            return query == target
-        raise ValueError(f"Unknown target persist level: {target}.")
-
-    @staticmethod
-    def get(field: Union[pd.DataFrame, Dict], str_key: str) -> Any:
-        """
-        Retrieves information for an AnnData field, returns None if
-        not present.
-        """
-        if str_key not in field:
-            return None
-        return field[str_key]
-
-    @staticmethod
-    def delete(field: Union[pd.DataFrame, Dict], str_key: str) -> None:
-        """
-        Deletes an AnnData entry if it is present, and logs it.
-        """
-        if str_key not in field:
-            return
-        del field[str_key]
-
-    @staticmethod
-    def get_field_from_str(adata: AnnData, field_str: str) -> Union[pd.DataFrame, Dict]:
-        """
-        Returns field {field_str} of {adata}. Raises an exception if {field_str} is
-        invalid.
-        """
-        if field_str == "obs":
-            return adata.obs
-        if field_str == "var":
-            return adata.var
-        if field_str == "obsm":
-            return adata.obsm
-        if field_str == "varm":
-            return adata.varm
-        if field_str == "obsp":
-            return adata.obsp
-        if field_str == "varp":
-            return adata.varp
-        if field_str == "uns":
-            if "transmorph" not in adata.uns:
-                adata.uns["transmorph"] = {}
-            return adata.uns["transmorph"]
-        raise ValueError(f"Unknown field {field_str}.")
-
-    def set_value(
-        self,
-        adata: AnnData,
-        key: Union[str, AnnDataKeyIdentifiers],
-        field: _TypeAnnDataFields,
-        value: Any,
-        persist: _TypePersistLevels = "pipeline",
-    ) -> None:
-        """
-        Stores information in an AnnData object, with a few sanity
-        checks.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to store information in.
-
-        key: AnnDataKeys
-            AnnDataKey identifier to safely store the information.
-
-        value: Any
-            Data to store.
-
-        field: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
-            AnnData subfield to store the information.
-            - "obs" vector-like data to label observations
-            - "var" vector-like data to label features
-            - "obsm" matrix-like data to represent observations
-            - "varm" matrix-like data to represent features
-            - "obsp" matrix-like data containing pairwise information
-              between observations
-            - "varp" matrix-like data containing pairwise information
-              between features
-            - "uns" any type of data to be stored (parameters, metadata,
-              local metric...)
-
-
-        persist: Literal["layer", "pipeline", "output"], default = "pipeline"
-            Life duration of the information.
-            - "layer": Information is deleted at the end of the layer that
-              created it.
-            - "pipeline": Information is deleted at the end of the pipeline.
-            - "output": Information is not deleted at the end of the pipeline.
-        """
-        str_key = AnnDataManager.gen_keystring(key)
-        if str_key not in self.keys:
-            self.keys[str_key] = AnnDataKey(str_key, field, persist)
-        else:  # We check consistance
-            _, old_field, old_persist = self.keys[str_key]
-            assert old_field == field
-            assert old_persist == persist
-        field_obj = AnnDataManager.get_field_from_str(adata, field)
-        field_obj[str_key] = value
-        str_descriptor = value
-        if isinstance(value, (np.ndarray, csr_matrix)):
-            str_descriptor = f"{type(value)} ({value.shape})"
-        AnnDataManager.log(f"Inserting {str_descriptor} in {field}[{str_key}]")
-
-    def get_value(
-        self,
-        adata: AnnData,
-        key: Union[str, AnnDataKeyIdentifiers],
-        field_str: Optional[_TypeAnnDataFields] = None,
-    ) -> Optional[Any]:
-        """
-        Retrieves value previously stored. Returns None if nothing is found.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to retrieve information from.
-
-        key: AnnDataKeys
-            Key to retrieve. if it was stored by transmorph, the field will
-            be remembered. Otherwise, you must provide it explicitly.
-
-        field_str: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
-            AnnData subfield containing the information.
-            - "obs" vector-like data to label observations
-            - "var" vector-like data to label features
-            - "obsm" matrix-like data to represent observations
-            - "varm" matrix-like data to represent features
-            - "obsp" matrix-like data containing pairwise information
-              between observations
-            - "varp" matrix-like data containing pairwise information
-              between features
-            - "uns" any type of data to be stored (parameters, metadata,
-              local metric...)
-        """
-        str_key = AnnDataManager.gen_keystring(key)
-
-        # By default, ADKI.BaseRepresentation returns .X if not set.
-        base_repr = AnnDataKeyIdentifiers.BaseRepresentation.value
-        if str_key == base_repr and AnnDataManager.get(adata.obsm, base_repr) is None:
-            return adata.X
-
-        if str_key in self.keys:
-            field_str = self.keys[str_key].field
-        if field_str is None:
-            return None
-
-        field = AnnDataManager.get_field_from_str(adata, field_str)
-        return AnnDataManager.get(field, str_key)
-
-    def isset_value(
-        self,
-        adata: AnnData,
-        key: Union[str, AnnDataKeyIdentifiers],
-        field: Optional[_TypeAnnDataFields] = None,
-    ) -> bool:
-        """
-        Detects if a key is stored in an AnnData object.
-
-        Parameters
-        ----------
-        adata: AnnData
-            AnnData object to retrieve information from.
-
-        key: AnnDataKeys
-            Key to retrieve. if it was stored by transmorph, the field will
-            be remembered. Otherwise, you must provide it explicitly.
-
-        field_str: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
-            AnnData subfield containing the information.
-            - "obs" vector-like data to label observations
-            - "var" vector-like data to label features
-            - "obsm" matrix-like data to represent observations
-            - "varm" matrix-like data to represent features
-            - "obsp" matrix-like data containing pairwise information
-              between observations
-            - "varp" matrix-like data containing pairwise information
-              between features
-            - "uns" any type of data to be stored (parameters, metadata,
-              local metric...)
-        """
-        return self.get_value(adata, key, field) is not None
-
-    def clean(
-        self,
-        datasets: Union[AnnData, List[AnnData]],
-        level: _TypePersistLevels = "pipeline",
-    ) -> None:
-        """
-        Deletes transmorph keys of the given persist level and below.
-
-        Parameters
-        ----------
-        datasets: Union[AnnData, List[AnnData]]
-            AnnData object(s) to clean.
-
-        level: Literal["output", "pipeline", "layer"]
-            All values with persist below this {level} are deleted.
-        """
-        if isinstance(datasets, AnnData):
-            datasets = [datasets]
-
-        for adata in datasets:
-            for admkey in self.keys.values():
-                key, field_str, persist = admkey
-                str_key = AnnDataManager.gen_keystring(key)
-                if not AnnDataManager.to_delete(persist, level):
-                    continue
-                AnnDataManager.log(f"Deleting entry {field_str}[{str_key}].")
-                field = AnnDataManager.get_field_from_str(adata, field_str)
-                AnnDataManager.delete(field, str_key)
-                if field_str == "uns" and field == {}:
-                    del adata.uns["transmorph"]
-
-    def get_anndata_id(self, adata: AnnData) -> int:
-        """
-        Creates a new identifier for specified AnnData if necessary,
-        then retrieves its identifier.
-        """
-        adata_id = self.get_value(adata, AnnDataKeyIdentifiers.AnnDataId)
-        if adata_id is None:
-            adata_id = self.current_id
-            self.set_value(
-                adata,
-                AnnDataKeyIdentifiers.AnnDataId,
-                "uns",
-                adata_id,
-            )
-            self.current_id += 1
-        return adata_id
-
-
-anndata_manager = AnnDataManager()
+#!/usr/bin/env python3
+
+import logging
+import numpy as np
+import pandas as pd
+
+from anndata import AnnData
+from collections import namedtuple
+from enum import Enum
+from scipy.sparse import csr_matrix
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
+
+from .._logging import logger
+
+_TypeAnnDataFields = Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
+_TypePairwiseSlice = Dict[Tuple[int, int], Tuple[np.ndarray, np.ndarray]]
+_TypeTotalSlice = List[np.ndarray]
+_TypePersistLevels = Literal["layer", "pipeline", "output"]
+
+
+def generate_features_slice(features: np.ndarray, selected: np.ndarray) -> np.ndarray:
+    """
+    Returns an integer selector to slice {features} to {selected}
+    """
+    assert (
+        np.unique(features).shape[0] == features.shape[0]
+    ), "Duplicated features detected. Please fix this ambiguity."
+    assert (
+        np.unique(selected).shape[0] == selected.shape[0]
+    ), "Duplicated selected features detected. Please report this issue."
+    fslice = np.zeros(selected.shape).astype(int)
+    for i, fname in enumerate(selected):
+        feature_idx = np.where(features == fname)[0]
+        assert feature_idx.shape[0] == 1, f"Missing features: {fname}."
+        fslice[i] = np.where(features == fname)[0]  # Yuk, could be done better
+    return fslice
+
+
+def get_pairwise_feature_slices(datasets: List[AnnData]) -> _TypePairwiseSlice:
+    """
+    Returns a dictionary where index (i, j) corresponds to integer
+    slices to use to put datasets i and j to the same feature space.
+    """
+    result: _TypePairwiseSlice = {}
+    for i, adata_i in enumerate(datasets):
+        features_i = adata_i.var_names.to_numpy()
+        slice_ii = generate_features_slice(
+            features=adata_i.var_names.to_numpy(),
+            selected=np.sort(adata_i.var_names.to_numpy()),
+        )
+        result[i, i] = (slice_ii, slice_ii)
+        for j, adata_j in enumerate(datasets):
+            if j <= i:
+                continue
+            features_j = adata_j.var_names.to_numpy()
+            common_features = np.intersect1d(features_i, features_j)
+            common_features = np.sort(common_features)
+            slice_i = generate_features_slice(
+                features=features_i,
+                selected=common_features,
+            )
+            slice_j = generate_features_slice(
+                features=features_j,
+                selected=common_features,
+            )
+            result[i, j] = (slice_i, slice_j)
+            result[j, i] = (slice_j, slice_i)
+    return result
+
+
+def get_total_feature_slices(datasets: List[AnnData]) -> _TypeTotalSlice:
+    """
+    Returns a list where array at index i corresponds to boolean
+    slice to use to slice dataset i in a common feature space.
+    """
+    result: _TypeTotalSlice = []
+    if len(datasets) == 0:
+        return []
+    common_features = datasets[0].var_names.to_numpy()
+    for adata in datasets[1:]:
+        common_features = np.intersect1d(
+            common_features,
+            adata.var_names.to_numpy(),
+        )
+    common_features = np.sort(common_features)
+    for adata in datasets:
+        result.append(
+            generate_features_slice(adata.var_names.to_numpy(), common_features)
+        )
+    return result
+
+
+def slice_common_features(datasets: List[AnnData]) -> List[np.ndarray]:
+    """
+    Returns a list of AnnData objects in a common features space.
+    """
+    slices = get_total_feature_slices(datasets)
+    return [adata.X[:, sl] for adata, sl in zip(datasets, slices)]
+
+
+# FIXME: this will cause issues in the future.
+# It was bad design
+class AnnDataKeyIdentifiers(Enum):
+    """
+    String constants to pass to AnnDataManager to easily manage
+    data storing in AnnData objects.
+
+    tr_... suggests the key is internal to the engine, and
+    helps avoiding key collisions with other packages.
+    """
+
+    # Default representation keys
+    BaseRepresentation = "tr_base_representation"
+    TransmorphRepresentation = "X_transmorph"
+
+    # AnnData metadata
+    AnnDataId = "tr_adata_id"
+    IsReference = "tr_is_reference"
+    Metric = "tr_default_metric"
+    MetricKwargs = "tr_default_metric_kwargs"
+
+    # Structural keys
+    DistanceMatrix = "tr_distance_matrix"
+    SimilarityMatrix = "tr_similarity_matrix"
+    SubsamplingAnchors = "tr_ssp_anchors"
+    SubsamplingReferences = "tr_ssp_references"
+
+    # Plotting keys
+    PlotRepresentation = "tr_plot_representation"
+
+
+AnnDataKey = namedtuple("AnnDataKey", ["identifier", "field", "persist"])
+
+
+class AnnDataManager:
+    """
+    This class allows to safely handle AnnData objects, either through
+    its static methods or using the global anndata manager object.
+    """
+
+    def __init__(self):
+        adataid_str = AnnDataKeyIdentifiers.AnnDataId.value
+        self.keys: Dict[str, AnnDataKey] = {
+            adataid_str: AnnDataKey(adataid_str, "uns", "pipeline")
+        }
+        self.current_id = 0
+
+    @staticmethod
+    def log(msg: str, level: int = logging.DEBUG) -> None:
+        logger.log(level, f"ADManager > {msg}")
+
+    @staticmethod
+    def gen_keystring(key: Union[str, AnnDataKeyIdentifiers]) -> str:
+        """
+        Adds a prefix to a given key to decrease collision cases
+        with other packages.
+        """
+        if isinstance(key, AnnDataKeyIdentifiers):
+            return key.value
+        return key
+
+    @staticmethod
+    def to_delete(query: _TypePersistLevels, target: _TypePersistLevels) -> bool:
+        """
+        Returns true if query level <= target level.
+        """
+        levels = ["layer", "pipeline", "output"]
+        assert query in levels, f"Unknown query level: {query}"
+        assert target in levels, f"Unknown target level: {target}"
+        if target == "output":
+            return True
+        if target == "pipeline":
+            return query != "output"
+        if target == "layer":
+            return query == target
+        raise ValueError(f"Unknown target persist level: {target}.")
+
+    @staticmethod
+    def get(field: Union[pd.DataFrame, Dict], str_key: str) -> Any:
+        """
+        Retrieves information for an AnnData field, returns None if
+        not present.
+        """
+        if str_key not in field:
+            return None
+        return field[str_key]
+
+    @staticmethod
+    def delete(field: Union[pd.DataFrame, Dict], str_key: str) -> None:
+        """
+        Deletes an AnnData entry if it is present, and logs it.
+        """
+        if str_key not in field:
+            return
+        del field[str_key]
+
+    @staticmethod
+    def get_field_from_str(adata: AnnData, field_str: str) -> Union[pd.DataFrame, Dict]:
+        """
+        Returns field {field_str} of {adata}. Raises an exception if {field_str} is
+        invalid.
+        """
+        if field_str == "obs":
+            return adata.obs
+        if field_str == "var":
+            return adata.var
+        if field_str == "obsm":
+            return adata.obsm
+        if field_str == "varm":
+            return adata.varm
+        if field_str == "obsp":
+            return adata.obsp
+        if field_str == "varp":
+            return adata.varp
+        if field_str == "uns":
+            if "transmorph" not in adata.uns:
+                adata.uns["transmorph"] = {}
+            return adata.uns["transmorph"]
+        raise ValueError(f"Unknown field {field_str}.")
+
+    def set_value(
+        self,
+        adata: AnnData,
+        key: Union[str, AnnDataKeyIdentifiers],
+        field: _TypeAnnDataFields,
+        value: Any,
+        persist: _TypePersistLevels = "pipeline",
+    ) -> None:
+        """
+        Stores information in an AnnData object, with a few sanity
+        checks.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to store information in.
+
+        key: AnnDataKeys
+            AnnDataKey identifier to safely store the information.
+
+        value: Any
+            Data to store.
+
+        field: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
+            AnnData subfield to store the information.
+            - "obs" vector-like data to label observations
+            - "var" vector-like data to label features
+            - "obsm" matrix-like data to represent observations
+            - "varm" matrix-like data to represent features
+            - "obsp" matrix-like data containing pairwise information
+              between observations
+            - "varp" matrix-like data containing pairwise information
+              between features
+            - "uns" any type of data to be stored (parameters, metadata,
+              local metric...)
+
+
+        persist: Literal["layer", "pipeline", "output"], default = "pipeline"
+            Life duration of the information.
+            - "layer": Information is deleted at the end of the layer that
+              created it.
+            - "pipeline": Information is deleted at the end of the pipeline.
+            - "output": Information is not deleted at the end of the pipeline.
+        """
+        str_key = AnnDataManager.gen_keystring(key)
+        if str_key not in self.keys:
+            self.keys[str_key] = AnnDataKey(str_key, field, persist)
+        else:  # We check consistance
+            _, old_field, old_persist = self.keys[str_key]
+            assert old_field == field
+            assert old_persist == persist
+        field_obj = AnnDataManager.get_field_from_str(adata, field)
+        field_obj[str_key] = value
+        str_descriptor = value
+        if isinstance(value, (np.ndarray, csr_matrix)):
+            str_descriptor = f"{type(value)} ({value.shape})"
+        AnnDataManager.log(f"Inserting {str_descriptor} in {field}[{str_key}]")
+
+    def get_value(
+        self,
+        adata: AnnData,
+        key: Union[str, AnnDataKeyIdentifiers],
+        field_str: Optional[_TypeAnnDataFields] = None,
+    ) -> Optional[Any]:
+        """
+        Retrieves value previously stored. Returns None if nothing is found.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to retrieve information from.
+
+        key: AnnDataKeys
+            Key to retrieve. if it was stored by transmorph, the field will
+            be remembered. Otherwise, you must provide it explicitly.
+
+        field_str: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
+            AnnData subfield containing the information.
+            - "obs" vector-like data to label observations
+            - "var" vector-like data to label features
+            - "obsm" matrix-like data to represent observations
+            - "varm" matrix-like data to represent features
+            - "obsp" matrix-like data containing pairwise information
+              between observations
+            - "varp" matrix-like data containing pairwise information
+              between features
+            - "uns" any type of data to be stored (parameters, metadata,
+              local metric...)
+        """
+        str_key = AnnDataManager.gen_keystring(key)
+
+        # By default, ADKI.BaseRepresentation returns .X if not set.
+        base_repr = AnnDataKeyIdentifiers.BaseRepresentation.value
+        if str_key == base_repr and AnnDataManager.get(adata.obsm, base_repr) is None:
+            return adata.X
+
+        if str_key in self.keys:
+            field_str = self.keys[str_key].field
+        if field_str is None:
+            return None
+
+        field = AnnDataManager.get_field_from_str(adata, field_str)
+        return AnnDataManager.get(field, str_key)
+
+    def isset_value(
+        self,
+        adata: AnnData,
+        key: Union[str, AnnDataKeyIdentifiers],
+        field: Optional[_TypeAnnDataFields] = None,
+    ) -> bool:
+        """
+        Detects if a key is stored in an AnnData object.
+
+        Parameters
+        ----------
+        adata: AnnData
+            AnnData object to retrieve information from.
+
+        key: AnnDataKeys
+            Key to retrieve. if it was stored by transmorph, the field will
+            be remembered. Otherwise, you must provide it explicitly.
+
+        field_str: Literal["obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
+            AnnData subfield containing the information.
+            - "obs" vector-like data to label observations
+            - "var" vector-like data to label features
+            - "obsm" matrix-like data to represent observations
+            - "varm" matrix-like data to represent features
+            - "obsp" matrix-like data containing pairwise information
+              between observations
+            - "varp" matrix-like data containing pairwise information
+              between features
+            - "uns" any type of data to be stored (parameters, metadata,
+              local metric...)
+        """
+        return self.get_value(adata, key, field) is not None
+
+    def clean(
+        self,
+        datasets: Union[AnnData, List[AnnData]],
+        level: _TypePersistLevels = "pipeline",
+    ) -> None:
+        """
+        Deletes transmorph keys of the given persist level and below.
+
+        Parameters
+        ----------
+        datasets: Union[AnnData, List[AnnData]]
+            AnnData object(s) to clean.
+
+        level: Literal["output", "pipeline", "layer"]
+            All values with persist below this {level} are deleted.
+        """
+        if isinstance(datasets, AnnData):
+            datasets = [datasets]
+
+        for adata in datasets:
+            for admkey in self.keys.values():
+                key, field_str, persist = admkey
+                str_key = AnnDataManager.gen_keystring(key)
+                if not AnnDataManager.to_delete(persist, level):
+                    continue
+                AnnDataManager.log(f"Deleting entry {field_str}[{str_key}].")
+                field = AnnDataManager.get_field_from_str(adata, field_str)
+                AnnDataManager.delete(field, str_key)
+                if field_str == "uns" and field == {}:
+                    del adata.uns["transmorph"]
+
+    def get_anndata_id(self, adata: AnnData) -> int:
+        """
+        Creates a new identifier for specified AnnData if necessary,
+        then retrieves its identifier.
+        """
+        adata_id = self.get_value(adata, AnnDataKeyIdentifiers.AnnDataId)
+        if adata_id is None:
+            adata_id = self.current_id
+            self.set_value(
+                adata,
+                AnnDataKeyIdentifiers.AnnDataId,
+                "uns",
+                adata_id,
+            )
+            self.current_id += 1
+        return adata_id
+
+
+anndata_manager = AnnDataManager()
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/dimred.py` & `transmorph-0.2.7/src/transmorph/utils/dimred.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-#!/usr/bin/env python3
-
-from logging import warn
-from typing import Optional
-import numpy as np
-
-from sica.base import StabilizedICA
-from sklearn.decomposition import PCA
-from umap.umap_ import UMAP, find_ab_params
-
-from .matrix import contains_duplicates, perturbate, scale_matrix
-from .._logging import logger
-
-
-def pca_projector(
-    X: np.ndarray,
-    n_components: int = 2,
-    use_subset: Optional[np.ndarray] = None,
-) -> PCA:
-    """
-    Returns a fitted sklearn PCA object.
-
-    Parameters
-    ----------
-    X: np.ndarray
-        (n, d) vectorized dataset to apply PCA on.
-
-    n_components: int, default = 2
-        Number of principal components to use. If > d, then it is set to d.
-
-    use_subset: Optional[np.ndarray]
-        Optional slice selector (n,) to pass. If passed, the specified subset
-        of X is used to fit PCA.
-    """
-    from .._settings import settings
-
-    assert n_components > 0, "Number of components must be positive."
-    n, d = X.shape
-    if n_components > d:
-        warn(
-            "Number of components higher than dataset dimensionality."
-            f"Setting it to {d} instead."
-        )
-        n_components = d
-
-    if use_subset is None:
-        X_fit = X
-    else:
-        X_fit = X[use_subset]
-
-    pca = PCA(n_components=n_components, random_state=settings.global_random_seed)
-    pca.fit(X_fit)
-    return pca
-
-
-def pca(
-    X: np.ndarray,
-    n_components: int = 2,
-    use_subset: Optional[np.ndarray] = None,
-) -> np.ndarray:
-    """
-    Small wrapper for sklearn.decomposition.PCA
-
-    Parameters
-    ----------
-    X: np.ndarray
-        (n, d) vectorized dataset to apply PCA on.
-
-    n_components: int, default = 2
-        Number of principal components to use. If > d, then it is set to d.
-
-    use_subset: Optional[np.ndarray]
-        Optional slice selector (n,) to pass. If passed, the specified subset
-        of X is used to fit PCA.
-    """
-    pca = pca_projector(X, n_components, use_subset)
-    return pca.transform(X)
-
-
-def ica(
-    X: np.ndarray,
-    n_components: int = 30,
-    max_iter: int = 1000,
-    n_runs: int = 10,
-    normalize_features: bool = True,
-) -> np.ndarray:
-    """
-    Computes an ICA representation of the data using StablilizedICA.
-    """
-    sica = StabilizedICA(
-        n_components=n_components,
-        max_iter=max_iter,
-        n_runs=n_runs,
-        n_jobs=-1,
-    )
-    if normalize_features:
-        X = scale_matrix(X, axis=0, std_mode=False)
-
-    return sica.fit_transform(X)
-
-
-def umap(X: np.ndarray, embedding_dimension: int = 2) -> np.ndarray:
-    """
-    Computes a UMAP representation of dataset X.
-    """
-    from .._settings import settings
-
-    nsamples = X.shape[0]
-    n_epochs = (
-        settings.umap_maxiter
-        if settings.umap_maxiter is not None
-        else 500
-        if nsamples < settings.large_dataset_threshold
-        else 200
-    )
-    if settings.umap_a is None or settings.umap_b is None:
-        a, b = find_ab_params(settings.umap_spread, settings.umap_min_dist)
-    else:
-        a, b = settings.umap_a, settings.umap_b
-
-    X_red = pca(X, n_components=settings.neighbors_n_pcs)
-    if contains_duplicates(X_red):
-        logger.debug("umap > Duplicates detected. Jittering data.")
-        X_red = perturbate(X_red, std=0.04)
-
-    return UMAP(
-        n_neighbors=settings.umap_n_neighbors,
-        n_components=embedding_dimension,
-        metric=settings.umap_metric,
-        metric_kwds=settings.umap_metric_kwargs,
-        n_epochs=n_epochs,
-        a=a,
-        b=b,
-        random_state=settings.umap_random_state,
-        negative_sample_rate=settings.umap_negative_sample_rate,
-        learning_rate=settings.umap_alpha,
-    ).fit_transform(X_red)
+#!/usr/bin/env python3
+
+from logging import warn
+from typing import Optional
+import numpy as np
+
+from sica.base import StabilizedICA
+from sklearn.decomposition import PCA
+from umap.umap_ import UMAP, find_ab_params
+
+from .matrix import contains_duplicates, perturbate, scale_matrix
+from .._logging import logger
+
+
+def pca_projector(
+    X: np.ndarray,
+    n_components: int = 2,
+    use_subset: Optional[np.ndarray] = None,
+) -> PCA:
+    """
+    Returns a fitted sklearn PCA object.
+
+    Parameters
+    ----------
+    X: np.ndarray
+        (n, d) vectorized dataset to apply PCA on.
+
+    n_components: int, default = 2
+        Number of principal components to use. If > d, then it is set to d.
+
+    use_subset: Optional[np.ndarray]
+        Optional slice selector (n,) to pass. If passed, the specified subset
+        of X is used to fit PCA.
+    """
+    from .._settings import settings
+
+    assert n_components > 0, "Number of components must be positive."
+    n, d = X.shape
+    if n_components > d:
+        warn(
+            "Number of components higher than dataset dimensionality."
+            f"Setting it to {d} instead."
+        )
+        n_components = d
+
+    if use_subset is None:
+        X_fit = X
+    else:
+        X_fit = X[use_subset]
+
+    pca = PCA(n_components=n_components, random_state=settings.global_random_seed)
+    pca.fit(X_fit)
+    return pca
+
+
+def pca(
+    X: np.ndarray,
+    n_components: int = 2,
+    use_subset: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """
+    Small wrapper for sklearn.decomposition.PCA
+
+    Parameters
+    ----------
+    X: np.ndarray
+        (n, d) vectorized dataset to apply PCA on.
+
+    n_components: int, default = 2
+        Number of principal components to use. If > d, then it is set to d.
+
+    use_subset: Optional[np.ndarray]
+        Optional slice selector (n,) to pass. If passed, the specified subset
+        of X is used to fit PCA.
+    """
+    pca = pca_projector(X, n_components, use_subset)
+    return pca.transform(X)
+
+
+def ica(
+    X: np.ndarray,
+    n_components: int = 30,
+    max_iter: int = 1000,
+    n_runs: int = 10,
+    normalize_features: bool = True,
+) -> np.ndarray:
+    """
+    Computes an ICA representation of the data using StablilizedICA.
+    """
+    sica = StabilizedICA(
+        n_components=n_components,
+        max_iter=max_iter,
+        n_runs=n_runs,
+        n_jobs=-1,
+    )
+    if normalize_features:
+        X = scale_matrix(X, axis=0, std_mode=False)
+
+    return sica.fit_transform(X)
+
+
+def umap(X: np.ndarray, embedding_dimension: int = 2) -> np.ndarray:
+    """
+    Computes a UMAP representation of dataset X.
+    """
+    from .._settings import settings
+
+    nsamples = X.shape[0]
+    n_epochs = (
+        settings.umap_maxiter
+        if settings.umap_maxiter is not None
+        else 500
+        if nsamples < settings.large_dataset_threshold
+        else 200
+    )
+    if settings.umap_a is None or settings.umap_b is None:
+        a, b = find_ab_params(settings.umap_spread, settings.umap_min_dist)
+    else:
+        a, b = settings.umap_a, settings.umap_b
+
+    X_red = pca(X, n_components=settings.neighbors_n_pcs)
+    if contains_duplicates(X_red):
+        logger.debug("umap > Duplicates detected. Jittering data.")
+        X_red = perturbate(X_red, std=0.04)
+
+    return UMAP(
+        n_neighbors=settings.umap_n_neighbors,
+        n_components=embedding_dimension,
+        metric=settings.umap_metric,
+        metric_kwds=settings.umap_metric_kwargs,
+        n_epochs=n_epochs,
+        a=a,
+        b=b,
+        random_state=settings.umap_random_state,
+        negative_sample_rate=settings.umap_negative_sample_rate,
+        learning_rate=settings.umap_alpha,
+    ).fit_transform(X_red)
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/geometry.py` & `transmorph-0.2.7/src/transmorph/utils/geometry.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-#!/usr/bin/env python3
-
-from logging import warn
-from numba.core.decorators import njit
-import numpy as np
-from scipy.sparse import coo_matrix, csr_matrix
-from scipy.spatial.distance import cdist
-
-
-def sparse_cdist(
-    X1: np.ndarray,
-    X2: np.ndarray = None,
-    T: csr_matrix = None,
-    metric: str = "sqeuclidean",
-) -> csr_matrix:
-    """
-    Sparse version of scipy.spatial.distance.cdist. Computes pairwise
-    distances between points of X1 and X2 on the non-zero indices of
-    matrix T, returning the result as a sparse matrix. Greatly speedups
-    pairwise distance comparison over a subsample of X1 and X2 (for instance
-    if we are just interested in distances along graph edges).
-
-    Parameters
-    ----------
-    X1: np.ndarray
-        Embedding of the first dataset.
-
-    X2: np.ndarray = None
-        Embedding of the second dataset. If None, uses the first
-        dataset instead.
-
-    T: scipy.sparse.csr_matrix, default = None
-        If T[i, j] != 0, distance between X1[i] and X2[j] will
-        be computed. If None, equivalent to cdist.
-
-    metric: str = "sqeuclidean"
-        Metric to use in distance computation. These metrics must
-        be implemented with the @njit tag, so only a few are available
-        at this point. More will come as needs grow.
-        Valid metrics: "sqeuclidean", "euclidean"
-    """
-    if X2 is None:
-        X2 = X1
-    if T is None:
-        warn(
-            "Using sparse_cdist without a matching is useless."
-            "Use scipy's cdist instead."
-        )
-        return csr_matrix(cdist(X1, X2, metric=metric))
-    T = T.tocoo()
-    if metric == "sqeuclidean":
-        dfunc = dfunc_sqeuclidean
-    elif metric == "euclidean":
-        dfunc = dfunc_euclidean
-    else:
-        raise NotImplementedError("Unrecognized metric.")
-    data = sparse_cdist_njit(X1, X2, T.row, T.col, dfunc)
-    return coo_matrix((data, (T.row, T.col)), shape=T.shape).tocsr()
-
-
-@njit(fastmath=True)
-def sparse_cdist_njit(X1, X2, row, col, dfunc):
-    data = np.zeros(row.shape)
-    for k, (i, j) in enumerate(zip(row, col)):
-        data[k] = dfunc(X1[i], X2[j])
-    return data
-
-
-@njit
-def dfunc_sqeuclidean(x, y):
-    return (x - y) @ (x - y)
-
-
-@njit
-def dfunc_euclidean(x, y):
-    return np.sqrt(dfunc_sqeuclidean(x, y))
+#!/usr/bin/env python3
+
+from logging import warn
+from numba.core.decorators import njit
+import numpy as np
+from scipy.sparse import coo_matrix, csr_matrix
+from scipy.spatial.distance import cdist
+
+
+def sparse_cdist(
+    X1: np.ndarray,
+    X2: np.ndarray = None,
+    T: csr_matrix = None,
+    metric: str = "sqeuclidean",
+) -> csr_matrix:
+    """
+    Sparse version of scipy.spatial.distance.cdist. Computes pairwise
+    distances between points of X1 and X2 on the non-zero indices of
+    matrix T, returning the result as a sparse matrix. Greatly speedups
+    pairwise distance comparison over a subsample of X1 and X2 (for instance
+    if we are just interested in distances along graph edges).
+
+    Parameters
+    ----------
+    X1: np.ndarray
+        Embedding of the first dataset.
+
+    X2: np.ndarray = None
+        Embedding of the second dataset. If None, uses the first
+        dataset instead.
+
+    T: scipy.sparse.csr_matrix, default = None
+        If T[i, j] != 0, distance between X1[i] and X2[j] will
+        be computed. If None, equivalent to cdist.
+
+    metric: str = "sqeuclidean"
+        Metric to use in distance computation. These metrics must
+        be implemented with the @njit tag, so only a few are available
+        at this point. More will come as needs grow.
+        Valid metrics: "sqeuclidean", "euclidean"
+    """
+    if X2 is None:
+        X2 = X1
+    if T is None:
+        warn(
+            "Using sparse_cdist without a matching is useless."
+            "Use scipy's cdist instead."
+        )
+        return csr_matrix(cdist(X1, X2, metric=metric))
+    T = T.tocoo()
+    if metric == "sqeuclidean":
+        dfunc = dfunc_sqeuclidean
+    elif metric == "euclidean":
+        dfunc = dfunc_euclidean
+    else:
+        raise NotImplementedError("Unrecognized metric.")
+    data = sparse_cdist_njit(X1, X2, T.row, T.col, dfunc)
+    return coo_matrix((data, (T.row, T.col)), shape=T.shape).tocsr()
+
+
+@njit(fastmath=True)
+def sparse_cdist_njit(X1, X2, row, col, dfunc):
+    data = np.zeros(row.shape)
+    for k, (i, j) in enumerate(zip(row, col)):
+        data[k] = dfunc(X1[i], X2[j])
+    return data
+
+
+@njit
+def dfunc_sqeuclidean(x, y):
+    return (x - y) @ (x - y)
+
+
+@njit
+def dfunc_euclidean(x, y):
+    return np.sqrt(dfunc_sqeuclidean(x, y))
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/graph.py` & `transmorph-0.2.7/src/transmorph/utils/graph.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,721 +1,721 @@
-#!/usr/bin/env python3
-
-import anndata as ad
-import igraph as ig
-import leidenalg as la
-import numpy as np
-import scanpy as sc
-import warnings
-
-from anndata import AnnData
-from numba import njit
-from numpy.random import RandomState
-from pynndescent import NNDescent
-from scipy.spatial.distance import cdist
-from scipy.sparse import csr_matrix
-from scipy.sparse.csgraph import dijkstra
-from sklearn import neighbors as skn
-from typing import Dict, List, Literal, Optional, Tuple
-
-from .anndata_manager import anndata_manager as adm
-from .geometry import sparse_cdist
-from .matrix import (
-    extract_chunks,
-    sort_sparse_matrix,
-    sparse_from_arrays,
-)
-
-
-def nearest_neighbors_custom(
-    X: np.ndarray,
-    mode: Literal["edges", "distances"],
-    n_neighbors: int = 15,
-    Y: Optional[np.ndarray] = None,
-) -> csr_matrix:
-    """
-    Wraps sklearn.neighbors.NearestNeighbors class.
-    """
-    if Y is None:
-        Y = X
-    nn_model = skn.NearestNeighbors(n_neighbors=n_neighbors).fit(Y)
-    if mode == "edges":
-        return nn_model.kneighbors_graph(X, mode="connectivity")
-    elif mode == "distances":
-        return nn_model.kneighbors_graph(X, mode="distance").toarray()
-    else:
-        raise ValueError(f"Unrecognized mode: {mode}")
-
-
-def nearest_neighbors(
-    adata: ad.AnnData,
-    mode: Literal["edges", "distances", "connectivities"],
-    neighbors_key: str = "neighbors",
-    n_neighbors: int = 15,
-    metric: str = "euclidean",
-    metric_kwargs: Dict = {},
-    use_pca: bool = True,
-    random_state: Optional[RandomState] = None,
-) -> csr_matrix:
-    """
-    Encapsulates k-nearest neighbors algorithms.
-
-    Parameters
-    ----------
-    X: np.ndarray
-        Vectorized dataset to compute nearest neighbors from.
-
-    metric: str or Callable, default = "sqeuclidean"
-        scipy-compatible metric used to compute nearest neighbors.
-
-    metric_kwargs: dict, default = {}
-        Additional metric arguments for scipy.spatial.distance.cdist.
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use between datasets.
-
-    mode: Literal["distances", "edges"], default = "distances"
-        Type of data contained in the returned matrix.
-
-    use_pcs: int, default = 30
-        If X.shape[1] > use_pcs, a PC view will be used instead of X.
-        Set it to None to disable this functionality.
-
-    algorithm: str, default = "auto"
-        Solver to use in "auto", "sklearn" and "nndescent". Use "sklearn"
-        for small datasets or if the solution must be exact, use "nndescent"
-        for large datasets if an approached solution is enough. With "auto",
-        the function will adapt to dataset size.
-    """
-    assert isinstance(
-        adata, ad.AnnData
-    ), f"AnnData expected, found {type(adata).__name__}."
-    assert mode in ["edges", "distances", "connectivities"]
-    if (
-        neighbors_key not in adata.uns
-        or "params" not in adata.uns[neighbors_key]
-        or "n_neighbors" not in adata.uns[neighbors_key]["params"]
-        or "metric" not in adata.uns[neighbors_key]["params"]
-        or adata.uns[neighbors_key]["params"]["n_neighbors"] < n_neighbors
-        or adata.uns[neighbors_key]["params"]["metric"] != metric
-    ):
-        from .._settings import settings, use_setting
-
-        if use_pca and "X_pca" not in adata.obsm:
-            sc.pp.pca(adata)
-        sc.pp.neighbors(
-            adata,
-            n_neighbors=n_neighbors,
-            metric=metric,
-            metric_kwds=metric_kwargs,
-            method="umap",
-            random_state=use_setting(random_state, settings.global_random_seed),
-        )
-    if mode == "edges":
-        return adata.obsp["distances"].astype(bool)
-    elif mode == "distances":
-        return adata.obsp["distances"]
-    elif mode == "connectivities":
-        return adata.obsp["connectivities"]
-
-
-def distance_to_knn(D: np.ndarray, k: int, axis: int):
-    """
-    Returns the distance of each point along the specified axis to its kth
-    nearest neighbor, given a distance matrix D.
-    """
-    if k == 0:  # 0-th neighbor of a point is itself
-        return np.zeros(D.shape[1 - axis], dtype=np.float32)
-    D_sorted = np.sort(D, axis=axis)
-    if axis == 0:
-        D_sorted = D_sorted.T
-    return D_sorted[:, k - 1]
-
-
-def generate_qtree(
-    X: np.ndarray, metric: str, metric_kwargs: Optional[Dict] = None
-) -> NNDescent:
-    """
-    Returns a fitted tree based on points from X, which can be
-    then queried for another set of points.
-    """
-    if metric_kwargs is None:
-        metric_kwargs = {}
-    qtree = NNDescent(X, metric=metric, metric_kwds=metric_kwargs)
-    qtree.prepare()
-    return qtree
-
-
-def qtree_k_nearest_neighbors(
-    X: np.ndarray,
-    qtY: NNDescent,
-    n_neighbors: int = 10,
-) -> csr_matrix:
-    """
-    Returns k nearest neighbors between X and Y using a k-d tree
-    algorithm, as a csr_matrix.
-
-    Parameters
-    ----------
-    X: np.ndarray
-        First dataset, will be in rows in the final matrix
-
-    Y: np.ndarray
-        Second dataset, in columns in the final matrix
-
-    qtX: NNDescent
-        Precomputed index for X samples
-
-    qtY: NNDescent
-        Precomputed index for Y samples
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use to build the intersection.
-    """
-    return sparse_from_arrays(
-        qtY.query(X, k=n_neighbors)[0],
-        n_cols=qtY._raw_data.shape[0],
-    )
-
-
-def qtree_mutual_nearest_neighbors(
-    X: np.ndarray,
-    Y: np.ndarray,
-    qtX: NNDescent,
-    qtY: NNDescent,
-    n_neighbors: int = 10,
-) -> csr_matrix:
-    """
-    Accelerated mutual nearest neighbors scheme using NNDescent.
-    It requires precomputed indexes that can be queried.
-
-    Parameters
-    ----------
-    X: np.ndarray
-        First dataset, will be in rows in the final matrix
-
-    Y: np.ndarray
-        Second dataset, in columns in the final matrix
-
-    qtX: NNDescent
-        Precomputed index for X samples
-
-    qtY: NNDescent
-        Precomputed index for Y samples
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use to build the intersection.
-    """
-    XYknn = qtree_k_nearest_neighbors(X, qtY, n_neighbors)
-    YXknn = qtree_k_nearest_neighbors(Y, qtX, n_neighbors)
-    return XYknn.multiply(YXknn.T).astype(np.float32)
-
-
-def raw_mutual_nearest_neighbors(
-    X: np.ndarray,
-    Y: np.ndarray,
-    metric: str = "sqeuclidean",
-    metric_kwargs: Dict = {},
-    n_neighbors: int = 10,
-) -> csr_matrix:
-    """
-    Runs mutual nearest neighbors algorithm between datasets X and Y.
-    x \\in X and y \\in Y are mutual nearest neighbors if
-    - y belongs to the $k nearest neighbors of x in Y
-    AND
-    - x belongs to the $k nearest neighbors of y in X
-
-    You can choose between two methods:
-    - The exact MNN solver, with high fiability but which can become
-      computationally prohibitive when datasets scale over tens of
-      thousands of samples.
-    - An experimental approached solver, which matches samples between
-      matched clusters, less fiable but more tractable for large problems.
-      This solver will be subject to improvements.
-
-    Parameters
-    ----------
-    X: np.ndarray
-        First dataset of shape (n,d)
-
-    Y: np.ndarray
-        Second dataset of shape (m,d)
-
-    metric: str, default = "sqeuclidean"
-        scipy-compatible metric to use.
-
-    metric_kwargs: Dict, default = {}
-        Additional parameters for metric
-
-    n_neighbors: int, default = 10
-        Number of neighbors to use between datasets.
-
-    algorithm: str, default = "auto"
-        Method to use ("auto", "exact" or "nndescent"). If "auto", will
-        choose "exact" for small datasets and "nndescent" for large ones.
-
-    low_memory: bool, default = False
-        Run pynndescent using high time/low memory profile for large
-        datasets. Turn it on for very large datasets where memory is an
-        issue.
-
-    n_jobs: int = -1
-        Number of jobs to pass to sklearn nearest_neighbors function.
-
-    Returns
-    -------
-    T = (n,m) csr_matrix where T[i,j] = (xi and yj MNN)
-    """
-    nx, ny = X.shape[0], Y.shape[0]
-    if min(nx, ny) < n_neighbors:
-        warnings.warn("Y.shape[0] < n_neighbors. " "Setting n_neighbors to Y.shape[0].")
-        n_neighbors = min(nx, ny)
-    D = cdist(X, Y, metric=metric, **metric_kwargs)
-    dx = distance_to_knn(D, n_neighbors, 1)
-    dy = distance_to_knn(D, n_neighbors, 0)
-    Dxy = np.minimum.outer(dx, dy)
-    return csr_matrix((D <= Dxy), shape=D.shape, dtype=np.float32)
-
-
-def combine_matchings(
-    matchings: Dict[Tuple[int, int], csr_matrix],
-    knn_graphs: Optional[List[csr_matrix]] = None,
-    symmetrize: bool = True,
-    target_edges: int = 10,
-) -> csr_matrix:
-    """
-    Concatenates any number of matchings Mij and knn-graph
-    adjacency matrices Ai in a single sparse matrix T. Diagonal
-    blocks of T is composed by Ai matrices, and ij block is
-    Mij if i < j otherwise Mji.T
-
-    matching: MatchingABC
-        A fitted MatchingABC object with no reference.
-
-    knn_graph: Optional[List[csr_matrix]]
-        List of knn-graphs, where knn-graph[i] is the knn-graph
-        associated to matching.datasets[i]. Ignored if left empty.
-    """
-    # Retrieves information in case knn_graph is missing
-    assert matchings.get((0, 1), None) is not None, "No matching provided."
-    ndatasets = max(max(matchings.keys(), key=lambda k: max(k))) + 1
-    sizes = [matchings[0, 1].shape[0]]
-    sizes += [matchings[0, i].shape[1] for i in range(1, ndatasets)]
-    # Loading these containers
-    rows, cols, data = [], [], []
-    # This mask allows to modify matching edges,
-    # in order to increase their weight to select
-    # them in priority compared to knn edges.
-    rowsm, colsm, datam = [], [], []
-    offset_i: int = 0
-    for i in range(ndatasets):
-        # Initial relations
-        if knn_graphs is not None:
-            knn_graph = knn_graphs[i].tocoo()
-            rows += list(knn_graph.row + offset_i)
-            cols += list(knn_graph.col + offset_i)
-            data += list(knn_graph.data)
-        offset_j: int = 0
-        for j in range(ndatasets):
-            if i == j:
-                offset_j += sizes[i]
-                continue
-            T = matchings[i, j].tocoo()
-            rows_k, cols_k, data_k = T.row, T.col, T.data
-            rows_k += offset_i
-            cols_k += offset_j
-            rows += list(rows_k)
-            cols += list(cols_k)
-            data += list(data_k)
-            rowsm += list(rows_k)
-            colsm += list(cols_k)
-            datam += [10000] * rows_k.shape[0]
-            offset_j += sizes[j]
-        offset_i += sizes[i]
-
-    # We select only top weighted edges, and in priority the ones
-    # from matching matrices by scaling them by a large factor
-    N = sum(sizes)
-    T = csr_matrix((data, (rows, cols)), shape=(N, N))
-    T_mask = csr_matrix((data, (rows, cols)), shape=(N, N))
-    ind, val = sort_sparse_matrix(T.multiply(T_mask), fill_empty=True, reverse=True)
-    T = sparse_from_arrays(ind[:, :target_edges], val[:, :target_edges])
-    T_mask.data = 1.0 / T_mask.data
-    T = T.multiply(T_mask)
-    T.data = np.clip(T.data, 0.0, 1.0)
-    if symmetrize:
-        T = T + T.T - T.multiply(T.T)  # symmetrize
-    return T
-
-
-def generate_membership_matrix(
-    G: csr_matrix,
-    X1: np.ndarray,
-    X2: np.ndarray,
-    max_iter: int = 64,
-    tol: float = 1e-5,
-    low_thr: float = 1e-6,
-) -> csr_matrix:
-    """
-    Converts a graph matrix G between two datasets X1 and X2 embedded in the same
-    space to a distance-based membership matrix, ready to be embedded by UMAP or
-    MDE optimizers. Adapted from umap-learn package.
-    """
-    # Sanity checks
-    assert G.shape == (X1.shape[0], X2.shape[0])
-
-    # Retrieving distances is possible, otherwise guessing them
-    if X1.shape[1] != X2.shape[1]:  # Not same space
-        G_dist = G / G.max()
-        G_dist.data = 1.0 / (1.0 + G_dist.data)  # FIXME?
-    else:  # Same space
-        G_dist = sparse_cdist(X1, X2, G, metric="euclidean")
-
-    # Initialization
-    indices, distances = sort_sparse_matrix(G_dist, fill_empty=True)
-    distances = _generate_membership_matrix_njit(
-        distances,
-        max_iter,
-        tol,
-    )
-    membership = sparse_from_arrays(indices, distances, n_cols=X2.shape[0])
-    assert membership.max() != np.inf, "np.inf deteceted in $membership."
-    membership.data[membership.data < low_thr] = 0.0
-    membership.eliminate_zeros()
-    return membership
-
-
-@njit(fastmath=True)
-def _generate_membership_matrix_njit(
-    distances: np.ndarray,
-    max_iter: int,
-    tol: float,
-) -> np.ndarray:
-    """
-    Numba accelerated helper
-    """
-    distances = distances.copy()
-
-    n1 = distances.shape[0]
-    # Binary search
-    for row_i in range(n1):
-
-        # Skip the line if empty
-        if distances[row_i, 0] == np.inf:
-            continue
-
-        low = 0.0
-        mid = 1.0
-        high = np.inf
-
-        rhos_i = distances[row_i, 0]
-        k = 0
-        for r in distances[row_i]:
-            if r != np.inf:
-                k += 1
-        target_log2k = np.log2(k)
-
-        for _ in range(max_iter):
-
-            cand_log2k = 0.0
-            for j in range(k):
-
-                # End of neighbors
-                if distances[row_i, j] == np.inf:
-                    continue
-
-                d = distances[row_i, j] - rhos_i
-                if d <= 0:
-                    cand_log2k += 1
-                else:
-                    cand_log2k += np.exp(-(d / mid))
-
-            if np.abs(cand_log2k - target_log2k) < tol:
-                break
-
-            if cand_log2k > target_log2k:
-                high = mid
-                mid = (low + high) / 2.0
-            else:
-                low = mid
-                if high is np.inf:
-                    mid *= 2.0
-                else:
-                    mid = (low + high) / 2.0
-
-        distances[row_i] = np.exp(-np.clip(distances[row_i] - rhos_i, 0, None) / mid)
-
-    return distances
-
-
-def get_nearest_vertex_from_set(
-    indices: np.ndarray,
-    distances: np.ndarray,
-    vset: np.ndarray,
-) -> np.ndarray:
-    """
-    Returns for each vertex the closest vertex from vset along graph G edges.
-    If the connected component of a vertex contains no vertex from vset,
-    its nearest vertex from vset if set to -1.
-
-    Parameters
-    ----------
-    indices, distances: np.ndarray
-        Edge/Distance matrices of shape (n, k) representing the knn graph.
-
-    vset: np.ndarray
-        Boolean vector representing vertices of the target set.
-
-    TODO: This could be done more intelligenlty without redundant pathing.
-          It will do the job for now.
-    """
-    nvertices = indices.shape[0]
-    # Default is -1
-    result = np.zeros((nvertices,), dtype=int) - 1
-    for i in range(nvertices):
-        # List of (idx, dist to vi)
-        to_visit = [(i, 0.0)]
-        visited = set([i])
-        while len(to_visit) > 0:
-            current_v, dv = to_visit.pop(0)
-            # Vertex from vset is found
-            if vset[current_v]:
-                result[i] = current_v
-                break
-            # Adds unvisited vertices to to_visit, sorted
-            for nb, dnb in zip(indices[current_v], distances[current_v]):
-                if nb == -1 or nb in visited:
-                    continue
-                visited.add(nb)
-                dnb += dv
-                inserted = False
-                for k, (_, tot_d) in enumerate(to_visit):
-                    if tot_d >= dnb:
-                        inserted = True
-                        to_visit.insert(k, (nb, dnb))
-                        break
-                if not inserted:
-                    to_visit.append((nb, dnb))
-    return result
-
-
-def cluster_anndatas(
-    datasets: List[AnnData],
-    use_rep: Optional[str] = None,
-    cluster_key: str = "cluster",
-    n_neighbors: int = 15,
-    resolution: float = 1.0,
-) -> None:
-    """
-    Runs Leiden algorithm on a set of concatenated anndatas objects embedded in a
-    common space. Writes clustering results in the AnnData objects.
-
-    Parameters
-    ----------
-    datasets: List[AnnData]
-        AnnData objects to concatenante and cluster.
-
-    use_rep: Optional[str], default = None
-        Embedding to use, if None will use .obsm["transmorph"] in priority or raise
-        an error if it is not found.
-
-    cluster_key: str, default = "cluster"
-        Key to save clusters in .obs
-
-    n_neighbors: int, default = 10
-        Number of neighbors to build the kNN graph.
-
-    resolution: float, default = 1.0
-        Leiden algorithm parameter.
-    """
-    if use_rep is None:
-        use_rep = "transmorph"
-    assert all(
-        adm.isset_value(adata, key=use_rep, field="obsm") for adata in datasets
-    ), f"{use_rep} missing in .obsm of some AnnDatas."
-    X = np.concatenate(
-        [adata.obsm[use_rep] for adata in datasets],
-        axis=0,
-    )
-    adj_matrix = nearest_neighbors_custom(X, mode="edges", n_neighbors=n_neighbors)
-    sources, targets = adj_matrix.nonzero()
-    edgelist = zip(sources.tolist(), targets.tolist())
-    partition = np.array(
-        la.find_partition(
-            ig.Graph(edgelist),
-            la.RBConfigurationVertexPartition,
-            resolution_parameter=resolution,
-        ).membership
-    )
-    cluster_obs = extract_chunks(partition, [adata.n_obs for adata in datasets])
-    for adata, obs in zip(datasets, cluster_obs):
-        adm.set_value(adata, key=cluster_key, field="obs", value=obs, persist="output")
-
-
-def node_geodesic_distances(adj: csr_matrix, directed: bool = True) -> np.ndarray:
-    """
-    Computes all distances between vertices of a graph
-    represented as matrix $adj, where edges are weighted
-    with length between vertices.
-
-    TODO: additional parameters?
-    """
-    return dijkstra(adj, directed=directed)
-
-
-def prune_edges_supervised(
-    matchings: Dict[Tuple[int, int], csr_matrix],
-    labels: List[np.ndarray],
-) -> Dict[Tuple[int, int], csr_matrix]:
-    """
-    Selects only matching edges connected samples from the same class.
-    """
-    results = {}
-    for i, j in matchings:
-        T = matchings[i, j].tocoo()
-        for k in range(T.data.shape[0]):
-            row, col = T.row[k], T.col[k]
-            if labels[i][row] != labels[j][col]:
-                T.data[k] = 0.0
-        T.eliminate_zeros()
-        results[i, j] = T.tocsr()
-    return results
-
-
-def count_total_matching_edges(matchings: Dict[Tuple[int, int], csr_matrix]) -> int:
-    nedges = 0
-    for key in matchings:
-        nedges += matchings[key].count_nonzero()
-    return nedges
-
-
-@njit()
-def csr_get_row(
-    indices: np.ndarray, K_indices: int, indptr: np.ndarray, K_indptrs: int, i: int
-) -> np.ndarray:
-    sj = indptr[i]
-    if i == K_indptrs - 1:
-        Sj = K_indices
-    else:
-        Sj = indptr[i + 1]
-    return indices[sj:Sj]
-
-
-@njit
-def prune_non_transitive_njit(
-    matching_indices: np.ndarray,
-    matching_indices_K: np.ndarray,
-    matching_indptrs: np.ndarray,
-    matching_indptrs_K: np.ndarray,
-    batch_i: int,
-    batch_j: int,
-    Tij_row: np.ndarray,
-    Tij_col: np.ndarray,
-    n_batches: int,
-    min_patterns: int,
-) -> np.ndarray:
-    new_edges = np.zeros(Tij_row.shape)
-    for idx in range(Tij_row.shape[0]):
-        sample_i, sample_j = Tij_row[idx], Tij_col[idx]
-        for batch_k in range(n_batches):
-            if batch_k in (batch_i, batch_j):
-                continue
-            matches_j = csr_get_row(
-                matching_indices[batch_j, batch_k],
-                matching_indices_K[batch_j, batch_k],
-                matching_indptrs[batch_j, batch_k],
-                matching_indptrs_K[batch_j, batch_k],
-                sample_j,
-            )
-            for sample_k in matches_j:
-                matches_k = csr_get_row(
-                    matching_indices[batch_k, batch_i],
-                    matching_indices_K[batch_k, batch_i],
-                    matching_indptrs[batch_k, batch_i],
-                    matching_indptrs_K[batch_k, batch_i],
-                    sample_k,
-                )
-                if sample_i in matches_k:
-                    new_edges[idx] += 1
-                    break
-    return new_edges > min_patterns
-
-
-def prune_edges_unsupervised(
-    matchings: Dict[Tuple[int, int], csr_matrix],
-    n_batches: int,
-    min_patterns: int,
-) -> Dict[Tuple[int, int], csr_matrix]:
-    """
-    Blabla
-    """
-    max_indices = np.max([matchings[key].indices.shape[0] for key in matchings])
-    max_indptrs = np.max([matchings[key].indptr.shape[0] for key in matchings])
-
-    # matching_indices[i, j] = Tij.indices, filled with -1 on the right
-    # matching_indices_K[i, j] = # of non-(-1) values
-    matching_indices = (
-        np.zeros(shape=(n_batches, n_batches, max_indices), dtype=int) - 1
-    )
-    matching_indices_K = np.zeros(shape=(n_batches, n_batches), dtype=int)
-
-    # matching_indptrs[i, j] = Tij.indptrs, filled with -1 on the right
-    # matching_indptrs_K[i, j] = # of non-(-1) values
-    matching_indptrs = (
-        np.zeros(shape=(n_batches, n_batches, max_indptrs), dtype=int) - 1
-    )
-    matching_indptrs_K = np.zeros(shape=(n_batches, n_batches), dtype=int)
-
-    for i in range(n_batches):
-        for j in range(n_batches):
-            if i == j:
-                continue
-            else:
-                Tij = matchings[i, j]
-
-                Kptr = Tij.indptr.shape[0]
-                matching_indptrs_K[i, j] = Kptr
-                matching_indptrs[i, j][0:Kptr] = Tij.indptr
-
-                Kind = Tij.indices.shape[0]
-                matching_indices_K[i, j] = Kind
-                matching_indices[i, j][0:Kind] = Tij.indices
-
-    result_matchings = {}
-    for i, j in matchings:
-        Tij_coo = matchings[i, j].tocoo()
-        new_edges = prune_non_transitive_njit(
-            matching_indices=matching_indices,
-            matching_indices_K=matching_indices_K,
-            matching_indptrs=matching_indptrs,
-            matching_indptrs_K=matching_indptrs_K,
-            batch_i=i,
-            batch_j=j,
-            Tij_col=Tij_coo.col,
-            Tij_row=Tij_coo.row,
-            n_batches=n_batches,
-            min_patterns=min_patterns,
-        )
-        result_matchings[i, j] = Tij_coo.tocsr()
-        result_matchings[i, j].data = new_edges
-        result_matchings[i, j].eliminate_zeros()
-
-    return result_matchings
-
-
-@njit
-def smooth_correction_vectors(
-    X: np.ndarray,
-    v: np.ndarray,
-    nn_indices: np.ndarray,
-    nn_distances: np.ndarray,
-    n_neighbors: int = 5,
-) -> np.ndarray:
-    """
-    Applies smoothing to a vector space.
-    """
-    new_correction = np.zeros(v.shape)
-    for i, vi in enumerate(v):
-        local_vs = v[nn_indices[i, :n_neighbors]]
-        for j, v_nb_j in enumerate(local_vs):
-            new_correction[i] += v_nb_j
-    return new_correction / n_neighbors
+#!/usr/bin/env python3
+
+import anndata as ad
+import igraph as ig
+import leidenalg as la
+import numpy as np
+import scanpy as sc
+import warnings
+
+from anndata import AnnData
+from numba import njit
+from numpy.random import RandomState
+from pynndescent import NNDescent
+from scipy.spatial.distance import cdist
+from scipy.sparse import csr_matrix
+from scipy.sparse.csgraph import dijkstra
+from sklearn import neighbors as skn
+from typing import Dict, List, Literal, Optional, Tuple
+
+from .anndata_manager import anndata_manager as adm
+from .geometry import sparse_cdist
+from .matrix import (
+    extract_chunks,
+    sort_sparse_matrix,
+    sparse_from_arrays,
+)
+
+
+def nearest_neighbors_custom(
+    X: np.ndarray,
+    mode: Literal["edges", "distances"],
+    n_neighbors: int = 15,
+    Y: Optional[np.ndarray] = None,
+) -> csr_matrix:
+    """
+    Wraps sklearn.neighbors.NearestNeighbors class.
+    """
+    if Y is None:
+        Y = X
+    nn_model = skn.NearestNeighbors(n_neighbors=n_neighbors).fit(Y)
+    if mode == "edges":
+        return nn_model.kneighbors_graph(X, mode="connectivity")
+    elif mode == "distances":
+        return nn_model.kneighbors_graph(X, mode="distance").toarray()
+    else:
+        raise ValueError(f"Unrecognized mode: {mode}")
+
+
+def nearest_neighbors(
+    adata: ad.AnnData,
+    mode: Literal["edges", "distances", "connectivities"],
+    neighbors_key: str = "neighbors",
+    n_neighbors: int = 15,
+    metric: str = "euclidean",
+    metric_kwargs: Dict = {},
+    use_pca: bool = True,
+    random_state: Optional[RandomState] = None,
+) -> csr_matrix:
+    """
+    Encapsulates k-nearest neighbors algorithms.
+
+    Parameters
+    ----------
+    X: np.ndarray
+        Vectorized dataset to compute nearest neighbors from.
+
+    metric: str or Callable, default = "sqeuclidean"
+        scipy-compatible metric used to compute nearest neighbors.
+
+    metric_kwargs: dict, default = {}
+        Additional metric arguments for scipy.spatial.distance.cdist.
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use between datasets.
+
+    mode: Literal["distances", "edges"], default = "distances"
+        Type of data contained in the returned matrix.
+
+    use_pcs: int, default = 30
+        If X.shape[1] > use_pcs, a PC view will be used instead of X.
+        Set it to None to disable this functionality.
+
+    algorithm: str, default = "auto"
+        Solver to use in "auto", "sklearn" and "nndescent". Use "sklearn"
+        for small datasets or if the solution must be exact, use "nndescent"
+        for large datasets if an approached solution is enough. With "auto",
+        the function will adapt to dataset size.
+    """
+    assert isinstance(
+        adata, ad.AnnData
+    ), f"AnnData expected, found {type(adata).__name__}."
+    assert mode in ["edges", "distances", "connectivities"]
+    if (
+        neighbors_key not in adata.uns
+        or "params" not in adata.uns[neighbors_key]
+        or "n_neighbors" not in adata.uns[neighbors_key]["params"]
+        or "metric" not in adata.uns[neighbors_key]["params"]
+        or adata.uns[neighbors_key]["params"]["n_neighbors"] < n_neighbors
+        or adata.uns[neighbors_key]["params"]["metric"] != metric
+    ):
+        from .._settings import settings, use_setting
+
+        if use_pca and "X_pca" not in adata.obsm:
+            sc.pp.pca(adata)
+        sc.pp.neighbors(
+            adata,
+            n_neighbors=n_neighbors,
+            metric=metric,
+            metric_kwds=metric_kwargs,
+            method="umap",
+            random_state=use_setting(random_state, settings.global_random_seed),
+        )
+    if mode == "edges":
+        return adata.obsp["distances"].astype(bool)
+    elif mode == "distances":
+        return adata.obsp["distances"]
+    elif mode == "connectivities":
+        return adata.obsp["connectivities"]
+
+
+def distance_to_knn(D: np.ndarray, k: int, axis: int):
+    """
+    Returns the distance of each point along the specified axis to its kth
+    nearest neighbor, given a distance matrix D.
+    """
+    if k == 0:  # 0-th neighbor of a point is itself
+        return np.zeros(D.shape[1 - axis], dtype=np.float32)
+    D_sorted = np.sort(D, axis=axis)
+    if axis == 0:
+        D_sorted = D_sorted.T
+    return D_sorted[:, k - 1]
+
+
+def generate_qtree(
+    X: np.ndarray, metric: str, metric_kwargs: Optional[Dict] = None
+) -> NNDescent:
+    """
+    Returns a fitted tree based on points from X, which can be
+    then queried for another set of points.
+    """
+    if metric_kwargs is None:
+        metric_kwargs = {}
+    qtree = NNDescent(X, metric=metric, metric_kwds=metric_kwargs)
+    qtree.prepare()
+    return qtree
+
+
+def qtree_k_nearest_neighbors(
+    X: np.ndarray,
+    qtY: NNDescent,
+    n_neighbors: int = 10,
+) -> csr_matrix:
+    """
+    Returns k nearest neighbors between X and Y using a k-d tree
+    algorithm, as a csr_matrix.
+
+    Parameters
+    ----------
+    X: np.ndarray
+        First dataset, will be in rows in the final matrix
+
+    Y: np.ndarray
+        Second dataset, in columns in the final matrix
+
+    qtX: NNDescent
+        Precomputed index for X samples
+
+    qtY: NNDescent
+        Precomputed index for Y samples
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use to build the intersection.
+    """
+    return sparse_from_arrays(
+        qtY.query(X, k=n_neighbors)[0],
+        n_cols=qtY._raw_data.shape[0],
+    )
+
+
+def qtree_mutual_nearest_neighbors(
+    X: np.ndarray,
+    Y: np.ndarray,
+    qtX: NNDescent,
+    qtY: NNDescent,
+    n_neighbors: int = 10,
+) -> csr_matrix:
+    """
+    Accelerated mutual nearest neighbors scheme using NNDescent.
+    It requires precomputed indexes that can be queried.
+
+    Parameters
+    ----------
+    X: np.ndarray
+        First dataset, will be in rows in the final matrix
+
+    Y: np.ndarray
+        Second dataset, in columns in the final matrix
+
+    qtX: NNDescent
+        Precomputed index for X samples
+
+    qtY: NNDescent
+        Precomputed index for Y samples
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use to build the intersection.
+    """
+    XYknn = qtree_k_nearest_neighbors(X, qtY, n_neighbors)
+    YXknn = qtree_k_nearest_neighbors(Y, qtX, n_neighbors)
+    return XYknn.multiply(YXknn.T).astype(np.float32)
+
+
+def raw_mutual_nearest_neighbors(
+    X: np.ndarray,
+    Y: np.ndarray,
+    metric: str = "sqeuclidean",
+    metric_kwargs: Dict = {},
+    n_neighbors: int = 10,
+) -> csr_matrix:
+    """
+    Runs mutual nearest neighbors algorithm between datasets X and Y.
+    x \\in X and y \\in Y are mutual nearest neighbors if
+    - y belongs to the $k nearest neighbors of x in Y
+    AND
+    - x belongs to the $k nearest neighbors of y in X
+
+    You can choose between two methods:
+    - The exact MNN solver, with high fiability but which can become
+      computationally prohibitive when datasets scale over tens of
+      thousands of samples.
+    - An experimental approached solver, which matches samples between
+      matched clusters, less fiable but more tractable for large problems.
+      This solver will be subject to improvements.
+
+    Parameters
+    ----------
+    X: np.ndarray
+        First dataset of shape (n,d)
+
+    Y: np.ndarray
+        Second dataset of shape (m,d)
+
+    metric: str, default = "sqeuclidean"
+        scipy-compatible metric to use.
+
+    metric_kwargs: Dict, default = {}
+        Additional parameters for metric
+
+    n_neighbors: int, default = 10
+        Number of neighbors to use between datasets.
+
+    algorithm: str, default = "auto"
+        Method to use ("auto", "exact" or "nndescent"). If "auto", will
+        choose "exact" for small datasets and "nndescent" for large ones.
+
+    low_memory: bool, default = False
+        Run pynndescent using high time/low memory profile for large
+        datasets. Turn it on for very large datasets where memory is an
+        issue.
+
+    n_jobs: int = -1
+        Number of jobs to pass to sklearn nearest_neighbors function.
+
+    Returns
+    -------
+    T = (n,m) csr_matrix where T[i,j] = (xi and yj MNN)
+    """
+    nx, ny = X.shape[0], Y.shape[0]
+    if min(nx, ny) < n_neighbors:
+        warnings.warn("Y.shape[0] < n_neighbors. " "Setting n_neighbors to Y.shape[0].")
+        n_neighbors = min(nx, ny)
+    D = cdist(X, Y, metric=metric, **metric_kwargs)
+    dx = distance_to_knn(D, n_neighbors, 1)
+    dy = distance_to_knn(D, n_neighbors, 0)
+    Dxy = np.minimum.outer(dx, dy)
+    return csr_matrix((D <= Dxy), shape=D.shape, dtype=np.float32)
+
+
+def combine_matchings(
+    matchings: Dict[Tuple[int, int], csr_matrix],
+    knn_graphs: Optional[List[csr_matrix]] = None,
+    symmetrize: bool = True,
+    target_edges: int = 10,
+) -> csr_matrix:
+    """
+    Concatenates any number of matchings Mij and knn-graph
+    adjacency matrices Ai in a single sparse matrix T. Diagonal
+    blocks of T is composed by Ai matrices, and ij block is
+    Mij if i < j otherwise Mji.T
+
+    matching: MatchingABC
+        A fitted MatchingABC object with no reference.
+
+    knn_graph: Optional[List[csr_matrix]]
+        List of knn-graphs, where knn-graph[i] is the knn-graph
+        associated to matching.datasets[i]. Ignored if left empty.
+    """
+    # Retrieves information in case knn_graph is missing
+    assert matchings.get((0, 1), None) is not None, "No matching provided."
+    ndatasets = max(max(matchings.keys(), key=lambda k: max(k))) + 1
+    sizes = [matchings[0, 1].shape[0]]
+    sizes += [matchings[0, i].shape[1] for i in range(1, ndatasets)]
+    # Loading these containers
+    rows, cols, data = [], [], []
+    # This mask allows to modify matching edges,
+    # in order to increase their weight to select
+    # them in priority compared to knn edges.
+    rowsm, colsm, datam = [], [], []
+    offset_i: int = 0
+    for i in range(ndatasets):
+        # Initial relations
+        if knn_graphs is not None:
+            knn_graph = knn_graphs[i].tocoo()
+            rows += list(knn_graph.row + offset_i)
+            cols += list(knn_graph.col + offset_i)
+            data += list(knn_graph.data)
+        offset_j: int = 0
+        for j in range(ndatasets):
+            if i == j:
+                offset_j += sizes[i]
+                continue
+            T = matchings[i, j].tocoo()
+            rows_k, cols_k, data_k = T.row, T.col, T.data
+            rows_k += offset_i
+            cols_k += offset_j
+            rows += list(rows_k)
+            cols += list(cols_k)
+            data += list(data_k)
+            rowsm += list(rows_k)
+            colsm += list(cols_k)
+            datam += [10000] * rows_k.shape[0]
+            offset_j += sizes[j]
+        offset_i += sizes[i]
+
+    # We select only top weighted edges, and in priority the ones
+    # from matching matrices by scaling them by a large factor
+    N = sum(sizes)
+    T = csr_matrix((data, (rows, cols)), shape=(N, N))
+    T_mask = csr_matrix((data, (rows, cols)), shape=(N, N))
+    ind, val = sort_sparse_matrix(T.multiply(T_mask), fill_empty=True, reverse=True)
+    T = sparse_from_arrays(ind[:, :target_edges], val[:, :target_edges])
+    T_mask.data = 1.0 / T_mask.data
+    T = T.multiply(T_mask)
+    T.data = np.clip(T.data, 0.0, 1.0)
+    if symmetrize:
+        T = T + T.T - T.multiply(T.T)  # symmetrize
+    return T
+
+
+def generate_membership_matrix(
+    G: csr_matrix,
+    X1: np.ndarray,
+    X2: np.ndarray,
+    max_iter: int = 64,
+    tol: float = 1e-5,
+    low_thr: float = 1e-6,
+) -> csr_matrix:
+    """
+    Converts a graph matrix G between two datasets X1 and X2 embedded in the same
+    space to a distance-based membership matrix, ready to be embedded by UMAP or
+    MDE optimizers. Adapted from umap-learn package.
+    """
+    # Sanity checks
+    assert G.shape == (X1.shape[0], X2.shape[0])
+
+    # Retrieving distances is possible, otherwise guessing them
+    if X1.shape[1] != X2.shape[1]:  # Not same space
+        G_dist = G / G.max()
+        G_dist.data = 1.0 / (1.0 + G_dist.data)  # FIXME?
+    else:  # Same space
+        G_dist = sparse_cdist(X1, X2, G, metric="euclidean")
+
+    # Initialization
+    indices, distances = sort_sparse_matrix(G_dist, fill_empty=True)
+    distances = _generate_membership_matrix_njit(
+        distances,
+        max_iter,
+        tol,
+    )
+    membership = sparse_from_arrays(indices, distances, n_cols=X2.shape[0])
+    assert membership.max() != np.inf, "np.inf deteceted in $membership."
+    membership.data[membership.data < low_thr] = 0.0
+    membership.eliminate_zeros()
+    return membership
+
+
+@njit(fastmath=True)
+def _generate_membership_matrix_njit(
+    distances: np.ndarray,
+    max_iter: int,
+    tol: float,
+) -> np.ndarray:
+    """
+    Numba accelerated helper
+    """
+    distances = distances.copy()
+
+    n1 = distances.shape[0]
+    # Binary search
+    for row_i in range(n1):
+
+        # Skip the line if empty
+        if distances[row_i, 0] == np.inf:
+            continue
+
+        low = 0.0
+        mid = 1.0
+        high = np.inf
+
+        rhos_i = distances[row_i, 0]
+        k = 0
+        for r in distances[row_i]:
+            if r != np.inf:
+                k += 1
+        target_log2k = np.log2(k)
+
+        for _ in range(max_iter):
+
+            cand_log2k = 0.0
+            for j in range(k):
+
+                # End of neighbors
+                if distances[row_i, j] == np.inf:
+                    continue
+
+                d = distances[row_i, j] - rhos_i
+                if d <= 0:
+                    cand_log2k += 1
+                else:
+                    cand_log2k += np.exp(-(d / mid))
+
+            if np.abs(cand_log2k - target_log2k) < tol:
+                break
+
+            if cand_log2k > target_log2k:
+                high = mid
+                mid = (low + high) / 2.0
+            else:
+                low = mid
+                if high is np.inf:
+                    mid *= 2.0
+                else:
+                    mid = (low + high) / 2.0
+
+        distances[row_i] = np.exp(-np.clip(distances[row_i] - rhos_i, 0, None) / mid)
+
+    return distances
+
+
+def get_nearest_vertex_from_set(
+    indices: np.ndarray,
+    distances: np.ndarray,
+    vset: np.ndarray,
+) -> np.ndarray:
+    """
+    Returns for each vertex the closest vertex from vset along graph G edges.
+    If the connected component of a vertex contains no vertex from vset,
+    its nearest vertex from vset if set to -1.
+
+    Parameters
+    ----------
+    indices, distances: np.ndarray
+        Edge/Distance matrices of shape (n, k) representing the knn graph.
+
+    vset: np.ndarray
+        Boolean vector representing vertices of the target set.
+
+    TODO: This could be done more intelligenlty without redundant pathing.
+          It will do the job for now.
+    """
+    nvertices = indices.shape[0]
+    # Default is -1
+    result = np.zeros((nvertices,), dtype=int) - 1
+    for i in range(nvertices):
+        # List of (idx, dist to vi)
+        to_visit = [(i, 0.0)]
+        visited = set([i])
+        while len(to_visit) > 0:
+            current_v, dv = to_visit.pop(0)
+            # Vertex from vset is found
+            if vset[current_v]:
+                result[i] = current_v
+                break
+            # Adds unvisited vertices to to_visit, sorted
+            for nb, dnb in zip(indices[current_v], distances[current_v]):
+                if nb == -1 or nb in visited:
+                    continue
+                visited.add(nb)
+                dnb += dv
+                inserted = False
+                for k, (_, tot_d) in enumerate(to_visit):
+                    if tot_d >= dnb:
+                        inserted = True
+                        to_visit.insert(k, (nb, dnb))
+                        break
+                if not inserted:
+                    to_visit.append((nb, dnb))
+    return result
+
+
+def cluster_anndatas(
+    datasets: List[AnnData],
+    use_rep: Optional[str] = None,
+    cluster_key: str = "cluster",
+    n_neighbors: int = 15,
+    resolution: float = 1.0,
+) -> None:
+    """
+    Runs Leiden algorithm on a set of concatenated anndatas objects embedded in a
+    common space. Writes clustering results in the AnnData objects.
+
+    Parameters
+    ----------
+    datasets: List[AnnData]
+        AnnData objects to concatenante and cluster.
+
+    use_rep: Optional[str], default = None
+        Embedding to use, if None will use .obsm["transmorph"] in priority or raise
+        an error if it is not found.
+
+    cluster_key: str, default = "cluster"
+        Key to save clusters in .obs
+
+    n_neighbors: int, default = 10
+        Number of neighbors to build the kNN graph.
+
+    resolution: float, default = 1.0
+        Leiden algorithm parameter.
+    """
+    if use_rep is None:
+        use_rep = "transmorph"
+    assert all(
+        adm.isset_value(adata, key=use_rep, field="obsm") for adata in datasets
+    ), f"{use_rep} missing in .obsm of some AnnDatas."
+    X = np.concatenate(
+        [adata.obsm[use_rep] for adata in datasets],
+        axis=0,
+    )
+    adj_matrix = nearest_neighbors_custom(X, mode="edges", n_neighbors=n_neighbors)
+    sources, targets = adj_matrix.nonzero()
+    edgelist = zip(sources.tolist(), targets.tolist())
+    partition = np.array(
+        la.find_partition(
+            ig.Graph(edgelist),
+            la.RBConfigurationVertexPartition,
+            resolution_parameter=resolution,
+        ).membership
+    )
+    cluster_obs = extract_chunks(partition, [adata.n_obs for adata in datasets])
+    for adata, obs in zip(datasets, cluster_obs):
+        adm.set_value(adata, key=cluster_key, field="obs", value=obs, persist="output")
+
+
+def node_geodesic_distances(adj: csr_matrix, directed: bool = True) -> np.ndarray:
+    """
+    Computes all distances between vertices of a graph
+    represented as matrix $adj, where edges are weighted
+    with length between vertices.
+
+    TODO: additional parameters?
+    """
+    return dijkstra(adj, directed=directed)
+
+
+def prune_edges_supervised(
+    matchings: Dict[Tuple[int, int], csr_matrix],
+    labels: List[np.ndarray],
+) -> Dict[Tuple[int, int], csr_matrix]:
+    """
+    Selects only matching edges connected samples from the same class.
+    """
+    results = {}
+    for i, j in matchings:
+        T = matchings[i, j].tocoo()
+        for k in range(T.data.shape[0]):
+            row, col = T.row[k], T.col[k]
+            if labels[i][row] != labels[j][col]:
+                T.data[k] = 0.0
+        T.eliminate_zeros()
+        results[i, j] = T.tocsr()
+    return results
+
+
+def count_total_matching_edges(matchings: Dict[Tuple[int, int], csr_matrix]) -> int:
+    nedges = 0
+    for key in matchings:
+        nedges += matchings[key].count_nonzero()
+    return nedges
+
+
+@njit()
+def csr_get_row(
+    indices: np.ndarray, K_indices: int, indptr: np.ndarray, K_indptrs: int, i: int
+) -> np.ndarray:
+    sj = indptr[i]
+    if i == K_indptrs - 1:
+        Sj = K_indices
+    else:
+        Sj = indptr[i + 1]
+    return indices[sj:Sj]
+
+
+@njit
+def prune_non_transitive_njit(
+    matching_indices: np.ndarray,
+    matching_indices_K: np.ndarray,
+    matching_indptrs: np.ndarray,
+    matching_indptrs_K: np.ndarray,
+    batch_i: int,
+    batch_j: int,
+    Tij_row: np.ndarray,
+    Tij_col: np.ndarray,
+    n_batches: int,
+    min_patterns: int,
+) -> np.ndarray:
+    new_edges = np.zeros(Tij_row.shape)
+    for idx in range(Tij_row.shape[0]):
+        sample_i, sample_j = Tij_row[idx], Tij_col[idx]
+        for batch_k in range(n_batches):
+            if batch_k in (batch_i, batch_j):
+                continue
+            matches_j = csr_get_row(
+                matching_indices[batch_j, batch_k],
+                matching_indices_K[batch_j, batch_k],
+                matching_indptrs[batch_j, batch_k],
+                matching_indptrs_K[batch_j, batch_k],
+                sample_j,
+            )
+            for sample_k in matches_j:
+                matches_k = csr_get_row(
+                    matching_indices[batch_k, batch_i],
+                    matching_indices_K[batch_k, batch_i],
+                    matching_indptrs[batch_k, batch_i],
+                    matching_indptrs_K[batch_k, batch_i],
+                    sample_k,
+                )
+                if sample_i in matches_k:
+                    new_edges[idx] += 1
+                    break
+    return new_edges > min_patterns
+
+
+def prune_edges_unsupervised(
+    matchings: Dict[Tuple[int, int], csr_matrix],
+    n_batches: int,
+    min_patterns: int,
+) -> Dict[Tuple[int, int], csr_matrix]:
+    """
+    Blabla
+    """
+    max_indices = np.max([matchings[key].indices.shape[0] for key in matchings])
+    max_indptrs = np.max([matchings[key].indptr.shape[0] for key in matchings])
+
+    # matching_indices[i, j] = Tij.indices, filled with -1 on the right
+    # matching_indices_K[i, j] = # of non-(-1) values
+    matching_indices = (
+        np.zeros(shape=(n_batches, n_batches, max_indices), dtype=int) - 1
+    )
+    matching_indices_K = np.zeros(shape=(n_batches, n_batches), dtype=int)
+
+    # matching_indptrs[i, j] = Tij.indptrs, filled with -1 on the right
+    # matching_indptrs_K[i, j] = # of non-(-1) values
+    matching_indptrs = (
+        np.zeros(shape=(n_batches, n_batches, max_indptrs), dtype=int) - 1
+    )
+    matching_indptrs_K = np.zeros(shape=(n_batches, n_batches), dtype=int)
+
+    for i in range(n_batches):
+        for j in range(n_batches):
+            if i == j:
+                continue
+            else:
+                Tij = matchings[i, j]
+
+                Kptr = Tij.indptr.shape[0]
+                matching_indptrs_K[i, j] = Kptr
+                matching_indptrs[i, j][0:Kptr] = Tij.indptr
+
+                Kind = Tij.indices.shape[0]
+                matching_indices_K[i, j] = Kind
+                matching_indices[i, j][0:Kind] = Tij.indices
+
+    result_matchings = {}
+    for i, j in matchings:
+        Tij_coo = matchings[i, j].tocoo()
+        new_edges = prune_non_transitive_njit(
+            matching_indices=matching_indices,
+            matching_indices_K=matching_indices_K,
+            matching_indptrs=matching_indptrs,
+            matching_indptrs_K=matching_indptrs_K,
+            batch_i=i,
+            batch_j=j,
+            Tij_col=Tij_coo.col,
+            Tij_row=Tij_coo.row,
+            n_batches=n_batches,
+            min_patterns=min_patterns,
+        )
+        result_matchings[i, j] = Tij_coo.tocsr()
+        result_matchings[i, j].data = new_edges
+        result_matchings[i, j].eliminate_zeros()
+
+    return result_matchings
+
+
+@njit
+def smooth_correction_vectors(
+    X: np.ndarray,
+    v: np.ndarray,
+    nn_indices: np.ndarray,
+    nn_distances: np.ndarray,
+    n_neighbors: int = 5,
+) -> np.ndarray:
+    """
+    Applies smoothing to a vector space.
+    """
+    new_correction = np.zeros(v.shape)
+    for i, vi in enumerate(v):
+        local_vs = v[nn_indices[i, :n_neighbors]]
+        for j, v_nb_j in enumerate(local_vs):
+            new_correction[i] += v_nb_j
+    return new_correction / n_neighbors
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/misc.py` & `transmorph-0.2.7/src/transmorph/utils/misc.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#!/usr/bin/env python3
-
-import numpy as np
-
-import anndata
-import random
-import string
-from typing import Any, Union, Tuple, Type
-
-MAX_ITER = 500
-
-
-def assert_type(value: Any, allowed: Union[Type, Tuple[Type, ...]]) -> None:
-    """
-    Small helper to type check.
-    """
-    if isinstance(value, allowed):
-        return
-    if isinstance(allowed, Type):
-        str_allowed = allowed.__name__
-    else:
-        str_allowed = ", ".join([_type.__name__ for _type in allowed])
-    raise TypeError(f"Unexpected type: {type(value)}. Expected {str_allowed}.")
-
-
-def rand_str(ln: int) -> str:
-    # Just a random string generator
-    return "".join(random.choices(string.ascii_letters, k=ln))
-
-
-def generate_str_elements(
-    n: int = 100,
-    ln: int = 8,
-    conserve_duplicates: bool = False,
-) -> np.ndarray:
-    # Helper function generating random features
-    elements = np.array([rand_str(ln) for _ in range(n)])
-    if conserve_duplicates:
-        return elements
-    return np.unique(elements)
-
-
-def generate_anndata(
-    obs: Union[int, np.ndarray] = 100,
-    var: Union[int, np.ndarray] = 20,
-    target_sparsity: float = 0.8,
-):
-    # Helper function generating random anndatas.
-    if isinstance(obs, int):
-        obs = np.unique(generate_str_elements(obs, 6))
-    if isinstance(var, int):
-        var = np.unique(generate_str_elements(var, 6))
-    nobs, nvar = obs.shape[0], var.shape[0]
-    X = np.random.random(size=(nobs, nvar))
-    X = X * (np.random.random(size=X.shape) > target_sparsity)
-    adata = anndata.AnnData(X, dtype=X.dtype)
-    adata.obs[None] = obs
-    adata.obs = adata.obs.set_index(None)
-    adata.var[None] = var
-    adata.var = adata.var.set_index(None)
-    return adata
+#!/usr/bin/env python3
+
+import numpy as np
+
+import anndata
+import random
+import string
+from typing import Any, Union, Tuple, Type
+
+MAX_ITER = 500
+
+
+def assert_type(value: Any, allowed: Union[Type, Tuple[Type, ...]]) -> None:
+    """
+    Small helper to type check.
+    """
+    if isinstance(value, allowed):
+        return
+    if isinstance(allowed, Type):
+        str_allowed = allowed.__name__
+    else:
+        str_allowed = ", ".join([_type.__name__ for _type in allowed])
+    raise TypeError(f"Unexpected type: {type(value)}. Expected {str_allowed}.")
+
+
+def rand_str(ln: int) -> str:
+    # Just a random string generator
+    return "".join(random.choices(string.ascii_letters, k=ln))
+
+
+def generate_str_elements(
+    n: int = 100,
+    ln: int = 8,
+    conserve_duplicates: bool = False,
+) -> np.ndarray:
+    # Helper function generating random features
+    elements = np.array([rand_str(ln) for _ in range(n)])
+    if conserve_duplicates:
+        return elements
+    return np.unique(elements)
+
+
+def generate_anndata(
+    obs: Union[int, np.ndarray] = 100,
+    var: Union[int, np.ndarray] = 20,
+    target_sparsity: float = 0.8,
+):
+    # Helper function generating random anndatas.
+    if isinstance(obs, int):
+        obs = np.unique(generate_str_elements(obs, 6))
+    if isinstance(var, int):
+        var = np.unique(generate_str_elements(var, 6))
+    nobs, nvar = obs.shape[0], var.shape[0]
+    X = np.random.random(size=(nobs, nvar))
+    X = X * (np.random.random(size=X.shape) > target_sparsity)
+    adata = anndata.AnnData(X, dtype=X.dtype)
+    adata.obs[None] = obs
+    adata.obs = adata.obs.set_index(None)
+    adata.var[None] = var
+    adata.var = adata.var.set_index(None)
+    return adata
```

### Comparing `transmorph-0.2.6b0/src/transmorph/utils/plotting.py` & `transmorph-0.2.7/src/transmorph/utils/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,575 +1,590 @@
-#!/usr/bin/env python3
-
-import matplotlib as mt
-import matplotlib.pyplot as plt
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-import numpy as np
-
-from anndata import AnnData
-from matplotlib import cm
-from numbers import Number
-from scipy.sparse import csr_matrix
-from typing import Dict, List, Literal, Optional, Union
-
-
-from ..engine import Model
-from ..engine.evaluators import (
-    evaluate_matching_layer,
-    matching_edge_accuracy_discrete,
-    matching_edge_penalty_continuous,
-)
-from ..engine.layers import (
-    Layer,
-    LayerMatching,
-    LayerMerging,
-)
-from ..engine.matching import CombineMatching
-from ..engine.traits import ContainsTransformations
-from ..utils.anndata_manager import (
-    anndata_manager as adm,
-    AnnDataKeyIdentifiers,
-    slice_common_features,
-)
-from ..utils.dimred import pca, umap
-from ..utils.matrix import extract_chunks, guess_is_discrete
-
-
-def reduce_dimension(
-    datasets: Union[AnnData, List[AnnData], Dict[str, AnnData]],
-    reducer: Literal["umap", "pca"] = "umap",
-    input_obsm: Optional[str] = None,
-    output_obsm: Optional[str] = None,
-) -> None:
-    """
-    Applies a dimensionality reduction algorithm to a list of AnnData objects
-    that must have a non-empty common feature space, for plotting purposes.
-
-    Parameters
-    ----------
-    datasets: Union[AnnData, List[AnnData]]
-        List of AnnData objects to embed in a plottable 2D space.
-
-    reducer: Literal["umap", "pca"]
-        Dimension reduction algorithm to use.
-
-    input_obsm: str, default = "tr_plot"
-        .obsm key to save representation in. Can then be provided
-        to scatter_plot.
-    """
-    if isinstance(datasets, AnnData):
-        datasets = [datasets]
-    if isinstance(datasets, Dict):
-        datasets = list(datasets.values())
-
-    if input_obsm is None:
-        representations = slice_common_features(datasets)
-        assert (
-            representations[0].shape[1] > 0
-        ), "No common gene space found for datasets. Try providing a custom obsm."
-    else:
-        representations = [
-            adm.get_value(adata, key=input_obsm, field_str="obsm") for adata in datasets
-        ]
-
-    for i, X in enumerate(representations):
-        if type(X) is csr_matrix:
-            representations[i] = X.toarray()
-
-    # Dimred if necessary
-    assert all(isinstance(X, np.ndarray) for X in representations)
-    repr_dim = representations[0].shape[1]
-    assert all(X.shape[1] == repr_dim for X in representations)
-    all_X = np.concatenate(representations, axis=0)
-    if repr_dim > 2:
-        if reducer == "umap":
-            all_X = umap(all_X, embedding_dimension=2)
-        elif reducer == "pca":
-            all_X = pca(all_X, n_components=2)
-        else:
-            raise ValueError(
-                f"Unrecognized reducer: {reducer}. Expected 'umap' or 'pca'."
-            )
-
-    if output_obsm is None:
-        output_obsm = AnnDataKeyIdentifiers.PlotRepresentation
-
-    # Saving representations
-    for adata, X in zip(
-        datasets,
-        extract_chunks(all_X, [adata.n_obs for adata in datasets]),
-    ):
-        adm.set_value(
-            adata=adata,
-            key=output_obsm,
-            field="obsm",
-            value=X,
-            persist="output",
-        )
-        adm.set_value(
-            adata=adata,
-            key=f"reducer_{output_obsm}",
-            field="uns",
-            value=reducer,
-            persist="output",
-        )
-
-
-def scatter_plot(
-    datasets: Union[AnnData, List[AnnData], Dict[str, AnnData]],
-    use_rep: Optional[str] = None,
-    color_by: Optional[str] = None,
-    xlabel: Optional[str] = None,
-    ylabel: Optional[str] = None,
-    title: Optional[str] = None,
-    dataset_labels: Optional[List[str]] = None,
-    labels_on_plot: bool = False,
-    palette: str = "rainbow",
-    dot_size: float = 0.5,
-    dpi: int = 100,
-):
-    """
-    Advanced plotting function for transmorph results.
-
-    Parameters
-    ----------
-    datasets: List[AnnData]
-        List of datasets to display, represented as annotated data. If they
-        have been processed by transmorph, integrated embedding will be used.
-        Otherwise, AnnData.X is chosen as fallback representation (in this
-        case, all datasets must be embedded in the same space).
-
-    use_rep: Optional[str]
-        AnnData.obsm key containing data embedding. If None, attempts to use
-        AnnData.X instead if dimensionality is 2.
-
-    color_by: Optional[str]
-        Labeling colors to use in the figure. None will color each
-        point depending of its dataset of origin. Otherwise, all keys of
-        AnnData.obs are valid. The function will try to guess discrete- or
-        continuous-ness of the labels, and color accordingly.
-
-    xlabel: Optional[str]
-        Labeling of the x axis.
-
-    ylabel: Optional[str]
-        Labeling of the y axis.
-
-    title: Optional[str]
-        Title of the plot.
-
-    dataset_labels: Optional[List[str]]
-        Labels to use in legend to describe each AnnData, if datasets
-        is not a Dict.
-
-    labels_on_plot: bool, default = False
-        Shows labels on plot instead of in legend.
-
-    palette: str, default = "rainbow"
-        Matplotlib colormap to pick colors from.
-
-    dot_size: float, default = 0.5
-        Scatter "size" parameter.
-
-    dpi: int, default = 200,
-        Dot per inch to use for the figure.
-    """
-    if isinstance(datasets, AnnData):
-        datasets = [datasets]
-    if isinstance(datasets, Dict):
-        dataset_labels = list(datasets.keys())
-        datasets = list(datasets.values())
-
-    # Checking parameters
-    assert all(
-        isinstance(adata, AnnData) for adata in datasets
-    ), "All datasets must be AnnData."
-
-    if use_rep is None:
-        assert all(
-            adata.X.shape[1] == 2 for adata in datasets
-        ), "No use_rep specified, and some adata.X are not 2 dimensional."
-
-    # Retrieving representation
-    default_xlabel = "Feature 1"
-    default_ylabel = "Feature 2"
-    if not all(adm.isset_value(adata, key=use_rep) for adata in datasets):
-        representations = [adata.X for adata in datasets]
-    else:
-        representations = [adm.get_value(adata, key=use_rep) for adata in datasets]
-        reducer = adm.get_value(datasets[0], key=f"reducer_{use_rep}")
-        if reducer == "umap":
-            default_xlabel = "UMAP1"
-            default_ylabel = "UMAP2"
-        elif reducer == "pca":
-            default_xlabel = "PC1"
-            default_ylabel = "PC2"
-
-    if xlabel is None:
-        xlabel = default_xlabel
-    if ylabel is None:
-        ylabel = default_ylabel
-
-    if color_by is None:  # Color by dataset
-        continuous_palette = False
-        if dataset_labels is not None:
-            all_labels = dataset_labels
-        else:
-            all_labels = [f"Dataset {i + 1}" for i, _ in enumerate(datasets)]
-    else:  # Colour by custom label
-        all_labels = set()
-        for adata in datasets:
-            all_labels = all_labels | set(adata.obs[color_by])
-        all_labels = sorted(all_labels)
-        # simple heuristic
-        continuous_palette = (len(all_labels) > 20) and all(
-            isinstance(y, Number) for y in all_labels
-        )
-
-    dot_alpha = 1
-    n_labels = len(all_labels)
-    n_datasets = len(datasets)
-
-    # Prepare the palette
-    cmap = cm.get_cmap(palette, n_labels)
-
-    # Do the plotting
-    fig = plt.figure(dpi=dpi)
-    ax_scatter = fig.add_subplot(111, aspect="equal")
-
-    scatter = None
-    for i, adata in enumerate(datasets):
-        X = representations[i]
-        if color_by is None:
-            if n_datasets == 1:
-                color = cmap(0.5)
-            else:
-                color = cmap(i / (n_datasets - 1))
-            scatter = ax_scatter.scatter(
-                *X.T, s=dot_size, alpha=dot_alpha, color=color, label=all_labels[i]
-            )
-        elif continuous_palette:
-            scatter = ax_scatter.scatter(
-                *X.T,
-                c=adata.obs[color_by],
-                alpha=dot_alpha,
-                s=dot_size,
-                cmap=palette,
-            )
-        else:
-            for k, label in enumerate(all_labels):
-                if n_labels == 1:
-                    color = cmap(0.5)
-                else:
-                    color = cmap(k / (n_labels - 1))
-                if i == 0:
-                    scatter = ax_scatter.scatter(
-                        *X[adata.obs[color_by] == label].T,
-                        alpha=dot_alpha,
-                        s=dot_size,
-                        color=color,
-                        label=label,
-                    )
-                else:
-                    scatter = ax_scatter.scatter(
-                        *X[adata.obs[color_by] == label].T,
-                        alpha=dot_alpha,
-                        s=dot_size,
-                        color=color,
-                    )
-
-    if continuous_palette:
-        divider = make_axes_locatable(ax_scatter)
-        ax_legend = divider.append_axes("right", size="5%", pad=0.1)
-        plt.colorbar(scatter, cax=ax_legend).set_label(color_by, fontsize=14)
-    elif labels_on_plot:
-        for ilabel, label in enumerate(all_labels):
-            nobs, cl_pos = 0, np.zeros((2,), dtype=np.float32)
-            for i, adata in enumerate(datasets):
-                if color_by == "__dataset__":
-                    if i == ilabel:
-                        selector = np.ones(adata.n_obs, dtype=bool)
-                    else:
-                        selector = np.zeros(adata.n_obs, dtype=bool)
-                else:
-                    selector = adata.obs[color_by] == label
-                nobs += selector.sum()
-                cl_pos += representations[i][selector].sum(axis=0)
-            cl_pos /= nobs
-            plt.text(
-                *cl_pos,
-                s=str(label),
-                bbox={"edgecolor": "none", "facecolor": "white", "alpha": 0.5},
-                fontsize=12,
-                ha="center",
-                va="center",
-            )
-    else:
-        divider = make_axes_locatable(ax_scatter)
-        ax_legend = divider.append_axes("right", size="5%", pad=0.1)
-        handles, labels = ax_scatter.get_legend_handles_labels()
-        order = np.argsort(labels)
-        for label in order:
-            ax_legend.scatter([], [], label=label)
-        legend = ax_legend.legend(
-            [handles[idx] for idx in order],
-            [labels[idx] for idx in order],
-            fontsize=12,
-            ncols=(1 + len(order) // 10),
-            loc="center left",
-        )
-        legend.legendHandles[0]._sizes = [15]
-        legend.legendHandles[1]._sizes = [15]
-        ax_legend.axis("off")
-
-    # Adding text pieces
-    ax_scatter.set_xlabel(xlabel, fontsize=16)
-    ax_scatter.set_ylabel(ylabel, fontsize=16)
-    ax_scatter.set_xticks([])
-    ax_scatter.set_yticks([])
-
-    if title is not None:
-        ax_scatter.set_title(title, fontsize=18)
-
-    plt.show()
-    plt.close()
-
-
-def plot_matching_eval(
-    model: Model,
-    datasets: Union[List[AnnData], Dict[str, AnnData]],
-    obs: str,
-    dataset_keys: Optional[List[str]] = None,
-    title: Optional[str] = None,
-    matshow_kwargs: Dict = {},
-) -> None:
-    """
-    Plots matching evaluation between datasets as a heatmap.
-
-    Parameters
-    ----------
-    layer_matching: LayerMatching
-        LayerMatching that has been evaluated.
-
-    evaluator: str
-        String identifier of the evaluator.
-
-    dataset_keys: Optional[List[str]], default = None
-        Dataset labels to add to the plot.
-
-    title: Optional[str], default = None
-        Title to use for the plot. If None, generates one.
-
-    matshow_kwargs: Dict[str, Any], default = {}
-        Additional matshow parameters.
-    """
-    if isinstance(datasets, AnnData):
-        datasets = {"Batch": datasets}
-    if isinstance(datasets, Dict):
-        dataset_keys = list(datasets.keys())
-        datasets = list(datasets.values())
-    layer_matchings = model.get_layers_by_type(LayerMatching)
-    assert len(layer_matchings) > 0, "No layer of type LayerMatching found."
-    layer_matching = layer_matchings[0]
-    is_discrete = all(guess_is_discrete(adata.obs[obs]) for adata in datasets)
-    if is_discrete:
-        evaluator = matching_edge_accuracy_discrete(obs)
-    else:
-        evaluator = matching_edge_penalty_continuous(obs)
-    scores = evaluate_matching_layer(layer_matching, datasets, evaluator)
-    ndatasets = scores.shape[0]
-    if dataset_keys is not None:
-        assert len(dataset_keys) == ndatasets, (
-            f"Inconsistent number of datasets in dataset_keys, expected {ndatasets}, "
-            f"found {len(dataset_keys)}."
-        )
-
-    plt.matshow(scores, **matshow_kwargs)
-    vmin, vmax = plt.gci().get_clim()
-    mid = 0.5 * (vmax - vmin)
-    for i in range(ndatasets):
-        for j in range(ndatasets):
-            if scores[i, j] > mid:
-                fontcolor = "k"
-            else:
-                fontcolor = "w"
-            plt.text(
-                i,
-                j,
-                "{:.1f}".format(scores[i, j]),
-                va="center",
-                ha="center",
-                c=fontcolor,
-            )
-        values = [scores[i, k] for k in range(ndatasets) if k != i]
-        plt.text(ndatasets, i, "{:.1f}".format(np.mean(values)), va="center")
-        plt.text(ndatasets + 1, i, "{:.1f}".format(np.std(values)), va="center")
-
-    plt.text(ndatasets, -0.5, "Mean", rotation=60, va="bottom")
-    plt.text(ndatasets + 1, -0.5, "STD", rotation=60, va="bottom")
-    if dataset_keys is not None:
-        plt.xticks(range(ndatasets), dataset_keys, rotation=60)
-        plt.yticks(range(ndatasets), dataset_keys)
-    else:
-        plt.xticks([])
-        plt.yticks([])
-    if title is None:
-        title = "Pairwise matching evaluation"
-    plt.title(title)
-
-
-def plot_label_distribution_heatmap(
-    datasets: Union[List[AnnData], Dict[str, AnnData]],
-    label: str,
-    dataset_keys: Optional[List[str]] = None,
-    title: Optional[str] = None,
-) -> None:
-    """ """
-    if isinstance(datasets, Dict):
-        dataset_keys = list(datasets.keys())
-        datasets = list(datasets.values())
-    all_labels = set()
-    for adata in datasets:
-        all_labels = all_labels | set(adata.obs[label])
-    all_labels = list(sorted(all_labels))
-
-    ndatasets, nlabels = len(datasets), len(all_labels)
-
-    labels_counts = np.zeros(nlabels, dtype=int)
-    labels_dist = np.zeros((ndatasets, nlabels), dtype=np.float32)
-    for i, adata in enumerate(datasets):
-        nsamples = adata.n_obs
-        for j, lb in enumerate(all_labels):
-            v = np.sum(adata.obs[label] == lb)
-            labels_dist[i, j] = v / nsamples
-            labels_counts[j] += v
-
-    vmin, vmax = 0.0, 1 / nlabels
-    plt.matshow(labels_dist, vmin=vmin, vmax=vmax)
-
-    for i, adata in enumerate(datasets):
-        nsamples = adata.n_obs
-        for j, lb in enumerate(all_labels):
-            val = np.sum(adata.obs[label] == lb) / nsamples
-            fc = "k" if val > vmax / 2 else "w"
-            plt.text(j, i, f"{int(val*100)}%", ha="center", va="center", c=fc)
-
-    for i, adata in enumerate(datasets):
-        plt.text(nlabels, i, adata.n_obs, ha="left", va="center")
-
-    for j, lb in enumerate(all_labels):
-        plt.text(j, ndatasets, labels_counts[j], ha="center", va="top", rotation=30)
-
-    plt.xticks(np.arange(nlabels), all_labels, rotation=60)
-    if dataset_keys is not None:
-        plt.yticks(np.arange(ndatasets), dataset_keys)
-    if title is not None:
-        plt.title(title)
-
-
-def plot_model(
-    model: Model,
-    layer_edgecolor: str = "royalblue",
-    layer_facecolor: str = "lightsteelblue",
-    algorithm_edgecolor: str = "darkorange",
-    algorithm_facecolor: str = "bisque",
-) -> None:
-    """
-    Plots a visual representation of a model.
-    """
-
-    BOX_WIDTH = 40
-    BOX_HEIGHT = 20
-
-    def _retrieve_elements(layer: Layer):
-        elements = []
-        if isinstance(layer, ContainsTransformations):
-            for transformation in layer.transformations:
-                elements.append(type(transformation).__name__)
-        if isinstance(layer, LayerMatching):
-            elements.append(type(layer.matching).__name__)
-            if isinstance(layer.matching, CombineMatching):
-                for matching in layer.matching.matchings:
-                    elements.append(type(matching).__name__)
-        if isinstance(layer, LayerMerging):
-            elements.append(type(layer.merging).__name__)
-        return elements
-
-    def _retrieve_n_rows(model: Model) -> int:
-        max_elements = 0
-        for layer in model.layers:
-            max_elements = max(max_elements, len(_retrieve_elements(layer)))
-        return max_elements
-
-    def _plot_textbox(x: int, y: int, text: str, ax: mt.axes.Axes, **rect_kwargs):
-        rect = mt.patches.Rectangle((x, y), BOX_WIDTH, BOX_HEIGHT, **rect_kwargs)
-        ax.add_patch(rect)
-        ax.text(
-            x + BOX_WIDTH / 2,
-            y + BOX_HEIGHT / 2,
-            text,
-            ha="center",
-            va="center",
-            fontsize=9,
-        )
-
-    def _plot_layer(layer: Layer, x_offset: int, ax: mt.axes.Axes):
-        _plot_textbox(
-            x_offset,
-            0,
-            type(layer).__name__[5:],
-            ax,
-            linewidth=1,
-            edgecolor=layer_edgecolor,
-            facecolor=layer_facecolor,
-        )
-        next_layers = layer.output_layers
-        if len(next_layers) > 1:
-            raise NotImplementedError
-        if len(next_layers) == 0:
-            return
-        plt.arrow(
-            x_offset + BOX_WIDTH,
-            BOX_HEIGHT / 2,
-            BOX_WIDTH / 2,
-            0,
-            length_includes_head=True,
-            facecolor="k",
-            head_width=3,
-            head_length=1.5,
-        )
-        y_offset = 0
-        for element in _retrieve_elements(layer):
-            plt.arrow(
-                x_offset + BOX_HEIGHT,
-                y_offset,
-                0,
-                -BOX_HEIGHT,
-                length_includes_head=True,
-                facecolor="k",
-                head_width=2,
-            )
-            _plot_textbox(
-                x_offset,
-                y_offset - BOX_HEIGHT * 2,
-                element,
-                ax,
-                linewidth=1,
-                edgecolor=algorithm_edgecolor,
-                facecolor=algorithm_facecolor,
-            )
-            y_offset -= BOX_HEIGHT * 2
-        _plot_layer(next_layers[0], x_offset + BOX_WIDTH * 1.5, ax)
-
-    assert isinstance(model, Model), f"Model expected, found {type(model)}."
-
-    n_layers = len(model.layers)
-    n_rows = _retrieve_n_rows(model)
-
-    if n_layers == 0:
-        return
-
-    fig = plt.figure(figsize=(2.5 * n_layers, 0.7 * (1 + n_rows)))
-    ax = fig.add_subplot(111)
-    plt.axis("off")
-
-    _plot_layer(model.layers[0], 0, ax)
+#!/usr/bin/env python3
+
+import matplotlib as mt
+import matplotlib.pyplot as plt
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+import numpy as np
+
+from anndata import AnnData
+from matplotlib import cm
+from numbers import Number
+from scipy.sparse import csr_matrix
+from typing import Dict, List, Literal, Optional, Tuple, Union
+
+
+from ..engine import Model
+from ..engine.evaluators import (
+    evaluate_matching_layer,
+    matching_edge_accuracy_discrete,
+    matching_edge_penalty_continuous,
+)
+from ..engine.layers import (
+    Layer,
+    LayerMatching,
+    LayerMerging,
+)
+from ..engine.matching import CombineMatching
+from ..engine.traits import ContainsTransformations
+from ..utils.anndata_manager import (
+    anndata_manager as adm,
+    AnnDataKeyIdentifiers,
+    slice_common_features,
+)
+from ..utils.dimred import pca, umap
+from ..utils.matrix import extract_chunks, guess_is_discrete
+
+
+def reduce_dimension(
+    datasets: Union[AnnData, List[AnnData], Dict[str, AnnData]],
+    reducer: Literal["umap", "pca"] = "umap",
+    input_obsm: Optional[str] = None,
+    output_obsm: Optional[str] = None,
+) -> None:
+    """
+    Applies a dimensionality reduction algorithm to a list of AnnData objects
+    that must have a non-empty common feature space, for plotting purposes.
+
+    Parameters
+    ----------
+    datasets: Union[AnnData, List[AnnData]]
+        List of AnnData objects to embed in a plottable 2D space.
+
+    reducer: Literal["umap", "pca"]
+        Dimension reduction algorithm to use.
+
+    input_obsm: str, default = "tr_plot"
+        .obsm key to save representation in. Can then be provided
+        to scatter_plot.
+    """
+    if isinstance(datasets, AnnData):
+        datasets = [datasets]
+    if isinstance(datasets, Dict):
+        datasets = list(datasets.values())
+
+    if input_obsm is None:
+        representations = slice_common_features(datasets)
+        assert (
+            representations[0].shape[1] > 0
+        ), "No common gene space found for datasets. Try providing a custom obsm."
+    else:
+        representations = [
+            adm.get_value(adata, key=input_obsm, field_str="obsm") for adata in datasets
+        ]
+
+    for i, X in enumerate(representations):
+        if type(X) is csr_matrix:
+            representations[i] = X.toarray()
+
+    # Dimred if necessary
+    assert all(isinstance(X, np.ndarray) for X in representations)
+    repr_dim = representations[0].shape[1]
+    assert all(X.shape[1] == repr_dim for X in representations)
+    all_X = np.concatenate(representations, axis=0)
+    if repr_dim > 2:
+        if reducer == "umap":
+            all_X = umap(all_X, embedding_dimension=2)
+        elif reducer == "pca":
+            all_X = pca(all_X, n_components=2)
+        else:
+            raise ValueError(
+                f"Unrecognized reducer: {reducer}. Expected 'umap' or 'pca'."
+            )
+
+    if output_obsm is None:
+        output_obsm = AnnDataKeyIdentifiers.PlotRepresentation
+
+    # Saving representations
+    for adata, X in zip(
+        datasets,
+        extract_chunks(all_X, [adata.n_obs for adata in datasets]),
+    ):
+        adm.set_value(
+            adata=adata,
+            key=output_obsm,
+            field="obsm",
+            value=X,
+            persist="output",
+        )
+        adm.set_value(
+            adata=adata,
+            key=f"reducer_{output_obsm}",
+            field="uns",
+            value=reducer,
+            persist="output",
+        )
+
+
+def scatter_plot(
+    datasets: Union[AnnData, List[AnnData], Dict[str, AnnData]],
+    use_rep: Optional[str] = None,
+    color_by: Optional[str] = None,
+    xlabel: Optional[str] = None,
+    ylabel: Optional[str] = None,
+    title: Optional[str] = None,
+    dataset_labels: Optional[List[str]] = None,
+    labels_on_plot: bool = False,
+    palette: str = "rainbow",
+    figsize: Tuple[int, int] = (5, 5),
+    s: float = 1.0,
+    marker: str = ".",
+    dpi: int = 100,
+    **kwargs,
+):
+    """
+    Advanced plotting function for transmorph results.
+
+    Parameters
+    ----------
+    datasets: List[AnnData]
+        List of datasets to display, represented as annotated data. If they
+        have been processed by transmorph, integrated embedding will be used.
+        Otherwise, AnnData.X is chosen as fallback representation (in this
+        case, all datasets must be embedded in the same space).
+
+    use_rep: Optional[str]
+        AnnData.obsm key containing data embedding. If None, attempts to use
+        AnnData.X instead if dimensionality is 2.
+
+    color_by: Optional[str]
+        Labeling colors to use in the figure. None will color each
+        point depending of its dataset of origin. Otherwise, all keys of
+        AnnData.obs are valid. The function will try to guess discrete- or
+        continuous-ness of the labels, and color accordingly.
+
+    xlabel: Optional[str]
+        Labeling of the x axis.
+
+    ylabel: Optional[str]
+        Labeling of the y axis.
+
+    title: Optional[str]
+        Title of the plot.
+
+    dataset_labels: Optional[List[str]]
+        Labels to use in legend to describe each AnnData, if datasets
+        is not a Dict.
+
+    labels_on_plot: bool, default = False
+        Shows labels on plot instead of in legend.
+
+    palette: str, default = "rainbow"
+        Matplotlib colormap to pick colors from.
+
+    dpi: int, default = 200,
+        Dot per inch to use for the figure.
+
+    **kwargs:
+        Additional keyword arguments to pass to plt.scatter.
+    """
+    if isinstance(datasets, AnnData):
+        datasets = [datasets]
+    if isinstance(datasets, Dict):
+        dataset_labels = list(datasets.keys())
+        datasets = list(datasets.values())
+
+    # Checking parameters
+    assert all(
+        isinstance(adata, AnnData) for adata in datasets
+    ), "All datasets must be AnnData."
+
+    if use_rep is None:
+        assert all(
+            adata.X.shape[1] == 2 for adata in datasets
+        ), "No use_rep specified, and some adata.X are not 2 dimensional."
+
+    # Retrieving representation
+    default_xlabel = "Feature 1"
+    default_ylabel = "Feature 2"
+    if not all(adm.isset_value(adata, key=use_rep) for adata in datasets):
+        if all(use_rep in adata.obsm for adata in datasets):
+            representations = [adata.obsm[use_rep] for adata in datasets]
+        else:
+            representations = [adata.X for adata in datasets]
+    else:
+        representations = [adm.get_value(adata, key=use_rep) for adata in datasets]
+        reducer = adm.get_value(datasets[0], key=f"reducer_{use_rep}")
+        if reducer == "umap":
+            default_xlabel = "UMAP1"
+            default_ylabel = "UMAP2"
+        elif reducer == "pca":
+            default_xlabel = "PC1"
+            default_ylabel = "PC2"
+
+    for i, X in enumerate(representations):
+        if X.shape[1] > 2:
+            representations[i] = X[:, :2].copy()
+
+    if xlabel is None:
+        xlabel = default_xlabel
+    if ylabel is None:
+        ylabel = default_ylabel
+
+    if color_by is None:  # Color by dataset
+        continuous_palette = False
+        if dataset_labels is not None:
+            all_labels = dataset_labels
+        else:
+            all_labels = [f"Dataset {i + 1}" for i, _ in enumerate(datasets)]
+    else:  # Colour by custom label
+        all_labels = set()
+        for adata in datasets:
+            all_labels = all_labels | set(adata.obs[color_by])
+        all_labels = sorted(all_labels)
+        # simple heuristic
+        continuous_palette = (len(all_labels) > 20) and all(
+            isinstance(y, Number) for y in all_labels
+        )
+
+    n_labels = len(all_labels)
+    n_datasets = len(datasets)
+
+    # Prepare the palette
+    cmap = cm.get_cmap(palette, n_labels)
+
+    # Do the plotting
+    fig = plt.figure(dpi=dpi, figsize=figsize)
+    ax_scatter = fig.add_subplot(111)
+
+    scatter = None
+    for i, adata in enumerate(datasets):
+        X = representations[i]
+        if color_by is None:
+            if n_datasets == 1:
+                color = cmap(0.5)
+            else:
+                color = cmap(i / (n_datasets - 1))
+            scatter = ax_scatter.scatter(
+                *X.T,
+                s=s,
+                marker=marker,
+                color=color,
+                label=all_labels[i],
+                **kwargs,
+            )
+        elif continuous_palette:
+            scatter = ax_scatter.scatter(
+                *X.T,
+                c=adata.obs[color_by],
+                s=s,
+                marker=marker,
+                cmap=palette,
+                **kwargs,
+            )
+        else:
+            for k, label in enumerate(all_labels):
+                if n_labels == 1:
+                    color = cmap(0.5)
+                else:
+                    color = cmap(k / (n_labels - 1))
+                if i == 0:
+                    scatter = ax_scatter.scatter(
+                        *X[adata.obs[color_by] == label].T,
+                        s=s,
+                        marker=marker,
+                        color=color,
+                        label=label,
+                        **kwargs,
+                    )
+                else:
+                    scatter = ax_scatter.scatter(
+                        *X[adata.obs[color_by] == label].T,
+                        s=s,
+                        marker=marker,
+                        color=color,
+                        **kwargs,
+                    )
+
+    if continuous_palette:
+        divider = make_axes_locatable(ax_scatter)
+        ax_legend = divider.append_axes("right", size="5%", pad=0.1)
+        plt.colorbar(scatter, cax=ax_legend).set_label(color_by, fontsize=14)
+    elif labels_on_plot:
+        for ilabel, label in enumerate(all_labels):
+            nobs, cl_pos = 0, np.zeros((2,), dtype=np.float32)
+            for i, adata in enumerate(datasets):
+                if color_by == "__dataset__":
+                    if i == ilabel:
+                        selector = np.ones(adata.n_obs, dtype=bool)
+                    else:
+                        selector = np.zeros(adata.n_obs, dtype=bool)
+                else:
+                    selector = adata.obs[color_by] == label
+                nobs += selector.sum()
+                cl_pos += representations[i][selector].sum(axis=0)
+            cl_pos /= nobs
+            plt.text(
+                *cl_pos,
+                s=str(label),
+                bbox={"edgecolor": "none", "facecolor": "white", "alpha": 0.5},
+                fontsize=12,
+                ha="center",
+                va="center",
+            )
+    else:
+        divider = make_axes_locatable(ax_scatter)
+        ax_legend = divider.append_axes("right", size="0%", pad=0.1)
+        handles, labels = ax_scatter.get_legend_handles_labels()
+        order = np.argsort(labels)
+        for label in order:
+            ax_legend.scatter([], [], label=label)
+        legend = ax_legend.legend(
+            [handles[idx] for idx in order],
+            [labels[idx] for idx in order],
+            fontsize=12,
+            ncols=(1 + len(order) // 15),
+            loc="center left",
+        )
+        for handle in legend.legendHandles:
+            handle._sizes = [60]
+        ax_legend.axis("off")
+
+    # Adding text pieces
+    ax_scatter.set_xlabel(xlabel, fontsize=16)
+    ax_scatter.set_ylabel(ylabel, fontsize=16)
+    ax_scatter.set_xticks([])
+    ax_scatter.set_yticks([])
+    ax_scatter.set_title(title, fontsize=18)
+
+    plt.show()
+    plt.close()
+
+
+def plot_matching_eval(
+    model: Model,
+    datasets: Union[List[AnnData], Dict[str, AnnData]],
+    obs: str,
+    dataset_keys: Optional[List[str]] = None,
+    title: Optional[str] = None,
+    matshow_kwargs: Dict = {},
+) -> None:
+    """
+    Plots matching evaluation between datasets as a heatmap.
+
+    Parameters
+    ----------
+    layer_matching: LayerMatching
+        LayerMatching that has been evaluated.
+
+    evaluator: str
+        String identifier of the evaluator.
+
+    dataset_keys: Optional[List[str]], default = None
+        Dataset labels to add to the plot.
+
+    title: Optional[str], default = None
+        Title to use for the plot. If None, generates one.
+
+    matshow_kwargs: Dict[str, Any], default = {}
+        Additional matshow parameters.
+    """
+    if isinstance(datasets, AnnData):
+        datasets = {"Batch": datasets}
+    if isinstance(datasets, Dict):
+        dataset_keys = list(datasets.keys())
+        datasets = list(datasets.values())
+    layer_matchings = model.get_layers_by_type(LayerMatching)
+    assert len(layer_matchings) > 0, "No layer of type LayerMatching found."
+    layer_matching = layer_matchings[0]
+    is_discrete = all(guess_is_discrete(adata.obs[obs]) for adata in datasets)
+    if is_discrete:
+        evaluator = matching_edge_accuracy_discrete(obs)
+    else:
+        evaluator = matching_edge_penalty_continuous(obs)
+    scores = evaluate_matching_layer(layer_matching, datasets, evaluator)
+    ndatasets = scores.shape[0]
+    if dataset_keys is not None:
+        assert len(dataset_keys) == ndatasets, (
+            f"Inconsistent number of datasets in dataset_keys, expected {ndatasets}, "
+            f"found {len(dataset_keys)}."
+        )
+
+    plt.matshow(scores, **matshow_kwargs)
+    vmin, vmax = plt.gci().get_clim()
+    mid = 0.5 * (vmax - vmin)
+    for i in range(ndatasets):
+        for j in range(ndatasets):
+            if scores[i, j] > mid:
+                fontcolor = "k"
+            else:
+                fontcolor = "w"
+            plt.text(
+                i,
+                j,
+                "{:.1f}".format(scores[i, j]),
+                va="center",
+                ha="center",
+                c=fontcolor,
+            )
+        values = [scores[i, k] for k in range(ndatasets) if k != i]
+        plt.text(ndatasets, i, "{:.1f}".format(np.mean(values)), va="center")
+        plt.text(ndatasets + 1, i, "{:.1f}".format(np.std(values)), va="center")
+
+    plt.text(ndatasets, -0.5, "Mean", rotation=60, va="bottom")
+    plt.text(ndatasets + 1, -0.5, "STD", rotation=60, va="bottom")
+    if dataset_keys is not None:
+        plt.xticks(range(ndatasets), dataset_keys, rotation=60)
+        plt.yticks(range(ndatasets), dataset_keys)
+    else:
+        plt.xticks([])
+        plt.yticks([])
+    if title is None:
+        title = "Pairwise matching evaluation"
+    plt.title(title)
+
+
+def plot_label_distribution_heatmap(
+    datasets: Union[List[AnnData], Dict[str, AnnData]],
+    label: str,
+    dataset_keys: Optional[List[str]] = None,
+    title: Optional[str] = None,
+) -> None:
+    """ """
+    if isinstance(datasets, Dict):
+        dataset_keys = list(datasets.keys())
+        datasets = list(datasets.values())
+    all_labels = set()
+    for adata in datasets:
+        all_labels = all_labels | set(adata.obs[label])
+    all_labels = list(sorted(all_labels))
+
+    ndatasets, nlabels = len(datasets), len(all_labels)
+
+    labels_counts = np.zeros(nlabels, dtype=int)
+    labels_dist = np.zeros((ndatasets, nlabels), dtype=np.float32)
+    for i, adata in enumerate(datasets):
+        nsamples = adata.n_obs
+        for j, lb in enumerate(all_labels):
+            v = np.sum(adata.obs[label] == lb)
+            labels_dist[i, j] = v / nsamples
+            labels_counts[j] += v
+
+    vmin, vmax = 0.0, 1 / nlabels
+    plt.matshow(labels_dist, vmin=vmin, vmax=vmax)
+
+    for i, adata in enumerate(datasets):
+        nsamples = adata.n_obs
+        for j, lb in enumerate(all_labels):
+            val = np.sum(adata.obs[label] == lb) / nsamples
+            fc = "k" if val > vmax / 2 else "w"
+            plt.text(j, i, f"{int(val*100)}%", ha="center", va="center", c=fc)
+
+    for i, adata in enumerate(datasets):
+        plt.text(nlabels, i, adata.n_obs, ha="left", va="center")
+
+    for j, lb in enumerate(all_labels):
+        plt.text(j, ndatasets, labels_counts[j], ha="center", va="top", rotation=30)
+
+    plt.xticks(np.arange(nlabels), all_labels, rotation=60)
+    if dataset_keys is not None:
+        plt.yticks(np.arange(ndatasets), dataset_keys)
+    if title is not None:
+        plt.title(title)
+
+
+def plot_model(
+    model: Model,
+    layer_edgecolor: str = "royalblue",
+    layer_facecolor: str = "lightsteelblue",
+    algorithm_edgecolor: str = "darkorange",
+    algorithm_facecolor: str = "bisque",
+) -> None:
+    """
+    Plots a visual representation of a model.
+    """
+
+    BOX_WIDTH = 40
+    BOX_HEIGHT = 20
+
+    def _retrieve_elements(layer: Layer):
+        elements = []
+        if isinstance(layer, ContainsTransformations):
+            for transformation in layer.transformations:
+                elements.append(type(transformation).__name__)
+        if isinstance(layer, LayerMatching):
+            elements.append(type(layer.matching).__name__)
+            if isinstance(layer.matching, CombineMatching):
+                for matching in layer.matching.matchings:
+                    elements.append(type(matching).__name__)
+        if isinstance(layer, LayerMerging):
+            elements.append(type(layer.merging).__name__)
+        return elements
+
+    def _retrieve_n_rows(model: Model) -> int:
+        max_elements = 0
+        for layer in model.layers:
+            max_elements = max(max_elements, len(_retrieve_elements(layer)))
+        return max_elements
+
+    def _plot_textbox(x: int, y: int, text: str, ax: mt.axes.Axes, **rect_kwargs):
+        rect = mt.patches.Rectangle((x, y), BOX_WIDTH, BOX_HEIGHT, **rect_kwargs)
+        ax.add_patch(rect)
+        ax.text(
+            x + BOX_WIDTH / 2,
+            y + BOX_HEIGHT / 2,
+            text,
+            ha="center",
+            va="center",
+            fontsize=9,
+        )
+
+    def _plot_layer(layer: Layer, x_offset: int, ax: mt.axes.Axes):
+        _plot_textbox(
+            x_offset,
+            0,
+            type(layer).__name__[5:],
+            ax,
+            linewidth=1,
+            edgecolor=layer_edgecolor,
+            facecolor=layer_facecolor,
+        )
+        next_layers = layer.output_layers
+        if len(next_layers) > 1:
+            raise NotImplementedError
+        if len(next_layers) == 0:
+            return
+        plt.arrow(
+            x_offset + BOX_WIDTH,
+            BOX_HEIGHT / 2,
+            BOX_WIDTH / 2,
+            0,
+            length_includes_head=True,
+            facecolor="k",
+            head_width=3,
+            head_length=1.5,
+        )
+        y_offset = 0
+        for element in _retrieve_elements(layer):
+            plt.arrow(
+                x_offset + BOX_HEIGHT,
+                y_offset,
+                0,
+                -BOX_HEIGHT,
+                length_includes_head=True,
+                facecolor="k",
+                head_width=2,
+            )
+            _plot_textbox(
+                x_offset,
+                y_offset - BOX_HEIGHT * 2,
+                element,
+                ax,
+                linewidth=1,
+                edgecolor=algorithm_edgecolor,
+                facecolor=algorithm_facecolor,
+            )
+            y_offset -= BOX_HEIGHT * 2
+        _plot_layer(next_layers[0], x_offset + BOX_WIDTH * 1.5, ax)
+
+    assert isinstance(model, Model), f"Model expected, found {type(model)}."
+
+    n_layers = len(model.layers)
+    n_rows = _retrieve_n_rows(model)
+
+    if n_layers == 0:
+        return
+
+    fig = plt.figure(figsize=(2.5 * n_layers, 0.7 * (1 + n_rows)))
+    ax = fig.add_subplot(111)
+    plt.axis("off")
+
+    _plot_layer(model.layers[0], 0, ax)
```

### Comparing `transmorph-0.2.6b0/src/transmorph.egg-info/PKG-INFO` & `transmorph-0.2.7/src/transmorph.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1
-Name: transmorph
-Version: 0.2.6b0
-Summary: A unifying data integration framework.
-Home-page: https://github.com/Risitop/transmorph
-Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
-Author-email: aziz.fouche@curie.fr
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
-
-[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
-[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
-[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
-[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
-[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
-
-**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
-
-<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
-
-Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
-
-## Documentation
-
-https://transmorph.readthedocs.io/en/latest/
-
-## Installation
-
-**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
-
-See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
-
-### Quick starting with a pre-built model
-
-All **transmorph** models take a list or a dictionary containing AnnData objects as input
-for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
-
-```python
-from transmorph.datasets import load_chen_10x
-chen_10x = load_chen_10x()
-```
-
-One can then either create a custom integration model, or load 
-a pre-built transmorph model. We will choose the *EmbedMNN* model with
-default parameters for this example, which embeds all datasets into 
-a common abstract 2D space. 
-
-```python
-from transmorph.models import EmbedMNN
-model = EmbedMNN()
-model.transform(chen_10x)
-```
-
-Integration embedding coordinates can be gathered in each AnnData object,
-in AnnData.obsm['X_transmorph'].
-
-```python
-chen_10x['P01'].obsm['X_transmorph']
-```
-
-One can for instance use a plotting function from transmorph to display integration results.
-
-```python
-from transmorph.utils.plotting import scatter_plot
-
-scatter_plot(chen_10x, use_rep="X_transmorph")
-scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
-```
-
-## Citing transmorph
-
-If you find transmorph useful for your research, please consider citing our pre-print
-which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
-
-```bibtex
-@article{fouche2022transmorph,
-  title={transmorph: a unifying computational framework for single-cell data integration},
-  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
-  journal={bioRxiv},
-  year={2022}
-}
-```
-
-# References
-
-[Chen 2020] [Chen, Y. P., Yin, J. H., Li, W. F., Li, H. J., Chen, D. P., Zhang, C. J., ... & Ma, J. (2020). Single-cell transcriptomics reveals regulators underlying immune cell diversity and immune subtypes associated with prognosis in nasopharyngeal carcinoma. Cell research, 30(11), 1024-1042.](https://www.nature.com/articles/s41422-020-0374-x)
+Metadata-Version: 2.1
+Name: transmorph
+Version: 0.2.7
+Summary: A unifying data integration framework.
+Home-page: https://github.com/Risitop/transmorph
+Author: Aziz Fouché, Loïc Chadoutaud, Andrei Zinovyev (Institut Curie, Paris)
+Author-email: aziz.fouche@curie.fr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [<img alt="Transmorph logo" src="img/logo_v2.png" height="90">](https://transmorph.readthedocs.io/en/latest/index.html)
+
+[![PyPI version](https://badge.fury.io/py/transmorph.svg)](https://badge.fury.io/py/transmorph)
+[![GitHub license](https://img.shields.io/github/license/Risitop/transmorph.svg)](https://github.com/Risitop/transmorph/blob/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/transmorph/badge/?version=latest)](https://transmorph.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/transmorph)](https://pepy.tech/project/transmorph)
+[![Downloads](https://pepy.tech/badge/transmorph/month)](https://pepy.tech/project/transmorph)
+
+**transmorph** is a python framework dedicated to data integration, with a focus on single-cell applications. Dataset integration describes the problem of embedding two or more datasets together, across different batches or feature spaces, so that similar samples end up close from one another. In transmorph we aim to provide a comprehensive framework to design, apply, report and benchmark data integration models using a system of interactive building blocks supported by statistical and plotting tools. We included pre-built models as well as benchmarking databanks in order to easily set up integration tasks. This package can be used in compatibility with **scanpy** and **anndata** packages, and works in jupyter notebooks.
+
+<img alt="Transmorph workflow" src="img/fig_presentation_github.png" height="400">
+
+Transmorph is also computationally efficient, and can scale to large datasets with competitive integration quality. 
+
+## Documentation
+
+https://transmorph.readthedocs.io/en/latest/
+
+## Installation
+
+**transmorph** can be installed either from source of from the python repository PyPi. PyPi version is commonly more stable, but may not contain latest features, while you can find the development version on GitHub. Using a python environment is highly recommended (for instance  [pipenv](https://pypi.org/project/pipenv/)) in order to easily handle dependencies and versions. **transmorph** has only be tested for python >=3.9, on Linux and Windows systems.
+
+See the instructions: [https://transmorph.readthedocs.io/en/latest/sections/installation.html](https://transmorph.readthedocs.io/en/latest/sections/installation.html)
+
+### Quick starting with a pre-built model
+
+All **transmorph** models take a list or a dictionary containing AnnData objects as input
+for data integration. Let us start by loading some benchmarking data, gathered from [Chen 2020] (3.4GB size).
+
+```python
+from transmorph.datasets import load_chen_10x
+chen_10x = load_chen_10x()
+```
+
+One can then either create a custom integration model, or load 
+a pre-built transmorph model. We will choose the *EmbedMNN* model with
+default parameters for this example, which embeds all datasets into 
+a common abstract 2D space. 
+
+```python
+from transmorph.models import EmbedMNN
+model = EmbedMNN()
+model.transform(chen_10x)
+```
+
+Integration embedding coordinates can be gathered in each AnnData object,
+in AnnData.obsm['X_transmorph'].
+
+```python
+chen_10x['P01'].obsm['X_transmorph']
+```
+
+One can for instance use a plotting function from transmorph to display integration results.
+
+```python
+from transmorph.utils.plotting import scatter_plot
+
+scatter_plot(chen_10x, use_rep="X_transmorph")
+scatter_plot(chen_10x, use_rep="X_transmorph", color_by="class")
+```
+
+## Citing transmorph
+
+If you find transmorph useful for your research, please consider citing our pre-print
+which can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2022.11.02.514912v1).
+
+```bibtex
+@article{fouche2022transmorph,
+  title={transmorph: a unifying computational framework for single-cell data integration},
+  author={Fouch{\'e}, Aziz, Chadoutaud, Lo{\¨i}c, Delattre, Olivier and Zinovyev, Andrei},
+  journal={bioRxiv},
+  year={2022}
+}
+```
+
+# References
+
+[Chen 2020] [Chen, Y. P., Yin, J. H., Li, W. F., Li, H. J., Chen, D. P., Zhang, C. J., ... & Ma, J. (2020). Single-cell transcriptomics reveals regulators underlying immune cell diversity and immune subtypes associated with prognosis in nasopharyngeal carcinoma. Cell research, 30(11), 1024-1042.](https://www.nature.com/articles/s41422-020-0374-x)
```

### Comparing `transmorph-0.2.6b0/src/transmorph.egg-info/SOURCES.txt` & `transmorph-0.2.7/src/transmorph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-.gitignore
-.projectile
-.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
-build.sh
 pyproject.toml
 setup.cfg
 setup.py
-img/logo.png
 src/transmorph/__init__.py
 src/transmorph/_logging.py
 src/transmorph/_profiling.py
 src/transmorph/_settings.py
 src/transmorph.egg-info/PKG-INFO
 src/transmorph.egg-info/SOURCES.txt
 src/transmorph.egg-info/dependency_links.txt
@@ -85,15 +80,17 @@
 src/transmorph/engine/transforming/algorithms/commonfeatures.py
 src/transmorph/engine/transforming/algorithms/ica.py
 src/transmorph/engine/transforming/algorithms/pca.py
 src/transmorph/engine/transforming/algorithms/pooling.py
 src/transmorph/engine/transforming/algorithms/standardize.py
 src/transmorph/models/__init__.py
 src/transmorph/models/embedmnn.py
+src/transmorph/models/harmony.py
 src/transmorph/models/mnncorrection.py
+src/transmorph/models/scvi_vae.py
 src/transmorph/models/transportcorrection.py
 src/transmorph/stats/__init__.py
 src/transmorph/stats/entropy.py
 src/transmorph/stats/integration.py
 src/transmorph/stats/lisi.py
 src/transmorph/stats/matching.py
 src/transmorph/utils/__init__.py
```

