# Comparing `tmp/PennyLane-0.8.1.tar.gz` & `tmp/PennyLane-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PennyLane-0.8.1.tar", last modified: Fri Feb 28 12:33:10 2020, max compression
+gzip compressed data, was "dist/PennyLane-0.9.0.tar", last modified: Fri May 15 01:45:32 2020, max compression
```

## Comparing `PennyLane-0.8.1.tar` & `PennyLane-0.9.0.tar`

### file list

```diff
@@ -1,143 +1,150 @@
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:10.000000 PennyLane-0.8.1/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2690 2019-09-27 17:22:11.000000 PennyLane-0.8.1/default_config.toml
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:06.000000 PennyLane-0.8.1/doc/
--rwxrwxrwx   0 josh      (1000) josh      (1000)    13296 2020-02-27 06:07:04.000000 PennyLane-0.8.1/doc/conf.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4134 2020-02-27 06:07:04.000000 PennyLane-0.8.1/doc/directives.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     6971 2020-02-27 06:13:26.000000 PennyLane-0.8.1/doc/index.rst
--rwxrwxrwx   0 josh      (1000) josh      (1000)      792 2020-02-27 06:07:04.000000 PennyLane-0.8.1/doc/Makefile
--rwxrwxrwx   0 josh      (1000) josh      (1000)      314 2020-02-27 06:07:04.000000 PennyLane-0.8.1/doc/requirements.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)    11357 2019-02-13 23:40:16.000000 PennyLane-0.8.1/LICENSE
--rwxrwxrwx   0 josh      (1000) josh      (1000)      112 2019-12-23 19:55:34.000000 PennyLane-0.8.1/MANIFEST.in
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1873 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/about.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/beta/
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/beta/plugins/
--rwxrwxrwx   0 josh      (1000) josh      (1000)    20893 2020-02-28 12:01:31.000000 PennyLane-0.8.1/pennylane/beta/plugins/default_tensor.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    12767 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/beta/plugins/default_tensor_tf.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      804 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/beta/plugins/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      669 2020-02-27 06:08:59.000000 PennyLane-0.8.1/pennylane/beta/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/circuit_drawer/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     5397 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/circuit_drawer/charsets.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    14569 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/circuit_drawer/circuit_drawer.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     5593 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/circuit_drawer/grid.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    15235 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/circuit_drawer/representation_resolver.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      870 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/circuit_drawer/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    19488 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/circuit_graph.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/collections/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2029 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/collections/apply.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4962 2020-02-28 04:09:53.000000 PennyLane-0.8.1/pennylane/collections/dot.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     5707 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/collections/map.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     9263 2020-02-28 04:09:53.000000 PennyLane-0.8.1/pennylane/collections/qnode_collection.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2210 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/collections/sum.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      827 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/collections/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4510 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/configuration.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    28906 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/init.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/interfaces/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3171 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/interfaces/autograd.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4193 2020-02-27 06:11:56.000000 PennyLane-0.8.1/pennylane/interfaces/tf.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7589 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/interfaces/torch.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      818 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/interfaces/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7462 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/io.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     6264 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/measure.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    44002 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/operation.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:07.000000 PennyLane-0.8.1/pennylane/ops/
--rwxrwxrwx   0 josh      (1000) josh      (1000)    29058 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/ops/cv.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    33763 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/ops/qubit.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1960 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/ops/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:08.000000 PennyLane-0.8.1/pennylane/optimize/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3014 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/optimize/adagrad.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4174 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/optimize/adam.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3887 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/optimize/gradient_descent.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2608 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/optimize/momentum.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2632 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/optimize/nesterov_momentum.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     6513 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/optimize/qng.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3030 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/optimize/rms_prop.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1340 2020-02-28 04:09:53.000000 PennyLane-0.8.1/pennylane/optimize/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:08.000000 PennyLane-0.8.1/pennylane/plugins/
--rwxrwxrwx   0 josh      (1000) josh      (1000)    27433 2020-02-28 12:01:31.000000 PennyLane-0.8.1/pennylane/plugins/default_gaussian.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     8468 2020-02-28 12:01:31.000000 PennyLane-0.8.1/pennylane/plugins/default_qubit.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1128 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/plugins/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:08.000000 PennyLane-0.8.1/pennylane/qnodes/
--rwxrwxrwx   0 josh      (1000) josh      (1000)    33354 2020-02-28 12:21:13.000000 PennyLane-0.8.1/pennylane/qnodes/base.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    12744 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/qnodes/cv.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7855 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/qnodes/decorator.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1913 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/qnodes/device_jacobian.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    16372 2020-02-28 04:09:53.000000 PennyLane-0.8.1/pennylane/qnodes/jacobian.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     5927 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/qnodes/passthru.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    17557 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/qnodes/qubit.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      911 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/qnodes/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:08.000000 PennyLane-0.8.1/pennylane/templates/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1880 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/decorator.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:09.000000 PennyLane-0.8.1/pennylane/templates/embeddings/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7999 2020-02-28 04:10:07.000000 PennyLane-0.8.1/pennylane/templates/embeddings/amplitude.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3000 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/angle.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2216 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/basis.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3023 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/displacement.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    10393 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/qaoa.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3043 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/squeezing.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1058 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/embeddings/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:09.000000 PennyLane-0.8.1/pennylane/templates/layers/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7163 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/layers/cv_neural_net.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     6438 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/layers/random.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4910 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/layers/strongly_entangling.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      941 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/layers/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:09.000000 PennyLane-0.8.1/pennylane/templates/state_preparations/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2497 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/state_preparations/basis.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     9706 2020-02-28 04:10:08.000000 PennyLane-0.8.1/pennylane/templates/state_preparations/mottonen.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      811 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/state_preparations/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:09.000000 PennyLane-0.8.1/pennylane/templates/subroutines/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7187 2020-02-27 06:07:06.000000 PennyLane-0.8.1/pennylane/templates/subroutines/interferometer.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      881 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/subroutines/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     6047 2020-02-28 04:10:08.000000 PennyLane-0.8.1/pennylane/templates/utils.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      838 2020-02-27 06:07:05.000000 PennyLane-0.8.1/pennylane/templates/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    15078 2020-02-28 04:10:08.000000 PennyLane-0.8.1/pennylane/utils.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7063 2020-02-28 04:10:08.000000 PennyLane-0.8.1/pennylane/variable.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:09.000000 PennyLane-0.8.1/pennylane/vqe/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7530 2020-02-27 06:09:00.000000 PennyLane-0.8.1/pennylane/vqe/vqe.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      760 2020-02-27 06:09:00.000000 PennyLane-0.8.1/pennylane/vqe/__init__.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    18953 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/_device.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    17023 2020-02-27 06:07:04.000000 PennyLane-0.8.1/pennylane/_qubit_device.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)      673 2020-02-28 12:01:31.000000 PennyLane-0.8.1/pennylane/_version.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7708 2020-02-27 06:08:59.000000 PennyLane-0.8.1/pennylane/__init__.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:06.000000 PennyLane-0.8.1/PennyLane.egg-info/
--rwxrwxrwx   0 josh      (1000) josh      (1000)        1 2020-02-28 12:33:04.000000 PennyLane-0.8.1/PennyLane.egg-info/dependency_links.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)      267 2020-02-28 12:33:04.000000 PennyLane-0.8.1/PennyLane.egg-info/entry_points.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)     9656 2020-02-28 12:33:04.000000 PennyLane-0.8.1/PennyLane.egg-info/PKG-INFO
--rwxrwxrwx   0 josh      (1000) josh      (1000)       65 2020-02-28 12:33:04.000000 PennyLane-0.8.1/PennyLane.egg-info/requires.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3590 2020-02-28 12:33:05.000000 PennyLane-0.8.1/PennyLane.egg-info/SOURCES.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)       10 2020-02-28 12:33:04.000000 PennyLane-0.8.1/PennyLane.egg-info/top_level.txt
--rwxrwxrwx   0 josh      (1000) josh      (1000)     9656 2020-02-28 12:33:10.000000 PennyLane-0.8.1/PKG-INFO
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7140 2020-02-28 12:32:57.000000 PennyLane-0.8.1/README.rst
--rwxrwxrwx   0 josh      (1000) josh      (1000)       38 2020-02-28 12:33:10.000000 PennyLane-0.8.1/setup.cfg
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2680 2020-02-28 04:14:33.000000 PennyLane-0.8.1/setup.py
-drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-02-28 12:33:10.000000 PennyLane-0.8.1/tests/
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4478 2020-02-27 06:07:05.000000 PennyLane-0.8.1/tests/conftest.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     4933 2020-02-27 06:07:05.000000 PennyLane-0.8.1/tests/gate_data.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1965 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_about.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     8126 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_classical_gradients.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     5724 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_configuration.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    28428 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_default_gaussian.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    66529 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_default_qubit.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    24490 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_device.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3766 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_hermitian_edge_cases.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7797 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_init.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3149 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_io.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     7784 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_measure.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     1255 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_observable.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    42668 2020-02-28 04:10:08.000000 PennyLane-0.8.1/tests/test_operation.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    21967 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_optimize.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2902 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_optimize_qng.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3474 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_prob.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    23761 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_quantum_gradients.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    24316 2020-02-28 04:10:08.000000 PennyLane-0.8.1/tests/test_qubit_device.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    34710 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     2948 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates_decorator.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    26481 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates_embeddings.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    16300 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates_layers.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    14305 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates_state_preparations.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     9671 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_templates_subroutines.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     8713 2020-02-28 04:10:08.000000 PennyLane-0.8.1/tests/test_templates_utils.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    16959 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_tensor_measurements.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    30893 2020-02-27 06:07:06.000000 PennyLane-0.8.1/tests/test_utils.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)     3389 2020-02-28 04:10:08.000000 PennyLane-0.8.1/tests/test_variable.py
--rwxrwxrwx   0 josh      (1000) josh      (1000)    18067 2020-02-27 06:09:00.000000 PennyLane-0.8.1/tests/test_vqe.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:32.000000 PennyLane-0.9.0/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    11357 2019-02-13 23:40:16.000000 PennyLane-0.9.0/LICENSE
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      112 2020-05-05 06:04:52.000000 PennyLane-0.9.0/MANIFEST.in
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9583 2020-05-15 01:45:32.000000 PennyLane-0.9.0/PKG-INFO
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9583 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/PKG-INFO
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3904 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/SOURCES.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)        1 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/dependency_links.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      267 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/entry_points.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)       65 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/requires.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)       10 2020-05-15 01:45:30.000000 PennyLane-0.9.0/PennyLane.egg-info/top_level.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7137 2020-05-15 01:45:20.000000 PennyLane-0.9.0/README.rst
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:30.000000 PennyLane-0.9.0/doc/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      792 2020-02-27 06:07:04.000000 PennyLane-0.9.0/doc/Makefile
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    13514 2020-05-15 01:43:25.000000 PennyLane-0.9.0/doc/conf.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     6154 2020-04-30 12:35:28.000000 PennyLane-0.9.0/doc/directives.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7349 2020-04-30 12:35:28.000000 PennyLane-0.9.0/doc/index.rst
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      314 2020-02-27 06:07:04.000000 PennyLane-0.9.0/doc/requirements.txt
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3140 2020-05-05 06:04:52.000000 PennyLane-0.9.0/example_config.toml
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:30.000000 PennyLane-0.9.0/pennylane/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7870 2020-04-23 04:59:21.000000 PennyLane-0.9.0/pennylane/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    19169 2020-05-15 00:46:54.000000 PennyLane-0.9.0/pennylane/_device.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    19059 2020-05-08 08:32:16.000000 PennyLane-0.9.0/pennylane/_qubit_device.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3702 2020-03-17 12:20:11.000000 PennyLane-0.9.0/pennylane/_queuing_context.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      673 2020-05-15 01:43:25.000000 PennyLane-0.9.0/pennylane/_version.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1873 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/about.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:30.000000 PennyLane-0.9.0/pennylane/beta/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      669 2020-02-27 06:08:59.000000 PennyLane-0.9.0/pennylane/beta/__init__.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:30.000000 PennyLane-0.9.0/pennylane/beta/plugins/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      804 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/beta/plugins/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    20979 2020-05-07 04:06:40.000000 PennyLane-0.9.0/pennylane/beta/plugins/default_tensor.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    14303 2020-05-15 00:46:54.000000 PennyLane-0.9.0/pennylane/beta/plugins/default_tensor_tf.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/circuit_drawer/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      870 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/circuit_drawer/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5437 2020-03-16 04:02:03.000000 PennyLane-0.9.0/pennylane/circuit_drawer/charsets.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    14569 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/circuit_drawer/circuit_drawer.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5593 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/circuit_drawer/grid.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    16085 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/circuit_drawer/representation_resolver.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    18777 2020-05-08 02:19:26.000000 PennyLane-0.9.0/pennylane/circuit_graph.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/collections/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      827 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/collections/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2029 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/collections/apply.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     4962 2020-02-28 04:09:53.000000 PennyLane-0.9.0/pennylane/collections/dot.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5773 2020-04-18 07:21:33.000000 PennyLane-0.9.0/pennylane/collections/map.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9267 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/collections/qnode_collection.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2210 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/collections/sum.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     4510 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/configuration.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    35022 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/init.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/interfaces/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      818 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/interfaces/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3171 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/interfaces/autograd.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5227 2020-05-14 15:23:23.000000 PennyLane-0.9.0/pennylane/interfaces/tf.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7615 2020-05-07 02:38:01.000000 PennyLane-0.9.0/pennylane/interfaces/torch.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7462 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/io.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5312 2020-04-23 06:35:47.000000 PennyLane-0.9.0/pennylane/measure.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    50491 2020-05-07 04:06:40.000000 PennyLane-0.9.0/pennylane/operation.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/ops/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2051 2020-05-07 04:06:40.000000 PennyLane-0.9.0/pennylane/ops/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    30990 2020-05-07 04:06:40.000000 PennyLane-0.9.0/pennylane/ops/cv.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    44553 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/ops/qubit.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/optimize/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1479 2020-03-17 12:20:11.000000 PennyLane-0.9.0/pennylane/optimize/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3008 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/optimize/adagrad.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     4170 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/optimize/adam.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3887 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/optimize/gradient_descent.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2608 2020-02-27 06:07:04.000000 PennyLane-0.9.0/pennylane/optimize/momentum.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2632 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/optimize/nesterov_momentum.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9104 2020-05-06 05:34:57.000000 PennyLane-0.9.0/pennylane/optimize/qng.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3024 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/optimize/rms_prop.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9300 2020-05-15 01:43:25.000000 PennyLane-0.9.0/pennylane/optimize/rotoselect.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5499 2020-05-15 01:43:25.000000 PennyLane-0.9.0/pennylane/optimize/rotosolve.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/plugins/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1128 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/plugins/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    27522 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/plugins/default_gaussian.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    11952 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/plugins/default_qubit.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/qnn/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      732 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/qnn/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    12555 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/qnn/keras.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/qnodes/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      911 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/qnodes/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    32684 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/qnodes/base.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    12744 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/qnodes/cv.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    12061 2020-05-15 00:46:54.000000 PennyLane-0.9.0/pennylane/qnodes/decorator.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1913 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/qnodes/device_jacobian.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    17950 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/qnodes/jacobian.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     6736 2020-05-14 15:23:23.000000 PennyLane-0.9.0/pennylane/qnodes/passthru.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    17557 2020-02-27 06:07:05.000000 PennyLane-0.9.0/pennylane/qnodes/qubit.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/templates/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      863 2020-03-16 04:01:56.000000 PennyLane-0.9.0/pennylane/templates/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    17034 2020-03-16 04:01:56.000000 PennyLane-0.9.0/pennylane/templates/broadcast (josh-workstation's conflicted copy 2020-03-16).py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    19463 2020-04-30 12:35:28.000000 PennyLane-0.9.0/pennylane/templates/broadcast.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1888 2020-03-16 04:01:56.000000 PennyLane-0.9.0/pennylane/templates/decorator.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/templates/embeddings/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1088 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/templates/embeddings/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7999 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/embeddings/amplitude.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3071 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/embeddings/angle.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2359 2020-04-18 07:21:33.000000 PennyLane-0.9.0/pennylane/templates/embeddings/basis.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3293 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/embeddings/displacement.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9519 2020-05-05 05:02:21.000000 PennyLane-0.9.0/pennylane/templates/embeddings/iqp.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    10031 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/embeddings/qaoa.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3431 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/embeddings/squeezing.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/templates/layers/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1046 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/layers/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5580 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/layers/basic_entangler.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7231 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/layers/cv_neural_net.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    10280 2020-04-30 12:35:29.000000 PennyLane-0.9.0/pennylane/templates/layers/random.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7128 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/layers/simplified_two_design.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5081 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/layers/strongly_entangling.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/templates/state_preparations/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      878 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/state_preparations/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2970 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/state_preparations/arbitrary_state_preparation.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2489 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/state_preparations/basis.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     9704 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/state_preparations/mottonen.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/templates/subroutines/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      929 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/subroutines/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3558 2020-05-07 04:06:41.000000 PennyLane-0.9.0/pennylane/templates/subroutines/arbitrary_unitary.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7177 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/subroutines/interferometer.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     6194 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/templates/utils.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    13946 2020-04-14 06:27:48.000000 PennyLane-0.9.0/pennylane/utils.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7063 2020-03-16 04:01:57.000000 PennyLane-0.9.0/pennylane/variable.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:31.000000 PennyLane-0.9.0/pennylane/vqe/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)      760 2020-02-27 06:09:00.000000 PennyLane-0.9.0/pennylane/vqe/__init__.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     8502 2020-05-06 05:34:57.000000 PennyLane-0.9.0/pennylane/vqe/vqe.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)       38 2020-05-15 01:45:32.000000 PennyLane-0.9.0/setup.cfg
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     2682 2020-05-15 01:43:25.000000 PennyLane-0.9.0/setup.py
+drwxrwxrwx   0 josh      (1000) josh      (1000)        0 2020-05-15 01:45:32.000000 PennyLane-0.9.0/tests/
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     4478 2020-05-07 06:21:55.000000 PennyLane-0.9.0/tests/conftest.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     5020 2020-05-07 04:06:41.000000 PennyLane-0.9.0/tests/gate_data.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1965 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_about.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     8126 2020-04-23 04:59:21.000000 PennyLane-0.9.0/tests/test_classical_gradients.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     6344 2020-05-05 06:04:52.000000 PennyLane-0.9.0/tests/test_configuration.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    28440 2020-05-07 04:06:41.000000 PennyLane-0.9.0/tests/test_default_gaussian.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    71361 2020-05-07 04:06:41.000000 PennyLane-0.9.0/tests/test_default_qubit.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    24490 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_device.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3766 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_hermitian_edge_cases.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    16848 2020-05-05 05:02:21.000000 PennyLane-0.9.0/tests/test_init.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3149 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_io.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7784 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_measure.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     1255 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_observable.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    43951 2020-05-07 04:06:41.000000 PennyLane-0.9.0/tests/test_operation.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    26926 2020-05-15 01:43:25.000000 PennyLane-0.9.0/tests/test_optimize.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     6360 2020-05-06 05:34:57.000000 PennyLane-0.9.0/tests/test_optimize_qng.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3907 2020-04-23 06:35:47.000000 PennyLane-0.9.0/tests/test_prob.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    23761 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_quantum_gradients.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    24474 2020-04-14 08:28:53.000000 PennyLane-0.9.0/tests/test_qubit_device.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     7433 2020-03-17 12:20:12.000000 PennyLane-0.9.0/tests/test_queuing_context.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    16959 2020-02-27 06:07:06.000000 PennyLane-0.9.0/tests/test_tensor_measurements.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    30966 2020-04-14 06:27:49.000000 PennyLane-0.9.0/tests/test_utils.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)     3389 2020-03-16 04:01:57.000000 PennyLane-0.9.0/tests/test_variable.py
+-rwxrwxrwx   0 josh      (1000) josh      (1000)    18784 2020-04-18 07:21:33.000000 PennyLane-0.9.0/tests/test_vqe.py
```

### Comparing `PennyLane-0.8.1/default_config.toml` & `PennyLane-0.9.0/example_config.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,89 +3,104 @@
 ## =================================================================
 ## This section contains the main PennyLane configuration options.
 ## These options apply globally to PennyLane and all loaded plugins
 ## and devices which support them.
 ##
 ## To overide these default configuration settings per device/plugin,
 ## please use the per-device settings below.
+##
+## Some example configuration settings are shown here in lines
+## commented with a single # character. For any of the options to take
+## effect, uncomment the line with a single # character and modify
+## the value (if desired).
 
-## set the default number of shots/runs used
-## to determine expectation value statistics
 [main]
-shots = 1000
+# shots = 1000
 
-# =================================================================
-#     PLUGIN AND DEVICE OPTIONS
-# =================================================================
+## =================================================================
+##     PLUGIN AND DEVICE OPTIONS
+## =================================================================
 ## This section contains the PennyLane configuration options for each
 ## installed plugin or device. These configuration options allow you
 ## to set global configuration options on a device-by-device basis.
 ## and to also set options specific to certain device.
+##
+## You may add additional plugin- and device-specific options here.
+## Options that apply globally to all devices within a single plugin
+## are grouped under the
+##
+##   [plugin.global]
+##
+## heading. Options that apply only to a specific device are grouped
+## under the
+##
+##   [plugin.device]
+##
+## heading.
 
 [default.gaussian]
-hbar = 2
+# hbar = 2
 
 
 [strawberryfields.global]
 ## Global options for the StrawberryFields plugin.
 ## If not specified, the PennyLane default is used.
 ##
 ## These global options may be overwritten by specifying
 ## the defaults for the Fock and Gaussian simulators below.
+##
+## For more details, see the PennyLane-SF documentation:
+## https://pennylane-sf.readthedocs.io
 
 ## Set the default value of hbar
-hbar = 1
+# hbar = 2
 
 ## set the default number of shots/runs used
 ## to determine expectation value statistics
 # shots = 1000
-# analytic = True
+# analytic = true
 
     [strawberryfields.fock]
     ## Default options for the Fock simulator
 
     ## Set the default Fock space truncation
-    cutoff_dim = 10
+    # cutoff_dim = 10
 
     ## set the default number of shots
     # shots = 1000
 
-    ## Set the default value of hbar
-    # hbar = 1
-
     [strawberryfields.gaussian]
     ## Default options for the Gaussian simulator
 
     ## set the default number of shots
     # shots = 1000
 
     ## Set the default value of hbar
-    # hbar = 1
+    # hbar = 2
 
-[projectq.global]
-## Options for the ProjectQ plugin.
+[qiskit.global]
+## Global options for the Qiskit plugin.
+## For more details, see the PennyLane-Qiskit documentation:
+## https://pennylaneqiskit.readthedocs.io/en/latest/index.html
 
-    [projectq.simulator]
-    ## If True, gates are cached and only executed once a
-    ## certain gate-size has been reached
-    # gate_fusion =
+# backend = "qasm_simulator"
 
-    ## Random seed (uses random.randint(0, 4294967295) by default)
-    # rnd_seed =
+    [qiskit.aer]
+    ## Default options for Qiskit Aer
 
-    [projectq.ibm]
-    ## IBM Quantum Experience user name and password
-    # user =
-    # password =
+    ## set the default backend for the Qiskit Aer device
+    # backend = "unitary_simulator"
+    # backend_options = {"validation_threshold" = 1e-6}
 
-    ## Whether to use the IBM quantum chip instead of the IBM simulator
-    # use_hardware = true
+    [qiskit.ibmq]
+    ## Default options for IBMQ
 
-    ## Device to use (‘ibmqx4’, or ‘ibmqx5’)
-    # device =
+    ## IBM Quantum Experience authentication token
+    # ibmqx_token = "XXX"
 
-    ## Number of runs used to collect statistics
-    # num_runs = 1024
+    ## hardware backend device
+    # backend = "ibmq_rome"
 
-    ## If True, statistics are printed, in addition to the
-    ## measurement result being registered (at the end of the circuit).
-    # verbose = false
+    ## pass optional provider information
+    # hub = "MYHUB"
+    # group = "MYGROUP"
+    # project = "MYPROJECT"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PennyLane-0.8.1/doc/conf.py` & `PennyLane-0.9.0/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
-
+import pyscf
 import sys, os, re
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.insert(0, os.path.abspath('_ext'))
@@ -93,16 +93,18 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'PennyLane'
-copyright = """
-    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan, and Nathan Killoran. <br>
+copyright = """\
+Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+Zeyue Niu, Antal Száva, and Nathan Killoran. <br>
 PennyLane: Automatic differentiation of hybrid quantum-classical computations. arXiv:1811.04968, 2018.<br>
 &copy; Copyright 2018-2020, Xanadu Quantum Technologies Inc."""
 author = 'Xanadu Inc.'
 
 add_module_names = False
 
 # The version info for the project you're documenting, acts as replacement for
@@ -402,13 +404,14 @@
 
 # the order in which autodoc lists the documented members
 autodoc_member_order = 'bysource'
 
 # inheritance_diagram graphviz attributes
 inheritance_node_attrs = dict(color='lightskyblue1', style='filled')
 
-from directives import UsageDetails, CustomGalleryItemDirective
+from directives import UsageDetails, CustomGalleryItemDirective, TitleCardDirective
 
 def setup(app):
     app.add_directive('customgalleryitem', CustomGalleryItemDirective)
+    app.add_directive('titlecard', TitleCardDirective)
     app.add_directive("usagedetails", UsageDetails)
     app.add_stylesheet('xanadu_gallery.css')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PennyLane-0.8.1/doc/directives.py` & `PennyLane-0.9.0/doc/directives.py`

 * *Files 23% similar despite different names*

```diff
@@ -122,7 +122,78 @@
         thumbnail_rst = GALLERY_TEMPLATE.format(thumbnail=thumbnail,
                                                 description=description,
                                                 link=link)
         thumbnail = StringList(thumbnail_rst.split('\n'))
         thumb = nodes.paragraph()
         self.state.nested_parse(thumbnail, self.content_offset, thumb)
         return [thumb]
+
+
+TITLE_CARD_TEMPLATE = """
+.. raw:: html
+
+    <div class="card" style="width: 15rem; float:left; margin: 10px;">
+        <a href={link}>
+            <div class="card-header">
+                <b>{name}</b>
+            </div>
+            <div class="card-body">
+                <p class="card-text"> {description} </p>
+            </div>
+        </a>
+    </div>
+"""
+
+
+class TitleCardDirective(Directive):
+    """Create a sphinx gallery style thumbnail.
+    tooltip and figure are self explanatory. Description could be a link to
+    a document like in below example.
+    Example usage:
+
+    .. customgalleryitem::
+        :name: Installation
+        :description: Description of page
+        :link: /path/to/page
+
+    """
+
+    required_arguments = 0
+    optional_arguments = 4
+    final_argument_whitespace = True
+    option_spec = {'name': directives.unchanged,
+                   'description': directives.unchanged,
+                   'link': directives.unchanged}
+
+    has_content = False
+    add_index = False
+
+    def run(self):
+        try:
+            if 'name' in self.options:
+                name = self.options['name']
+
+            if 'description' in self.options:
+                description = self.options['description']
+            else:
+                raise ValueError('description not found')
+
+            if 'link' in self.options:
+                link = self.options['link']
+            else:
+                link = "code/qml_templates"
+
+        except FileNotFoundError as e:
+            print(e)
+            return []
+        except ValueError as e:
+            print(e)
+            raise
+            return []
+
+        thumbnail_rst = TITLE_CARD_TEMPLATE.format(name=name,
+                                                   description=description,
+                                                   link=link)
+        thumbnail = StringList(thumbnail_rst.split('\n'))
+        thumb = nodes.paragraph()
+        self.state.nested_parse(thumbnail, self.content_offset, thumb)
+        return [thumb]
```

### Comparing `PennyLane-0.8.1/doc/index.rst` & `PennyLane-0.9.0/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -109,43 +109,47 @@
   devices, including **Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**,
   **Microsoft QDK**, and **ProjectQ**.
 
 
 Getting started
 ---------------
 
-For getting started with PennyLane, check out some of the
-`key concepts <https://pennylane.ai/qml/concepts.html>`_ behind quantum machine
-learning, before moving on to some `introductory tutorials <https://pennylane.ai/qml/beginner.html>`_.
+For an introduction to quantum machine learning, we have several guides and resources available
+on our `QML website <https://pennylane.ai/qml/>`_, including
+`What is QML? <https://pennylane.ai/qml/whatisqml.html>`_,
+`frequently asked questions <https://pennylane.ai/faq.html>`_,
+a `glossary of key concepts <https://pennylane.ai/qml/glossary.html>`_, and a curated selection
+of `QML videos <https://pennylane.ai/qml/videos.html>`_.
 
 Then, take a deeper dive into quantum machine learning by
 exploring cutting-edge algorithms using PennyLane and near-term quantum hardware,
 with our collection of
-`QML tutorials <https://pennylane.ai/qml/implementations.html>`_.
+`QML demonstrations <https://pennylane.ai/qml/demonstrations.html>`_.
 
 You can also check out the :doc:`Using PennyLane <introduction/pennylane>` section for
 more details on the :doc:`quantum operations <introduction/operations>`, and to explore
 the available :doc:`optimization tools <introduction/optimizers>` provided by PennyLane.
 We also have a detailed guide on :doc:`how to write your own <development/plugins>`
 PennyLane-compatible quantum device.
 
 Finally, play around with the numerous `devices and plugins <https://pennylane.ai/plugins.html>`_
 available for running your hybrid optimizations—these include
-IBM Q, provided by the `PennyLane-Qiskit <https://pennylane-qiskit.rtfd.io>`__ plugin,
-as well as the Rigetti Aspen-1 QPU provided by `PennyLane-Forest <https://pennylane-forest.rtfd.io>`__.
+IBM Q, provided by the `PennyLane-Qiskit <https://pennylaneqiskit.rtfd.io>`__ plugin,
+as well as the Rigetti Aspen QPU provided by `PennyLane-Forest <https://pennylane-forest.rtfd.io>`__.
 
 How to cite
 -----------
 
 If you are doing research using PennyLane, please cite
 
 .. rst-class:: admonition warning
 
-    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan,
-    and Nathan Killoran.
+    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+    Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+    Zeyue Niu, Antal Száva, and Nathan Killoran.
     *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
     `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
 
 Support and contribution
 ------------------------
 
 - **Source Code:** https://github.com/XanaduAI/PennyLane
@@ -185,25 +189,27 @@
 .. toctree::
    :maxdepth: 1
    :caption: Development
    :hidden:
 
    development/guide
    development/plugins
+   development/adding_templates
    development/release_notes.md
 
 .. toctree::
    :maxdepth: 1
    :caption: API
    :hidden:
 
    code/qml
    code/qml_init
    code/qml_interfaces
    code/qml_operation
    code/qml_plugins
    code/qml_qchem
+   code/qml_qnn
    code/qml_qnodes
    code/qml_templates
    code/qml_utils
    code/qml_variable
    code/qml_beta
```

#### html2text {}

```diff
@@ -14,38 +14,43 @@
 differentiation** of quantum circuits. .. - *Best of both worlds*. Support for
 **hybrid quantum and classical** models; connect quantum hardware with PyTorch,
 TensorFlow, and NumPy. .. - *Batteries included*. Provides **optimization and
 machine learning** tools. .. - *Device independent*. The same quantum circuit
 model can be **run on different backends**. Install `plugins
 pennylane.ai/plugins.html>`_ to access even more devices, including
 **Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**,
-**Microsoft QDK**, and **ProjectQ**. Getting started --------------- For
-getting started with PennyLane, check out some of the `key concepts
-pennylane.ai/qml/concepts.html>`_ behind quantum machine learning, before
-moving on to some `introductory tutorials
-pennylane.ai/qml/beginner.html>`_. Then, take a deeper dive into quantum
-machine learning by exploring cutting-edge algorithms using PennyLane and near-
-term quantum hardware, with our collection of `QML tutorials
-pennylane.ai/qml/implementations.html>`_. You can also check out the :doc:
-`Using PennyLane
+**Microsoft QDK**, and **ProjectQ**. Getting started --------------- For an
+introduction to quantum machine learning, we have several guides and resources
+available on our `QML website
+pennylane.ai/qml/>`_, including `What is QML?
+pennylane.ai/qml/whatisqml.html>`_, `frequently asked questions
+pennylane.ai/faq.html>`_, a `glossary of key concepts
+pennylane.ai/qml/glossary.html>`_, and a curated selection of `QML videos
+pennylane.ai/qml/videos.html>`_. Then, take a deeper dive into quantum machine
+learning by exploring cutting-edge algorithms using PennyLane and near-term
+quantum hardware, with our collection of `QML demonstrations
+pennylane.ai/qml/demonstrations.html>`_. You can also check out the :doc:`Using
+PennyLane
 ennylane>` section for more details on the :doc:`quantum operations
 perations>`, and to explore the available :doc:`optimization tools
 ptimizers>` provided by PennyLane. We also have a detailed guide on :doc:`how
 to write your own
 lugins>` PennyLane-compatible quantum device. Finally, play around with the
 numerous `devices and plugins
 pennylane.ai/plugins.html>`_ available for running your hybrid
 optimizationsâthese include IBM Q, provided by the `PennyLane-Qiskit
-pennylane-qiskit.rtfd.io>`__ plugin, as well as the Rigetti Aspen-1 QPU
-provided by `PennyLane-Forest
+pennylaneqiskit.rtfd.io>`__ plugin, as well as the Rigetti Aspen QPU provided
+by `PennyLane-Forest
 pennylane-forest.rtfd.io>`__. How to cite ----------- If you are doing research
 using PennyLane, please cite .. rst-class:: admonition warning Ville Bergholm,
-Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan, and
-Nathan Killoran. *PennyLane: Automatic differentiation of hybrid quantum-
-classical computations.* 2018. `arXiv:1811.04968
+Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri
+McKiernan, Johannes Jakob Meyer, Zeyue Niu, Antal SzÃ¡va, and Nathan Killoran.
+*PennyLane: Automatic differentiation of hybrid quantum-classical
+computations.* 2018. `arXiv:1811.04968
 arxiv.org/abs/1811.04968>`_ Support and contribution ------------------------ -
 **Source Code:** https://github.com/XanaduAI/PennyLane - **Issue Tracker:**
 https://github.com/XanaduAI/PennyLane/issues If you are having issues, please
 let us know by posting the issue on our GitHub issue tracker. We encourage
 contributions â simply fork the PennyLane repository, and then make a `pull
 request
 help.github.com/articles/about-pull-requests/>`_ containing your contribution.
@@ -57,11 +62,11 @@
 discuss.pennylane.ai>`_. License ------- PennyLane is **free** and **open
 source**, released under the Apache License, Version 2.0. .. toctree:: :
 maxdepth: 1 :caption: Using PennyLane :hidden: introduction/pennylane
 introduction/circuits introduction/interfaces introduction/operations
 introduction/measurements introduction/templates introduction/optimizers
 introduction/chemistry introduction/configuration .. toctree:: :maxdepth: 1 :
 caption: Development :hidden: development/guide development/plugins
-development/release_notes.md .. toctree:: :maxdepth: 1 :caption: API :hidden:
-code/qml code/qml_init code/qml_interfaces code/qml_operation code/qml_plugins
-code/qml_qchem code/qml_qnodes code/qml_templates code/qml_utils code/
-qml_variable code/qml_beta
+development/adding_templates development/release_notes.md .. toctree:: :
+maxdepth: 1 :caption: API :hidden: code/qml code/qml_init code/qml_interfaces
+code/qml_operation code/qml_plugins code/qml_qchem code/qml_qnn code/qml_qnodes
+code/qml_templates code/qml_utils code/qml_variable code/qml_beta
```

### Comparing `PennyLane-0.8.1/doc/Makefile` & `PennyLane-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/LICENSE` & `PennyLane-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/about.py` & `PennyLane-0.9.0/pennylane/about.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/beta/plugins/default_tensor.py` & `PennyLane-0.9.0/pennylane/beta/plugins/default_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
 Experimental simulator plugin based on tensor network contractions
 """
-
+import math
+import cmath
 import warnings
 from itertools import product
 
 import numpy as np
 from numpy.linalg import eigh
 
 try:
@@ -61,21 +62,21 @@
 
 I = np.eye(2)
 # Pauli matrices
 X = np.array([[0, 1], [1, 0]])  #: Pauli-X matrix
 Y = np.array([[0, -1j], [1j, 0]])  #: Pauli-Y matrix
 Z = np.array([[1, 0], [0, -1]])  #: Pauli-Z matrix
 
-H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)  #: Hadamard gate
+H = np.array([[1, 1], [1, -1]]) / math.sqrt(2)  #: Hadamard gate
 # Two qubit gates
 CNOT = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])  #: CNOT gate
 SWAP = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])  #: SWAP gate
 CZ = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])  #: CZ gate
 S = np.array([[1, 0], [0, 1j]])  #: Phase Gate
-T = np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])  #: T Gate
+T = np.array([[1, 0], [0, cmath.exp(1j * np.pi / 4)]])  #: T Gate
 # Three qubit gates
 CSWAP = np.array(
     [
         [1, 0, 0, 0, 0, 0, 0, 0],
         [0, 1, 0, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 0, 1, 0, 0, 0, 0],
@@ -98,48 +99,48 @@
     r"""One-qubit phase shift.
 
     Args:
         phi (float): phase shift angle
     Returns:
         array: unitary 2x2 phase shift matrix
     """
-    return np.array([[1, 0], [0, np.exp(1j * phi)]])
+    return np.array([[1, 0], [0, cmath.exp(1j * phi)]])
 
 
 def Rotx(theta):
     r"""One-qubit rotation about the x axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_x \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * X
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * X
 
 
 def Roty(theta):
     r"""One-qubit rotation about the y axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_y \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Y
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * Y
 
 
 def Rotz(theta):
     r"""One-qubit rotation about the z axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_z \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Z
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * Z
 
 
 def Rot3(a, b, c):
     r"""Arbitrary one-qubit rotation using three Euler angles.
 
     Args:
         a,b,c (float): rotation angles
@@ -157,16 +158,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_x(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.cos(theta / 2), -1j * np.sin(theta / 2)],
-            [0, 0, -1j * np.sin(theta / 2), np.cos(theta / 2)],
+            [0, 0, math.cos(theta / 2), -1j * math.sin(theta / 2)],
+            [0, 0, -1j * math.sin(theta / 2), math.cos(theta / 2)],
         ]
     )
 
 
 def CRoty(theta):
     r"""Two-qubit controlled rotation about the y axis.
 
@@ -175,16 +176,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_y(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.cos(theta / 2), -np.sin(theta / 2)],
-            [0, 0, np.sin(theta / 2), np.cos(theta / 2)],
+            [0, 0, math.cos(theta / 2), -math.sin(theta / 2)],
+            [0, 0, math.sin(theta / 2), math.cos(theta / 2)],
         ]
     )
 
 
 def CRotz(theta):
     r"""Two-qubit controlled rotation about the z axis.
 
@@ -193,16 +194,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_z(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.exp(-1j * theta / 2), 0],
-            [0, 0, 0, np.exp(1j * theta / 2)],
+            [0, 0, cmath.exp(-1j * theta / 2), 0],
+            [0, 0, 0, cmath.exp(1j * theta / 2)],
         ]
     )
 
 
 def CRot3(a, b, c):
     r"""Arbitrary two-qubit controlled rotation using three Euler angles.
 
@@ -214,22 +215,22 @@
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
             [
                 0,
                 0,
-                np.exp(-1j * (a + c) / 2) * np.cos(b / 2),
-                -np.exp(1j * (a - c) / 2) * np.sin(b / 2),
+                cmath.exp(-1j * (a + c) / 2) * math.cos(b / 2),
+                -cmath.exp(1j * (a - c) / 2) * math.sin(b / 2),
             ],
             [
                 0,
                 0,
-                np.exp(-1j * (a - c) / 2) * np.sin(b / 2),
-                np.exp(1j * (a + c) / 2) * np.cos(b / 2),
+                cmath.exp(-1j * (a - c) / 2) * math.sin(b / 2),
+                cmath.exp(1j * (a + c) / 2) * math.cos(b / 2),
             ],
         ]
     )
 
 
 # ========================================================
 #  Arbitrary states and operators
@@ -300,16 +301,16 @@
 
     Args:
         wires (int): the number of modes to initialize the device in
     """
 
     name = "PennyLane TensorNetwork simulator plugin"
     short_name = "default.tensor"
-    pennylane_requires = "0.8"
-    version = "0.8.1"
+    pennylane_requires = "0.9"
+    version = "0.9.0"
     author = "Xanadu Inc."
     _capabilities = {"model": "qubit", "tensor_observables": True}
 
     _operation_map = {
         "BasisState": None,
         "QubitStateVector": None,
         "QubitUnitary": unitary,
```

### Comparing `PennyLane-0.8.1/pennylane/beta/plugins/default_tensor_tf.py` & `PennyLane-0.9.0/pennylane/beta/plugins/default_tensor_tf.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,42 +196,75 @@
 
     To use this device, you will need to install TensorFlow and TensorNetwork:
 
     .. code-block:: bash
 
         pip install tensornetwork>=0.2 tensorflow>=2.0
 
-    **Example:**
+    **Example**
 
-    >>> dev = qml.device("default.tensor.tf", wires=1)
-    >>> @qml.qnode(dev, interface="autograd", diff_method="best")
-    >>> def circuit(x):
-    ...     qml.RX(x[1], wires=0)
-    ...     qml.Rot(x[0], x[1], x[2], wires=0)
-    ...     return qml.expval(qml.PauliZ(0))
-    >>> grad_fn = qml.grad(circuit, argnum=[0])
-    >>> print(grad_fn([0.2, 0.5, 0.1]))
-    ([array(-0.22526717), array(-1.00864546), array(6.9388939e-18)],)
-
-    .. note::
-
-        TensorFlow is used as the device backend, and is independent
-        of the chosen QNode interface. In the example above, we combine
-        ``default.tensor.tf`` with the ``autograd`` interface.
-        It can also be used with the ``torch`` and the ``tf`` interface.
+    The ``default.tensor.tf`` device supports various differentiation modes.
+
+    * *End-to-end classical backpropagation with the TensorFlow interface*.
+      Using this method, the created QNode is a 'white-box', and is
+      tightly integrated with your TensorFlow computation:
+
+      >>> dev = qml.device("default.tensor.tf", wires=1)
+      >>> @qml.qnode(dev, interface="tf", diff_method="backprop")
+      >>> def circuit(x):
+      ...     qml.RX(x[1], wires=0)
+      ...     qml.Rot(x[0], x[1], x[2], wires=0)
+      ...     return qml.expval(qml.PauliZ(0))
+      >>> vars = tf.Variable([0.2, 0.5, 0.1])
+      >>> with tf.GradientTape() as tape:
+      ...     res = circuit(vars)
+      >>> tape.gradient(res, vars)
+      <tf.Tensor: shape=(3,), dtype=float32, numpy=array([-2.2526717e-01, -1.0086454e+00,  1.3877788e-17], dtype=float32)>
+
+      In this mode, you must use the ``"tf"`` interface, as TensorFlow
+      is used as the device backend.
+
+    * *Device differentiation*. Using this method, the created QNode
+      is a 'black-box' to your classical computation. PennyLane will automatically
+      accept classical tensors from any supported interface, and query the
+      device directly for the quantum gradient when required.
+
+      >>> dev = qml.device("default.tensor.tf", wires=1)
+      >>> @qml.qnode(dev, interface="autograd", diff_method="device")
+      >>> def circuit(x):
+      ...     qml.RX(x[1], wires=0)
+      ...     qml.Rot(x[0], x[1], x[2], wires=0)
+      ...     return qml.expval(qml.PauliZ(0))
+      >>> grad_fn = qml.grad(circuit, argnum=[0])
+      >>> print(grad_fn([0.2, 0.5, 0.1]))
+      ([array(-0.22526717), array(-1.00864546), array(6.9388939e-18)],)
+
+      In this mode, even though TensorFlow is used as the device backend, it
+      is independent of the chosen QNode interface. In the example above, we combine
+      ``default.tensor.tf`` with the ``autograd`` interface.
+      It can also be used with the ``torch`` and the ``tf`` interface.
+
+    In addition to end-to-end classical backpropagation and device differentiation,
+    the ``default.tensor.tf`` device also supports ``parameter-shift`` and
+    ``finite-diff`` differentiation methods.
 
     Args:
         wires (int): the number of modes to initialize the device in
         shots (int): the number of shots used for returning samples
     """
 
     # pylint: disable=too-many-instance-attributes
     name = "PennyLane TensorNetwork (TensorFlow) simulator plugin"
     short_name = "default.tensor.tf"
-    _capabilities = {"model": "qubit", "tensor_observables": True, "provides_jacobian": True}
+    _capabilities = {
+        "model": "qubit",
+        "tensor_observables": True,
+        "provides_jacobian": True,
+        "passthru_interface": "tf",
+    }
 
     _operation_map = copy.copy(DefaultTensor._operation_map)
     _operation_map.update(
         {
             "PhaseShift": Rphi,
             "RX": Rotx,
             "RY": Roty,
```

### Comparing `PennyLane-0.8.1/pennylane/beta/plugins/__init__.py` & `PennyLane-0.9.0/pennylane/beta/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/beta/__init__.py` & `PennyLane-0.9.0/pennylane/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/circuit_drawer/charsets.py` & `PennyLane-0.9.0/pennylane/circuit_drawer/charsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,27 +124,29 @@
         "3": "³",
         "4": "⁴",
         "5": "⁵",
         "6": "⁶",
         "7": "⁷",
         "8": "⁸",
         "9": "⁹",
+        "-": "⁻",
     }
 
     _subscript_dict = {
         "0": "₀",
         "1": "₁",
         "2": "₂",
         "3": "₃",
         "4": "₅",
         "5": "⁵",
         "6": "₆",
         "7": "₇",
         "8": "₈",
         "9": "₉",
+        "-": "₋",
     }
 
     @staticmethod
     def to_superscript(num):
         """Convert the given number to a superscripted string."""
         ret = str(num)
         for old, new in UnicodeCharSet._superscript_dict.items():
```

### Comparing `PennyLane-0.8.1/pennylane/circuit_drawer/circuit_drawer.py` & `PennyLane-0.9.0/pennylane/circuit_drawer/circuit_drawer.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/circuit_drawer/grid.py` & `PennyLane-0.9.0/pennylane/circuit_drawer/grid.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/circuit_drawer/representation_resolver.py` & `PennyLane-0.9.0/pennylane/circuit_drawer/representation_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "Toffoli": "X",
         "CSWAP": "SWAP",
         "PauliY": "Y",
         "PauliZ": "Z",
         "CZ": "Z",
         "Identity": "I",
         "Hadamard": "H",
+        "MultiRZ": "RZ",
         "CRX": "RX",
         "CRY": "RY",
         "CRZ": "RZ",
         "CRot": "Rot",
         "PhaseShift": "Rϕ",
         "Beamsplitter": "BS",
         "Squeezing": "S",
@@ -103,22 +104,25 @@
 
         return len(target_list) - 1
 
     def single_parameter_representation(self, par):
         """Resolve the representation of an Operator's parameter.
 
         Args:
-            par (Union[~.variable.Variable, int, float]): The parameter to be rendered
+            par (Union[~.variable.Variable, int, float, str]): The parameter to be rendered
 
         Returns:
             str: String representation of the parameter
         """
         if isinstance(par, qml.variable.Variable):
             return par.render(self.show_variable_names)
 
+        if isinstance(par, str):
+            return par
+
         return str(round(par, 3))
 
     @staticmethod
     def _format_matrix_operation(operation, symbol, cache):
         """Format an operation that corresponds to a single matrix.
 
         Args:
@@ -173,15 +177,15 @@
 
         if coefficient == -1.0:
             return "-" + str(variable)
 
         return "{:+.3g}{}".format(coefficient, variable)
 
     def _format_polyxp_order1(self, coefficients):
-        """Format a first-order polynmomial of x and p operators.
+        """Format a first-order polynomial of x and p operators.
 
         Args:
             coefficients (array[float]): The polynomial coefficients as a vector
 
         Returns:
             str: A string representing the polynomial
         """
@@ -199,15 +203,15 @@
             poly_str += RepresentationResolver._format_poly_term(
                 coefficients[y], "p{}".format(self.charset.to_subscript(idx))
             )
 
         return poly_str
 
     def _format_polyxp_order2(self, coefficients):
-        """Format a second-order polynmomial of x and p operators.
+        """Format a second-order polynomial of x and p operators.
 
         Args:
             coefficients (array[float]): The polynomial coefficients as a matrix
 
         Returns:
             str: A string representing the polynomial
         """
@@ -297,15 +301,15 @@
         order = len(coefficients.shape)
 
         if order == 1:
             return self._format_polyxp_order1(coefficients)
 
         return self._format_polyxp_order2(coefficients)
 
-    # pylint: disable=too-many-return-statements
+    # pylint: disable=too-many-branches
     def operator_representation(self, op, wire):
         """Return the string representation of an Operator.
 
         Args:
             op (pennylane.operation.Operator): The Operator instance whose representation shall be returned
             wire (int): The Operator's wire for which the string representation shall be returned
 
@@ -315,75 +319,92 @@
         if isinstance(op, qml.operation.Tensor):
             constituent_representations = [
                 self.operator_representation(tensor_obs, wire) for tensor_obs in op.obs
             ]
 
             return (" " + self.charset.OTIMES + " ").join(constituent_representations)
 
-        name = op.name
+        representation = ""
+        base_name = getattr(op, "base_name", op.name)
+        name = base_name
 
         # Use a shorter name if applicable
         if name in RepresentationResolver.resolution_dict:
             name = RepresentationResolver.resolution_dict[name]
 
         # Display a control symbol for all controlling qubits of a controlled Operation
-        if op.name in self.control_wire_dict and wire in [
-            op.wires[control_idx] for control_idx in self.control_wire_dict[op.name]
+        if base_name in self.control_wire_dict and wire in [
+            op.wires[control_idx] for control_idx in self.control_wire_dict[base_name]
         ]:
+            # No need to add a -1 for inverse here
             return self.charset.CONTROL
 
         if op.num_params == 0:
-            return name
+            representation = name
+
+        elif base_name == "PauliRot":
+            representation = "R{0}({1})".format(
+                op.params[1][op.wires.index(wire)],
+                self.single_parameter_representation(op.params[0]),
+            )
 
-        if op.name == "QubitUnitary":
-            return RepresentationResolver._format_matrix_operation(
+        elif base_name == "QubitUnitary":
+            representation = RepresentationResolver._format_matrix_operation(
                 op, "U", self.unitary_matrix_cache
             )
 
-        if op.name == "Hermitian":
-            return RepresentationResolver._format_matrix_operation(
+        elif base_name == "Hermitian":
+            representation = RepresentationResolver._format_matrix_operation(
                 op, "H", self.hermitian_matrix_cache
             )
 
-        if op.name == "QuadOperator":
+        elif base_name == "QuadOperator":
             par_rep = self.single_parameter_representation(op.params[0])
 
-            return "cos({0})x+sin({0})p".format(par_rep)
+            representation = "cos({0})x+sin({0})p".format(par_rep)
 
-        if op.name == "FockStateProjector":
+        elif base_name == "FockStateProjector":
             n_str = ",".join([str(n) for n in op.params[0]])
 
-            return (
+            representation = (
                 self.charset.PIPE + n_str + self.charset.CROSSED_LINES + n_str + self.charset.PIPE
             )
 
-        if op.name == "PolyXP":
-            return self._format_polyxp(op)
+        elif base_name == "PolyXP":
+            representation = self._format_polyxp(op)
 
-        if op.name == "FockState":
-            return self.charset.PIPE + str(op.params[0]) + self.charset.RANGLE
+        elif base_name == "FockState":
+            representation = self.charset.PIPE + str(op.params[0]) + self.charset.RANGLE
 
-        if op.name in {"BasisState", "FockStateVector"}:
-            return self.charset.PIPE + str(op.params[0][op.wires.index(wire)]) + self.charset.RANGLE
+        elif base_name in {"BasisState", "FockStateVector"}:
+            representation = (
+                self.charset.PIPE + str(op.params[0][op.wires.index(wire)]) + self.charset.RANGLE
+            )
 
         # Operations that only have matrix arguments
-        if op.name in {
+        elif base_name in {
             "GaussianState",
             "FockDensityMatrix",
             "FockStateVector",
             "QubitStateVector",
             "Interferometer",
         }:
-            return name + RepresentationResolver._format_matrix_arguments(
+            representation = name + RepresentationResolver._format_matrix_arguments(
                 op.params, "M", self.matrix_cache
             )
 
-        return "{}({})".format(
-            name, ", ".join([self.single_parameter_representation(par) for par in op.params])
-        )
+        else:
+            representation = "{}({})".format(
+                name, ", ".join([self.single_parameter_representation(par) for par in op.params])
+            )
+
+        if getattr(op, "inverse", False):
+            representation += self.charset.to_superscript("-1")
+
+        return representation
 
     def output_representation(self, obs, wire):
         """Return the string representation of a circuit's output.
 
         Args:
             obs (pennylane.ops.Observable): The Observable instance whose representation shall be returned
             wire (int): The Observable's wire for which the string representation shall be returned
@@ -401,14 +422,17 @@
 
         if obs.return_type == qml.operation.Variance:
             return "Var[{}]".format(self.operator_representation(obs, wire))
 
         if obs.return_type == qml.operation.Sample:
             return "Sample[{}]".format(self.operator_representation(obs, wire))
 
+        if obs.return_type == qml.operation.Probability:
+            return "Probs"
+
         # Unknown return_type
         return "{}[{}]".format(str(obs.return_type), self.operator_representation(obs, wire))
 
     def element_representation(self, element, wire):
         """Return the string representation of an element in the circuit's Grid.
 
         Args:
```

### Comparing `PennyLane-0.8.1/pennylane/circuit_drawer/__init__.py` & `PennyLane-0.9.0/pennylane/circuit_drawer/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/circuit_graph.py` & `PennyLane-0.9.0/pennylane/circuit_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,35 +140,20 @@
 
     def print_contents(self):
         """Prints the contents of the quantum circuit."""
 
         print("Operations")
         print("==========")
         for op in self.operations:
-            if op.parameters:
-                params = ", ".join([str(p) for p in op.parameters])
-                print("{}({}, wires={})".format(op.name, params, op.wires))
-            else:
-                print("{}(wires={})".format(op.name, op.wires))
-
-        return_map = {
-            qml.operation.Expectation: "expval",
-            qml.operation.Variance: "var",
-            qml.operation.Sample: "sample",
-        }
+            print(repr(op))
 
         print("\nObservables")
         print("===========")
         for op in self.observables:
-            return_type = return_map[op.return_type]
-            if op.parameters:
-                params = "".join([str(p) for p in op.parameters])
-                print("{}({}({}, wires={}))".format(return_type, op.name, params, op.wires))
-            else:
-                print("{}({}(wires={}))".format(return_type, op.name, op.wires))
+            print(repr(op))
 
     def serialize(self):
         """Serialize the quantum circuit graph based on the operations and
         observables in the circuit graph and the index of the variables
         used by them.
 
         The string that is produced can be later hashed to assign a unique value to the circuit graph.
```

### Comparing `PennyLane-0.8.1/pennylane/collections/apply.py` & `PennyLane-0.9.0/pennylane/collections/apply.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/collections/dot.py` & `PennyLane-0.9.0/pennylane/collections/dot.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/collections/map.py` & `PennyLane-0.9.0/pennylane/collections/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,23 @@
 
 from .qnode_collection import QNodeCollection
 
 
 MEASURE_MAP = {"expval": expval, "var": var, "sample": sample}
 
 
-def map(template, observables, device, measure="expval", interface="autograd", diff_method="best"):
+def map(
+    template,
+    observables,
+    device,
+    measure="expval",
+    interface="autograd",
+    diff_method="best",
+    **kwargs
+):
     """Map a quantum template over a list of observables to create
     a :class:`QNodeCollection`.
 
     The number of QNodes within the created QNode collection will match the number
     of observables passed. The device and the measurement type will either be
     applied to all QNodes in the collection, or can be provided as a list for more
     fine-grained control.
@@ -117,16 +125,16 @@
         wires = list(range(dev.num_wires))
 
         # Note: in the following template definition, we pass the observable, measurement,
         # and wires as *default arguments* to named parameters. This is to avoid
         # Python's late binding closure behaviour
         # (see https://docs.python-guide.org/writing/gotchas/#late-binding-closures)
         def circuit(
-            params, _obs=obs, _m=m, _wires=wires, **kwargs
+            params, _obs=obs, _m=m, _wires=wires, **circuit_kwargs
         ):  # pylint: disable=dangerous-default-value, function-redefined
-            template(params, wires=_wires, **kwargs)
+            template(params, wires=_wires, **circuit_kwargs)
             return MEASURE_MAP[_m](_obs)
 
-        qnode = QNode(circuit, dev, interface=interface, diff_method=diff_method)
+        qnode = QNode(circuit, dev, interface=interface, diff_method=diff_method, **kwargs)
         qnodes.append(qnode)
 
     return qnodes
```

### Comparing `PennyLane-0.8.1/pennylane/collections/qnode_collection.py` & `PennyLane-0.9.0/pennylane/collections/qnode_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     .. warning::
 
         Asynchronous evaluation is experimental --- please report all bugs and issues
         to our GitHub page. It currently works with all interfaces, however backpropagation
         and gradient computation is limited to Autograd and PyTorch. **Quantum gradients
         using TensorFlow in asynchronous mode is currently not supported**.
 
-    By default, the QNodes within the QNode cluster are executed sequentially.
+    By default, the QNodes within the QNodeCollection are executed sequentially.
 
     However, experimental asynchronous support is now available using the
     `Dask <https://dask.org/>`_ parallelism library. This can be activated
     by passing the ``parallel=True`` keyword argument when evaluating the
     QNodeCollection.
 
     For example, let's create the following two QVM simulation devices:
@@ -212,15 +212,15 @@
                     "Dask must be installed for parallel evaluation. "
                     "\nDask can be installed using pip:"
                     "\n\npip install dask[delayed]"
                 )
 
             if self.interface == "tf":
                 warnings.warn(
-                    "Parallel execution of QNode clusters is "
+                    "Parallel execution of QNodeCollections is "
                     "an experimental feature, and currently doesn't "
                     "work with TensorFlow backpropagation. Please use "
                     "the PyTorch or Autograd interfaces instead.",
                     UserWarning,
                 )
 
             for q in self.qnodes:
```

### Comparing `PennyLane-0.8.1/pennylane/collections/sum.py` & `PennyLane-0.9.0/pennylane/collections/sum.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/collections/__init__.py` & `PennyLane-0.9.0/pennylane/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/configuration.py` & `PennyLane-0.9.0/pennylane/configuration.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/init.py` & `PennyLane-0.9.0/pennylane/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -157,17 +157,22 @@
 
     Returns:
         array: parameter array
     """
     if seed is not None:
         np.random.seed(seed)
 
+    # set default
     if n_rots is None:
         n_rots = n_wires
 
+    # no circuit if there are no wires
+    if n_wires == 0:
+        n_rots = 0
+
     params = np.random.uniform(low=low, high=high, size=(n_layers, n_rots))
     return params
 
 
 def random_layers_normal(n_layers, n_wires, n_rots=None, mean=0, std=0.1, seed=None):
     r"""Creates a parameter array for :func:`~.RandomLayers`, drawn from a normal distribution.
 
@@ -187,17 +192,22 @@
 
     Returns:
         array: parameter array
     """
     if seed is not None:
         np.random.seed(seed)
 
+    # set default
     if n_rots is None:
         n_rots = n_wires
 
+    # no circuit if there are no wires
+    if n_wires == 0:
+        n_rots = 0
+
     params = np.random.normal(loc=mean, scale=std, size=(n_layers, n_rots))
     return params
 
 
 def cvqnn_layers_all(n_layers, n_wires, seed=None):
     r"""Creates a list of all eleven parameter arrays for :func:`~.CVNeuralNetLayers`.
 
@@ -831,7 +841,173 @@
         array: parameter array
     """
     if seed is not None:
         np.random.seed(seed)
 
     varphi = np.random.normal(loc=mean, scale=std, size=(n_wires,))
     return varphi
+
+
+def simplified_two_design_initial_layer_uniform(n_wires, low=0, high=2 * pi, seed=None):
+    r"""Creates a parameter array for the ``initial_layer`` argument of :func:`~.SimplifiedTwoDesign`,
+    drawn from a uniform distribution.
+
+    The shape of the parameter array is ``(n_wires,)`` and each parameter is drawn uniformly at random \
+    from between ``low`` and ``high``. The parameters define the Pauli-Y rotation angles
+    applied in the initial layer.
+
+    Args:
+        n_wires (int): number of qubits
+        low (float): minimum value of uniform distribution
+        high (float): maximum value of uniform distribution
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    params = np.random.uniform(low=low, high=high, size=(n_wires,))
+    return params
+
+
+def simplified_two_design_initial_layer_normal(n_wires, mean=0, std=0.1, seed=None):
+    r"""Creates a parameter array for the ``initial_layer`` argument of :func:`~.SimplifiedTwoDesign`,
+    drawn from a uniform distribution.
+
+    The shape of the parameter array is ``(n_wires,)`` and each parameter is drawn
+    from a normal distribution with mean ``mean`` and standard deviation ``std``.
+    The parameters define the Pauli-Y rotation angles
+    applied in the initial layer.
+
+    Args:
+        n_wires (int): number of qubits
+        mean (float): mean of parameters
+        std (float): standard deviation of parameters
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    params = np.random.normal(loc=mean, scale=std, size=(n_wires,))
+    return params
+
+
+def simplified_two_design_weights_uniform(n_layers, n_wires, low=0, high=2 * pi, seed=None):
+    r"""Creates a parameter array for the ``weights`` argument of :func:`~.SimplifiedTwoDesign`,
+    drawn from a uniform distribution.
+
+    The shape of the parameter array is ``(n_layers, n_wires - 1, 2)``
+    and each parameter is drawn uniformly at random \
+    from between ``low`` and ``high``. The parameters define the Pauli-Y rotation angles
+    applied in each layer.
+
+    Args:
+        n_layers (int): number of layers
+        n_wires (int): number of qubits
+        low (float): minimum value of uniform distribution
+        high (float): maximum value of uniform distribution
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    n_unitaries_per_layer = n_wires - 1
+
+    if n_unitaries_per_layer in [0, -1]:
+        params = np.array([])
+    else:
+        params = np.random.uniform(low=low, high=high, size=(n_layers, n_unitaries_per_layer, 2))
+
+    return params
+
+
+def simplified_two_design_weights_normal(n_layers, n_wires, mean=0, std=0.1, seed=None):
+    r"""Creates a parameter array for the ``weights`` argument of :func:`~.SimplifiedTwoDesign`,
+    drawn from a uniform distribution.
+
+    The shape of the parameter array is ``(n_layers, n_wires - 1, 2)``
+    and each parameter is drawn
+    from a normal distribution with mean ``mean`` and standard deviation ``std``.
+    The parameters define the Pauli-Y rotation angles
+    applied in each layer.
+
+    Args:
+        n_layers (int): number of layers
+        n_wires (int): number of qubits
+        mean (float): mean of parameters
+        std (float): standard deviation of parameters
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    n_unitaries_per_layer = n_wires - 1
+
+    if n_unitaries_per_layer in [0, -1]:
+        params = np.array([])
+    else:
+        params = np.random.normal(loc=mean, scale=std, size=(n_layers, n_unitaries_per_layer, 2))
+
+    return params
+
+
+def basic_entangler_layers_normal(n_layers, n_wires, mean=0, std=0.1, seed=None):
+    r"""Creates a parameter array for :func:`~.BasicEntanglerLayers`, drawn from a normal
+    distribution.
+
+    The shape of the parameter array is ``(n_layers, n_wires)`` and each parameter is drawn
+    from a normal distribution with mean ``mean`` and standard deviation ``std``.
+    The parameters define the rotation angles applied in each layer.
+
+    Args:
+        n_layers (int): number of layers
+        n_wires (int): number of qubits
+        mean (float): mean of parameters
+        std (float): standard deviation of parameters
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    params = np.random.normal(loc=mean, scale=std, size=(n_layers, n_wires))
+
+    return params
+
+
+def basic_entangler_layers_uniform(n_layers, n_wires, low=0, high=2 * pi, seed=None):
+    r"""Creates a parameter array for :func:`~.BasicEntanglerLayers`, drawn from a uniform
+    distribution.
+
+    The shape of the parameter array is ``(n_layers, n_wires)`` and each parameter is drawn uniformly at random
+    from between ``low`` and ``high``. The parameters define the rotation angles
+    applied in each layer.
+
+    Args:
+        n_layers (int): number of layers
+        n_wires (int): number of qubits
+        low (float): minimum value of uniform distribution
+        high (float): maximum value of uniform distribution
+        seed (int): seed used in sampling the parameters, makes function call deterministic
+
+    Returns:
+        array: parameter array
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    params = np.random.uniform(low=low, high=high, size=(n_layers, n_wires))
+
+    return params
```

### Comparing `PennyLane-0.8.1/pennylane/interfaces/autograd.py` & `PennyLane-0.9.0/pennylane/interfaces/autograd.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/interfaces/torch.py` & `PennyLane-0.9.0/pennylane/interfaces/torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
             """REPL representation"""
             return self.__str__()
 
         print_applied = qnode.print_applied
         jacobian = qnode.jacobian
         metric_tensor = qnode.metric_tensor
         draw = qnode.draw
+        func = qnode.func
 
     @qnode_str
     def custom_apply(*args, **kwargs):
         """Custom apply wrapper, to allow passing kwargs to the TorchQNode"""
 
         # get default kwargs that weren't passed
         keyword_sig = _get_default_args(qnode.func)
```

### Comparing `PennyLane-0.8.1/pennylane/interfaces/__init__.py` & `PennyLane-0.9.0/pennylane/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/io.py` & `PennyLane-0.9.0/pennylane/io.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/measure.py` & `PennyLane-0.9.0/tests/test_measure.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,219 +7,237 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# pylint: disable=protected-access
-"""
-This module contains the functions for computing different types of measurement
-outcomes from quantum observables - expectation values, variances of expectations,
-and measurement samples.
-"""
+"""Unit tests for the measure module"""
+import pytest
+import numpy as np
+
 import pennylane as qml
-from .operation import Observable, Sample, Variance, Expectation, Probability, Tensor
-from .qnodes import QuantumFunctionError
+from pennylane.qnodes import QuantumFunctionError
+from pennylane.operation import Sample, Variance, Expectation
 
 
-def _remove_if_in_queue(op):
-    r"""Helper function to handle removing ops from the QNode queue"""
-    if op in qml._current_context.queue:
-        qml._current_context.queue.remove(op)
+def test_no_measure(tol):
+    """Test that failing to specify a measurement
+    raises an exception"""
+    dev = qml.device("default.qubit", wires=2)
 
+    @qml.qnode(dev)
+    def circuit(x):
+        qml.RX(x, wires=0)
+        return qml.PauliY(0)
 
-def expval(op):
-    r"""Expectation value of the supplied observable.
+    with pytest.raises(QuantumFunctionError, match="does not have the measurement"):
+        res = circuit(0.65)
 
-    **Example:**
 
-    .. code-block:: python3
+class TestExpval:
+    """Tests for the expval function"""
 
+    def test_value(self, tol):
+        """Test that the expval interface works"""
         dev = qml.device("default.qubit", wires=2)
 
         @qml.qnode(dev)
         def circuit(x):
             qml.RX(x, wires=0)
-            qml.Hadamard(wires=1)
-            qml.CNOT(wires=[0, 1])
             return qml.expval(qml.PauliY(0))
 
-    Executing this QNode:
+        x = 0.54
+        res = circuit(x)
+        expected = -np.sin(x)
+
+        assert np.allclose(res, expected, atol=tol, rtol=0)
+
+    def test_not_an_observable(self):
+        """Test that a QuantumFunctionError is raised if the provided
+        argument is not an observable"""
+        dev = qml.device("default.qubit", wires=2)
 
-    >>> circuit(0.5)
-    -0.4794255386042029
+        @qml.qnode(dev)
+        def circuit():
+            qml.RX(0.52, wires=0)
+            return qml.expval(qml.CNOT(wires=[0, 1]))
 
-    Args:
-        op (Observable): a quantum observable object
+        with pytest.raises(QuantumFunctionError, match="CNOT is not an observable"):
+            res = circuit()
 
-    Raises:
-        QuantumFunctionError: `op` is not an instance of :class:`~.Observable`
-    """
-    if not isinstance(op, Observable):
-        raise QuantumFunctionError(
-            "{} is not an observable: cannot be used with expval".format(op.name)
-        )
+    def test_observable_return_type_is_expectation(self):
+        """Test that the return type of the observable is :attr:`ObservableReturnTypes.Expectation`"""
+        dev = qml.device("default.qubit", wires=2)
 
-    if qml._current_context is not None:
-        # delete observables from QNode operation queue if needed
-        if isinstance(op, Tensor):
-            for o in op.obs:
-                _remove_if_in_queue(o)
-        else:
-            _remove_if_in_queue(op)
+        @qml.qnode(dev)
+        def circuit():
+            res = qml.expval(qml.PauliZ(0))
+            assert res.return_type is Expectation
+            return res
 
-    # set return type to be an expectation value
-    op.return_type = Expectation
+        circuit()
 
-    if qml._current_context is not None:
-        # add observable to QNode observable queue
-        qml._current_context._append_op(op)
 
-    return op
+class TestVar:
+    """Tests for the var function"""
 
+    def test_value(self, tol):
+        """Test that the var function works"""
+        dev = qml.device("default.qubit", wires=2)
 
-def var(op):
-    r"""Variance of the supplied observable.
+        @qml.qnode(dev)
+        def circuit(x):
+            qml.RX(x, wires=0)
+            return qml.var(qml.PauliZ(0))
 
-    **Example:**
+        x = 0.54
+        res = circuit(x)
+        expected = np.sin(x)**2
 
-    .. code-block:: python3
+        assert np.allclose(res, expected, atol=tol, rtol=0)
 
+    def test_not_an_observable(self):
+        """Test that a QuantumFunctionError is raised if the provided
+        argument is not an observable"""
         dev = qml.device("default.qubit", wires=2)
 
         @qml.qnode(dev)
-        def circuit(x):
-            qml.RX(x, wires=0)
-            qml.Hadamard(wires=1)
-            qml.CNOT(wires=[0, 1])
-            return qml.var(qml.PauliY(0))
+        def circuit():
+            qml.RX(0.52, wires=0)
+            return qml.var(qml.CNOT(wires=[0, 1]))
 
-    Executing this QNode:
+        with pytest.raises(QuantumFunctionError, match="CNOT is not an observable"):
+            res = circuit()
 
-    >>> circuit(0.5)
-    0.7701511529340698
+    def test_observable_return_type_is_variance(self):
+        """Test that the return type of the observable is :attr:`ObservableReturnTypes.Variance`"""
+        dev = qml.device("default.qubit", wires=2)
 
-    Args:
-        op (Observable): a quantum observable object
+        @qml.qnode(dev)
+        def circuit():
+            res = qml.var(qml.PauliZ(0))
+            assert res.return_type is Variance
+            return res
 
-    Raises:
-        QuantumFunctionError: `op` is not an instance of :class:`~.Observable`
-    """
-    if not isinstance(op, Observable):
-        raise QuantumFunctionError(
-            "{} is not an observable: cannot be used with var".format(op.name)
-        )
+        circuit()
 
-    if qml._current_context is not None:
-        # delete operations from QNode queue
-        if isinstance(op, Tensor):
-            for o in op.obs:
-                _remove_if_in_queue(o)
-        else:
-            _remove_if_in_queue(op)
 
-    # set return type to be a variance
-    op.return_type = Variance
+class TestSample:
+    """Tests for the sample function"""
 
-    if qml._current_context is not None:
-        # add observable to QNode observable queue
-        qml._current_context._append_op(op)
+    def test_sample_dimension(self, tol):
+        """Test that the sample function outputs samples of the right size"""
+        n_sample = 10
 
-    return op
+        dev = qml.device("default.qubit", wires=2, shots=n_sample)
 
+        @qml.qnode(dev)
+        def circuit():
+            qml.RX(0.54, wires=0)
+            return qml.sample(qml.PauliZ(0)), qml.sample(qml.PauliX(1))
 
-def sample(op):
-    r"""Sample from the supplied observable, with the number of shots
-    determined from the ``dev.shots`` attribute of the corresponding device.
+        sample = circuit()
 
-    **Example:**
+        assert np.array_equal(sample.shape, (2,n_sample))
 
-    .. code-block:: python3
+    def test_sample_combination(self, tol):
+        """Test the output of combining expval, var and sample"""
+        n_sample = 10
 
-        dev = qml.device("default.qubit", wires=2, shots=4)
+        dev = qml.device("default.qubit", wires=3, shots=n_sample)
 
         @qml.qnode(dev)
-        def circuit(x):
-            qml.RX(x, wires=0)
-            qml.Hadamard(wires=1)
-            qml.CNOT(wires=[0, 1])
-            return qml.sample(qml.PauliY(0))
+        def circuit():
+            qml.RX(0.54, wires=0)
 
-    Executing this QNode:
+            return qml.sample(qml.PauliZ(0)), qml.expval(qml.PauliX(1)), qml.var(qml.PauliY(2))
 
-    >>> circuit(0.5)
-    array([ 1.,  1.,  1., -1.])
+        result = circuit()
 
-    Args:
-        op (Observable): a quantum observable object
+        assert np.array_equal(result.shape, (3,))
+        assert np.array_equal(result[0].shape, (n_sample,))
+        assert isinstance(result[1], float)
+        assert isinstance(result[2], float)
 
-    Raises:
-        QuantumFunctionError: `op` is not an instance of :class:`~.Observable`
-    """
-    if not isinstance(op, Observable):
-        raise QuantumFunctionError(
-            "{} is not an observable: cannot be used with sample".format(op.name)
-        )
+    def test_single_wire_sample(self, tol):
+        """Test the return type and shape of sampling a single wire"""
+        n_sample = 10
 
-    if qml._current_context is not None:
-        # delete operations from QNode queue
-        if isinstance(op, Tensor):
-            for o in op.obs:
-                _remove_if_in_queue(o)
-        else:
-            _remove_if_in_queue(op)
+        dev = qml.device("default.qubit", wires=1, shots=n_sample)
 
-    # set return type to be a sample
-    op.return_type = Sample
+        @qml.qnode(dev)
+        def circuit():
+            qml.RX(0.54, wires=0)
 
-    if qml._current_context is not None:
-        # add observable to QNode observable queue
-        qml._current_context._append_op(op)
+            return qml.sample(qml.PauliZ(0))
 
-    return op
+        result = circuit()
 
+        assert isinstance(result, np.ndarray)
+        assert np.array_equal(result.shape, (n_sample,))
 
-def probs(wires):
-    r"""Probability of each computational basis state.
+    def test_multi_wire_sample_regular_shape(self, tol):
+        """Test the return type and shape of sampling multiple wires
+           where a rectangular array is expected"""
+        n_sample = 10
 
-    This measurement function accepts no observables, and instead
-    instructs the QNode to return a flat array containing the
-    probabilities of each quantum state.
+        dev = qml.device("default.qubit", wires=3, shots=n_sample)
 
-    Marginal probabilities may also be requested by restricting
-    the wires to a subset of the full system; the size of the
-    returned array will be ``[2**len(wires)]``.
+        @qml.qnode(dev)
+        def circuit():
+            return qml.sample(qml.PauliZ(0)), qml.sample(qml.PauliZ(1)), qml.sample(qml.PauliZ(2))
 
-    **Example:**
+        result = circuit()
 
-    .. code-block:: python3
+        # If all the dimensions are equal the result will end up to be a proper rectangular array
+        assert isinstance(result, np.ndarray)
+        assert np.array_equal(result.shape, (3, n_sample))
+        assert result.dtype == np.dtype("int")
 
-        dev = qml.device("default.qubit", wires=2)
+    def test_sample_output_type_in_combination(self, tol):
+        """Test the return type and shape of sampling multiple works
+           in combination with expvals and vars"""
+        n_sample = 10
+
+        dev = qml.device("default.qubit", wires=3, shots=n_sample)
 
         @qml.qnode(dev)
         def circuit():
-            qml.Hadamard(wires=1)
-            qml.CNOT(wires=[0, 1])
-            return qml.probs(wires=[0, 1])
+            return qml.expval(qml.PauliZ(0)), qml.var(qml.PauliZ(1)), qml.sample(qml.PauliZ(2))
 
-    Executing this QNode:
+        result = circuit()
+
+        # If all the dimensions are equal the result will end up to be a proper rectangular array
+        assert isinstance(result, np.ndarray)
+        assert result.dtype == np.dtype("object")
+        assert np.array_equal(result.shape, (3,))
+        assert isinstance(result[0], float)
+        assert isinstance(result[1], float)
+        assert result[2].dtype == np.dtype("int")
+        assert np.array_equal(result[2].shape, (n_sample,))
+
+    def test_not_an_observable(self):
+        """Test that a QuantumFunctionError is raised if the provided
+        argument is not an observable"""
+        dev = qml.device("default.qubit", wires=2)
 
-    >>> circuit()
-    array([0.5, 0.5, 0. , 0. ])
+        @qml.qnode(dev)
+        def circuit():
+            qml.RX(0.52, wires=0)
+            return qml.sample(qml.CNOT(wires=[0, 1]))
 
-    The returned array is in lexicographic order, so corresponds
-    to a :math:`50\%` chance of measuring either :math:`|00\rangle`
-    or :math:`|01\rangle`.
+        with pytest.raises(QuantumFunctionError, match="CNOT is not an observable"):
+            sample = circuit()
 
-    Args:
-        wires (Sequence[int] or int): the wire the operation acts on
-    """
-    # pylint: disable=protected-access
-    op = qml.Identity(wires=wires, do_queue=False)
-    op.return_type = Probability
+    def test_observable_return_type_is_sample(self):
+        """Test that the return type of the observable is :attr:`ObservableReturnTypes.Sample`"""
+        n_shots = 10
+        dev = qml.device("default.qubit", wires=1, shots=n_shots)
 
-    if qml._current_context is not None:
-        # add observable to QNode observable queue
-        qml._current_context._append_op(op)
+        @qml.qnode(dev)
+        def circuit():
+            res = qml.sample(qml.PauliZ(0))
+            assert res.return_type is Sample
+            return res
 
-    return op
+        circuit()
```

### Comparing `PennyLane-0.8.1/pennylane/operation.py` & `PennyLane-0.9.0/pennylane/operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -115,46 +115,48 @@
 from .variable import Variable
 
 # =============================================================================
 # Wire types
 # =============================================================================
 
 
-class Wires(IntEnum):
+class ActsOn(IntEnum):
     """Integer enumeration class
     to represent the number of wires
     an operation acts on"""
 
-    Any = -1
-    All = 0
+    AnyWires = -1
+    AllWires = 0
 
 
-All = Wires.All
+AllWires = ActsOn.AllWires
 """IntEnum: An enumeration which represents all wires in the
 subsystem. It is equivalent to an integer with value 0."""
 
-Any = Wires.Any
+AnyWires = ActsOn.AnyWires
 """IntEnum: An enumeration which represents any wires in the
 subsystem. It is equivalent to an integer with value -1."""
 
 
 # =============================================================================
 # ObservableReturnTypes types
 # =============================================================================
 
 
 class ObservableReturnTypes(Enum):
-    """Enumeration class to
-    represent the type of
-    return types of an observable."""
-
-    Sample = 1
-    Variance = 2
-    Expectation = 3
-    Probability = 4
+    """Enumeration class to represent the return types of an observable."""
+
+    Sample = "sample"
+    Variance = "var"
+    Expectation = "expval"
+    Probability = "probs"
+
+    def __repr__(self):
+        """String representation of the return types."""
+        return self.value
 
 
 Sample = ObservableReturnTypes.Sample
 """Enum: An enumeration which represents sampling an observable."""
 
 Variance = ObservableReturnTypes.Variance
 """Enum: An enumeration which represents returning the variance of
@@ -164,14 +166,15 @@
 """Enum: An enumeration which represents returning the expectation
 value of an observable on specified wires."""
 
 Probability = ObservableReturnTypes.Probability
 """Enum: An enumeration which represents returning probabilities
 of all computational basis states."""
 
+
 # =============================================================================
 # Class property
 # =============================================================================
 
 
 class ClassPropertyDescriptor:  # pragma: no cover
     """Allows a class property to be defined"""
@@ -225,27 +228,24 @@
     Args:
         params (tuple[float, int, array, Variable]): operator parameters
 
     Keyword Args:
         wires (Sequence[int]): Subsystems it acts on. If not given, args[-1]
             is interpreted as wires.
         do_queue (bool): Indicates whether the operator should be
-            immediately pushed into a :class:`BaseQNode` circuit queue.
-            The circuit queue is determined by the presence of an
-            applicable `qml._current_context`. If no context is
-            available, this argument is ignored.
+            immediately pushed into the Operator queue.
     """
     do_check_domain = True  #: bool: flag: should we perform a domain check for the parameters?
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         """Matrix representation of the operator
         in the computational basis.
 
-        This is a *static method* that should be defined for all
+        This is a *class method* that should be defined for all
         new operations and observables, that returns the matrix representing
         the operator in the computational basis.
 
         This private method allows matrices to be computed
         directly without instantiating the operators first.
 
         To return the matrices of *instantiated* operators,
@@ -259,14 +259,77 @@
 
         Returns:
             array: matrix representation
         """
         raise NotImplementedError
 
     @property
+    def matrix(self):
+        r"""Matrix representation of an instantiated operator
+        in the computational basis.
+
+        **Example:**
+
+        >>> U = qml.RY(0.5, wires=1)
+        >>> U.matrix
+        >>> array([[ 0.96891242+0.j, -0.24740396+0.j],
+                   [ 0.24740396+0.j,  0.96891242+0.j]])
+
+        Returns:
+            array: matrix representation
+        """
+        return self._matrix(*self.parameters)
+
+    @classmethod
+    def _eigvals(cls, *params):
+        """Eigenvalues of the operator.
+
+        This is a *class method* that should be defined for all
+        new operations and observables that returns the eigenvalues
+        of the operator. Note that the eigenvalues are not guaranteed
+        to be in any particular order.
+
+        This private method allows eigenvalues to be computed
+        directly without instantiating the operators first.
+
+        The default implementation relies on the presence of the
+        :attr:`_matrix` method.
+
+        To return the eigenvalues of *instantiated* operators,
+        please use the :attr:`~.Operator.eigvals` property instead.
+
+        **Example:**
+
+        >>> qml.RZ._eigvals(0.5)
+        >>> array([0.96891242-0.24740396j, 0.96891242+0.24740396j])
+
+        Returns:
+            array: eigenvalue representation
+        """
+        return np.linalg.eigvals(cls._matrix(*params))
+
+    @property
+    def eigvals(self):
+        r"""Eigenvalues of an instantiated operator.
+
+        Note that the eigenvalues are not guaranteed to be in any
+        particular order.
+
+        **Example:**
+
+        >>> U = qml.RZ(0.5, wires=1)
+        >>> U.eigvals
+        >>> array([0.96891242-0.24740396j, 0.96891242+0.24740396j])
+
+        Returns:
+            array: eigvals representation
+        """
+        return self._eigvals(*self.parameters)
+
+    @property
     @abc.abstractmethod
     def num_params(self):
         """Number of parameters the operator takes."""
 
     @property
     @abc.abstractmethod
     def num_wires(self):
@@ -285,31 +348,14 @@
 
     @property
     def name(self):
         """String for the name of the operator.
         """
         return self._name
 
-    @property
-    def matrix(self):
-        r"""Matrix representation of an instantiated operator
-        in the computational basis.
-
-        **Example:**
-
-        >>> U = qml.RY(0.5, wires=1)
-        >>> U.matrix
-        >>> array([[ 0.96891242+0.j, -0.24740396+0.j],
-                   [ 0.24740396+0.j,  0.96891242+0.j]])
-
-        Returns:
-            array: matrix representation
-        """
-        return self._matrix(*self.parameters)
-
     @name.setter
     def name(self, value):
         self._name = value
 
     def __init__(self, *params, wires=None, do_queue=True):
         # pylint: disable=too-many-branches
         self._name = self.__class__.__name__  #: str: name of the operator
@@ -317,36 +363,46 @@
 
         if wires is None:
             raise ValueError("Must specify the wires that {} acts on".format(self.name))
 
         if len(params) != self.num_params:
             raise ValueError(
                 "{}: wrong number of parameters. "
-                "{} parameters passed, {} expected.".format(self.name, params, self.num_params)
+                "{} parameters passed, {} expected.".format(self.name, len(params), self.num_params)
             )
 
         # check the validity of the params
         if self.do_check_domain:
             for p in params:
                 self.check_domain(p)
         self.params = list(params)  #: list[Any]: parameters of the operator
 
         # apply the operator on the given wires
         if not isinstance(wires, Sequence):
             wires = [wires]
         self._check_wires(wires)
         self._wires = wires  #: tuple[int]: wires on which the operator acts
 
-        if do_queue and (qml._current_context is not None):
+        if do_queue:
             self.queue()
 
     def __str__(self):
-        """Print the operator name and some information."""
+        """Operator name and some information."""
         return "{}: {} params, wires {}".format(self.name, len(self.params), self.wires)
 
+    def __repr__(self):
+        """Constructor-call-like representation."""
+        # FIXME using self.parameters here instead of self.params is dangerous, it assumes the params can be evaluated
+        # which is only true if something suitable happens to remain in VariableRef.positional_arg_values etc. after
+        # the last evaluation.
+        if self.parameters:
+            params = ", ".join([repr(p) for p in self.parameters])
+            return "{}({}, wires={})".format(self.name, params, self.wires)
+        return "{}(wires={})".format(self.name, self.wires)
+
     def _check_wires(self, wires):
         """Check the validity of the operator wires.
 
         Args:
             wires (Sequence[Any]): wires to check
         Raises:
             TypeError, ValueError: list of wires is invalid
@@ -357,15 +413,19 @@
             if not isinstance(w, numbers.Integral):
                 raise TypeError(
                     "{}: Wires must be integers, or integer-valued nondifferentiable parameters in mutable circuits.".format(
                         self.name
                     )
                 )
 
-        if self.num_wires != All and self.num_wires != Any and len(wires) != self.num_wires:
+        if (
+            self.num_wires != AllWires
+            and self.num_wires != AnyWires
+            and len(wires) != self.num_wires
+        ):
             raise ValueError(
                 "{}: wrong number of wires. "
                 "{} wires given, {} expected.".format(self.name, len(wires), self.num_wires)
             )
 
         if len(set(wires)) != len(wires):
             raise ValueError("{}: wires must be unique, got {}.".format(self.name, wires))
@@ -460,17 +520,17 @@
             if isinstance(p, Variable):
                 p = self.check_domain(p.val)
             return p
 
         return [evaluate(p) for p in self.params]
 
     def queue(self):
-        """Append the operator to a BaseQNode queue."""
+        """Append the operator to the Operator queue."""
+        qml.QueuingContext.append_operator(self)
 
-        qml._current_context._append_op(self)
         return self  # so pre-constructed Observable instances can be queued and returned in a single statement
 
 
 # =============================================================================
 # Base Operation class
 # =============================================================================
 
@@ -613,18 +673,29 @@
             :class:`Operator`: operation to be inverted
         """
         self.inverse = not self._inverse
         return self
 
     @property
     def matrix(self):
+        op_matrix = self._matrix(*self.parameters)
+
         if self.inverse:
-            return np.linalg.inv(self._matrix(*self.parameters))
+            return op_matrix.conj().T
 
-        return self._matrix(*self.parameters)
+        return op_matrix
+
+    @property
+    def eigvals(self):
+        op_eigvals = self._eigvals(*self.parameters)
+
+        if self.inverse:
+            return op_eigvals.conj()
+
+        return op_eigvals
 
     @property
     def base_name(self):
         """Get base name of the operator.
         """
         return self.__class__.__name__
 
@@ -660,14 +731,99 @@
                 ), "Gradient recipe must have one entry for each parameter!"
         else:
             assert self.grad_recipe is None, "Gradient recipe is only used by the A method!"
 
         super().__init__(*params, wires=wires, do_queue=do_queue)
 
 
+class DiagonalOperation(Operation):
+    r"""Base class for diagonal quantum operations supported by a device.
+
+    As with :class:`~.Operation`, the following class attributes must be
+    defined for all operations:
+
+    * :attr:`~.Operator.num_params`
+    * :attr:`~.Operator.num_wires`
+    * :attr:`~.Operator.par_domain`
+
+    The following two class attributes are optional, but in most cases
+    should be clearly defined to avoid unexpected behavior during
+    differentiation.
+
+    * :attr:`~.Operation.grad_method`
+    * :attr:`~.Operation.grad_recipe`
+
+    Finally, there are some additional optional class attributes
+    that may be set, and used by certain quantum optimizers:
+
+    * :attr:`~.Operation.generator`
+
+    Args:
+        params (tuple[float, int, array, Variable]): operation parameters
+
+    Keyword Args:
+        wires (Sequence[int]): Subsystems it acts on. If not given, args[-1]
+            is interpreted as wires.
+        do_queue (bool): Indicates whether the operation should be
+            immediately pushed into a :class:`BaseQNode` circuit queue.
+            This flag is useful if there is some reason to run an Operation
+            outside of a BaseQNode context.
+    """
+    # pylint: disable=abstract-method
+
+    @classmethod
+    def _eigvals(cls, *params):
+        """Eigenvalues of the operator.
+
+        The order of the eigenvalues needs to match the order of
+        the computational basis vectors.
+
+        This is a *class method* that must be defined for all
+        new diagonal operations, that returns the eigenvalues
+        of the operator in the computational basis.
+
+        This private method allows eigenvalues to be computed
+        directly without instantiating the operators first.
+
+        To return the eigenvalues of *instantiated* operators,
+        please use the :attr:`~.Operator.eigvals` property instead.
+
+        **Example:**
+
+        >>> qml.RZ._eigvals(0.5)
+        >>> array([0.96891242-0.24740396j, 0.96891242+0.24740396j])
+
+        Returns:
+            array: eigenvalue representation
+        """
+        raise NotImplementedError
+
+    @property
+    def eigvals(self):
+        r"""Eigenvalues of an instantiated diagonal operation.
+
+        The order of the eigenvalues needs to match the order of
+        the computational basis vectors.
+
+        **Example:**
+
+        >>> U = qml.RZ(0.5, wires=1)
+        >>> U.eigvals
+        >>> array([0.96891242-0.24740396j, 0.96891242+0.24740396j])
+
+        Returns:
+            array: eigvals representation
+        """
+        return super().eigvals
+
+    @classmethod
+    def _matrix(cls, *params):
+        return np.diag(cls._eigvals(*params))
+
+
 # =============================================================================
 # Base Observable class
 # =============================================================================
 
 
 class Observable(Operator):
     """Base class for observables supported by a device.
@@ -684,45 +840,96 @@
     Args:
         params (tuple[float, int, array, Variable]): observable parameters
 
     Keyword Args:
         wires (Sequence[int]): subsystems it acts on.
             Currently, only one subsystem is supported.
         do_queue (bool): Indicates whether the operation should be
-            immediately pushed into a :class:`BaseQNode` observable queue.
-            The observable queue is determined by the presence of an
-            applicable `qml._current_context`. If no context is
-            available, this argument is ignored.
+            immediately pushed into the Operator queue.
     """
 
     # pylint: disable=abstract-method
     return_type = None
 
+    @classmethod
+    def _eigvals(cls, *params):
+        """Eigenvalues of the observable.
+
+        The order of the eigenvalues needs to match the order of
+        the computational basis vectors when the observable is
+        diagonalized using :attr:`diagonalizing_gates`.
+
+        This is a *class method* that must be defined for all
+        new diagonal operations, that returns the eigenvalues
+        of the operator in the computational basis.
+
+        This private method allows eigenvalues to be computed
+        directly without instantiating the operators first.
+
+        To return the eigenvalues of *instantiated* operators,
+        please use the :attr:`~.Operator.eigvals` property instead.
+
+        **Example:**
+
+        >>> qml.PauliZ._eigvals()
+        >>> array([1, -1])
+
+        Returns:
+            array: eigenvalue representation
+        """
+        raise NotImplementedError
+
+    @property
+    def eigvals(self):
+        r"""Eigenvalues of an instantiated observable.
+
+        The order of the eigenvalues needs to match the order of
+        the computational basis vectors when the observable is
+        diagonalized using :attr:`diagonalizing_gates`. This is a requirement for using qubit observables in quantum functions.
+
+        **Example:**
+
+        >>> U = qml.PauliZ(wires=1)
+        >>> U.eigvals
+        >>> array([1, -1])
+
+        Returns:
+            array: eigvals representation
+        """
+        return super().eigvals
+
     def __init__(self, *params, wires=None, do_queue=True):
         # extract the arguments
         if wires is None:
             wires = params[-1]
             params = params[:-1]
 
         super().__init__(*params, wires=wires, do_queue=do_queue)
 
+    def __repr__(self):
+        """Constructor-call-like representation."""
+        temp = super().__repr__()
+
+        if self.return_type is None:
+            return temp
+
+        if self.return_type is Probability:
+            return repr(self.return_type) + "(wires={})".format(self.wires)
+
+        return repr(self.return_type) + "(" + temp + ")"
+
     def __matmul__(self, other):
         if isinstance(other, Tensor):
             return other.__rmatmul__(self)
 
         if isinstance(other, Observable):
             return Tensor(self, other)
 
         raise ValueError("Can only perform tensor products between observables.")
 
-    @property
-    def eigvals(self):
-        r"""Returns the eigenvalues of the observable"""
-        raise NotImplementedError
-
     def diagonalizing_gates(self):
         r"""Returns the list of operations such that they
         diagonalize the observable in the computational basis.
 
         Returns:
             list(qml.Operation): A list of gates that diagonalize
             the observable in the computational basis.
@@ -749,15 +956,15 @@
     # pylint: disable=abstract-method
     return_type = None
     tensor = True
     par_domain = None
 
     def __init__(self, *args):  # pylint: disable=super-init-not-called
 
-        self._eigvals = None
+        self._eigvals_cache = None
         self.obs = []
 
         for o in args:
             if isinstance(o, Tensor):
                 self.obs.extend(o.obs)
             elif isinstance(o, Observable):
                 self.obs.append(o)
@@ -766,14 +973,18 @@
 
     def __str__(self):
         """Print the tensor product and some information."""
         return "Tensor product {}: {} params, wires {}".format(
             [i.name for i in self.obs], len(self.params), self.wires
         )
 
+    def __repr__(self):
+        """Constructor-call-like representation."""
+        return "Tensor(" + ", ".join([repr(o) for o in self.obs]) + ")"
+
     @property
     def name(self):
         """All constituent observable names making up the tensor product.
 
         Returns:
             list[str]: list containing all observable names
         """
@@ -863,44 +1074,44 @@
         This method uses pre-stored eigenvalues for standard observables where
         possible.
 
         Returns:
             array[float]: array containing the eigenvalues of the tensor product
             observable
         """
-        if self._eigvals is not None:
-            return self._eigvals
+        if self._eigvals_cache is not None:
+            return self._eigvals_cache
 
         standard_observables = {"PauliX", "PauliY", "PauliZ", "Hadamard"}
 
         # observable should be Z^{\otimes n}
-        self._eigvals = pauli_eigs(len(self.wires))
+        self._eigvals_cache = pauli_eigs(len(self.wires))
 
         # TODO: check for edge cases of the sorting, e.g. Tensor(Hermitian(obs, wires=[0, 2]),
         # Hermitian(obs, wires=[1, 3, 4])
         # Sorting the observables based on wires, so that the order of
         # the eigenvalues is correct
         obs_sorted = sorted(self.obs, key=lambda x: x.wires)
 
         # check if there are any non-standard observables (such as Identity)
         if set(self.name) - standard_observables:
             # Tensor product of observables contains a mixture
             # of standard and non-standard observables
-            self._eigvals = np.array([1])
+            self._eigvals_cache = np.array([1])
             for k, g in itertools.groupby(obs_sorted, lambda x: x.name in standard_observables):
                 if k:
                     # Subgroup g contains only standard observables.
-                    self._eigvals = np.kron(self._eigvals, pauli_eigs(len(list(g))))
+                    self._eigvals_cache = np.kron(self._eigvals_cache, pauli_eigs(len(list(g))))
                 else:
                     # Subgroup g contains only non-standard observables.
                     for ns_ob in g:
                         # loop through all non-standard observables
-                        self._eigvals = np.kron(self._eigvals, ns_ob.eigvals)
+                        self._eigvals_cache = np.kron(self._eigvals_cache, ns_ob.eigvals)
 
-        return self._eigvals
+        return self._eigvals_cache
 
     def diagonalizing_gates(self):
         """Return the gate set that diagonalizes a circuit according to the
         specified tensor observable.
 
         This method uses pre-stored eigenvalues for standard observables where
         possible and stores the corresponding eigenvectors from the eigendecomposition.
```

### Comparing `PennyLane-0.8.1/pennylane/ops/cv.py` & `PennyLane-0.9.0/pennylane/ops/cv.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,22 @@
 
 .. note::
 
    For the Heisenberg matrix representation of CV operations, we use the ordering
    :math:`(\hat{\mathbb{1}}, \hat{x}, \hat{p})` for single modes
    and :math:`(\hat{\mathbb{1}}, \hat{x}_1, \hat{p}_2, \hat{x}_1,\hat{p}_2)` for two modes .
 """
+# As the qubit based ``decomposition``, ``_matrix``, ``diagonalizing_gates``
+# abstract methods are not defined in the CV case, disabling the related check
+# pylint: disable=abstract-method
+import math
 import numpy as np
 from scipy.linalg import block_diag
 
-from pennylane.operation import Any, CVOperation, CVObservable
+from pennylane.operation import AnyWires, CVOperation, CVObservable
 
 
 def _rotation(phi, bare=False):
     r"""Utility function, returns the Heisenberg transformation of a phase rotation gate.
 
     The transformation matrix returned is:
 
@@ -52,16 +56,16 @@
     Args:
         phi (float): rotation angle.
         bare (bool): if True, return a simple 2d rotation matrix
 
     Returns:
         array[float]: transformation matrix
     """
-    c = np.cos(phi)
-    s = np.sin(phi)
+    c = math.cos(phi)
+    s = math.sin(phi)
     temp = np.array([[c, -s], [s, c]])
     if bare:
         return temp
     return block_diag(1, temp)  # pylint: disable=no-member
 
 
 class Rotation(CVOperation):
@@ -130,20 +134,20 @@
     """
     num_wires = 1
     num_params = 2
     par_domain = "R"
     grad_method = "A"
 
     shift = 0.1
-    grad_recipe = [(0.5 / np.sinh(shift), shift), None]
+    grad_recipe = [(0.5 / math.sinh(shift), shift), None]
 
     @staticmethod
     def _heisenberg_rep(p):
         R = _rotation(p[1] / 2)
-        return R @ np.diag([1, np.exp(-p[0]), np.exp(p[0])]) @ R.T
+        return R @ np.diag([1, math.exp(-p[0]), math.exp(p[0])]) @ R.T
 
 
 class Displacement(CVOperation):
     r"""pennylane.Displacement(a, phi, wires)
     Phase space displacement.
 
     .. math::
@@ -176,16 +180,16 @@
     grad_method = "A"
 
     shift = 0.1
     grad_recipe = [(0.5 / shift, shift), None]
 
     @staticmethod
     def _heisenberg_rep(p):
-        c = np.cos(p[1])
-        s = np.sin(p[1])
+        c = math.cos(p[1])
+        s = math.sin(p[1])
         scale = 2  # sqrt(2 * hbar)
         return np.array([[1, 0, 0], [scale * c * p[0], 1, 0], [scale * s * p[0], 0, 1]])
 
 
 class Beamsplitter(CVOperation):
     r"""pennylane.Beamsplitter(theta, phi, wires)
     Beamsplitter interaction.
@@ -223,16 +227,16 @@
     par_domain = "R"
     grad_method = "A"
 
     # For the beamsplitter, both parameters are rotation-like
     @staticmethod
     def _heisenberg_rep(p):
         R = _rotation(p[1], bare=True)
-        c = np.cos(p[0])
-        s = np.sin(p[0])
+        c = math.cos(p[0])
+        s = math.sin(p[0])
         U = c * np.eye(5)
         U[0, 0] = 1
         U[1:3, 3:5] = -s * R.T
         U[3:5, 1:3] = s * R
         return U
 
 
@@ -271,22 +275,22 @@
     """
     num_params = 2
     num_wires = 2
     par_domain = "R"
 
     grad_method = "A"
     shift = 0.1
-    grad_recipe = [(0.5 / np.sinh(shift), shift), None]
+    grad_recipe = [(0.5 / math.sinh(shift), shift), None]
 
     @staticmethod
     def _heisenberg_rep(p):
         R = _rotation(p[1], bare=True)
 
-        S = np.sinh(p[0]) * np.diag([1, -1])
-        U = np.cosh(p[0]) * np.identity(5)
+        S = math.sinh(p[0]) * np.diag([1, -1])
+        U = math.cosh(p[0]) * np.identity(5)
 
         U[0, 0] = 1
         U[1:3, 3:5] = S @ R.T
         U[3:5, 1:3] = S @ R.T
         return U
 
 
@@ -524,15 +528,15 @@
     where :math:`S` is the Gaussian symplectic transformation representing the interferometer.
 
     Args:
         U (array): A shape ``(len(wires), len(wires))`` complex unitary matrix
         wires (Sequence[int] or int): the wires the operation acts on
     """
     num_params = 1
-    num_wires = Any
+    num_wires = AnyWires
     par_domain = "A"
     grad_method = None
     grad_recipe = None
 
     @staticmethod
     def _heisenberg_rep(p):
         N = len(p[0])
@@ -658,15 +662,15 @@
     * Gradient recipe: None
 
     Args:
         r (array): a length :math:`2N` vector of means, of the
             form :math:`(\x_0,\dots,\x_{N-1},\p_0,\dots,\p_{N-1})`
         V (array): the :math:`2N\times 2N` (real and positive definite) covariance matrix
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 2
     par_domain = "A"
     grad_method = "F"
 
 
 class FockState(CVOperation):
     r"""pennylane.FockState(n, wires)
@@ -698,15 +702,15 @@
     * Number of parameters: 1
     * Gradient recipe: None (uses finite difference)
 
     Args:
         state (array): a single ket vector, for single mode state preparation,
             or a multimode ket, with one array dimension per mode
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 1
     par_domain = "A"
     grad_method = "F"
 
 
 class FockDensityMatrix(CVOperation):
     r"""pennylane.FockDensityMatrix(state, wires)
@@ -718,15 +722,15 @@
     * Number of parameters: 1
     * Gradient recipe: None (uses finite difference)
 
     Args:
         state (array): a single mode matrix :math:`\rho_{ij}`, or
             a multimode tensor :math:`\rho_{ij,kl,\dots,mn}`, with two indices per mode
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 1
     par_domain = "A"
     grad_method = "F"
 
 
 class CatState(CVOperation):
     r"""pennylane.CatState(a, phi, p, wires)
@@ -799,14 +803,70 @@
 
     @staticmethod
     def _heisenberg_rep(p):
         hbar = 2
         return np.diag([-0.5, 0.5 / hbar, 0.5 / hbar])
 
 
+class TensorN(CVObservable):
+    r"""pennylane.ops.TensorN(wires)
+    The tensor product of the :class:`~.NumberOperator` acting on different wires.
+
+    If a single wire is defined, returns a :class:`~.NumberOperator` instance for convenient gradient computations.
+
+    When used with the :func:`~.expval` function, the expectation value
+    :math:`\langle \hat{n}_{i_0} \hat{n}_{i_1}\dots \hat{n}_{i_{N-1}}\rangle`
+    for a (sub)set of modes :math:`[i_0, i_1, \dots, i_{N-1}]` of the system is
+    returned.
+
+    **Details:**
+
+    * Number of wires: Any
+    * Number of parameters: 0
+
+    Args:
+        wires (Sequence[int] or int): the wire the operation acts on
+
+    .. UsageDetails::
+
+        Example for multiple modes:
+
+        >>> cv_obs = qml.TensorN(wires=[0, 1])
+        >>> cv_obs
+        TensorN(wires=[0, 1])
+        >>> cv_obs.ev_order is None
+        True
+
+        Example for a single mode (yields a :class:`~.NumberOperator`):
+
+        >>> cv_obs = qml.TensorN(wires=[1])
+        >>> cv_obs
+        NumberOperator(wires=[1])
+        >>> cv_obs.ev_order
+        2
+    """
+    num_wires = AnyWires
+    num_params = 0
+    par_domain = None
+    ev_order = None
+
+    def __new__(cls, *params, wires=None, do_queue=True):
+        # Custom definition for __new__ needed such that a NumberOperator can
+        # be returned when a single mode is defined
+
+        if wires is None:
+            wires = params[-1]
+            params = params[:-1]
+
+        if isinstance(wires, int) or len(wires) == 1:
+            return NumberOperator(*params, wires=wires, do_queue=do_queue)
+
+        return super().__new__(cls)
+
+
 class X(CVObservable):
     r"""pennylane.ops.X(wires)
     The position quadrature observable :math:`\hat{x}`.
 
     When used with the :func:`~.expval` function, the position expectation
     value :math:`\braket{\hat{n}}` is returned. This corresponds to
     the mean displacement in the phase space along the :math:`x` axis.
@@ -893,15 +953,15 @@
 
     grad_method = "A"
     ev_order = 1
 
     @staticmethod
     def _heisenberg_rep(p):
         phi = p[0]
-        return np.array([0, np.cos(phi), np.sin(phi)])  # TODO check
+        return np.array([0, math.cos(phi), math.sin(phi)])  # TODO check
 
 
 class PolyXP(CVObservable):
     r"""pennylane.ops.PolyXP(q, wires)
     An arbitrary second-order polynomial observable.
 
     Represents an arbitrary observable :math:`P(\x,\p)` that is a second order
@@ -921,15 +981,15 @@
     * Number of parameters: 1
     * Observable order: 2nd order in the quadrature operators
     * Heisenberg representation: :math:`A`
 
     Args:
         q (array[float]): expansion coefficients
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 1
     par_domain = "A"
 
     grad_method = "F"
     ev_order = 2
 
     @staticmethod
@@ -975,15 +1035,15 @@
 
             For example, to return the observable :math:`\ket{0,4,2}\bra{0,4,2}` acting on
             wires 0, 1, and 3 of a QNode, you would call ``FockStateProjector(np.array([0, 4, 2], wires=[0, 1, 3]))``.
 
             Note that ``len(n)==len(wires)``, and that ``len(n)`` cannot exceed the
             total number of wires in the QNode.
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 1
     par_domain = "A"
 
     grad_method = None
     ev_order = None
 
 
@@ -1008,11 +1068,19 @@
     "FockStateVector",
     "SqueezedState",
     "ThermalState",
     "GaussianState",
 }
 
 
-obs = {"QuadOperator", "NumberOperator", "P", "X", "PolyXP", "FockStateProjector"}
+obs = {
+    "QuadOperator",
+    "NumberOperator",
+    "TensorN",
+    "P",
+    "X",
+    "PolyXP",
+    "FockStateProjector",
+}
 
 
 __all__ = list(ops | obs)
```

### Comparing `PennyLane-0.8.1/pennylane/ops/qubit.py` & `PennyLane-0.9.0/pennylane/ops/qubit.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 This module contains the available built-in discrete-variable
 quantum operations supported by PennyLane, as well as their conventions.
 """
 # pylint:disable=abstract-method,arguments-differ,protected-access
+import math
+import cmath
+import functools
 import numpy as np
-from scipy.linalg import block_diag
 
-from pennylane.operation import Any, Observable, Operation
+from pennylane.templates import template
+from pennylane.operation import AnyWires, Observable, Operation, DiagonalOperation
 from pennylane.templates.state_preparations import BasisStatePreparation, MottonenStatePreparation
-from pennylane.utils import OperationRecorder, pauli_eigs
+from pennylane.utils import OperationRecorder, pauli_eigs, expand
+
+INV_SQRT2 = 1 / math.sqrt(2)
 
 
 class Hadamard(Observable, Operation):
     r"""Hadamard(wires)
     The Hadamard operator
 
     .. math:: H = \frac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1\\ 1 & -1\end{bmatrix}.
@@ -38,18 +43,23 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
     eigvals = pauli_eigs(1)
+    matrix = np.array([[INV_SQRT2, INV_SQRT2], [INV_SQRT2, -INV_SQRT2]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 1], [1, -1]]) / np.sqrt(2)
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
 
     def diagonalizing_gates(self):
         r"""Rotates the specified wires such that they
         are in the eigenbasis of the Hadamard operator.
 
         For the Hadamard operator,
 
@@ -78,18 +88,23 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
     eigvals = pauli_eigs(1)
+    matrix = np.array([[0, 1], [1, 0]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[0, 1], [1, 0]])
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
 
     def diagonalizing_gates(self):
         r"""Rotates the specified wires such that they
         are in the eigenbasis of the Pauli-X operator.
 
         For the Pauli-X operator,
 
@@ -116,18 +131,23 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
     eigvals = pauli_eigs(1)
+    matrix = np.array([[0, -1j], [1j, 0]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[0, -1j], [1j, 0]])
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
 
     def diagonalizing_gates(self):
         r"""Rotates the specified wires such that they
         are in the eigenbasis of PauliY.
 
         For the Pauli-Y observable,
 
@@ -138,15 +158,15 @@
         Returns:
             list(~.Operation): A list of gates that diagonalize PauliY in the
                 computational basis.
         """
         return [PauliZ(wires=self.wires), S(wires=self.wires), Hadamard(wires=self.wires)]
 
 
-class PauliZ(Observable, Operation):
+class PauliZ(Observable, DiagonalOperation):
     r"""PauliZ(wires)
     The Pauli Z operator
 
     .. math:: \sigma_z = \begin{bmatrix} 1 & 0 \\ 0 & -1\end{bmatrix}.
 
     **Details:**
 
@@ -156,24 +176,29 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
     eigvals = pauli_eigs(1)
+    matrix = np.array([[1, 0], [0, -1]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 0], [0, -1]])
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
 
     def diagonalizing_gates(self):
         return []
 
 
-class S(Operation):
+class S(DiagonalOperation):
     r"""S(wires)
     The single-qubit phase gate
 
     .. math:: S = \begin{bmatrix}
                 1 & 0 \\
                 0 & i
             \end{bmatrix}.
@@ -186,20 +211,24 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         return np.array([[1, 0], [0, 1j]])
 
+    @classmethod
+    def _eigvals(cls, *params):
+        return np.array([1, 1j])
 
-class T(Operation):
+
+class T(DiagonalOperation):
     r"""T(wires)
     The single-qubit T gate
 
     .. math:: T = \begin{bmatrix}
                 1 & 0 \\
                 0 & e^{\frac{i\pi}{4}}
             \end{bmatrix}.
@@ -212,17 +241,21 @@
     Args:
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 0
     num_wires = 1
     par_domain = None
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])
+    @classmethod
+    def _matrix(cls, *params):
+        return np.array([[1, 0], [0, cmath.exp(1j * np.pi / 4)]])
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return np.array([1, cmath.exp(1j * np.pi / 4)])
 
 
 class CNOT(Operation):
     r"""CNOT(wires)
     The controlled-NOT operator
 
     .. math:: CNOT = \begin{bmatrix}
@@ -241,21 +274,22 @@
 
     Args:
         wires (Sequence[int] or int): the wires the operation acts on
     """
     num_params = 0
     num_wires = 2
     par_domain = None
+    matrix = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
+    @classmethod
+    def _matrix(cls, *params):
+        return CNOT.matrix
 
 
-class CZ(Operation):
+class CZ(DiagonalOperation):
     r"""CZ(wires)
     The controlled-Z operator
 
     .. math:: CZ = \begin{bmatrix}
             1 & 0 & 0 & 0 \\
             0 & 1 & 0 & 0\\
             0 & 0 & 1 & 0\\
@@ -271,18 +305,24 @@
 
     Args:
         wires (Sequence[int] or int): the wires the operation acts on
     """
     num_params = 0
     num_wires = 2
     par_domain = None
+    eigvals = np.array([1, 1, 1, -1])
+    matrix = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
+
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
 
 
 class SWAP(Operation):
     r"""SWAP(wires)
     The swap operator
 
     .. math:: SWAP = \begin{bmatrix}
@@ -299,18 +339,19 @@
 
     Args:
         wires (Sequence[int] or int): the wires the operation acts on
     """
     num_params = 0
     num_wires = 2
     par_domain = None
+    matrix = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
 
 
 class CSWAP(Operation):
     r"""CSWAP(wires)
     The controlled-swap operator
 
     .. math:: CSWAP = \begin{bmatrix}
@@ -333,29 +374,30 @@
 
     Args:
         wires (Sequence[int] or int): the wires the operation acts on
     """
     num_params = 0
     num_wires = 3
     par_domain = None
+    matrix = np.array(
+        [
+            [1, 0, 0, 0, 0, 0, 0, 0],
+            [0, 1, 0, 0, 0, 0, 0, 0],
+            [0, 0, 1, 0, 0, 0, 0, 0],
+            [0, 0, 0, 1, 0, 0, 0, 0],
+            [0, 0, 0, 0, 1, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0, 1, 0],
+            [0, 0, 0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 1],
+        ]
+    )
 
-    @staticmethod
-    def _matrix(*params):
-        return np.array(
-            [
-                [1, 0, 0, 0, 0, 0, 0, 0],
-                [0, 1, 0, 0, 0, 0, 0, 0],
-                [0, 0, 1, 0, 0, 0, 0, 0],
-                [0, 0, 0, 1, 0, 0, 0, 0],
-                [0, 0, 0, 0, 1, 0, 0, 0],
-                [0, 0, 0, 0, 0, 0, 1, 0],
-                [0, 0, 0, 0, 0, 1, 0, 0],
-                [0, 0, 0, 0, 0, 0, 0, 1],
-            ]
-        )
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
 
 
 class Toffoli(Operation):
     r"""Toffoli(wires)
     Toffoli (controlled-controlled-X) gate.
 
     .. math::
@@ -379,20 +421,30 @@
 
     Args:
         wires (int): the subsystem the gate acts on
     """
     num_params = 0
     num_wires = 3
     par_domain = None
+    matrix = np.array(
+        [
+            [1, 0, 0, 0, 0, 0, 0, 0],
+            [0, 1, 0, 0, 0, 0, 0, 0],
+            [0, 0, 1, 0, 0, 0, 0, 0],
+            [0, 0, 0, 1, 0, 0, 0, 0],
+            [0, 0, 0, 0, 1, 0, 0, 0],
+            [0, 0, 0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 0, 0, 1],
+            [0, 0, 0, 0, 0, 0, 1, 0],
+        ]
+    )
 
-    @staticmethod
-    def _matrix(*params):
-        mat = np.diag([1 for i in range(8)])
-        mat[6:8, 6:8] = np.array([[0, 1], [1, 0]])
-        return mat
+    @classmethod
+    def _matrix(cls, *params):
+        return cls.matrix
 
 
 class RX(Operation):
     r"""RX(phi, wires)
     The single qubit X rotation
 
     .. math:: R_x(\phi) = e^{-i\phi\sigma_x/2} = \begin{bmatrix}
@@ -413,18 +465,21 @@
     """
     num_params = 1
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
     generator = [PauliX, -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         theta = params[0]
-        return np.cos(theta / 2) * np.eye(2) + 1j * np.sin(-theta / 2) * PauliX._matrix()
+        c = math.cos(theta / 2)
+        js = 1j * math.sin(-theta / 2)
+
+        return np.array([[c, js], [js, c]])
 
 
 class RY(Operation):
     r"""RY(phi, wires)
     The single qubit Y rotation
 
     .. math:: R_y(\phi) = e^{-i\phi\sigma_y/2} = \begin{bmatrix}
@@ -445,21 +500,24 @@
     """
     num_params = 1
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
     generator = [PauliY, -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         theta = params[0]
-        return np.cos(theta / 2) * np.eye(2) + 1j * np.sin(-theta / 2) * PauliY._matrix()
+        c = math.cos(theta / 2)
+        s = math.sin(theta / 2)
 
+        return np.array([[c, -s], [s, c]])
 
-class RZ(Operation):
+
+class RZ(DiagonalOperation):
     r"""RZ(phi, wires)
     The single qubit Z rotation
 
     .. math:: R_z(\phi) = e^{-i\phi\sigma_z/2} = \begin{bmatrix}
                 e^{-i\phi/2} & 0 \\
                 0 & e^{i\phi/2}
             \end{bmatrix}.
@@ -477,21 +535,30 @@
     """
     num_params = 1
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
     generator = [PauliZ, -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
+        theta = params[0]
+        p = cmath.exp(-0.5j * theta)
+
+        return np.array([[p, 0], [0, p.conjugate()]])
+
+    @classmethod
+    def _eigvals(cls, *params):
         theta = params[0]
-        return np.cos(theta / 2) * np.eye(2) + 1j * np.sin(-theta / 2) * PauliZ._matrix()
+        p = cmath.exp(-0.5j * theta)
+
+        return np.array([p, p.conjugate()])
 
 
-class PhaseShift(Operation):
+class PhaseShift(DiagonalOperation):
     r"""PhaseShift(phi, wires)
     Arbitrary single qubit local phase shift
 
     .. math:: R_\phi(\phi) = e^{i\phi/2}R_z(\phi) = \begin{bmatrix}
                 1 & 0 \\
                 0 & e^{i\phi}
             \end{bmatrix}.
@@ -509,18 +576,23 @@
     """
     num_params = 1
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
     generator = [np.array([[0, 0], [0, 1]]), 1]
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
+        phi = params[0]
+        return np.array([[1, 0], [0, cmath.exp(1j * phi)]])
+
+    @classmethod
+    def _eigvals(cls, *params):
         phi = params[0]
-        return np.array([[1, 0], [0, np.exp(1j * phi)]])
+        return np.array([1, cmath.exp(1j * phi)])
 
 
 class Rot(Operation):
     r"""Rot(phi, theta, omega, wires)
     Arbitrary single qubit rotation
 
     .. math::
@@ -550,25 +622,239 @@
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 3
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
 
-    @staticmethod
-    def _matrix(*params):
-        a, b, c = params
-        return RZ._matrix(c) @ (RY._matrix(b) @ RZ._matrix(a))
+    @classmethod
+    def _matrix(cls, *params):
+        phi, theta, omega = params
+        c = math.cos(theta / 2)
+        s = math.sin(theta / 2)
+
+        return np.array(
+            [
+                [cmath.exp(-0.5j * (phi + omega)) * c, -cmath.exp(0.5j * (phi - omega)) * s],
+                [cmath.exp(-0.5j * (phi - omega)) * s, cmath.exp(0.5j * (phi + omega)) * c],
+            ]
+        )
 
     @staticmethod
     def decomposition(phi, theta, omega, wires):
         decomp_ops = [RZ(phi, wires=wires), RY(theta, wires=wires), RZ(omega, wires=wires)]
         return decomp_ops
 
 
+class MultiRZ(DiagonalOperation):
+    r"""MultiRZ(theta, wires)
+    Arbitrary multi Z rotation.
+
+    .. math::
+
+        MultiRZ(\theta) = \exp(-i \frac{\theta}{2} Z^{\otimes n})
+
+    **Details:**
+
+    * Number of wires: Any
+    * Number of parameters: 1
+    * Gradient recipe: :math:`\frac{d}{d\theta}f(MultiRZ(\theta)) = \frac{1}{2}\left[f(MultiRZ(\theta +\pi/2)) - f(MultiRZ(\theta-\pi/2))\right]`
+      where :math:`f` is an expectation value depending on :math:`MultiRZ(\theta)`.
+
+    .. note::
+
+        If the ``MultiRZ`` gate is not supported on the targeted device, PennyLane
+        will decompose the gate using :class:`~.RZ` and :class:`~.CNOT` gates.
+
+    Args:
+        theta (float): rotation angle :math:`\theta`
+        wires (Sequence[int] or int): the wires the operation acts on
+    """
+    num_params = 1
+    num_wires = AnyWires
+    par_domain = "R"
+    grad_method = "A"
+
+    @classmethod
+    def _matrix(cls, theta, n):
+        """Matrix representation of a MultiRZ gate.
+
+        Args:
+            theta (float): Rotation angle.
+            n (int): Number of wires the rotation acts on. This has
+                to be given explicitly in the static method as the
+                wires object is not available.
+
+        Returns:
+            array[complex]: The matrix representation
+        """
+        multi_Z_rot_eigs = MultiRZ._eigvals(theta, n)
+        multi_Z_rot_matrix = np.diag(multi_Z_rot_eigs)
+
+        return multi_Z_rot_matrix
+
+    @property
+    def matrix(self):
+        # Redefine the property here to pass additionally the number of wires to the ``_matrix`` method
+        if self.inverse:
+            # The matrix is diagonal, so there is no need to transpose
+            return self._matrix(*self.parameters, len(self.wires)).conj()
+
+        return self._matrix(*self.parameters, len(self.wires))
+
+    @classmethod
+    def _eigvals(cls, theta, n):
+        return np.exp(-1j * theta / 2 * pauli_eigs(n))
+
+    @property
+    def eigvals(self):
+        # Redefine the property here to pass additionally the number of wires to the ``_eigvals`` method
+        if self.inverse:
+            return self._eigvals(*self.parameters, len(self.wires)).conj()
+
+        return self._eigvals(*self.parameters, len(self.wires))
+
+    @staticmethod
+    @template
+    def decomposition(theta, wires):
+        for i in range(len(wires) - 1, 0, -1):
+            CNOT(wires=[wires[i], wires[i - 1]])
+
+        RZ(theta, wires=wires[0])
+
+        for i in range(len(wires) - 1):
+            CNOT(wires=[wires[i + 1], wires[i]])
+
+
+class PauliRot(Operation):
+    r"""PauliRot(theta, pauli_word, wires)
+    Arbitrary Pauli word rotation.
+
+    .. math::
+
+        RP(\theta, P) = \exp(-i \frac{\theta}{2} P)
+
+    **Details:**
+
+    * Number of wires: Any
+    * Number of parameters: 2 (1 differentiable parameter)
+    * Gradient recipe: :math:`\frac{d}{d\theta}f(RP(\theta)) = \frac{1}{2}\left[f(RP(\theta +\pi/2)) - f(RP(\theta-\pi/2))\right]`
+      where :math:`f` is an expectation value depending on :math:`RP(\theta)`.
+
+    .. note::
+
+        If the ``PauliRot`` gate is not supported on the targeted device, PennyLane
+        will decompose the gate using :class:`~.RX`, :class:`~.Hadamard`, :class:`~.RZ`
+        and :class:`~.CNOT` gates.
+
+    Args:
+        theta (float): rotation angle :math:`\theta`
+        pauli_word (string): the Pauli word defining the rotation
+        wires (Sequence[int] or int): the wire the operation acts on
+    """
+    num_params = 2
+    num_wires = AnyWires
+    do_check_domain = False
+    par_domain = "R"
+    grad_method = "A"
+
+    _ALLOWED_CHARACTERS = "IXYZ"
+
+    _PAULI_CONJUGATION_MATRICES = {
+        "X": Hadamard._matrix(),
+        "Y": RX._matrix(np.pi / 2),
+        "Z": np.array([[1, 0], [0, 1]]),
+    }
+
+    def __init__(self, *params, wires=None, do_queue=True):
+        super().__init__(*params, wires=wires, do_queue=True)
+
+        pauli_word = params[1]
+
+        if not PauliRot._check_pauli_word(pauli_word):
+            raise ValueError(
+                'The given Pauli word "{}" contains characters that are not allowed.'
+                " Allowed characters are I, X, Y and Z".format(pauli_word)
+            )
+
+        if not len(pauli_word) == len(wires):
+            raise ValueError(
+                "The given Pauli word has length {}, length {} was expected for wires {}".format(
+                    len(pauli_word), len(wires), wires
+                )
+            )
+
+    @staticmethod
+    def _check_pauli_word(pauli_word):
+        """Check that the given Pauli word has correct structure.
+
+        Args:
+            pauli_word (str): Pauli word to be checked
+
+        Returns:
+            bool: Whether the Pauli word has correct structure.
+        """
+        return all(pauli in PauliRot._ALLOWED_CHARACTERS for pauli in pauli_word)
+
+    @classmethod
+    def _matrix(cls, *params):
+        theta = params[0]
+        pauli_word = params[1]
+
+        if not PauliRot._check_pauli_word(pauli_word):
+            raise ValueError(
+                'The given Pauli word "{}" contains characters that are not allowed.'
+                " Allowed characters are I, X, Y and Z".format(pauli_word)
+            )
+
+        # We first generate the matrix excluding the identity parts and expand it afterwards.
+        # To this end, we have to store on which wires the non-identity parts act
+        non_identity_wires, non_identity_gates = zip(
+            *[(wire, gate) for wire, gate in enumerate(pauli_word) if gate != "I"]
+        )
+
+        multi_Z_rot_matrix = MultiRZ._matrix(theta, len(non_identity_gates))
+
+        # now we conjugate with Hadamard and RX to create the Pauli string
+        conjugation_matrix = functools.reduce(
+            np.kron, [PauliRot._PAULI_CONJUGATION_MATRICES[gate] for gate in non_identity_gates],
+        )
+
+        return expand(
+            conjugation_matrix.T.conj() @ multi_Z_rot_matrix @ conjugation_matrix,
+            non_identity_wires,
+            list(range(len(pauli_word))),
+        )
+
+    @classmethod
+    def _eigvals(cls, theta, pauli_word):
+        return MultiRZ._eigvals(theta, len(pauli_word))
+
+    @staticmethod
+    @template
+    def decomposition(theta, pauli_word, wires):
+        active_wires, active_gates = zip(
+            *[(wire, gate) for wire, gate in zip(wires, pauli_word) if gate != "I"]
+        )
+
+        for wire, gate in zip(active_wires, active_gates):
+            if gate == "X":
+                Hadamard(wires=[wire])
+            elif gate == "Y":
+                RX(np.pi / 2, wires=[wire])
+
+        MultiRZ(theta, wires=list(active_wires))
+
+        for wire, gate in zip(active_wires, active_gates):
+            if gate == "X":
+                Hadamard(wires=[wire])
+            elif gate == "Y":
+                RX(-np.pi / 2, wires=[wire])
+
+
 class CRX(Operation):
     r"""CRX(phi, wires)
     The controlled-RX operator
 
     .. math::
 
         \begin{align}
@@ -609,17 +895,21 @@
     """
     num_params = 1
     num_wires = 2
     par_domain = "R"
     grad_method = "A"
     generator = [np.array([[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]), -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
-        return block_diag(np.eye(2), RX._matrix(*params))
+    @classmethod
+    def _matrix(cls, *params):
+        theta = params[0]
+        c = math.cos(theta / 2)
+        js = 1j * math.sin(-theta / 2)
+
+        return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, c, js], [0, 0, js, c]])
 
     @staticmethod
     def decomposition(theta, wires):
         decomp_ops = [
             RZ(np.pi / 2, wires=wires[1]),
             RY(theta / 2, wires=wires[1]),
             CNOT(wires=wires),
@@ -633,15 +923,15 @@
 class CRY(Operation):
     r"""CRY(phi, wires)
     The controlled-RY operator
 
     .. math::
 
         \begin{align}
-             CRY(\phi) &= I_{1}\otimes U3_{2}(\pi / 2) ~\cdot~ CNOT_{12} ~\cdot~ I_{1}\otimes U3_{2}(-\pi / 2) ~\cdot~ CNOT_{12} \notag \\[10pt]
+             CRY(\phi) &= I_{1}\otimes RY_{2}(\pi / 2) ~\cdot~ CNOT_{12} ~\cdot~ I_{1}\otimes RY_{2}(-\pi / 2) ~\cdot~ CNOT_{12} \notag \\[10pt]
             &=
         \begin{bmatrix}
             1 & 0 & 0 & 0 \\
             0 & 1 & 0 & 0\\
             0 & 0 & \cos(\phi/2) & -\sin(\phi/2)\\
             0 & 0 & \sin(\phi/2) & \cos(\phi/2)
         \end{bmatrix}.
@@ -655,15 +945,15 @@
     * Number of parameters: 1
     * Gradient recipe: :math:`\frac{d}{d\phi}f(CR_y(\phi)) = \frac{1}{2}\left[f(CR_y(\phi+\pi/2)) - f(CR_y(\phi-\pi/2))\right]`
       where :math:`f` is an expectation value depending on :math:`CR_y(\phi)`.
 
     **Decomposition**
 
     If the ``CRY`` gate is not supported on the targeted device, PennyLane
-    will attempt to decompose the gate into :class:`~.U3` and :class:`~.CNOT` gates the following way:
+    will attempt to decompose the gate into :class:`~.RY` and :class:`~.CNOT` gates the following way:
 
     .. image:: ../../_static/cry_circuit.png
         :align: center
         :width: 650px
 
 
     Args:
@@ -672,30 +962,34 @@
     """
     num_params = 1
     num_wires = 2
     par_domain = "R"
     grad_method = "A"
     generator = [np.array([[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, -1j], [0, 0, 1j, 0]]), -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
-        return block_diag(np.eye(2), RY._matrix(*params))
+    @classmethod
+    def _matrix(cls, *params):
+        theta = params[0]
+        c = math.cos(theta / 2)
+        s = math.sin(theta / 2)
+
+        return np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, c, -s], [0, 0, s, c]])
 
     @staticmethod
     def decomposition(theta, wires):
         decomp_ops = [
-            U3(theta / 2, 0, 0, wires=wires[1]),
+            RY(theta / 2, wires=wires[1]),
             CNOT(wires=wires),
-            U3(-theta / 2, 0, 0, wires=wires[1]),
+            RY(-theta / 2, wires=wires[1]),
             CNOT(wires=wires),
         ]
         return decomp_ops
 
 
-class CRZ(Operation):
+class CRZ(DiagonalOperation):
     r"""CRZ(phi, wires)
     The controlled-RZ operator
 
     .. math::
 
         \begin{align}
              CRZ(\phi) &= I_{1}\otimes PhaseShift_{2}(\pi / 2) ~\cdot~ CNOT_{12} ~\cdot~ I_{1}\otimes PhaseShift_{2}(-\pi / 2) ~\cdot~ CNOT_{12} \notag \\[10pt]
@@ -733,17 +1027,30 @@
     """
     num_params = 1
     num_wires = 2
     par_domain = "R"
     grad_method = "A"
     generator = [np.array([[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]]), -1 / 2]
 
-    @staticmethod
-    def _matrix(*params):
-        return block_diag(np.eye(2), RZ._matrix(*params))
+    @classmethod
+    def _matrix(cls, *params):
+        theta = params[0]
+        return np.array(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, cmath.exp(-0.5j * theta), 0],
+                [0, 0, 0, cmath.exp(0.5j * theta)],
+            ]
+        )
+
+    @classmethod
+    def _eigvals(cls, *params):
+        theta = params[0]
+        return np.array([1, 1, cmath.exp(-0.5j * theta), cmath.exp(0.5j * theta),])
 
     @staticmethod
     def decomposition(lam, wires):
         decomp_ops = [
             PhaseShift(lam / 2, wires=wires[1]),
             CNOT(wires=wires),
             PhaseShift(-lam / 2, wires=wires[1]),
@@ -780,18 +1087,28 @@
         wires (Sequence[int] or int): the wire the operation acts on
     """
     num_params = 3
     num_wires = 2
     par_domain = "R"
     grad_method = "A"
 
-    @staticmethod
-    def _matrix(*params):
-        a, b, c = params
-        return CRZ._matrix(c) @ (CRY._matrix(b) @ CRZ._matrix(a))
+    @classmethod
+    def _matrix(cls, *params):
+        phi, theta, omega = params
+        c = math.cos(theta / 2)
+        s = math.sin(theta / 2)
+
+        return np.array(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, cmath.exp(-0.5j * (phi + omega)) * c, -cmath.exp(0.5j * (phi - omega)) * s],
+                [0, 0, cmath.exp(-0.5j * (phi - omega)) * s, cmath.exp(0.5j * (phi + omega)) * c],
+            ]
+        )
 
 
 class U1(Operation):
     r"""U1(phi)
     U1 gate.
 
     .. math:: U_1(\phi) = e^{i\phi/2}R_z(\phi) = \begin{bmatrix}
@@ -816,17 +1133,18 @@
     """
     num_params = 1
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
     generator = [np.array([[0, 0], [0, 1]]), 1]
 
-    @staticmethod
-    def _matrix(*params):
-        return PhaseShift._matrix(*params)
+    @classmethod
+    def _matrix(cls, *params):
+        phi = params[0]
+        return np.array([[1, 0], [0, cmath.exp(1j * phi)]])
 
     @staticmethod
     def decomposition(phi, wires):
         return [PhaseShift(phi, wires=wires)]
 
 
 class U2(Operation):
@@ -864,18 +1182,20 @@
         wires (Sequence[int] or int): the subsystem the gate acts on
     """
     num_params = 2
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         phi, lam = params
-        return PhaseShift._matrix(phi + lam) @ Rot._matrix(lam, np.pi / 2, -lam)
+        return INV_SQRT2 * np.array(
+            [[1, -cmath.exp(1j * lam)], [cmath.exp(1j * phi), cmath.exp(1j * (phi + lam))]]
+        )
 
     @staticmethod
     def decomposition(phi, lam, wires):
         decomp_ops = [
             Rot(lam, np.pi / 2, -lam, wires=wires),
             PhaseShift(lam, wires=wires),
             PhaseShift(phi, wires=wires),
@@ -919,18 +1239,26 @@
         wires (Sequence[int] or int): the subsystem the gate acts on
     """
     num_params = 3
     num_wires = 1
     par_domain = "R"
     grad_method = "A"
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         theta, phi, lam = params
-        return PhaseShift._matrix(phi + lam) @ Rot._matrix(lam, theta, -lam)
+        c = math.cos(theta / 2)
+        s = math.sin(theta / 2)
+
+        return np.array(
+            [
+                [c, -s * cmath.exp(1j * lam)],
+                [s * cmath.exp(1j * phi), c * cmath.exp(1j * (phi + lam))],
+            ]
+        )
 
     @staticmethod
     def decomposition(theta, phi, lam, wires):
         decomp_ops = [
             Rot(lam, theta, -lam, wires=wires),
             PhaseShift(lam, wires=wires),
             PhaseShift(phi, wires=wires),
@@ -954,31 +1282,64 @@
     * Gradient recipe: None
 
     Args:
         U (array[complex]): square unitary matrix
         wires (Sequence[int] or int): the wire(s) the operation acts on
     """
     num_params = 1
-    num_wires = Any
+    num_wires = AnyWires
     par_domain = "A"
     grad_method = None
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         U = np.asarray(params[0])
 
         if U.shape[0] != U.shape[1]:
             raise ValueError("Operator must be a square matrix.")
 
         if not np.allclose(U @ U.conj().T, np.identity(U.shape[0])):
             raise ValueError("Operator must be unitary.")
 
         return U
 
 
+class DiagonalQubitUnitary(DiagonalOperation):
+    r"""DiagonalQubitUnitary(D, wires)
+    Apply an arbitrary fixed diagonal unitary matrix.
+
+    **Details:**
+
+    * Number of wires: Any (the operation can act on any number of wires)
+    * Number of parameters: 1
+    * Gradient recipe: None
+
+    Args:
+        D (array[complex]): diagonal of unitary matrix
+        wires (Sequence[int] or int): the wire(s) the operation acts on
+    """
+    num_params = 1
+    num_wires = AnyWires
+    par_domain = "A"
+    grad_method = None
+
+    @classmethod
+    def _eigvals(cls, *params):
+        D = np.asarray(params[0])
+
+        if not np.allclose(D * D.conj(), np.ones_like(D)):
+            raise ValueError("Operator must be unitary.")
+
+        return D
+
+    @staticmethod
+    def decomposition(D, wires):
+        return [QubitUnitary(np.diag(D), wires=wires)]
+
+
 # =============================================================================
 # State preparation
 # =============================================================================
 
 
 class BasisState(Operation):
     r"""BasisState(n, wires)
@@ -999,15 +1360,15 @@
     Args:
         n (array): prepares the basis state :math:`\ket{n}`, where ``n`` is an
             array of integers from the set :math:`\{0, 1\}`, i.e.,
             if ``n = np.array([0, 1, 0])``, prepares the state :math:`|010\rangle`.
         wires (Sequence[int] or int): the wire(s) the operation acts on
     """
     num_params = 1
-    num_wires = Any
+    num_wires = AnyWires
     par_domain = "A"
     grad_method = None
 
     @staticmethod
     def decomposition(n, wires):
         with OperationRecorder() as rec:
             BasisStatePreparation(n, wires)
@@ -1033,15 +1394,15 @@
         2005).
 
     Args:
         state (array[complex]): a state vector of size 2**len(wires)
         wires (Sequence[int] or int): the wire(s) the operation acts on
     """
     num_params = 1
-    num_wires = Any
+    num_wires = AnyWires
     par_domain = "A"
     grad_method = None
 
     @staticmethod
     def decomposition(state, wires):
         with OperationRecorder() as rec:
             MottonenStatePreparation(state, wires)
@@ -1074,22 +1435,22 @@
     * Number of parameters: 1
     * Gradient recipe: None
 
     Args:
         A (array): square hermitian matrix
         wires (Sequence[int] or int): the wire(s) the operation acts on
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 1
     par_domain = "A"
     grad_method = "F"
     _eigs = {}
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _matrix(cls, *params):
         A = np.asarray(params[0])
 
         if A.shape[0] != A.shape[1]:
             raise ValueError("Observable must be a square matrix.")
 
         if not np.allclose(A, A.conj().T):
             raise ValueError("Observable must be Hermitian.")
@@ -1110,15 +1471,14 @@
         """
         Hmat = self.matrix
         Hkey = tuple(Hmat.flatten().tolist())
         if Hkey not in Hermitian._eigs:
             w, U = np.linalg.eigh(Hmat)
             Hermitian._eigs[Hkey] = {"eigvec": U, "eigval": w}
 
-        Hmat = self.matrix
         return Hermitian._eigs[Hkey]
 
     @property
     def eigvals(self):
         """Return the eigenvalues of the specified Hermitian observable.
 
         This method uses pre-stored eigenvalues for standard observables where
@@ -1143,14 +1503,16 @@
 
 
 ops = {
     "Hadamard",
     "PauliX",
     "PauliY",
     "PauliZ",
+    "PauliRot",
+    "MultiRZ",
     "S",
     "T",
     "CNOT",
     "CZ",
     "SWAP",
     "CSWAP",
     "Toffoli",
@@ -1165,14 +1527,15 @@
     "CRot",
     "U1",
     "U2",
     "U3",
     "BasisState",
     "QubitStateVector",
     "QubitUnitary",
+    "DiagonalQubitUnitary",
 }
 
 
 obs = {"Hadamard", "PauliX", "PauliY", "PauliZ", "Hermitian"}
 
 
 __all__ = list(ops | obs)
```

### Comparing `PennyLane-0.8.1/pennylane/ops/__init__.py` & `PennyLane-0.9.0/pennylane/ops/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """
 This module contains core quantum operations supported by PennyLane -
 such as gates, state preparations and observables.
 """
 import numpy as np
 
-from pennylane.operation import Any, Observable, CVObservable
+from pennylane.operation import AnyWires, Observable, CVObservable
 
 from .cv import *
 from .qubit import *
 
 from .cv import __all__ as _cv__all__
 from .cv import ops as _cv__ops__
 from .cv import obs as _cv__obs__
@@ -42,24 +42,28 @@
 
     .. math::
         E[\I] = \text{Tr}(\I \rho)
 
     corresponds to the trace of the quantum state, which in exact
     simulators should always be equal to 1.
     """
-    num_wires = Any
+    num_wires = AnyWires
     num_params = 0
     par_domain = None
     grad_method = None
 
     ev_order = 1
     eigvals = np.array([1, 1])
 
-    @staticmethod
-    def _matrix(*params):
+    @classmethod
+    def _eigvals(cls, *params):
+        return cls.eigvals
+
+    @classmethod
+    def _matrix(cls, *params):
         return np.eye(2)
 
     @staticmethod
     def _heisenberg_rep(p):
         return np.array([1, 0, 0])
 
     def diagonalizing_gates(self):
```

### Comparing `PennyLane-0.8.1/pennylane/optimize/adagrad.py` & `PennyLane-0.9.0/pennylane/optimize/adagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Adagrad optimizer"""
-
-import numpy as np
+import math
 
 from pennylane.utils import _flatten, unflatten
 from .gradient_descent import GradientDescentOptimizer
 
 
 class AdagradOptimizer(GradientDescentOptimizer):
     r"""Gradient-descent optimizer with past-gradient-dependent
@@ -70,15 +69,15 @@
 
         if self.accumulation is None:
             self.accumulation = [g * g for g in grad_flat]
         else:
             self.accumulation = [a + g * g for a, g in zip(self.accumulation, grad_flat)]
 
         x_new_flat = [
-            e - (self._stepsize / np.sqrt(a + self.eps)) * g
+            e - (self._stepsize / math.sqrt(a + self.eps)) * g
             for a, g, e in zip(self.accumulation, grad_flat, x_flat)
         ]
 
         return unflatten(x_new_flat, x)
 
     def reset(self):
         """Reset optimizer by erasing memory of past steps."""
```

### Comparing `PennyLane-0.8.1/pennylane/optimize/adam.py` & `PennyLane-0.9.0/pennylane/optimize/adam.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Adam optimizer"""
-
-import numpy as np
+import math
 
 from pennylane.utils import _flatten, unflatten
 from .gradient_descent import GradientDescentOptimizer
 
 
 class AdamOptimizer(GradientDescentOptimizer):
     r"""Gradient-descent optimizer with adaptive learning rate, first and second moment.
@@ -92,19 +91,19 @@
         else:
             self.sm = [
                 self.beta2 * f + (1 - self.beta2) * g * g for f, g in zip(self.sm, grad_flat)
             ]
 
         # Update step size (instead of correcting for bias)
         new_stepsize = (
-            self._stepsize * np.sqrt(1 - self.beta2 ** self.t) / (1 - self.beta1 ** self.t)
+            self._stepsize * math.sqrt(1 - self.beta2 ** self.t) / (1 - self.beta1 ** self.t)
         )
 
         x_new_flat = [
-            e - new_stepsize * f / (np.sqrt(s) + self.eps)
+            e - new_stepsize * f / (math.sqrt(s) + self.eps)
             for f, s, e in zip(self.fm, self.sm, x_flat)
         ]
 
         return unflatten(x_new_flat, x)
 
     def reset(self):
         """Reset optimizer by erasing memory of past steps."""
```

### Comparing `PennyLane-0.8.1/pennylane/optimize/gradient_descent.py` & `PennyLane-0.9.0/pennylane/optimize/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/optimize/momentum.py` & `PennyLane-0.9.0/pennylane/optimize/momentum.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/optimize/nesterov_momentum.py` & `PennyLane-0.9.0/pennylane/optimize/nesterov_momentum.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/optimize/qng.py` & `PennyLane-0.9.0/pennylane/optimize/qng.py`

 * *Files 25% similar despite different names*

```diff
@@ -69,27 +69,74 @@
     For more details, see:
 
         James Stokes, Josh Izaac, Nathan Killoran, Giuseppe Carleo.
         "Quantum Natural Gradient." `arXiv:1909.02108 <https://arxiv.org/abs/1909.02108>`_, 2019.
 
     .. note::
 
-        The QNG optimizer **only supports single QNodes** as objective functions.
+        The QNG optimizer supports single QNodes or :class:`~.VQECost` objects as objective functions.
+        Alternatively, the metric tensor can directly be provided to the :func:`step` method of the optimizer,
+        using the ``metric_tensor_fn`` argument.
 
-        In particular:
+        For the following cases, providing metric_tensor_fn may be useful:
 
         * For hybrid classical-quantum models, the "mixed geometry" of the model
           makes it unclear which metric should be used for which parameter.
           For example, parameters of quantum nodes are better suited to
           one metric (such as the QNG), whereas others (e.g., parameters of classical nodes)
           are likely better suited to another metric.
 
         * For multi-QNode models, we don't know what geometry is appropriate
           if a parameter is shared amongst several QNodes.
 
+        If the objective function is VQE/VQE-like, i.e., a function of a group
+        of QNodes that share an ansatz, there are two ways to use the optimizer:
+
+        * Realize the objective function as a :class:`~.VQECost` object, which has
+          a ``metric_tensor`` method.
+
+        * Manually provide the ``metric_tensor_fn`` corresponding to the metric tensor of
+          of the QNode(s) involved in the objective function.
+
+    **Examples:**
+
+    For VQE/VQE-like problems, the objective function for the optimizer can be
+    realized as a VQECost object.
+
+    >>> dev = qml.device("default.qubit", wires=1)
+    >>> def circuit(params, wires=0):
+    ...     qml.RX(params[0], wires=wires)
+    ...     qml.RY(params[1], wires=wires)
+    >>> coeffs = [1, 1]
+    >>> obs = [qml.PauliX(0), qml.PauliZ(0)]
+    >>> H = qml.Hamiltonian(coeffs, obs)
+    >>> cost_fn = qml.VQECost(circuit, H, dev)
+
+    Once constructed, the cost function can be passed directly to the
+    optimizer's ``step`` function:
+
+    >>> eta = 0.01
+    >>> init_params = [0.011, 0.012]
+    >>> opt = qml.QNGOptimizer(eta)
+    >>> theta_new = opt.step(cost_fn, init_params)
+    >>> print(theta_new)
+    [0.011445239214543481, -0.027519522461477233]
+
+    Alternatively, the same objective function can be used for the optimizer
+    by manually providing the ``metric_tensor_fn``.
+
+    >>> qnodes = qml.map(circuit, obs, dev, 'expval')
+    >>> cost_fn = qml.dot(coeffs, qnodes)
+    >>> eta = 0.01
+    >>> init_params = [0.011, 0.012]
+    >>> opt = qml.QNGOptimizer(eta)
+    >>> theta_new = opt.step(cost_fn, init_params, metric_tensor_fn=qnodes.qnodes[0].metric_tensor)
+    >>> print(theta_new)
+    [0.011445239214543481, -0.027519522461477233]
+
     .. seealso::
 
         See the :ref:`quantum natural gradient example <quantum_natural_gradient>`
         for more details on Fubini-Study metric tensor and this optimization class.
 
     Args:
         stepsize (float): the user-defined hyperparameter :math:`\eta`
@@ -103,34 +150,44 @@
 
     def __init__(self, stepsize=0.01, diag_approx=False, lam=0):
         super().__init__(stepsize)
         self.diag_approx = diag_approx
         self.metric_tensor = None
         self.lam = lam
 
-    def step(self, qnode, x, recompute_tensor=True):
+    def step(self, qnode, x, recompute_tensor=True, metric_tensor_fn=None):
         """Update x with one step of the optimizer.
 
         Args:
             qnode (QNode): the QNode for optimization
             x (array): NumPy array containing the current values of the variables to be updated
             recompute_tensor (bool): Whether or not the metric tensor should
                 be recomputed. If not, the metric tensor from the previous
                 optimization step is used.
+            metric_tensor_fn (function): Optional metric tensor function
+                with respect to the variables ``x``.
+                If ``None``, the metric tensor function is computed automatically.
 
         Returns:
             array: the new variable values :math:`x^{(t+1)}`
         """
         # pylint: disable=arguments-differ
-        if not hasattr(qnode, "metric_tensor"):
-            raise ValueError("Objective function must be encoded as a single QNode")
+        if not hasattr(qnode, "metric_tensor") and not metric_tensor_fn:
+            raise ValueError(
+                "The objective function must either be encoded as a single QNode or "
+                "a VQECost object for the natural gradient to be automatically computed. "
+                "Otherwise, metric_tensor_fn must be explicitly provided to the optimizer."
+            )
 
         if recompute_tensor or self.metric_tensor is None:
-            # pseudo-inverse metric tensor
-            self.metric_tensor = qnode.metric_tensor([x], diag_approx=self.diag_approx)
+            if not metric_tensor_fn:
+                # pseudo-inverse metric tensor
+                self.metric_tensor = qnode.metric_tensor([x], diag_approx=self.diag_approx)
+            else:
+                self.metric_tensor = metric_tensor_fn([x], diag_approx=self.diag_approx)
             self.metric_tensor += self.lam * np.identity(self.metric_tensor.shape[0])
 
         g = self.compute_grad(qnode, x)
         x_out = self.apply_grad(g, x)
         return x_out
 
     def apply_grad(self, grad, x):
```

### Comparing `PennyLane-0.8.1/pennylane/optimize/rms_prop.py` & `PennyLane-0.9.0/pennylane/optimize/rms_prop.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Root mean square propagation optimizer"""
-
-import numpy as np
+import math
 
 from pennylane.utils import _flatten, unflatten
 from .adagrad import AdagradOptimizer
 
 
 class RMSPropOptimizer(AdagradOptimizer):
     r"""Root mean squared propagation optimizer.
@@ -70,12 +69,12 @@
         else:
             self.accumulation = [
                 self.decay * a + (1 - self.decay) * g * g
                 for a, g in zip(self.accumulation, grad_flat)
             ]
 
         x_new_flat = [
-            e - (self._stepsize / np.sqrt(a + self.eps)) * g
+            e - (self._stepsize / math.sqrt(a + self.eps)) * g
             for a, g, e in zip(self.accumulation, grad_flat, x_flat)
         ]
 
         return unflatten(x_new_flat, x)
```

### Comparing `PennyLane-0.8.1/pennylane/optimize/__init__.py` & `PennyLane-0.9.0/pennylane/optimize/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 from .adagrad import AdagradOptimizer
 from .adam import AdamOptimizer
 from .gradient_descent import GradientDescentOptimizer
 from .momentum import MomentumOptimizer
 from .nesterov_momentum import NesterovMomentumOptimizer
 from .rms_prop import RMSPropOptimizer
 from .qng import QNGOptimizer
+from .rotosolve import RotosolveOptimizer
+from .rotoselect import RotoselectOptimizer
 
 
 # Optimizers to display in the docs
 __all__ = [
     "AdagradOptimizer",
     "AdamOptimizer",
     "GradientDescentOptimizer",
     "MomentumOptimizer",
     "NesterovMomentumOptimizer",
     "RMSPropOptimizer",
     "QNGOptimizer",
+    "RotosolveOptimizer",
+    "RotoselectOptimizer",
 ]
```

### Comparing `PennyLane-0.8.1/pennylane/plugins/default_gaussian.py` & `PennyLane-0.9.0/pennylane/plugins/default_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 device plugins for new CV backends.
 
 It implements the necessary :class:`~pennylane._device.Device` methods as well as all built-in
 :mod:`continuous-variable Gaussian operations <pennylane.ops.cv>`, and provides a very simple simulation of a
 Gaussian-based quantum circuit architecture.
 """
 # pylint: disable=attribute-defined-outside-init,too-many-arguments
+import math
+import cmath
 import numpy as np
 
 from scipy.special import factorial as fac
 
 import pennylane as qml
 from pennylane import Device
 
@@ -100,15 +102,15 @@
         float: probability of detecting the event
     """
     # number of modes
     N = len(mu) // 2
     I = np.identity(N)
 
     # mean displacement of each mode
-    alpha = (mu[:N] + 1j * mu[N:]) / np.sqrt(2 * hbar)
+    alpha = (mu[:N] + 1j * mu[N:]) / math.sqrt(2 * hbar)
     # the expectation values (<a_1>, <a_2>,...,<a_N>, <a^\dagger_1>, ..., <a^\dagger_N>)
     beta = np.concatenate([alpha, alpha.conj()])
 
     x = cov[:N, :N] * 2 / hbar
     xp = cov[:N, N:] * 2 / hbar
     p = cov[N:, N:] * 2 / hbar
     # the (Hermitian) matrix elements <a_i^\dagger a_j>
@@ -119,17 +121,17 @@
     # calculate the covariance matrix sigma_Q appearing in the Q function:
     # Q(alpha) = exp[-(alpha-beta).sigma_Q^{-1}.(alpha-beta)/2]/|sigma_Q|
     Q = np.block([[aidaj, aiaj.conj()], [aiaj, aidaj.conj()]]) + np.identity(2 * N)
 
     # inverse Q matrix
     Qinv = np.linalg.inv(Q)
     # 1/sqrt(|Q|)
-    sqrt_Qdet = 1 / np.sqrt(np.linalg.det(Q).real)
+    sqrt_Qdet = 1 / math.sqrt(np.linalg.det(Q).real)
 
-    prefactor = np.exp(-beta @ Qinv @ beta.conj() / 2)
+    prefactor = cmath.exp(-beta @ Qinv @ beta.conj() / 2)
 
     if np.all(np.array(event) == 0):
         # all PNRs detect the vacuum state
         return (prefactor * sqrt_Qdet).real / np.prod(fac(event))
 
     # the matrix X_n = [[0, I_n], [I_n, 0]]
     O = np.zeros_like(I)
@@ -165,48 +167,48 @@
 
     Args:
         phi (float): rotation parameter
 
     Returns:
         array: symplectic transformation matrix
     """
-    return np.array([[np.cos(phi), -np.sin(phi)], [np.sin(phi), np.cos(phi)]])
+    return np.array([[math.cos(phi), -math.sin(phi)], [math.sin(phi), math.cos(phi)]])
 
 
 def displacement(state, wire, alpha, hbar=2):
     """Displacement in the phase space.
 
     Args:
         state (tuple): contains means vector and covariance matrix
         wire (int): wire that the displacement acts on
         alpha (float): complex displacement
 
     Returns:
         tuple: contains the vector of means and covariance matrix
     """
     mu = state[0]
-    mu[wire] += alpha.real * np.sqrt(2 * hbar)
-    mu[wire + len(mu) // 2] += alpha.imag * np.sqrt(2 * hbar)
+    mu[wire] += alpha.real * math.sqrt(2 * hbar)
+    mu[wire + len(mu) // 2] += alpha.imag * math.sqrt(2 * hbar)
     return mu, state[1]
 
 
 def squeezing(r, phi):
     """Squeezing in the phase space.
 
     Args:
         r (float): squeezing magnitude
         phi (float): rotation parameter
 
     Returns:
         array: symplectic transformation matrix
     """
-    cp = np.cos(phi)
-    sp = np.sin(phi)
-    ch = np.cosh(r)
-    sh = np.sinh(r)
+    cp = math.cos(phi)
+    sp = math.sin(phi)
+    ch = math.cosh(r)
+    sh = math.sinh(r)
     return np.array([[ch - cp * sh, -sp * sh], [-sp * sh, ch + cp * sh]])
 
 
 def quadratic_phase(s):
     """Quadratic phase shift.
 
     Args:
@@ -224,18 +226,18 @@
     Args:
         theta (float): transmittivity angle (:math:`t=\cos\theta`)
         phi (float): phase angle (:math:`r=e^{i\phi}\sin\theta`)
 
     Returns:
         array: symplectic transformation matrix
     """
-    cp = np.cos(phi)
-    sp = np.sin(phi)
-    ct = np.cos(theta)
-    st = np.sin(theta)
+    cp = math.cos(phi)
+    sp = math.sin(phi)
+    ct = math.cos(theta)
+    st = math.sin(theta)
 
     S = np.array(
         [
             [ct, -cp * st, 0, -st * sp],
             [cp * st, ct, -st * sp, 0],
             [0, st * sp, ct, -cp * st],
             [st * sp, 0, cp * st, ct],
@@ -252,18 +254,18 @@
     Args:
         r (float): squeezing magnitude
         phi (float): rotation parameter
 
     Returns:
         array: symplectic transformation matrix
     """
-    cp = np.cos(phi)
-    sp = np.sin(phi)
-    ch = np.cosh(r)
-    sh = np.sinh(r)
+    cp = math.cos(phi)
+    sp = math.sin(phi)
+    ch = math.cosh(r)
+    sh = math.sinh(r)
 
     S = np.array(
         [
             [ch, cp * sh, 0, sp * sh],
             [cp * sh, ch, sp * sh, 0],
             [0, sp * sh, ch, -cp * sh],
             [sp * sh, 0, -cp * sh, ch],
@@ -331,15 +333,15 @@
         r (float): the squeezing magnitude
         p (float): the squeezing phase :math:`\phi`
         hbar (float): (default 2) the value of :math:`\hbar` in the commutation
             relation :math:`[\x,\p]=i\hbar`
     Returns:
         array: the squeezed state
     """
-    cov = np.array([[np.exp(-2 * r), 0], [0, np.exp(2 * r)]]) * hbar / 2
+    cov = np.array([[math.exp(-2 * r), 0], [0, math.exp(2 * r)]]) * hbar / 2
 
     R = rotation(phi / 2)
 
     return R @ cov @ R.T
 
 
 def vacuum_state(wires, hbar=2.0):
@@ -365,16 +367,16 @@
         a (complex) : the displacement
         phi (float): the phase
         hbar (float): (default 2) the value of :math:`\hbar` in the commutation
             relation :math:`[\x,\p]=i\hbar`
     Returns:
         array: the coherent state
     """
-    alpha = a * np.exp(1j * phi)
-    means = np.array([alpha.real, alpha.imag]) * np.sqrt(2 * hbar)
+    alpha = a * cmath.exp(1j * phi)
+    means = np.array([alpha.real, alpha.imag]) * math.sqrt(2 * hbar)
     cov = np.identity(2) * hbar / 2
     state = [means, cov]
     return state
 
 
 def squeezed_state(r, phi, hbar=2.0):
     r"""Returns a squeezed state.
@@ -403,16 +405,16 @@
         phi_r (float): the squeezing phase :math:`\phi_r`
         hbar (float): (default 2) the value of :math:`\hbar` in the commutation
             relation :math:`[\x,\p]=i\hbar`
 
     Returns:
         array: the squeezed coherent state
     """
-    alpha = a * np.exp(1j * phi_a)
-    means = np.array([alpha.real, alpha.imag]) * np.sqrt(2 * hbar)
+    alpha = a * cmath.exp(1j * phi_a)
+    means = np.array([alpha.real, alpha.imag]) * math.sqrt(2 * hbar)
     state = [means, squeezed_cov(r, phi_r, hbar)]
     return state
 
 
 def thermal_state(nbar, hbar=2.0):
     r"""Returns a thermal state.
 
@@ -647,16 +649,16 @@
         hbar (float): (default 2) the value of :math:`\hbar` in the commutation
             relation :math:`[\x,\p]=i\hbar`
         analytic (bool): indicates if the device should calculate expectations
             and variances analytically
     """
     name = "Default Gaussian PennyLane plugin"
     short_name = "default.gaussian"
-    pennylane_requires = "0.8"
-    version = "0.8.1"
+    pennylane_requires = "0.9"
+    version = "0.9.0"
     author = "Xanadu Inc."
 
     _capabilities = {"model": "cv"}
 
     _operation_map = {
         "Beamsplitter": beamsplitter,
         "ControlledAddition": controlled_addition,
@@ -695,15 +697,15 @@
         self.reset()
 
     def pre_apply(self):
         self.reset()
 
     def apply(self, operation, wires, par):
         if operation == "Displacement":
-            self._state = displacement(self._state, wires[0], par[0] * np.exp(1j * par[1]))
+            self._state = displacement(self._state, wires[0], par[0] * cmath.exp(1j * par[1]))
             return  # we are done here
 
         if operation == "GaussianState":
             if wires != list(range(self.num_wires)):
                 raise ValueError(
                     "GaussianState means vector or covariance matrix is "
                     "the incorrect size for the number of subsystems."
@@ -774,15 +776,15 @@
             mu, cov, wires, par, self.num_wires, hbar=self.hbar
         )
 
         if not self.analytic:
             # estimate the ev
             # use central limit theorem, sample normal distribution once, only ok if n_eval is large
             # (see https://en.wikipedia.org/wiki/Berry%E2%80%93Esseen_theorem)
-            ev = np.random.normal(ev, np.sqrt(var / self.shots))
+            ev = np.random.normal(ev, math.sqrt(var / self.shots))
 
         return ev
 
     def var(self, observable, wires, par):
         mu, cov = self.reduced_state(wires)
         _, var = self._observable_map[observable](
             mu, cov, wires, par, hbar=self.hbar, total_wires=self.num_wires
@@ -822,15 +824,15 @@
 
         mu, cov = self.reduced_state(wires)
         rot = rotation(phi)
 
         muphi = rot.T @ mu
         covphi = rot.T @ cov @ rot
 
-        stdphi = np.sqrt(covphi[0, 0])
+        stdphi = math.sqrt(covphi[0, 0])
         meanphi = muphi[0]
         return np.random.normal(meanphi, stdphi, self.shots)
 
     def reset(self):
         """Reset the device"""
         # init the state vector to |00..0>
         self._state = vacuum_state(self.num_wires, self.hbar)
```

### Comparing `PennyLane-0.8.1/pennylane/plugins/__init__.py` & `PennyLane-0.9.0/pennylane/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/qnodes/base.py` & `PennyLane-0.9.0/pennylane/qnodes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from collections import namedtuple, OrderedDict
 import inspect
 import itertools
 
 import numpy as np
 
 import pennylane as qml
-from pennylane.operation import Observable, CV, Wires, ObservableReturnTypes
+from pennylane.operation import Observable, CV, ActsOn, ObservableReturnTypes
 from pennylane.utils import _flatten, unflatten
 from pennylane.circuit_graph import CircuitGraph, _is_observable
 from pennylane.variable import Variable
 
 
 ParameterDependency = namedtuple("ParameterDependency", ["op", "par_idx"])
 """Represents the dependence of an Operator on a positional parameter of the quantum function.
@@ -94,14 +94,17 @@
     new_ops = []
 
     for op in ops:
         if device.supports_operation(op.name):
             new_ops.append(op)
         else:
             decomposed_ops = op.decomposition(*op.params, wires=op.wires)
+            if op.inverse:
+                decomposed_ops = qml.inv(decomposed_ops)
+
             decomposition = _decompose_queue(decomposed_ops, device)
             new_ops.extend(decomposition)
 
     return new_ops
 
 
 def decompose_queue(ops, device):
@@ -124,15 +127,15 @@
             raise qml.DeviceError(
                 "Gate {} not supported on device {}".format(op.name, device.short_name)
             )
 
     return new_ops
 
 
-class BaseQNode:
+class BaseQNode(qml.QueuingContext):
     """Base class for quantum nodes in the hybrid computational graph.
 
     A *quantum node* encapsulates a :ref:`quantum function <intro_vcirc_qfunc>`
     (corresponding to a :ref:`variational circuit <glossary_variational_circuit>`)
     and the computational device it is executed on.
 
     The QNode calls the quantum function to construct a :class:`.CircuitGraph` instance represeting
@@ -154,35 +157,38 @@
 
     Args:
         func (callable): The *quantum function* of the QNode.
             A Python function containing :class:`~.operation.Operation` constructor calls,
             and returning a tuple of measured :class:`~.operation.Observable` instances.
         device (~pennylane._device.Device): computational device to execute the function on
         mutable (bool): whether the circuit is mutable, see above
-        properties (dict[str, Any] or None): additional keyword properties for adjusting the QNode behavior
+
+    Keyword Args:
+        vis_check (bool): whether to check for operations that cannot affect the output
+        par_check (bool): whether to check for unused positional params
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, func, device, *, mutable=True, properties=None):
+    def __init__(self, func, device, *, mutable=True, **kwargs):
         self.func = func  #: callable: quantum function
         self.device = device  #: Device: device that executes the circuit
         self.num_wires = device.num_wires  #: int: number of subsystems (wires) in the circuit
         #: int: number of flattened differentiable parameters in the circuit
         self.num_variables = None
         self.arg_vars = None
         self.kwarg_vars = None
 
         #: List[Operator]: quantum circuit, in the order the quantum function defines it
         self.ops = []
 
         self.circuit = None  #: CircuitGraph: DAG representation of the quantum circuit
 
         self.mutable = mutable  #: bool: whether the circuit is mutable
-        #: dict[str, Any]: additional keyword properties for adjusting the QNode behavior
-        self.properties = properties or {}
+        #: dict[str, Any]: additional keyword kwargs for adjusting the QNode behavior
+        self.kwargs = kwargs or {}
 
         self.variable_deps = {}
         """dict[int, list[ParameterDependency]]: Mapping from flattened qfunc positional parameter
         index to the list of :class:`~pennylane.operation.Operator` instances (in this circuit)
         that depend on it.
         """
 
@@ -197,30 +203,14 @@
         self.model = self.device.capabilities()["model"]  #: str: circuit type, in {'cv', 'qubit'}
 
     def __repr__(self):
         """String representation."""
         detail = "<QNode: device='{}', func={}, wires={}>"
         return detail.format(self.device.short_name, self.func.__name__, self.num_wires)
 
-    def __enter__(self):
-        """Make this node the current execution context for quantum functions.
-        """
-        if qml._current_context is None:
-            qml._current_context = self
-        else:
-            raise QuantumFunctionError(
-                "qml._current_context must not be modified outside this method."
-            )
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        """Reset the quantum function execution context to None.
-        """
-        qml._current_context = None
-
     def print_applied(self):
         """Prints the most recently applied operations from the QNode.
         """
         if self.circuit is None:
             print("QNode has not yet been executed.")
             return
         self.circuit.print_contents()
@@ -304,56 +294,47 @@
         succ = self.circuit.descendants_in_order((op,))
         if only == "O":
             return list(filter(_is_observable, succ))
         if only == "G":
             return list(itertools.filterfalse(_is_observable, succ))
         return succ
 
-    def _remove_op(self, op):
-        """Remove a quantum operation from the circuit queue.
-
-        Args:
-            op (:class:`~.operation.Operation`): quantum operation to be removed from the circuit
-        """
-        self.queue.remove(op)
-
-    def _append_op(self, op):
-        """Append a quantum operation into the circuit queue.
-
-        Args:
-            op (:class:`~.operation.Operation`): quantum operation to be added to the circuit
+    def _remove_operator(self, operator):
+        if isinstance(operator, Observable) and operator.return_type is not None:
+            self.obs_queue.remove(operator)
+        else:
+            self.queue.remove(operator)
 
-        Raises:
-            ValueError: if `op` does not act on all wires
-            QuantumFunctionError: if state preparations and gates do not precede measured observables
-        """
-        if op.num_wires == Wires.All:
-            if set(op.wires) != set(range(self.num_wires)):
-                raise QuantumFunctionError("Operator {} must act on all wires".format(op.name))
+    def _append_operator(self, operator):
+        if operator.num_wires == ActsOn.AllWires:
+            if set(operator.wires) != set(range(self.num_wires)):
+                raise QuantumFunctionError(
+                    "Operator {} must act on all wires".format(operator.name)
+                )
 
         # Make sure only existing wires are used.
-        for w in _flatten(op.wires):
+        for w in _flatten(operator.wires):
             if w < 0 or w >= self.num_wires:
                 raise QuantumFunctionError(
                     "Operation {} applied to invalid wire {} "
-                    "on device with {} wires.".format(op.name, w, self.num_wires)
+                    "on device with {} wires.".format(operator.name, w, self.num_wires)
                 )
 
         # observables go to their own, temporary queue
-        if isinstance(op, Observable):
-            if op.return_type is None:
-                self.queue.append(op)
+        if isinstance(operator, Observable):
+            if operator.return_type is None:
+                self.queue.append(operator)
             else:
-                self.obs_queue.append(op)
+                self.obs_queue.append(operator)
         else:
             if self.obs_queue:
                 raise QuantumFunctionError(
                     "State preparations and gates must precede measured observables."
                 )
-            self.queue.append(op)  # TODO rename self.queue to self.op_queue
+            self.queue.append(operator)
 
     def _determine_structured_variable_name(self, parameter_value, prefix):
         """Determine the variable names corresponding to a parameter.
 
         This method unrolls the parameter value if it has an array
         or list structure.
 
@@ -494,25 +475,22 @@
 
         Args:
             args (tuple[Any]): Positional arguments passed to the quantum function.
                 During the construction we are not concerned with the numerical values, but with
                 the nesting structure.
                 Each positional argument is replaced with a :class:`~.Variable` instance.
             kwargs (dict[str, Any]): Auxiliary arguments passed to the quantum function.
-
-        Raises:
-            QuantumFunctionError: if :data:`pennylane._current_context` is attempted to be modified
-                inside of this method, the quantum function returns incorrect values or if
-                both continuous and discrete operations are specified in the same quantum circuit
         """
+        # TODO: Update the docstring to reflect the kwargs and the raising conditions
         # pylint: disable=attribute-defined-outside-init, too-many-branches, too-many-statements
 
         self.arg_vars, self.kwarg_vars = self._make_variables(args, kwargs)
 
         # temporary queues for operations and observables
+        # TODO rename self.queue to self.op_queue
         self.queue = []  #: list[Operation]: applied operations
         self.obs_queue = []  #: list[Observable]: applied observables
 
         # set up the context for Operator entry
         with self:
             try:
                 # generate the program queue by executing the quantum circuit function
@@ -545,23 +523,23 @@
                     if not p.is_kwarg:  # ignore auxiliary arguments
                         self.variable_deps[p.idx].append(ParameterDependency(op, j))
 
         # generate the DAG
         self.circuit = CircuitGraph(self.ops, self.variable_deps)
 
         # check for unused positional params
-        if self.properties.get("par_check", False):
+        if self.kwargs.get("par_check", False):
             unused = [k for k, v in self.variable_deps.items() if not v]
             if unused:
                 raise QuantumFunctionError(
                     "The positional parameters {} are unused.".format(unused)
                 )
 
         # check for operations that cannot affect the output
-        if self.properties.get("vis_check", False):
+        if self.kwargs.get("vis_check", False):
             invisible = self.circuit.invisible_operations()
             if invisible:
                 raise QuantumFunctionError(
                     "The operations {} cannot affect the circuit output.".format(invisible)
                 )
 
     @staticmethod
@@ -752,26 +730,30 @@
     def evaluate(self, args, kwargs):
         """Evaluate the quantum function on the specified device.
 
         Args:
             args (tuple[Any]): positional arguments to the quantum function (differentiable)
             kwargs (dict[str, Any]): auxiliary arguments (not differentiable)
 
+        Keyword Args:
+            use_native_type (bool): If True, return the result in whatever type the device uses
+                internally, otherwise convert it into array[float]. Default: False.
+
         Returns:
             float or array[float]: output measured value(s)
         """
         kwargs = self._default_args(kwargs)
         self._set_variables(args, kwargs)
 
         if self.circuit is None or self.mutable:
             self._construct(args, kwargs)
 
         self.device.reset()
 
-        temp = self.properties.get("use_native_type", False)
+        temp = self.kwargs.get("use_native_type", False)
         if isinstance(self.device, qml.QubitDevice):
             # TODO: remove this if statement once all devices are ported to the QubitDevice API
             ret = self.device.execute(self.circuit, return_native_type=temp)
         else:
             ret = self.device.execute(
                 self.circuit.operations,
                 self.circuit.observables,
```

### Comparing `PennyLane-0.8.1/pennylane/qnodes/cv.py` & `PennyLane-0.9.0/pennylane/qnodes/cv.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/qnodes/device_jacobian.py` & `PennyLane-0.9.0/pennylane/qnodes/device_jacobian.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/qnodes/jacobian.py` & `PennyLane-0.9.0/pennylane/qnodes/jacobian.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,33 +19,65 @@
 import numpy as np
 
 from pennylane.operation import ObservableReturnTypes
 from pennylane.utils import _flatten, _inv_dict
 
 from .base import BaseQNode, QuantumFunctionError
 
+DEFAULT_STEP_SIZE = 0.3
+DEFAULT_STEP_SIZE_ANALYTIC = 1e-7
+
 
 class JacobianQNode(BaseQNode):
     """Quantum node that can be differentiated with respect to its positional parameters.
     """
 
-    def __init__(self, func, device, mutable=True, properties=None):
-        super().__init__(func, device, mutable=mutable, properties=properties)
+    def __init__(self, func, device, mutable=True, **kwargs):
+        super().__init__(func, device, mutable=mutable, **kwargs)
 
         self.par_to_grad_method = None
         """dict[int, str]: map from flattened quantum function positional parameter index
         to the gradient method to be used with that parameter"""
 
+        analytic = getattr(self.device, "analytic", False)
+        """bool: whether the device runs in analytic mode; this attribute is
+        not defined for hardware devices so set to False in such cases"""
+
+        default_step_size = DEFAULT_STEP_SIZE_ANALYTIC if analytic else DEFAULT_STEP_SIZE
+        self._h = kwargs.get("h", default_step_size)
+        """float: step size for the finite difference method"""
+
+        self._order = kwargs.get("order", 1)
+        """float: order for the finite difference method"""
+
     metric_tensor = None
 
     @property
     def interface(self):
         """str, None: automatic differentiation interface used by the node, if any"""
         return None
 
+    @property
+    def h(self):
+        """float: step size for the finite difference method"""
+        return self._h
+
+    @h.setter
+    def h(self, value):
+        self._h = value
+
+    @property
+    def order(self):
+        """float: order for the finite difference method"""
+        return self._order
+
+    @order.setter
+    def order(self, value):
+        self._order = value
+
     def __repr__(self):
         """String representation."""
         detail = "<QNode (differentiable): device='{}', func={}, wires={}, interface={}>"
         return detail.format(
             self.device.short_name, self.func.__name__, self.num_wires, self.interface
         )
 
@@ -138,15 +170,19 @@
 
         * Analytic method (``'A'``). Analytic, if implemented by the inheriting QNode.
 
         * Best known method for each parameter (``'best'``): uses the analytic method if
           possible, otherwise finite difference.
 
         * Device method (``'device'``): Delegates the computation of the Jacobian to the
-          device executing the circuit.
+          device executing the circuit. Only supported by devices that provide their
+          own method for computing derivatives; support can be checked by
+          querying the device capabilities: ``dev.capabilities()['provides_jacobian']`` must
+          return ``True``. Examples of supported devices include the experimental
+          :class:`"default.tensor.tf" <~.DefaultTensorTF>` device.
 
         .. note::
            The finite difference method is sensitive to statistical noise in the circuit output,
            since it compares the output at two points infinitesimally close to each other. Hence the
            'F' method requires exact expectation values, i.e., ``analytic=True`` in simulation plugins.
 
         Args:
@@ -170,14 +206,20 @@
         kwargs = kwargs or {}
 
         # apply defaults
         kwargs = self._default_args(kwargs)
 
         options = options or {}
 
+        # Add the step size into the options, if it was not there already
+        if "h" not in options.keys():
+            options = {"h": self.h, **options}
+        if "order" not in options.keys():
+            options = {"order": self._order, **options}
+
         # (re-)construct the circuit if necessary
         if self.circuit is None or self.mutable:
             self._construct(args, kwargs)
 
         returns_samples = [
             str(ob)
             for ob in self.circuit.observables
@@ -290,20 +332,20 @@
             y0 (array[float], None): value of the circuit at the given arguments
             h (float): step size
             order (int): finite difference method order, 1 or 2
 
         Returns:
             array[float]: partial derivative of the node
         """
-        y0 = options.get("y0", None)
-        h = options.get("h", 1e-7)
-        order = options.get("order", 1)
+        h = options.get("h", self.h)
+        order = options.get("order", self.order)
 
         shift_args = args.copy()
         if order == 1:
+            y0 = options.get("y0", None)
             # shift the parameter by h
             shift_args[idx] += h
             y = np.asarray(self.evaluate(shift_args, kwargs))
             return (y - y0) / h
 
         if order == 2:
             # symmetric difference
```

### Comparing `PennyLane-0.8.1/pennylane/qnodes/passthru.py` & `PennyLane-0.9.0/pennylane/qnodes/passthru.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,22 +65,30 @@
     of the simulation are visible in the computational graph.
 
     Args:
         func (callable): The *quantum function* of the QNode.
             A Python function containing :class:`~.operation.Operation` constructor calls,
             and returning a tuple of measured :class:`~.operation.Observable` instances.
         device (~pennylane._device.Device): computational device to execute the function on
-        properties (dict[str, Any] or None): additional keyword properties for adjusting the QNode behavior
+
+    Keyword Args:
+        use_native_type (bool): If True, return the result in whatever type the device uses
+            internally, otherwise convert it into array[float]. Default: True.
     """
 
-    def __init__(self, func, device, properties=None):
+    def __init__(self, func, device, **kwargs):
         # make the device return the result in its native type
-        properties = properties or {}
-        properties.setdefault("use_native_type", True)
-        super().__init__(func, device, mutable=True, properties=properties)
+        kwargs = kwargs or {}
+        kwargs.setdefault("use_native_type", True)
+        kwargs.setdefault("mutable", True)
+
+        if not kwargs.get("mutable"):
+            raise ValueError("PassthruQNode does not support immutable mode.")
+
+        super().__init__(func, device, **kwargs)
 
     def __repr__(self):
         """String representation."""
         detail = "<PassthruQNode: device='{}', func={}, wires={}>"
         return detail.format(self.device.short_name, self.func.__name__, self.num_wires)
 
     def _set_variables(self, args, kwargs):
@@ -94,34 +102,46 @@
         """
         # temporary queues for operations and observables
         self.queue = []  #: list[Operation]: applied operations
         self.obs_queue = []  #: list[Observable]: applied observables
 
         # set up the context for Operator entry
         with self:
+            # use a try/finally block such that if any errors arise during
+            # checking, and the user manually catches the exception, the class
+            # attribute pennylane.operation.Operator.do_check_domain is
+            # properly reset to True
             try:
                 # turn off domain checking since PassthruQNode qfuncs can take any class as input
                 pennylane.operation.Operator.do_check_domain = False
                 # generate the program queue by executing the quantum circuit function
                 res = self.func(*args, **kwargs)
             finally:
                 pennylane.operation.Operator.do_check_domain = True
 
-        # check the validity of the circuit
-        self._check_circuit(res)
+        # use a try/finally block here too
+        try:
+            # check the validity of the circuit
+            # turn off domain checking, but outside of the context such that no
+            # queuing takes place (e.g. from decompositions)
+            pennylane.operation.Operator.do_check_domain = False
+            self._check_circuit(res)
+        finally:
+            pennylane.operation.Operator.do_check_domain = True
+
         del self.queue
         del self.obs_queue
 
         # no output conversion
         self.output_conversion = lambda x: x
 
         # no Variables, self.variable_deps is empty!
         # generate the DAG
         self.circuit = pennylane.circuit_graph.CircuitGraph(self.ops, self.variable_deps)
 
         # check for operations that cannot affect the output
-        if self.properties.get("vis_check", False):
+        if self.kwargs.get("vis_check", False):
             invisible = self.circuit.invisible_operations()
             if invisible:
                 raise QuantumFunctionError(
                     "The operations {} cannot affect the circuit output.".format(invisible)
                 )
```

### Comparing `PennyLane-0.8.1/pennylane/qnodes/qubit.py` & `PennyLane-0.9.0/pennylane/qnodes/qubit.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/qnodes/__init__.py` & `PennyLane-0.9.0/pennylane/qnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/templates/decorator.py` & `PennyLane-0.9.0/pennylane/templates/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         @qml.template
         def bell_state_preparation(wires):
             qml.Hadamard(wires=wires[0])
             qml.CNOT(wires=wires)
 
     This registers the template with PennyLane, making it compatible with
-    functions that act on templates, such as :func:`~.inv`:
+    functions that act on templates, such as :func:`pennylane.inv`:
 
     .. code-block:: python3
 
         dev = qml.device('default.qubit', wires=2)
 
         @qml.qnode(dev)
         def circuit():
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/amplitude.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/amplitude.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
 Contains the ``AmplitudeEmbedding`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
+import math
 import numpy as np
 from pennylane.templates.decorator import template
 from pennylane.ops import QubitStateVector
 from pennylane.templates.utils import (
-    _check_shape,
-    _check_no_variable,
-    _check_wires,
-    _check_type,
-    _get_shape,
+    check_shape,
+    check_no_variable,
+    check_wires,
+    check_type,
+    get_shape,
 )
 from pennylane.variable import Variable
 
 # tolerance for normalization
 TOLERANCE = 1e-10
 
 
@@ -166,45 +167,45 @@
         after other Operations have already been applied on a default.qubit device.
 
     """
 
     #############
     # Input checks
 
-    _check_no_variable(pad, msg="'pad' cannot be differentiable")
-    _check_no_variable(normalize, msg="'normalize' cannot be differentiable")
+    check_no_variable(pad, msg="'pad' cannot be differentiable")
+    check_no_variable(normalize, msg="'normalize' cannot be differentiable")
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     n_amplitudes = 2 ** len(wires)
     expected_shape = (n_amplitudes,)
     if pad is None:
-        shape = _check_shape(
+        shape = check_shape(
             features,
             expected_shape,
             msg="'features' must be of shape {}; got {}. Use the 'pad' "
             "argument for automated padding."
-            "".format(expected_shape, _get_shape(features)),
+            "".format(expected_shape, get_shape(features)),
         )
     else:
-        shape = _check_shape(
+        shape = check_shape(
             features,
             expected_shape,
             bound="max",
             msg="'features' must be of shape {} or smaller "
             "to be padded; got {}"
-            "".format(expected_shape, _get_shape(features)),
+            "".format(expected_shape, get_shape(features)),
         )
 
-    _check_type(
+    check_type(
         pad,
         [float, complex, type(None)],
         msg="'pad' must be a float or complex; got {}".format(pad),
     )
-    _check_type(normalize, [bool], msg="'normalize' must be a boolean; got {}".format(normalize))
+    check_type(normalize, [bool], msg="'normalize' must be a boolean; got {}".format(normalize))
 
     ###############
 
     #############
     # Preprocessing
 
     # pad
@@ -219,15 +220,15 @@
         feature_values = [s.val for s in features]
         norm = np.sum(np.abs(feature_values) ** 2)
     else:
         norm = np.sum(np.abs(features) ** 2)
 
     if not np.isclose(norm, 1.0, atol=TOLERANCE):
         if normalize or pad:
-            features = features / np.sqrt(norm)
+            features = features / math.sqrt(norm)
         else:
             raise ValueError(
                 "'features' must be a vector of length 1.0; got length {}."
                 "Use 'normalization=True' to automatically normalize.".format(norm)
             )
 
     ###############
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/angle.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/angle.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # limitations under the License.
 r"""
 Contains the ``AngleEmbedding`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
 from pennylane.ops import RX, RY, RZ
+from pennylane.templates import broadcast
 from pennylane.templates.utils import (
-    _check_shape,
-    _check_no_variable,
-    _check_wires,
-    _check_is_in_options,
-    _check_type,
-    _get_shape,
+    check_shape,
+    check_no_variable,
+    check_wires,
+    check_is_in_options,
+    check_type,
+    get_shape,
 )
 
 
 @template
 def AngleEmbedding(features, wires, rotation="X"):
     r"""
     Encodes :math:`N` features into the rotation angles of :math:`n` qubits, where :math:`N \leq n`.
@@ -53,37 +54,36 @@
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     #############
     # Input checks
 
-    _check_no_variable(rotation, msg="'rotation' cannot be differentiable")
+    check_no_variable(rotation, msg="'rotation' cannot be differentiable")
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
-    _check_shape(
+    check_shape(
         features,
         (len(wires),),
         bound="max",
         msg="'features' must be of shape {} or smaller; "
-        "got {}.".format((len(wires),), _get_shape(features)),
+        "got {}.".format((len(wires),), get_shape(features)),
     )
-    _check_type(rotation, [str], msg="'rotation' must be a string; got {}".format(rotation))
+    check_type(rotation, [str], msg="'rotation' must be a string; got {}".format(rotation))
 
-    _check_is_in_options(
+    check_is_in_options(
         rotation,
         ["X", "Y", "Z"],
         msg="did not recognize option {} for 'rotation'.".format(rotation),
     )
 
     ###############
 
     if rotation == "X":
-        for f, w in zip(features, wires):
-            RX(f, wires=w)
+        broadcast(unitary=RX, pattern="single", wires=wires, parameters=features)
+
     elif rotation == "Y":
-        for f, w in zip(features, wires):
-            RY(f, wires=w)
+        broadcast(unitary=RY, pattern="single", wires=wires, parameters=features)
+
     elif rotation == "Z":
-        for f, w in zip(features, wires):
-            RZ(f, wires=w)
+        broadcast(unitary=RZ, pattern="single", wires=wires, parameters=features)
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/basis.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/basis.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
 Contains the ``BasisEmbedding`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
-import numpy as np
+from collections import Iterable
 
 from pennylane.templates.decorator import template
-from pennylane.ops import BasisState
-from pennylane.templates.utils import _check_shape, _check_wires, _get_shape
+from pennylane.templates.utils import check_shape, check_wires, get_shape, check_type
+import pennylane as qml
 
 
 @template
 def BasisEmbedding(features, wires):
     r"""Encodes :math:`n` binary features into a basis state of :math:`n` qubits.
 
     For example, for ``features=np.array([0, 1, 0])``, the quantum system will be
@@ -42,24 +42,28 @@
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     #############
     # Input checks
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
+
+    check_type(
+        features, [Iterable], msg="'features' must be iterable; got type {}".format(type(features))
+    )
 
     expected_shape = (len(wires),)
-    _check_shape(
+    check_shape(
         features,
         expected_shape,
-        msg="'features' must be of shape {}; got {}"
-        "".format(expected_shape, _get_shape(features)),
+        msg="'features' must be of shape {}; got {}" "".format(expected_shape, get_shape(features)),
     )
 
     if any([b not in [0, 1] for b in features]):
         raise ValueError("'basis_state' must only consist of 0s and 1s; got {}".format(features))
 
     ###############
 
-    features = np.array(features)
-    BasisState(features, wires=wires)
+    for wire, bit in zip(wires, features):
+        if bit == 1:
+            qml.PauliX(wire)
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/displacement.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/displacement.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # limitations under the License.
 r"""
 Contains the ``DisplacementEmbedding`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
 from pennylane.ops import Displacement
+from pennylane.templates import broadcast
 from pennylane.templates.utils import (
-    _check_shape,
-    _check_no_variable,
-    _check_wires,
-    _check_is_in_options,
-    _get_shape,
+    check_shape,
+    check_no_variable,
+    check_wires,
+    check_is_in_options,
+    get_shape,
 )
 
 
 @template
 def DisplacementEmbedding(features, wires, method="amplitude", c=0.1):
     r"""Encodes :math:`N` features into the displacement amplitudes :math:`r` or phases :math:`\phi` of :math:`M` modes,
      where :math:`N\leq M`.
@@ -52,34 +53,46 @@
     Raises:
         ValueError: if inputs do not have the correct format
    """
 
     #############
     # Input checks
 
-    _check_no_variable(method, msg="'method' cannot be differentiable")
-    _check_no_variable(c, msg="'c' cannot be differentiable")
+    check_no_variable(method, msg="'method' cannot be differentiable")
+    check_no_variable(c, msg="'c' cannot be differentiable")
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     expected_shape = (len(wires),)
-    _check_shape(
+    check_shape(
         features,
         expected_shape,
         bound="max",
         msg="'features' must be of shape {} or smaller; got {}."
-        "".format(expected_shape, _get_shape(features)),
+        "".format(expected_shape, get_shape(features)),
     )
 
-    _check_is_in_options(
+    check_is_in_options(
         method,
         ["amplitude", "phase"],
         msg="did not recognize option {} for 'method'" "".format(method),
     )
 
     #############
 
-    for idx, f in enumerate(features):
-        if method == "amplitude":
-            Displacement(f, c, wires=wires[idx])
-        elif method == "phase":
-            Displacement(c, f, wires=wires[idx])
+    constants = [c] * len(features)
+
+    if method == "amplitude":
+        broadcast(
+            unitary=Displacement,
+            pattern="single",
+            wires=wires,
+            parameters=list(zip(features, constants)),
+        )
+
+    elif method == "phase":
+        broadcast(
+            unitary=Displacement,
+            pattern="single",
+            wires=wires,
+            parameters=list(zip(constants, features)),
+        )
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/qaoa.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/qaoa.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,102 +12,91 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
 Contains the ``QAOAEmbedding`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
-from pennylane.ops import RX, RY, RZ, CNOT, Hadamard
+from pennylane.ops import RX, RY, RZ, MultiRZ, Hadamard
+from pennylane.templates import broadcast
 from pennylane.templates.utils import (
-    _check_shape,
-    _check_wires,
-    _check_is_in_options,
-    _check_number_of_layers,
-    _get_shape,
+    check_shape,
+    check_wires,
+    check_is_in_options,
+    check_number_of_layers,
+    get_shape,
 )
 
 
-def qaoa_feature_encoding_hamiltonian(features, n_features, wires):
+def qaoa_feature_encoding_hamiltonian(features, wires):
     """Implements the encoding Hamiltonian of the QAOA embedding.
 
     Args:
         features (array): array of features to encode
-        n_features (int): number of features to encode
+        wires (list[int]): qubit indices that the template acts on
     """
-    for idx, w in enumerate(wires):
-        # Either feed in feature
-        if idx < n_features:
-            RX(features[idx], wires=w)
-        # or a Hadamard
-        else:
-            Hadamard(wires=w)
 
+    feature_encoding_wires = wires[: len(features)]
+    remaining_wires = wires[len(features) :]
 
-def qaoa_ising_hamiltonian(weights, wires, local_fields, l):
+    broadcast(unitary=RX, pattern="single", wires=feature_encoding_wires, parameters=features)
+    broadcast(unitary=Hadamard, pattern="single", wires=remaining_wires)
+
+
+def qaoa_ising_hamiltonian(weights, wires, local_fields):
     """Implements the Ising-like Hamiltonian of the QAOA embedding.
 
     Args:
-        weights (array): array of weights
-        wires (Sequence[int] or int): `n` qubit indices that the template acts on
+        weights (array): array of weights for one layer
+        wires (list[int]): qubit indices that the template acts on
         local_fields (str): gate implementing the local field
-        l (int): layer index
     """
-    # trainable "Ising" ansatz
+
     if len(wires) == 1:
-        local_fields(weights[l][0], wires=wires[0])
+        weights_zz = []
+        weights_fields = weights
 
     elif len(wires) == 2:
-        # ZZ coupling
-        CNOT(wires=[wires[0], wires[1]])
-        RZ(2 * weights[l][0], wires=wires[0])
-        CNOT(wires=[wires[0], wires[1]])
-
-        # local fields
-        for i, _ in enumerate(wires):
-            local_fields(weights[l][i + 1], wires=wires[i])
+        # for 2 wires the periodic boundary condition is dropped in broadcast's "ring" pattern
+        # only feed in 1 parameter
+        weights_zz = weights[:1]
+        weights_fields = weights[1:]
 
     else:
-        for i, _ in enumerate(wires):
-            if i < len(wires) - 1:
-                # ZZ coupling
-                CNOT(wires=[wires[i], wires[i + 1]])
-                RZ(2 * weights[l][i], wires=wires[i])
-                CNOT(wires=[wires[i], wires[i + 1]])
-            else:
-                # ZZ coupling to enforce periodic boundary condition
-                CNOT(wires=[wires[i], wires[0]])
-                RZ(2 * weights[l][i], wires=wires[i])
-                CNOT(wires=[wires[i], wires[0]])
-        # local fields
-        for i, _ in enumerate(wires):
-            local_fields(weights[l][len(wires) + i], wires=wires[i])
+        weights_zz = weights[: len(wires)]
+        weights_fields = weights[len(wires) :]
+
+    # zz couplings
+    broadcast(unitary=MultiRZ, pattern="ring", wires=wires, parameters=weights_zz)
+    # local fields
+    broadcast(unitary=local_fields, pattern="single", wires=wires, parameters=weights_fields)
 
 
 @template
 def QAOAEmbedding(features, weights, wires, local_field="Y"):
     r"""
     Encodes :math:`N` features into :math:`n>N` qubits, using a layered, trainable quantum
     circuit that is inspired by the QAOA ansatz.
 
     A single layer applies two circuits or "Hamiltonians": The first encodes the features, and the second is
     a variational ansatz inspired by a 1-dimensional Ising model. The feature-encoding circuit associates features with
     the angles of :class:`RX` rotations. The Ising ansatz consists of trainable two-qubit ZZ interactions
-    :math:`e^{-i \alpha \sigma_z \otimes \sigma_z}`,
+    :math:`e^{-i \frac{\alpha}{2} \sigma_z \otimes \sigma_z}` (in PennyLane represented by the :class:`~.MultiRZ` gate),
     and trainable local fields :math:`e^{-i \frac{\beta}{2} \sigma_{\mu}}`, where :math:`\sigma_{\mu}`
     can be chosen to be :math:`\sigma_{x}`, :math:`\sigma_{y}` or :math:`\sigma_{z}`
     (default choice is :math:`\sigma_{y}` or the ``RY`` gate), and :math:`\alpha, \beta` are adjustable gate parameters.
 
     The number of features has to be smaller or equal to the number of qubits. If there are fewer features than
     qubits, the feature-encoding rotation is replaced by a Hadamard gate.
 
     The argument ``weights`` contains an array of the :math:`\alpha, \beta` parameters for each layer.
     The number of layers :math:`L` is derived from the first dimension of ``weights``, which has the following
     shape:
 
-    * :math:`(L, )`, if the embedding acts on a single wire,
+    * :math:`(L, 1)`, if the embedding acts on a single wire,
     * :math:`(L, 3)`, if the embedding acts on two wires,
     * :math:`(L, 2n)` else.
 
     After the :math:`L` th layer, another set of feature-encoding :class:`RX` gates is applied.
 
     This is an example for the full embedding circuit using 2 layers, 3 features, 4 wires, and ``RY`` local fields:
 
@@ -221,69 +210,67 @@
         Choosing ``'Z'`` fields implements a QAOAEmbedding where the second Hamiltonian is a
         1-dimensional Ising model.
 
     """
     #############
     # Input checks
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     expected_shape = (len(wires),)
-    _check_shape(
+    check_shape(
         features,
         expected_shape,
         bound="max",
         msg="'features' must be of shape {} or smaller; got {}"
-        "".format((len(wires),), _get_shape(features)),
+        "".format((len(wires),), get_shape(features)),
     )
 
-    _check_is_in_options(
+    check_is_in_options(
         local_field,
         ["X", "Y", "Z"],
         msg="did not recognize option {} for 'local_field'" "".format(local_field),
     )
 
-    repeat = _check_number_of_layers([weights])
+    repeat = check_number_of_layers([weights])
 
     if len(wires) == 1:
         expected_shape = (repeat, 1)
-        _check_shape(
+        check_shape(
             weights,
             expected_shape,
             msg="'weights' must be of shape {}; got {}"
-            "".format(expected_shape, _get_shape(features)),
+            "".format(expected_shape, get_shape(features)),
         )
     elif len(wires) == 2:
         expected_shape = (repeat, 3)
-        _check_shape(
+        check_shape(
             weights,
             expected_shape,
             msg="'weights' must be of shape {}; got {}"
-            "".format(expected_shape, _get_shape(features)),
+            "".format(expected_shape, get_shape(features)),
         )
     else:
         expected_shape = (repeat, 2 * len(wires))
-        _check_shape(
+        check_shape(
             weights,
             expected_shape,
             msg="'weights' must be of shape {}; got {}"
-            "".format(expected_shape, _get_shape(features)),
+            "".format(expected_shape, get_shape(features)),
         )
 
     #####################
 
-    n_features = _get_shape(features)[0]
-
     if local_field == "Z":
         local_fields = RZ
     elif local_field == "X":
         local_fields = RX
     else:
         local_fields = RY
 
     for l in range(repeat):
         # apply alternating Hamiltonians
-        qaoa_feature_encoding_hamiltonian(features, n_features, wires)
-        qaoa_ising_hamiltonian(weights, wires, local_fields, l)
+        qaoa_feature_encoding_hamiltonian(features, wires)
+        qaoa_ising_hamiltonian(weights[l], wires, local_fields)
 
     # repeat the feature encoding once more at the end
-    qaoa_feature_encoding_hamiltonian(features, n_features, wires)
+    qaoa_feature_encoding_hamiltonian(features, wires)
```

### Comparing `PennyLane-0.8.1/pennylane/templates/embeddings/__init__.py` & `PennyLane-0.9.0/pennylane/templates/embeddings/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 used at the beginning of a circuit.
 """
 
 from .angle import AngleEmbedding
 from .amplitude import AmplitudeEmbedding
 from .basis import BasisEmbedding
 from .displacement import DisplacementEmbedding
+from .iqp import IQPEmbedding
 from .qaoa import QAOAEmbedding
 from .squeezing import SqueezingEmbedding
```

### Comparing `PennyLane-0.8.1/pennylane/templates/layers/cv_neural_net.py` & `PennyLane-0.9.0/pennylane/templates/layers/cv_neural_net.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 r"""
 Contains the ``CVNeuralNetLayers`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
 from pennylane.ops import Squeezing, Displacement, Kerr
 from pennylane.templates.subroutines import Interferometer
-from pennylane.templates.utils import _check_wires, _check_number_of_layers, _check_shapes
+from pennylane.templates import broadcast
+from pennylane.templates.utils import check_wires, check_number_of_layers, check_shapes
 
 
 def cv_neural_net_layer(
     theta_1, phi_1, varphi_1, r, phi_r, theta_2, phi_2, varphi_2, a, phi_a, k, wires
 ):
     r"""A single continuous-variable neural network layer.
 
@@ -44,24 +45,22 @@
             :class:`~pennylane.ops.Displacement` operations
         phi_a (array[float]): length :math:`(M, )` array of displacement angles for
             :class:`~pennylane.ops.Displacement` operations
         k (array[float]): length :math:`(M, )` array of kerr parameters for :class:`~pennylane.ops.Kerr` operations
         wires (Sequence[int]): sequence of mode indices that the template acts on
     """
     Interferometer(theta=theta_1, phi=phi_1, varphi=varphi_1, wires=wires)
-    for i, wire in enumerate(wires):
-        Squeezing(r[i], phi_r[i], wires=wire)
+
+    broadcast(unitary=Squeezing, pattern="single", wires=wires, parameters=list(zip(r, phi_r)))
 
     Interferometer(theta=theta_2, phi=phi_2, varphi=varphi_2, wires=wires)
 
-    for i, wire in enumerate(wires):
-        Displacement(a[i], phi_a[i], wires=wire)
+    broadcast(unitary=Displacement, pattern="single", wires=wires, parameters=list(zip(a, phi_a)))
 
-    for i, wire in enumerate(wires):
-        Kerr(k[i], wires=wire)
+    broadcast(unitary=Kerr, pattern="single", wires=wires, parameters=k)
 
 
 @template
 def CVNeuralNetLayers(
     theta_1, phi_1, varphi_1, r, phi_r, theta_2, phi_2, varphi_2, a, phi_a, k, wires
 ):
     r"""A sequence of layers of a continuous-variable quantum neural network,
@@ -108,35 +107,35 @@
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     #############
     # Input checks
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     n_wires = len(wires)
     n_if = n_wires * (n_wires - 1) // 2
     weights_list = [theta_1, phi_1, varphi_1, r, phi_r, theta_2, phi_2, varphi_2, a, phi_a, k]
-    repeat = _check_number_of_layers(weights_list)
+    repeat = check_number_of_layers(weights_list)
 
     expected_shapes = [
         (repeat, n_if),
         (repeat, n_if),
         (repeat, n_wires),
         (repeat, n_wires),
         (repeat, n_wires),
         (repeat, n_if),
         (repeat, n_if),
         (repeat, n_wires),
         (repeat, n_wires),
         (repeat, n_wires),
         (repeat, n_wires),
     ]
-    _check_shapes(weights_list, expected_shapes, msg="wrong shape of weight input(s) detected")
+    check_shapes(weights_list, expected_shapes, msg="wrong shape of weight input(s) detected")
 
     ###############
 
     for l in range(repeat):
         cv_neural_net_layer(
             theta_1=theta_1[l],
             phi_1=phi_1[l],
```

### Comparing `PennyLane-0.8.1/pennylane/templates/layers/strongly_entangling.py` & `PennyLane-0.9.0/pennylane/templates/layers/basic_entangler.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,118 +8,154 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
-Contains the ``StronglyEntanglingLayers`` template.
+Contains the ``BasicEntanglerLayers`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
-from pennylane.ops import CNOT, Rot
+from pennylane.ops import CNOT, RX
+from pennylane.templates import broadcast
 from pennylane.templates.utils import (
-    _check_shape,
-    _check_no_variable,
-    _check_wires,
-    _check_type,
-    _check_number_of_layers,
-    _get_shape,
+    check_shape,
+    check_no_variable,
+    check_wires,
+    check_number_of_layers,
+    get_shape,
 )
 
 
-def strongly_entangling_layer(weights, wires, r, imprimitive):
-    r"""A layer applying rotations on each qubit followed by cascades of 2-qubit entangling gates.
+@template
+def BasicEntanglerLayers(weights, wires, rotation=None):
+    r"""Layers consisting of one-parameter single-qubit rotations on each qubit, followed by a closed chain
+    or *ring* of CNOT gates.
+
+    The ring of CNOT gates connects every qubit with its neighbour,
+    with the last qubit being considered as a neighbour to the first qubit.
+
+    .. figure:: ../../_static/templates/layers/basic_entangler.png
+        :align: center
+        :width: 40%
+        :target: javascript:void(0);
+
+    The number of layers :math:`L` is determined by the first dimension of the argument ``weights``.
+    When using a single wire, the template only applies the single
+    qubit gates in each layer.
+
+    .. note::
+
+        This template follows the convention of dropping the entanglement between the last and the first
+        qubit when using only two wires, so the entangler is not repeated on the same wires.
+        In this case, only one CNOT gate is applied in each layer:
+
+        .. figure:: ../../_static/templates/layers/basic_entangler_2wires.png
+            :align: center
+            :width: 30%
+            :target: javascript:void(0);
 
     Args:
-        weights (array[float]): array of weights of shape ``(len(wires), 3)``
-        wires (Sequence[int]): sequence of qubit indices that the template acts on
-        r (int): range of the imprimitive gates of this layer, defaults to 1
-        imprimitive (pennylane.ops.Operation): two-qubit gate to use, defaults to :class:`~pennylane.ops.CNOT`
-    """
+        weights (array[float]): array of weights with shape ``(L, len(wires))``, each weight is used as a parameter
+                                for the rotation
+        wires (Sequence[int] or int): qubit indices that the template acts on
+        rotation (pennylane.ops.Operation): one-parameter single-qubit gate to use,
+                                            if ``None``, :class:`~pennylane.ops.RX` is used as default
+    Raises:
+        ValueError: if inputs do not have the correct format
 
-    for i, wire in enumerate(wires):
-        Rot(weights[i, 0], weights[i, 1], weights[i, 2], wires=wire)
+    .. UsageDetails::
 
-    n_wires = len(wires)
-    if n_wires > 1:
-        for i in range(n_wires):
-            imprimitive(wires=[wires[i], wires[(i + r) % n_wires]])
+        The template is used inside a qnode:
 
+        .. code-block:: python
 
-@template
-def StronglyEntanglingLayers(weights, wires, ranges=None, imprimitive=CNOT):
-    r"""Layers consisting of single qubit rotations and entanglers, inspired by the circuit-centric classifier design
-    `arXiv:1804.00633 <https://arxiv.org/abs/1804.00633>`_.
-
-    The argument ``weights`` contains the weights for each layer. The number of layers :math:`L` is therefore derived
-    from the first dimension of ``weights``.
-
-    The 2-qubit gates, whose type is specified by the ``imprimitive`` argument,
-    act chronologically on the :math:`M` wires, :math:`i = 1,...,M`. The second qubit of each gate is given by
-    :math:`(i+r)\mod M`, where :math:`r` is a  hyperparameter called the *range*, and :math:`0 < r < M`.
-    If applied to one qubit only, this template will use no imprimitive gates.
+            import pennylane as qml
+            from pennylane.templates import BasicEntanglerLayers
+            from math import pi
 
-    This is an example of two 4-qubit strongly entangling layers (ranges :math:`r=1` and :math:`r=2`, respectively) with
-    rotations :math:`R` and CNOTs as imprimitives:
+            n_wires = 3
+            dev = qml.device('default.qubit', wires=n_wires)
 
-    .. figure:: ../../_static/layer_sec.png
-        :align: center
-        :width: 60%
-        :target: javascript:void(0);
+            @qml.qnode(dev)
+            def circuit(weights):
+                BasicEntanglerLayers(weights=weights, wires=range(n_wires))
+                return [qml.expval(qml.PauliZ(wires=i)) for i in range(n_wires)]
 
-    Args:
+        >>> circuit([[pi, pi, pi]])
+        [1., 1., -1.]
 
-        weights (array[float]): array of weights of shape ``(:math:`L`, :math:`M`, 3)``
-        wires (Sequence[int] or int): qubit indices that the template acts on
-        ranges (Sequence[int]): sequence determining the range hyperparameter for each subsequent layer; if None
-                                using :math:`r=l \mod M` for the :math:`l`th layer and :math:`M` wires.
-        imprimitive (pennylane.ops.Operation): two-qubit gate to use, defaults to :class:`~pennylane.ops.CNOT`
+        **Parameter initialization function**
 
-    Raises:
-        ValueError: if inputs do not have the correct format
+        The :mod:`~pennylane.init` module has two parameter initialization functions, ``basic_entangler_layers_normal``
+        and ``basic_entangler_layers_uniform``.
+
+        .. code-block:: python
+
+            from pennylane.init import basic_entangler_layers_normal
+
+            n_layers = 4
+            weights = basic_entangler_layers_normal(n_layers=n_layers, n_wires=n_wires)
+
+            circuit(weights)
+
+
+        **No periodic boundary for two wires**
+
+        When using two wires, the convention is to drop the periodic boundary condition.
+        This means that the connection from the second to the first wire is omitted.
+
+        .. code-block:: python
+
+            n_wires = 2
+            dev = qml.device('default.qubit', wires=n_wires)
+
+            @qml.qnode(dev)
+            def circuit(weights):
+                BasicEntanglerLayers(weights=weights, wires=range(n_wires))
+                return [qml.expval(qml.PauliZ(wires=i)) for i in range(n_wires)]
+
+        >>> circuit([[pi, pi]])
+        [-1, 1]
+
+
+        **Changing the rotation gate**
+
+        Any single-qubit gate can be used as a rotation gate, as long as it only takes a single parameter. The default is the ``RX`` gate.
+
+        .. code-block:: python
+
+            @qml.qnode(dev)
+            def circuit(weights):
+                BasicEntanglerLayers(weights=weights, wires=range(n_wires), rotation=qml.RZ)
+                return [qml.expval(qml.PauliZ(wires=i)) for i in range(n_wires)]
+
+        Accidentally using a gate that expects more parameters throws a
+        ``ValueError: Wrong number of parameters``.
     """
 
     #############
     # Input checks
 
-    _check_no_variable(ranges, msg="'ranges' cannot be differentiable")
-    _check_no_variable(imprimitive, msg="'imprimitive' cannot be differentiable")
+    if rotation is None:
+        rotation = RX
 
-    wires = _check_wires(wires)
+    check_no_variable(rotation, msg="'rotation' cannot be differentiable")
 
-    repeat = _check_number_of_layers([weights])
+    wires = check_wires(wires)
 
-    expected_shape = (repeat, len(wires), 3)
-    _check_shape(
-        weights,
-        expected_shape,
-        msg="'weights' must be of shape {}; got {}" "".format(expected_shape, _get_shape(weights)),
-    )
+    repeat = check_number_of_layers([weights])
 
-    if ranges is None:
-        # tile ranges with iterations of range(1, n_wires)
-        ranges = [(l % (len(wires) - 1)) + 1 for l in range(repeat)]
-
-    expected_shape = (repeat,)
-    _check_shape(
-        ranges,
+    expected_shape = (repeat, len(wires))
+    check_shape(
+        weights,
         expected_shape,
-        msg="'ranges' must be of shape {}; got {}" "".format(expected_shape, _get_shape(weights)),
+        msg="'weights' must be of shape {}; got {}" "".format(expected_shape, get_shape(weights)),
     )
 
-    _check_type(ranges, [list], msg="'ranges' must be a list; got {}" "".format(ranges))
-    for r in ranges:
-        _check_type(r, [int], msg="'ranges' must be a list of integers; got {}" "".format(ranges))
-    if any((r >= len(wires) or r == 0) for r in ranges):
-        raise ValueError(
-            "the range for all layers needs to be smaller than the number of "
-            "qubits; got ranges {}.".format(ranges)
-        )
-
     ###############
 
-    for l in range(repeat):
+    for layer in range(repeat):
 
-        strongly_entangling_layer(
-            weights=weights[l], wires=wires, r=ranges[l], imprimitive=imprimitive
-        )
+        broadcast(unitary=rotation, pattern="single", wires=wires, parameters=weights[layer])
+        broadcast(unitary=CNOT, pattern="ring", wires=wires)
```

### Comparing `PennyLane-0.8.1/pennylane/templates/layers/__init__.py` & `PennyLane-0.9.0/pennylane/templates/layers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 Layers are trainable templates that are typically repeated, using different adjustable parameters in each repetition.
 They implement a transformation from a quantum state to another quantum state.
 """
 
 from .strongly_entangling import StronglyEntanglingLayers
 from .random import RandomLayers
 from .cv_neural_net import CVNeuralNetLayers
+from .simplified_two_design import SimplifiedTwoDesign
+from .basic_entangler import BasicEntanglerLayers
```

### Comparing `PennyLane-0.8.1/pennylane/templates/state_preparations/basis.py` & `PennyLane-0.9.0/pennylane/templates/state_preparations/basis.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 r"""
 Contains the ``BasisStatePreparation`` template.
 """
 
 import pennylane as qml
 
 from pennylane.templates.decorator import template
-from pennylane.templates.utils import _check_wires, _check_no_variable, _check_shape, _get_shape
+from pennylane.templates.utils import check_wires, check_no_variable, check_shape, get_shape
 
 
 @template
 def BasisStatePreparation(basis_state, wires):
     r"""
     Prepares a basis state on the given wires using a sequence of Pauli X gates.
 
@@ -41,26 +41,26 @@
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     ######################
     # Input checks
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     expected_shape = (len(wires),)
-    _check_shape(
+    check_shape(
         basis_state,
         expected_shape,
         msg=" 'basis_state' must be of shape {}; got {}."
-        "".format(expected_shape, _get_shape(basis_state)),
+        "".format(expected_shape, get_shape(basis_state)),
     )
 
     # basis_state cannot be trainable
-    _check_no_variable(
+    check_no_variable(
         basis_state,
         msg="'basis_state' cannot be differentiable; must be passed as a keyword argument "
         "to the quantum node",
     )
 
     # basis_state is guaranteed to be a list of binary values
     if any([b not in [0, 1] for b in basis_state]):
```

### Comparing `PennyLane-0.8.1/pennylane/templates/state_preparations/mottonen.py` & `PennyLane-0.9.0/pennylane/templates/state_preparations/mottonen.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import math
 import numpy as np
 from scipy import sparse
 
 import pennylane as qml
 
 from pennylane.templates.decorator import template
-from pennylane.templates.utils import _check_wires, _check_shape, _get_shape
+from pennylane.templates.utils import check_wires, check_shape, get_shape
 from pennylane.variable import Variable
 
 
 # pylint: disable=len-as-condition,arguments-out-of-order
 def gray_code(rank):
     """Generates the Gray code of given rank.
 
@@ -202,17 +202,17 @@
         is_part_numerator = 1 <= l <= 2 ** (k - 1)
 
         if is_part_numerator:
             numerator[j - 1, 0] += e * e
         denominator[j - 1, 0] += e * e
 
     for (j, _), e in numerator.items():
-        numerator[j, 0] = np.sqrt(e)
+        numerator[j, 0] = math.sqrt(e)
     for (j, _), e in denominator.items():
-        denominator[j, 0] = 1 / np.sqrt(e)
+        denominator[j, 0] = 1 / math.sqrt(e)
 
     pre_alpha = numerator.multiply(denominator)  # type: sparse.csr_matrix
     for (j, _), e in pre_alpha.todok().items():
         alpha[j, 0] = 2 * np.arcsin(e)
 
     return alpha
 
@@ -242,23 +242,23 @@
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     ###############
     # Input checks
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     n_wires = len(wires)
     expected_shape = (2 ** n_wires,)
-    _check_shape(
+    check_shape(
         state_vector,
         expected_shape,
         msg="'state_vector' must be of shape {}; got {}."
-        "".format(expected_shape, _get_shape(state_vector)),
+        "".format(expected_shape, get_shape(state_vector)),
     )
 
     # check if state_vector is normalized
     if isinstance(state_vector[0], Variable):
         state_vector_values = [s.val for s in state_vector]
         norm = np.sum(np.abs(state_vector_values) ** 2)
     else:
```

### Comparing `PennyLane-0.8.1/pennylane/templates/state_preparations/__init__.py` & `PennyLane-0.9.0/pennylane/templates/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-r"""
-State preperations are templates that prepare a given quantum state,
-by decomposing it into elementary operations.
+"""
+This module contains templates, which are pre-coded routines that can be used in a quantum node.
 """
 
-from .mottonen import MottonenStatePreparation
-from .basis import BasisStatePreparation
+from .broadcast import *
+from .decorator import *
+from .layers import *
+from .embeddings import *
+from .subroutines import *
+from .state_preparations import *
```

### Comparing `PennyLane-0.8.1/pennylane/templates/subroutines/interferometer.py` & `PennyLane-0.9.0/pennylane/templates/subroutines/interferometer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 r"""
 Contains the ``Interferometer`` template.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from pennylane.templates.decorator import template
 from pennylane.ops import Beamsplitter, Rotation
 from pennylane.templates.utils import (
-    _check_shapes,
-    _check_no_variable,
-    _check_wires,
-    _check_is_in_options,
+    check_shapes,
+    check_no_variable,
+    check_wires,
+    check_is_in_options,
 )
 
 
 @template
 def Interferometer(theta, phi, varphi, wires, mesh="rectangular", beamsplitter="pennylane"):
     r"""General linear interferometer, an array of beamsplitters and phase shifters.
 
@@ -103,31 +103,31 @@
 
     Raises:
         ValueError: if inputs do not have the correct format
     """
 
     #############
     # Input checks
-    _check_no_variable(beamsplitter, msg="'beamsplitter' cannot be differentiable")
-    _check_no_variable(mesh, msg="'mesh' cannot be differentiable")
+    check_no_variable(beamsplitter, msg="'beamsplitter' cannot be differentiable")
+    check_no_variable(mesh, msg="'mesh' cannot be differentiable")
 
-    wires = _check_wires(wires)
+    wires = check_wires(wires)
 
     weights_list = [theta, phi, varphi]
     n_wires = len(wires)
     n_if = n_wires * (n_wires - 1) // 2
     expected_shapes = [(n_if,), (n_if,), (n_wires,)]
-    _check_shapes(weights_list, expected_shapes, msg="wrong shape of weight input(s) detected")
+    check_shapes(weights_list, expected_shapes, msg="wrong shape of weight input(s) detected")
 
-    _check_is_in_options(
+    check_is_in_options(
         beamsplitter,
         ["clements", "pennylane"],
         msg="did not recognize option {} for 'beamsplitter'" "".format(beamsplitter),
     )
-    _check_is_in_options(
+    check_is_in_options(
         mesh,
         ["triangular", "rectangular"],
         msg="did not recognize option {} for 'mesh'" "".format(mesh),
     )
     ###############
 
     M = len(wires)
```

### Comparing `PennyLane-0.8.1/pennylane/templates/subroutines/__init__.py` & `PennyLane-0.9.0/pennylane/templates/subroutines/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 # limitations under the License.
 r"""
 Subroutines are the most basic template, consisting of a collection of quantum operations, and not fulfilling
 any of the characteristics of other templates (i.e. to prepare a specific state, to be repeated or to encode features).
 """
 
 from .interferometer import Interferometer
+from .arbitrary_unitary import ArbitraryUnitary
```

### Comparing `PennyLane-0.8.1/pennylane/templates/utils.py` & `PennyLane-0.9.0/pennylane/templates/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,48 +8,50 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
-Utility functions used in the templates.
+Utility functions provided for the templates. These are useful for standard input checks,
+for example to make sure that arguments have the right shape, range or type.
 """
 # pylint: disable-msg=too-many-branches,too-many-arguments,protected-access
 from collections.abc import Iterable
 
 import numpy as np
 from pennylane.variable import Variable
 
 
-def _check_no_variable(arg, msg):
-    """Checks that `arg` does not represent or contain a :func:`~.pennylane.Variable` object.
+def check_no_variable(arg, msg):
+    """Checks that ``arg`` does not represent or contain a :func:`~.pennylane.Variable` object.
 
-    This ensures that the user has not passed `arg` to the qnode as a
-    positional argument.
+    This ensures that the user has not passed ``arg`` to the qnode as a
+    primary argument.
 
     Args:
         arg: argument to check
         msg (str): error message to display
     """
 
     if isinstance(arg, Variable):
         raise ValueError(msg)
 
     if isinstance(arg, Iterable):
         if any([isinstance(a_, Variable) for a_ in arg]):
             raise ValueError(msg)
 
 
-def _check_wires(wires):
-    """Standard checks for the wires argument.
+def check_wires(wires):
+    """Checks that ``wires`` is either a non-negative integer or a list of non-negative integers.
+
+    If ``wires`` is an integer, wrap it by a list.
 
     Args:
-        wires (int or list): (subset of) wires of a quantum node, a list of positive integers
-                             or a single positive integer
+        wires (int or list[int]): (subset of) wires of a quantum node
 
     Return:
         list: list of wire indices
 
     Raises:
         ValueError: if the wires argument is invalid
     """
@@ -64,24 +66,25 @@
     if not all([isinstance(w, int) for w in wires]):
         raise ValueError(msg)
     if any([w < 0 for w in wires]):
         raise ValueError(msg)
     return wires
 
 
-def _get_shape(inpt):
-    """Turn ``inpt`` to an array and return its shape.
+def get_shape(inpt):
+    """Turn ``inpt`` into an array and return its shape.
 
     Args:
-        inpt (list): input to a qnode
+        inpt (scalar, list or array): input to a qnode
 
     Returns:
         tuple: shape of ``inpt``
     """
 
+    # avoids incorrect assignment of shape
     if isinstance(inpt, (float, int, complex)):
         shape = ()
 
     else:
         # turn lists into array to get shape
         if isinstance(inpt, list):
             inpt = np.array(inpt)
@@ -93,45 +96,45 @@
 
         # turn result into tuple to avoid type TensorShape
         shape = tuple(shape)
 
     return shape
 
 
-def _check_shape(inpt, target_shape, msg, bound=None):
-    """Checks that the shape of ``inpt`` is equal to the target shape.
+def check_shape(inpt, target_shape, msg, bound=None):
+    """Check that the shape of ``inpt`` is equal to ``target_shape``.
 
     Args:
         inpt (list): input to a qnode
         target_shape (tuple[int]): expected shape of inpt
         msg (str): error message to display if the shapes are different
         bound (str): If 'max' or 'min', the target shape is merely required to be a bound on the input shape
 
     Raises:
         ValueError
     """
 
-    shape = _get_shape(inpt)
+    shape = get_shape(inpt)
 
     if bound == "max":
         if shape > target_shape:
             raise ValueError(msg)
     elif bound == "min":
         if shape < target_shape:
             raise ValueError(msg)
     else:
         if shape != target_shape:
             raise ValueError(msg)
 
     return shape
 
 
-def _check_shapes(inpt_list, target_shapes, msg, bounds=None):
-    """Checks that the shape of elements in the ``inpt`` list are equal to the shapes of elements
-    in the ``target shape`` list.
+def check_shapes(inpt_list, target_shapes, msg, bounds=None):
+    """Check that the shape of elements in the ``inpt`` list are equal to the shapes of elements
+    in the ``target_shapes`` list.
 
     Args:
         inpt_list (list): list of elements of which to check the shape
         target_shapes (list): list of target shapes, of same length as ``inpt_list``
         msg (str): error message to display
         bounds (list): list of 'max' or 'min', indicating the bound that the target shape imposes on the input
             shape
@@ -140,60 +143,59 @@
         ValueError
     """
 
     if bounds is None:
         bounds = [None] * len(inpt_list)
 
     shape_list = [
-        _check_shape(l, t, bound=b, msg=msg) for l, t, b in zip(inpt_list, target_shapes, bounds)
+        check_shape(l, t, bound=b, msg=msg) for l, t, b in zip(inpt_list, target_shapes, bounds)
     ]
     return shape_list
 
 
-def _check_is_in_options(element, options, msg):
-    """Checks that the value of ``element`` is in ``options``.
+def check_is_in_options(element, options, msg):
+    """Check that the value of ``element`` is in ``options``.
 
     Args:
         element: arbitraty variable
         options: possible options for ``element``
         msg (str): error message to display
     """
 
     if element not in options:
         raise ValueError(msg)
 
 
-def _check_type(element, types, msg):
-    """Checks that the type of ``element'' is one of ``types``.
+def check_type(element, types, msg):
+    """Check that the type of ``element`` is one of ``types``.
 
     Args:
         element: variable to check
         types (list): possible types for ``element``
          msg (str): error message to display
     """
 
     if not any([isinstance(element, t) for t in types]):
         raise ValueError(msg)
 
 
-def _check_number_of_layers(list_of_weights):
-    """Checks that all weights in ``list_of_weights`` have the same first dimension, which is interpreted
-    as the number of layers.
+def check_number_of_layers(list_of_weights):
+    """Check that all sequences in ``list_of_weights`` have the same first dimension.
 
     Args:
         list_of_weights (list): list of all weights to the template
 
     Returns:
         int: number of layers
 
     Raises:
         ValueError
     """
 
-    shapes = [_get_shape(weight) for weight in list_of_weights]
+    shapes = [get_shape(weight) for weight in list_of_weights]
 
     if any(len(s) == 0 for s in shapes):
         raise ValueError(
             "the first dimension of the weight parameters must be the number of layers in the "
             "template; got scalar weights."
         )
```

### Comparing `PennyLane-0.8.1/pennylane/templates/__init__.py` & `PennyLane-0.9.0/pennylane/templates/state_preparations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-This module contains templates, which are pre-coded routines that can be used in a quantum node.
+r"""
+State preperations are templates that prepare a given quantum state,
+by decomposing it into elementary operations.
 """
 
-from .decorator import *
-from .layers import *
-from .embeddings import *
-from .subroutines import *
-from .state_preparations import *
+from .mottonen import MottonenStatePreparation
+from .basis import BasisStatePreparation
+from .arbitrary_state_preparation import ArbitraryStatePreparation
```

### Comparing `PennyLane-0.8.1/pennylane/utils.py` & `PennyLane-0.9.0/pennylane/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # pylint: disable=protected-access
 from collections.abc import Iterable
 from collections import OrderedDict
 import copy
 import numbers
 import functools
 import inspect
-import itertools
 
 import numpy as np
 
 import pennylane as qml
 from pennylane.variable import Variable
 
 
@@ -132,64 +131,14 @@
     return {
         k: (idx, v.default)
         for idx, (k, v) in enumerate(signature.parameters.items())
         if v.default is not inspect.Parameter.empty
     }
 
 
-def expand(U, wires, num_wires):
-    r"""Expand a multi-qubit operator into a full system operator.
-
-    Args:
-        U (array): :math:`2^n \times 2^n` matrix where n = len(wires).
-        wires (Sequence[int]): Target subsystems (order matters! the
-            left-most Hilbert space is at index 0).
-
-    Raises:
-        ValueError: if wrong wires of the system were targeted or
-            the size of the unitary is incorrect
-
-    Returns:
-        array: :math:`2^N\times 2^N` matrix. The full system operator.
-    """
-    if num_wires == 1:
-        # total number of wires is 1, simply return the matrix
-        return U
-
-    N = num_wires
-    wires = np.asarray(wires)
-
-    if np.any(wires < 0) or np.any(wires >= N) or len(set(wires)) != len(wires):
-        raise ValueError("Invalid target subsystems provided in 'wires' argument.")
-
-    if U.shape != (2 ** len(wires), 2 ** len(wires)):
-        raise ValueError("Matrix parameter must be of size (2**len(wires), 2**len(wires))")
-
-    # generate N qubit basis states via the cartesian product
-    tuples = np.array(list(itertools.product([0, 1], repeat=N)))
-
-    # wires not acted on by the operator
-    inactive_wires = list(set(range(N)) - set(wires))
-
-    # expand U to act on the entire system
-    U = np.kron(U, np.identity(2 ** len(inactive_wires)))
-
-    # move active wires to beginning of the list of wires
-    rearranged_wires = np.array(list(wires) + inactive_wires)
-
-    # convert to computational basis
-    # i.e., converting the list of basis state bit strings into
-    # a list of decimal numbers that correspond to the computational
-    # basis state. For example, [0, 1, 0, 1, 1] = 2^3+2^1+2^0 = 11.
-    perm = np.ravel_multi_index(tuples[:, rearranged_wires].T, [2] * N)
-
-    # permute U to take into account rearranged wires
-    return U[:, perm][perm]
-
-
 @functools.lru_cache()
 def pauli_eigs(n):
     r"""Eigenvalues for :math:`A^{\otimes n}`, where :math:`A` is
     Pauli operator, or shares its eigenvalues.
 
     As an example if n==2, then the eigenvalues of a tensor product consisting
     of two matrices sharing the eigenvalues with Pauli matrices is returned.
@@ -200,62 +149,15 @@
         list: the eigenvalues of the specified observable
     """
     if n == 1:
         return np.array([1, -1])
     return np.concatenate([pauli_eigs(n - 1), -pauli_eigs(n - 1)])
 
 
-class Recorder:
-    """Recorder class used by the :class:`~.OperationRecorder`.
-
-    The Recorder class is a very minimal QNode, that simply
-    provides a QNode context for operator queueing."""
-
-    # pylint: disable=too-few-public-methods
-    def __init__(self, old_context):
-        self._old_context = old_context
-        self._ops = []
-        self.num_wires = 1
-
-    def _append_op(self, op):
-        """:class:`~.Operator` objects call this method
-        and append themselves upon initialization."""
-        self._ops.append(op)
-
-        # this ensure the recorder does not interfere with
-        # any QNode contexts
-        if self._old_context:
-            self._old_context._append_op(op)
-
-    def _remove_op(self, op):
-        """Remove an Operation from the queue."""
-        self._ops.remove(op)
-
-        # this ensure the recorder does not interfere with
-        # any QNode contexts
-        if self._old_context:
-            self._old_context._remove_op(op)
-
-    @property
-    def queue(self):
-        """Queue of the underlying QNode if existant, otherwise the internal operator list."""
-        if self._old_context:
-            return self._old_context.queue
-
-        return self._ops
-
-    # Spoof all attributes of the underlying QNode if there is one
-    def __getattr__(self, name):
-        if self._old_context:
-            return self._old_context.__getattribute__(name)
-
-        raise AttributeError("Attribute {} of Recorder mock QNode does not exist.".format(name))
-
-
-class OperationRecorder:
+class OperationRecorder(qml.QueuingContext):
     """A template and quantum function inspector,
     allowing easy introspection of operators that have been
     applied without requiring a QNode.
 
     **Example**:
 
     The OperationRecorder is a context manager. Executing templates
@@ -276,51 +178,38 @@
     CNOT(wires=[1, 0])
 
     Alternatively, the :attr:`~.OperationRecorder.queue` attribute can be used
     to directly accessed the applied :class:`~.Operation` and :class:`~.Observable`
     objects.
 
     Attributes:
-        rec (~.Recorder): a very minimal QNode, that simply
-            acts as a QNode context for operator queueing
         queue (List[~.Operators]): list of operators applied within
             the OperatorRecorder context, includes operations and observables
         operations (List[~.Operations]): list of operations applied within
             the OperatorRecorder context
         observables (List[~.Observables]): list of observables applied within
             the OperatorRecorder context
     """
 
     def __init__(self):
-        self.rec = None
-
-        self.queue = None
+        self.queue = []
         self.operations = None
         self.observables = None
 
-        self.old_context = None
+    def _append_operator(self, operator):
+        self.queue.append(operator)
 
-    def __enter__(self):
-        self.rec = Recorder(qml._current_context)
+    def _remove_operator(self, operator):
+        self.queue.remove(operator)
 
-        # store the old context to be returned later
-        self.old_context = qml._current_context
+    def __exit__(self, exception_type, exception_value, traceback):
+        super().__exit__(exception_type, exception_value, traceback)
 
-        # set the recorder as the QNode context
-        qml._current_context = self.rec
-
-        self.queue = None
-        self.operations = None
-        self.observables = None
-
-        return self
-
-    def __exit__(self, *args, **kwargs):
         # Remove duplicates that might have arisen from measurements
-        self.queue = list(OrderedDict.fromkeys(self.rec._ops))
+        self.queue = list(OrderedDict.fromkeys(self.queue))
         self.operations = list(
             filter(
                 lambda op: not (
                     isinstance(op, qml.operation.Observable) and not op.return_type is None
                 ),
                 self.queue,
             )
@@ -328,43 +217,26 @@
         self.observables = list(
             filter(
                 lambda op: isinstance(op, qml.operation.Observable) and not op.return_type is None,
                 self.queue,
             )
         )
 
-        qml._current_context = self.old_context
-
     def __str__(self):
         output = ""
         output += "Operations\n"
         output += "==========\n"
         for op in self.operations:
-            if op.parameters:
-                params = ", ".join([str(p) for p in op.parameters])
-                output += "{}({}, wires={})\n".format(op.name, params, op.wires)
-            else:
-                output += "{}(wires={})\n".format(op.name, op.wires)
-
-        return_map = {
-            qml.operation.Expectation: "expval",
-            qml.operation.Variance: "var",
-            qml.operation.Sample: "sample",
-        }
+            output += repr(op) + "\n"
+
         output += "\n"
         output += "Observables\n"
         output += "==========\n"
         for op in self.observables:
-            if op.parameters:
-                params = ", ".join([str(p) for p in op.parameters])
-                output += "{}({}({}, wires={}))\n".format(
-                    return_map[op.return_type], op.name, params, op.wires
-                )
-            else:
-                output += "{}({}(wires={}))\n".format(return_map[op.return_type], op.name, op.wires)
+            output += repr(op) + "\n"
 
         return output
 
 
 def inv(operation_list):
     """Invert a list of operations or a :doc:`template </introduction/templates>`.
 
@@ -451,18 +323,115 @@
             "The given operation_list does not only contain Operations."
             + "The following elements of the iterable were not Operations:"
             + ",".join(string_reps)
         )
 
     inv_ops = [op.inv() for op in reversed(copy.deepcopy(operation_list))]
 
-    if qml._current_context is not None:
-        ops_in_queue = {op for op in operation_list if op in qml._current_context.queue}
-
-        for op in ops_in_queue:
-            qml._current_context._remove_op(op)
+    for op in operation_list:
+        qml.QueuingContext.remove_operator(op)
 
-        for inv_op in inv_ops:
-            qml._current_context._append_op(inv_op)
-            inv_op.queue_idx = qml._current_context.queue.index(inv_op)
+    for inv_op in inv_ops:
+        qml.QueuingContext.append_operator(inv_op)
 
     return inv_ops
+
+
+def expand(matrix, original_wires, expanded_wires):
+    r"""Expand a an operator matrix to more wires.
+
+    Args:
+        matrix (array): :math:`2^n \times 2^n` matrix where n = len(original_wires).
+        original_wires (Sequence[int]): original wires of matrix
+        expanded_wires (Union[Sequence[int], int]): expanded wires of matrix, can be shuffled.
+            If a single int m is given, corresponds to list(range(m))
+
+    Returns:
+        array: :math:`2^m \times 2^m` matrix where m = len(expanded_wires).
+    """
+    if isinstance(expanded_wires, numbers.Integral):
+        expanded_wires = list(range(expanded_wires))
+
+    N = len(original_wires)
+    M = len(expanded_wires)
+    D = M - N
+
+    if not set(expanded_wires).issuperset(original_wires):
+        raise ValueError("Invalid target subsystems provided in 'original_wires' argument.")
+
+    if matrix.shape != (2 ** N, 2 ** N):
+        raise ValueError(
+            "Matrix parameter must be of size (2**len(original_wires), 2**len(original_wires))"
+        )
+
+    dims = [2] * (2 * N)
+    tensor = matrix.reshape(dims)
+
+    if D > 0:
+        extra_dims = [2] * (2 * D)
+        identity = np.eye(2 ** D).reshape(extra_dims)
+        expanded_tensor = np.tensordot(tensor, identity, axes=0)
+        # Fix order of tensor factors
+        expanded_tensor = np.moveaxis(expanded_tensor, range(2 * N, 2 * N + D), range(N, N + D))
+    else:
+        expanded_tensor = tensor
+
+    wire_indices = []
+    for wire in original_wires:
+        wire_indices.append(expanded_wires.index(wire))
+
+    wire_indices = np.array(wire_indices)
+
+    # Order tensor factors according to wires
+    original_indices = np.array(range(N))
+    expanded_tensor = np.moveaxis(expanded_tensor, original_indices, wire_indices)
+    expanded_tensor = np.moveaxis(expanded_tensor, original_indices + M, wire_indices + M)
+
+    return expanded_tensor.reshape((2 ** M, 2 ** M))
+
+
+def expand_vector(vector, original_wires, expanded_wires):
+    r"""Expand a vector to more wires.
+
+    Args:
+        vector (array): :math:`2^n` vector where n = len(original_wires).
+        original_wires (Sequence[int]): original wires of vector
+        expanded_wires (Union[Sequence[int], int]): expanded wires of vector, can be shuffled
+            If a single int m is given, corresponds to list(range(m))
+
+    Returns:
+        array: :math:`2^m` vector where m = len(expanded_wires).
+    """
+    if isinstance(expanded_wires, numbers.Integral):
+        expanded_wires = list(range(expanded_wires))
+
+    N = len(original_wires)
+    M = len(expanded_wires)
+    D = M - N
+
+    if not set(expanded_wires).issuperset(original_wires):
+        raise ValueError("Invalid target subsystems provided in 'original_wires' argument.")
+
+    if vector.shape != (2 ** N,):
+        raise ValueError("Vector parameter must be of length 2**len(original_wires)")
+
+    dims = [2] * N
+    tensor = vector.reshape(dims)
+
+    if D > 0:
+        extra_dims = [2] * D
+        ones = np.ones(2 ** D).reshape(extra_dims)
+        expanded_tensor = np.tensordot(tensor, ones, axes=0)
+    else:
+        expanded_tensor = tensor
+
+    wire_indices = []
+    for wire in original_wires:
+        wire_indices.append(expanded_wires.index(wire))
+
+    wire_indices = np.array(wire_indices)
+
+    # Order tensor factors according to wires
+    original_indices = np.array(range(N))
+    expanded_tensor = np.moveaxis(expanded_tensor, original_indices, wire_indices)
+
+    return expanded_tensor.reshape(2 ** M)
```

### Comparing `PennyLane-0.8.1/pennylane/variable.py` & `PennyLane-0.9.0/pennylane/variable.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/vqe/vqe.py` & `PennyLane-0.9.0/pennylane/vqe/vqe.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,24 +122,25 @@
 
 
 class VQECost:
     """Create a VQE cost function, i.e., a cost function returning the
     expectation value of a Hamiltonian.
 
     Args:
-        ansatz (callable): The ansatz for the circuit before the final measurement step
+        ansatz (callable): The ansatz for the circuit before the final measurement step.
             Note that the ansatz **must** have the following signature:
 
             .. code-block:: python
 
                 ansatz(params, **kwargs)
 
             where ``params`` are the trainable weights of the variational circuit, and
             ``kwargs`` are any additional keyword arguments that need to be passed
             to the template.
+        hamiltonian (~.Hamiltonian): Hamiltonian operator whose expectation value should be measured
         device (Device, Sequence[Device]): Corresponding device(s) where the resulting
             cost function should be executed. This can either be a single device, or a list
             of devices of length matching the number of terms in the Hamiltonian.
         interface (str, None): Which interface to use.
             This affects the types of objects that can be passed to/returned to the cost function.
             Supports all interfaces supported by the :func:`~.qnode` decorator.
         diff_method (str, None): The method of differentiation to use with the created cost function.
@@ -189,23 +190,43 @@
     >>> cost(params)
     tensor(0.0245, dtype=torch.float64)
 
     The cost function can be minimized using any gradient descent-based
     :doc:`optimizer </introduction/optimizers>`.
     """
 
-    def __init__(self, ansatz, hamiltonian, device, interface="autograd", diff_method="best"):
+    def __init__(
+        self, ansatz, hamiltonian, device, interface="autograd", diff_method="best", **kwargs
+    ):
         coeffs, observables = hamiltonian.terms
         self.hamiltonian = hamiltonian
         """Hamiltonian: the hamiltonian defining the VQE problem."""
 
         self.qnodes = qml.map(
-            ansatz, observables, device, interface=interface, diff_method=diff_method
+            ansatz, observables, device, interface=interface, diff_method=diff_method, **kwargs
         )
         """QNodeCollection: The QNodes to be evaluated. Each QNode corresponds to the
         the expectation value of each observable term after applying the circuit ansatz.
         """
 
         self.cost_fn = qml.dot(coeffs, self.qnodes)
 
     def __call__(self, *args, **kwargs):
         return self.cost_fn(*args, **kwargs)
+
+    def metric_tensor(self, args, kwargs=None, diag_approx=False, only_construct=False):
+        """Evaluate the value of the metric tensor.
+
+        Args:
+            args (tuple[Any]): positional (differentiable) arguments
+            kwargs (dict[str, Any]): auxiliary arguments
+            diag_approx (bool): iff True, use the diagonal approximation
+            only_construct (bool): Iff True, construct the circuits used for computing
+                the metric tensor but do not execute them, and return None.
+
+        Returns:
+            array[float]: metric tensor
+        """
+        # We know that for VQE, all the qnodes share the same ansatz so we select the first
+        return self.qnodes.qnodes[0].metric_tensor(
+            args=args, kwargs=kwargs, diag_approx=diag_approx, only_construct=only_construct
+        )
```

### Comparing `PennyLane-0.8.1/pennylane/vqe/__init__.py` & `PennyLane-0.9.0/pennylane/vqe/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/pennylane/_device.py` & `PennyLane-0.9.0/pennylane/_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,28 @@
 
         self._op_queue = None
         self._obs_queue = None
         self._parameters = None
 
     def __repr__(self):
         """String representation."""
-        return "{}.\nInstance: ".format(self.__module__, self.__class__.__name__, self.name)
+        return "<{} device (wires={}, shots={}) at {}>".format(
+            self.__class__.__name__, self.num_wires, self.shots, hex(id(self))
+        )
 
     def __str__(self):
         """Verbose string representation."""
-        return "{}\nName: \nAPI version: \nPlugin version: \nAuthor: ".format(
-            self.name, self.pennylane_requires, self.version, self.author
+        return "{}\nShort name: {}\nPackage: {}\nPlugin version: {}\nAuthor: {}\nWires: {}\nShots: {}".format(
+            self.name,
+            self.short_name,
+            self.__module__.split(".")[0],
+            self.version,
+            self.author,
+            self.num_wires,
+            self.shots,
         )
 
     @property
     @abc.abstractmethod
     def name(self):
         """The full name of the device."""
```

### Comparing `PennyLane-0.8.1/pennylane/_qubit_device.py` & `PennyLane-0.9.0/pennylane/_qubit_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,28 +27,32 @@
 from pennylane.qnodes import QuantumFunctionError
 from pennylane import Device
 
 
 class QubitDevice(Device):
     """Abstract base class for PennyLane qubit devices.
 
-    The following abstract methods **must** be defined:
-
-    * :meth:`~.probability`: returns the probability or marginal probability from the
-      device after circuit execution. :meth:`~.marginal_prob` may be used here.
+    The following abstract method **must** be defined:
 
     * :meth:`~.apply`: append circuit operations, compile the circuit (if applicable),
       and perform the quantum computation.
 
-    Where relevant, devices that generate their own samples (such as hardware) should
-    overwrite the following methods:
+    Devices that generate their own samples (such as hardware) may optionally
+    overwrite :meth:`~.probabilty`. This method otherwise automatically
+    computes the probabilities from the generated samples, and **must**
+    overwrite the following method:
 
     * :meth:`~.generate_samples`: Generate samples from the device from the
       exact or approximate probability distribution.
 
+    Analytic devices **must** overwrite the following method:
+
+    * :meth:`~.analytic_probability`: returns the probability or marginal probability from the
+      device after circuit execution. :meth:`~.marginal_prob` may be used here.
+
     This device contains common utility methods for qubit-based devices. These
     do not need to be overwritten. Utility methods include:
 
     * :meth:`~.expval`, :meth:`~.var`, :meth:`~.sample`: return expectation values,
       variances, and samples of observables after the circuit has been rotated
       into the observable eigenbasis.
 
@@ -169,15 +173,15 @@
         return self._asarray(results)
 
     @abc.abstractmethod
     def apply(self, operations, **kwargs):
         """Apply quantum operations, rotate the circuit into the measurement
         basis, and compile and execute the quantum circuit.
 
-        This method recieves a list of quantum operations queued by the QNode,
+        This method receives a list of quantum operations queued by the QNode,
         and should be responsible for:
 
         * Constructing the quantum program
         * (Optional) Rotating the quantum circuit using the rotation
           operations provided. This diagonalizes the circuit so that arbitrary
           observables can be measured in the computational basis.
         * Compile the circuit
@@ -276,15 +280,17 @@
             generate their own computational basis samples, with the resulting
             computational basis samples stored as ``self._samples``.
 
         Returns:
              array[complex]: array of samples in the shape ``(dev.shots, dev.num_wires)``
         """
         number_of_states = 2 ** self.num_wires
-        rotated_prob = self.probability()
+
+        rotated_prob = self.analytic_probability()
+
         samples = self.sample_basis_states(number_of_states, rotated_prob)
         return QubitDevice.states_to_binary(samples, self.num_wires)
 
     def sample_basis_states(self, number_of_states, state_probability):
         """Sample from the computational basis states based on the state
         probability.
 
@@ -331,16 +337,15 @@
         .. note::
 
             Only state vector simulators support this property. Please see the
             plugin documentation for more details.
         """
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def probability(self, wires=None):
+    def analytic_probability(self, wires=None):
         r"""Return the (marginal) probability of each computational basis
         state from the last run of the device.
 
         PennyLane uses the convention
         :math:`|q_0,q_1,\dots,q_{N-1}\rangle` where :math:`q_0` is the most
         significant bit.
 
@@ -356,14 +361,64 @@
             wires (Sequence[int]): Sequence of wires to return
                 marginal probabilities for. Wires not provided
                 are traced out of the system.
 
         Returns:
             List[float]: list of the probabilities
         """
+        raise NotImplementedError
+
+    def estimate_probability(self, wires=None):
+        """Return the estimated probability of each computational basis state
+        using the generated samples.
+
+        Args:
+            wires (Sequence[int]): Sequence of wires to return
+                marginal probabilities for. Wires not provided
+                are traced out of the system.
+
+        Returns:
+            List[float]: list of the probabilities
+        """
+        # consider only the requested wires
+        wires = np.hstack(wires)
+
+        samples = self._samples[:, np.array(wires)]
+
+        # convert samples from a list of 0, 1 integers, to base 10 representation
+        unraveled_indices = [2] * len(wires)
+        indices = np.ravel_multi_index(samples.T, unraveled_indices)
+
+        # count the basis state occurrences, and construct the probability vector
+        basis_states, counts = np.unique(indices, return_counts=True)
+        prob = np.zeros([2 ** len(wires)], dtype=np.float64)
+        prob[basis_states] = counts / self.shots
+        return prob
+
+    def probability(self, wires=None):
+        """Return either the analytic probability or estimated probability of
+        each computational basis state.
+
+        If no :attr:`~.analytic` attributes exists for the device, then return the
+        estimated probability.
+
+        Args:
+            wires (Sequence[int]): Sequence of wires to return
+                marginal probabilities for. Wires not provided
+                are traced out of the system.
+
+        Returns:
+            List[float]: list of the probabilities
+        """
+        wires = wires or range(self.num_wires)
+
+        if hasattr(self, "analytic") and self.analytic:
+            return self.analytic_probability(wires=wires)
+
+        return self.estimate_probability(wires=wires)
 
     def marginal_prob(self, prob, wires=None):
         r"""Return the marginal probability of the computational basis
         states by summing the probabiliites on the non-specified wires.
 
         If no wires are specified, then all the basis states representable by
         the device are considered and no marginalization takes place.
```

### Comparing `PennyLane-0.8.1/pennylane/_version.py` & `PennyLane-0.9.0/pennylane/qnn/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,13 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""This module contains classes and functions for constructing quantum neural networks from QNodes."""
 
-"""
-Version number (major.minor.patch[-label])
-"""
-
-__version__ = "0.8.1"
+from .keras import KerasLayer
```

### Comparing `PennyLane-0.8.1/pennylane/__init__.py` & `PennyLane-0.9.0/pennylane/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 
 from autograd import numpy
 from autograd import grad as _grad
 from autograd import jacobian as _jacobian
 
 from semantic_version import Version, Spec
 
+# QueuingContext needs to be imported before all other pennylane imports
+from ._queuing_context import QueuingContext  # pylint: disable=wrong-import-order
 import pennylane.operation
 
 import pennylane.init
 import pennylane.templates
-from pennylane.templates import template
+import pennylane.qnn
+from pennylane.templates import template, broadcast
 from pennylane.about import about
 from pennylane.vqe import Hamiltonian, VQECost
 
 from .circuit_graph import CircuitGraph
 from .configuration import Configuration
 from ._device import Device, DeviceError
 from .collections import apply, map, sum, dot, QNodeCollection
@@ -41,17 +44,14 @@
 from .optimize import *
 from .qnodes import qnode, QNode, QuantumFunctionError
 from .utils import inv
 from ._version import __version__
 from .io import *
 
 
-_current_context = None
-
-
 # overwrite module docstrings
 numpy.__doc__ = "NumPy with automatic differentiation support, provided by Autograd."
 
 
 # Look for an existing configuration file
 default_config = Configuration("config.toml")
```

### Comparing `PennyLane-0.8.1/PennyLane.egg-info/PKG-INFO` & `PennyLane-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: PennyLane
-Version: 0.8.1
+Version: 0.9.0
 Summary: PennyLane is a Python quantum machine learning library by Xanadu Inc.
 Home-page: https://github.com/XanaduAI/pennylane
 Maintainer: Xanadu Inc.
-Maintainer-email: nathan@xanadu.ai
+Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: .. image:: doc/_static/pennylane_thin.png
             :alt: PennyLane
         
         ###################################
         
         .. |CI| image:: https://img.shields.io/travis/com/XanaduAI/pennylane/master.svg?style=popout-square
@@ -41,43 +41,56 @@
         
         .. |LIC| image:: https://img.shields.io/pypi/l/PennyLane.svg?style=popout-square
             :alt: PyPI - License
             :target: https://www.apache.org/licenses/LICENSE-2.0
         
         |CI|  |COV| |PEP| |DOC| |VERS| |PY| |FORUM|
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine learning,
-        automatic differentiation, and optimization of hybrid quantum-classical computations.
+        `PennyLane <https://pennylane.ai>`_ is a cross-platform Python library for `differentiable programming <https://en.wikipedia.org/wiki/Differentiable_programming>`__ of quantum computers. 
         
-        Learn more about quantum machine learning with PennyLane: view and download QML examples
-        and demos over at https://pennylane.ai/qml.
+        PennyLane provides open-source tools for quantum machine learning, quantum computing, quantum chemistry, and hybrid quantum-classical computing. Extensive examples, tutorials, and demos are available at https://pennylane.ai/qml.
         
-        Features
-        ========
+        Key Features
+        ============
         
-        - **Follow the gradient**. Built-in **automatic differentiation** of quantum circuits
+        - *Device independent*.
+          Access quantum hardware and simulators from **Xanadu Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
+          **Microsoft QDK**.
         
-        - **Best of both worlds**.
-          Support for **hybrid quantum and classical** models; connect quantum
-          hardware with PyTorch, TensorFlow, and NumPy.
+        - *Best of both worlds*.
+          Build hybrid models by connecting quantum hardware to **PyTorch**, **TensorFlow**, **Keras**, and **NumPy**.
         
-        - **Batteries included**. Provides **optimization and machine learning** tools
+        - *Follow the gradient*. Hardware-friendly **automatic differentiation** of quantum circuits.
         
-        - **Device independent**.
-          The same quantum circuit model can be **run on different backends**. Install
-          `plugins <https://pennylane.ai/plugins.html>`__ to access even more
-          devices, including **Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
-          **Microsoft QDK**.
+        - *Batteries included*. Built-in tools for **quantum machine learning**, **optimization**, and **quantum chemistry**.
+        
+        Getting started
+        ===============
+        
+        For an introduction to quantum machine learning, we have several guides and resources available
+        on PennyLane's `quantum machine learning page <https://pennylane.ai/qml/>`_:
+        
+        * `What is quantum machine learning? <https://pennylane.ai/qml/whatisqml.html>`_
+        * `QML tutorials and demonstrations <https://pennylane.ai/qml/demonstrations.html>`_
+        * `Frequently asked questions <https://pennylane.ai/faq.html>`_
+        * `Glossary of key concepts <https://pennylane.ai/qml/glossary.html>`_
+        * `Curated selection of QML videos <https://pennylane.ai/qml/videos.html>`_
+        
+        You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
+        `quickstart guides <https://pennylane.readthedocs.io/en/stable/introduction/pennylane.html>`_
+        to using PennyLane, and detailed developer guides on
+        `how to write your own <https://pennylane.readthedocs.io/en/stable/development/plugins.html>`_
+        PennyLane-compatible quantum device.
         
         Available plugins
         =================
         
         * `PennyLane-SF <https://github.com/XanaduAI/pennylane-sf>`_: Supports integration with
           `Strawberry Fields <https://github.com/XanaduAI/strawberryfields>`__, a full-stack
-          Python library for simulating continuous variable (CV) quantum optical circuits.
+          Python library for simulating photonic quantum computing.
         
         
         * `PennyLane-qiskit <https://github.com/XanaduAI/pennylane-qiskit>`_: Supports
           integration with `Qiskit <https://qiskit.org>`__, an open-source quantum
           computation framework by IBM. Provides device support for the Qiskit Aer quantum
           simulators, and IBM Q hardware devices.
         
@@ -108,38 +121,14 @@
         PennyLane requires Python version 3.5 and above. Installation of PennyLane, as well
         as all dependencies, can be done using pip:
         
         .. code-block:: bash
         
             $ python -m pip install pennylane
         
-        
-        Getting started
-        ===============
-        
-        For getting started with PennyLane, check out some of the
-        `key concepts <https://pennylane.ai/qml/concepts.html>`_ behind quantum machine
-        learning, before moving on to some `introductory tutorials <https://pennylane.ai/qml/beginner.html>`_.
-        
-        Then, take a deeper dive into quantum machine learning by
-        exploring cutting-edge algorithms using PennyLane and near-term quantum hardware,
-        with our collection of
-        `QML tutorials <https://pennylane.ai/qml/implementations.html>`_.
-        
-        You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
-        more details on the quantum operations, and to explore the available optimization
-        tools provided by PennyLane, and detailed guides on
-        `how to write your own <https://pennylane.readthedocs.io/en/latest/development/plugins.html>`_
-        PennyLane-compatible quantum device.
-        
-        Finally, play around with the numerous `devices and plugins <https://pennylane.ai/plugins.html>`_
-        available for running your hybrid optimizations — these include
-        IBM Q, provided by the PennyLane-Qiskit plugin, as well as the Rigetti Aspen-1 QPU.
-        
-        
         Contributing to PennyLane
         =========================
         
         We welcome contributions — simply fork the PennyLane repository, and then make a
         `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
         All contributers to PennyLane will be listed as authors on the releases. All users who contribute
         significantly to the code (new plugins, new functionality, etc.) will be listed on the PennyLane arXiv paper.
@@ -150,19 +139,21 @@
         See our `contributions page <https://github.com/XanaduAI/pennylane/blob/master/.github/CONTRIBUTING.md>`_
         for more details.
         
         
         Authors
         =======
         
-        Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
+        PennyLane is the work of `many contributors <https://github.com/XanaduAI/pennylane/graphs/contributors>`_.
         
         If you are doing research using PennyLane, please cite `our paper <https://arxiv.org/abs/1811.04968>`_:
         
-            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan, and Nathan Killoran.
+            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+            Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+            Zeyue Niu, Antal Száva, and Nathan Killoran.
             *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
         
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane
```

### Comparing `PennyLane-0.8.1/PennyLane.egg-info/SOURCES.txt` & `PennyLane-0.9.0/PennyLane.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
-default_config.toml
+example_config.toml
 setup.py
 PennyLane.egg-info/PKG-INFO
 PennyLane.egg-info/SOURCES.txt
 PennyLane.egg-info/dependency_links.txt
 PennyLane.egg-info/entry_points.txt
 PennyLane.egg-info/requires.txt
 PennyLane.egg-info/top_level.txt
@@ -13,14 +13,15 @@
 doc/conf.py
 doc/directives.py
 doc/index.rst
 doc/requirements.txt
 pennylane/__init__.py
 pennylane/_device.py
 pennylane/_qubit_device.py
+pennylane/_queuing_context.py
 pennylane/_version.py
 pennylane/about.py
 pennylane/circuit_graph.py
 pennylane/configuration.py
 pennylane/init.py
 pennylane/io.py
 pennylane/measure.py
@@ -53,43 +54,54 @@
 pennylane/optimize/adagrad.py
 pennylane/optimize/adam.py
 pennylane/optimize/gradient_descent.py
 pennylane/optimize/momentum.py
 pennylane/optimize/nesterov_momentum.py
 pennylane/optimize/qng.py
 pennylane/optimize/rms_prop.py
+pennylane/optimize/rotoselect.py
+pennylane/optimize/rotosolve.py
 pennylane/plugins/__init__.py
 pennylane/plugins/default_gaussian.py
 pennylane/plugins/default_qubit.py
+pennylane/qnn/__init__.py
+pennylane/qnn/keras.py
 pennylane/qnodes/__init__.py
 pennylane/qnodes/base.py
 pennylane/qnodes/cv.py
 pennylane/qnodes/decorator.py
 pennylane/qnodes/device_jacobian.py
 pennylane/qnodes/jacobian.py
 pennylane/qnodes/passthru.py
 pennylane/qnodes/qubit.py
 pennylane/templates/__init__.py
+pennylane/templates/broadcast (josh-workstation's conflicted copy 2020-03-16).py
+pennylane/templates/broadcast.py
 pennylane/templates/decorator.py
 pennylane/templates/utils.py
 pennylane/templates/embeddings/__init__.py
 pennylane/templates/embeddings/amplitude.py
 pennylane/templates/embeddings/angle.py
 pennylane/templates/embeddings/basis.py
 pennylane/templates/embeddings/displacement.py
+pennylane/templates/embeddings/iqp.py
 pennylane/templates/embeddings/qaoa.py
 pennylane/templates/embeddings/squeezing.py
 pennylane/templates/layers/__init__.py
+pennylane/templates/layers/basic_entangler.py
 pennylane/templates/layers/cv_neural_net.py
 pennylane/templates/layers/random.py
+pennylane/templates/layers/simplified_two_design.py
 pennylane/templates/layers/strongly_entangling.py
 pennylane/templates/state_preparations/__init__.py
+pennylane/templates/state_preparations/arbitrary_state_preparation.py
 pennylane/templates/state_preparations/basis.py
 pennylane/templates/state_preparations/mottonen.py
 pennylane/templates/subroutines/__init__.py
+pennylane/templates/subroutines/arbitrary_unitary.py
 pennylane/templates/subroutines/interferometer.py
 pennylane/vqe/__init__.py
 pennylane/vqe/vqe.py
 tests/conftest.py
 tests/gate_data.py
 tests/test_about.py
 tests/test_classical_gradients.py
@@ -104,18 +116,12 @@
 tests/test_observable.py
 tests/test_operation.py
 tests/test_optimize.py
 tests/test_optimize_qng.py
 tests/test_prob.py
 tests/test_quantum_gradients.py
 tests/test_qubit_device.py
-tests/test_templates.py
-tests/test_templates_decorator.py
-tests/test_templates_embeddings.py
-tests/test_templates_layers.py
-tests/test_templates_state_preparations.py
-tests/test_templates_subroutines.py
-tests/test_templates_utils.py
+tests/test_queuing_context.py
 tests/test_tensor_measurements.py
 tests/test_utils.py
 tests/test_variable.py
 tests/test_vqe.py
```

### Comparing `PennyLane-0.8.1/PKG-INFO` & `PennyLane-0.9.0/PennyLane.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: PennyLane
-Version: 0.8.1
+Version: 0.9.0
 Summary: PennyLane is a Python quantum machine learning library by Xanadu Inc.
 Home-page: https://github.com/XanaduAI/pennylane
 Maintainer: Xanadu Inc.
-Maintainer-email: nathan@xanadu.ai
+Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: .. image:: doc/_static/pennylane_thin.png
             :alt: PennyLane
         
         ###################################
         
         .. |CI| image:: https://img.shields.io/travis/com/XanaduAI/pennylane/master.svg?style=popout-square
@@ -41,43 +41,56 @@
         
         .. |LIC| image:: https://img.shields.io/pypi/l/PennyLane.svg?style=popout-square
             :alt: PyPI - License
             :target: https://www.apache.org/licenses/LICENSE-2.0
         
         |CI|  |COV| |PEP| |DOC| |VERS| |PY| |FORUM|
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine learning,
-        automatic differentiation, and optimization of hybrid quantum-classical computations.
+        `PennyLane <https://pennylane.ai>`_ is a cross-platform Python library for `differentiable programming <https://en.wikipedia.org/wiki/Differentiable_programming>`__ of quantum computers. 
         
-        Learn more about quantum machine learning with PennyLane: view and download QML examples
-        and demos over at https://pennylane.ai/qml.
+        PennyLane provides open-source tools for quantum machine learning, quantum computing, quantum chemistry, and hybrid quantum-classical computing. Extensive examples, tutorials, and demos are available at https://pennylane.ai/qml.
         
-        Features
-        ========
+        Key Features
+        ============
         
-        - **Follow the gradient**. Built-in **automatic differentiation** of quantum circuits
+        - *Device independent*.
+          Access quantum hardware and simulators from **Xanadu Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
+          **Microsoft QDK**.
         
-        - **Best of both worlds**.
-          Support for **hybrid quantum and classical** models; connect quantum
-          hardware with PyTorch, TensorFlow, and NumPy.
+        - *Best of both worlds*.
+          Build hybrid models by connecting quantum hardware to **PyTorch**, **TensorFlow**, **Keras**, and **NumPy**.
         
-        - **Batteries included**. Provides **optimization and machine learning** tools
+        - *Follow the gradient*. Hardware-friendly **automatic differentiation** of quantum circuits.
         
-        - **Device independent**.
-          The same quantum circuit model can be **run on different backends**. Install
-          `plugins <https://pennylane.ai/plugins.html>`__ to access even more
-          devices, including **Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
-          **Microsoft QDK**.
+        - *Batteries included*. Built-in tools for **quantum machine learning**, **optimization**, and **quantum chemistry**.
+        
+        Getting started
+        ===============
+        
+        For an introduction to quantum machine learning, we have several guides and resources available
+        on PennyLane's `quantum machine learning page <https://pennylane.ai/qml/>`_:
+        
+        * `What is quantum machine learning? <https://pennylane.ai/qml/whatisqml.html>`_
+        * `QML tutorials and demonstrations <https://pennylane.ai/qml/demonstrations.html>`_
+        * `Frequently asked questions <https://pennylane.ai/faq.html>`_
+        * `Glossary of key concepts <https://pennylane.ai/qml/glossary.html>`_
+        * `Curated selection of QML videos <https://pennylane.ai/qml/videos.html>`_
+        
+        You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
+        `quickstart guides <https://pennylane.readthedocs.io/en/stable/introduction/pennylane.html>`_
+        to using PennyLane, and detailed developer guides on
+        `how to write your own <https://pennylane.readthedocs.io/en/stable/development/plugins.html>`_
+        PennyLane-compatible quantum device.
         
         Available plugins
         =================
         
         * `PennyLane-SF <https://github.com/XanaduAI/pennylane-sf>`_: Supports integration with
           `Strawberry Fields <https://github.com/XanaduAI/strawberryfields>`__, a full-stack
-          Python library for simulating continuous variable (CV) quantum optical circuits.
+          Python library for simulating photonic quantum computing.
         
         
         * `PennyLane-qiskit <https://github.com/XanaduAI/pennylane-qiskit>`_: Supports
           integration with `Qiskit <https://qiskit.org>`__, an open-source quantum
           computation framework by IBM. Provides device support for the Qiskit Aer quantum
           simulators, and IBM Q hardware devices.
         
@@ -108,38 +121,14 @@
         PennyLane requires Python version 3.5 and above. Installation of PennyLane, as well
         as all dependencies, can be done using pip:
         
         .. code-block:: bash
         
             $ python -m pip install pennylane
         
-        
-        Getting started
-        ===============
-        
-        For getting started with PennyLane, check out some of the
-        `key concepts <https://pennylane.ai/qml/concepts.html>`_ behind quantum machine
-        learning, before moving on to some `introductory tutorials <https://pennylane.ai/qml/beginner.html>`_.
-        
-        Then, take a deeper dive into quantum machine learning by
-        exploring cutting-edge algorithms using PennyLane and near-term quantum hardware,
-        with our collection of
-        `QML tutorials <https://pennylane.ai/qml/implementations.html>`_.
-        
-        You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
-        more details on the quantum operations, and to explore the available optimization
-        tools provided by PennyLane, and detailed guides on
-        `how to write your own <https://pennylane.readthedocs.io/en/latest/development/plugins.html>`_
-        PennyLane-compatible quantum device.
-        
-        Finally, play around with the numerous `devices and plugins <https://pennylane.ai/plugins.html>`_
-        available for running your hybrid optimizations — these include
-        IBM Q, provided by the PennyLane-Qiskit plugin, as well as the Rigetti Aspen-1 QPU.
-        
-        
         Contributing to PennyLane
         =========================
         
         We welcome contributions — simply fork the PennyLane repository, and then make a
         `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
         All contributers to PennyLane will be listed as authors on the releases. All users who contribute
         significantly to the code (new plugins, new functionality, etc.) will be listed on the PennyLane arXiv paper.
@@ -150,19 +139,21 @@
         See our `contributions page <https://github.com/XanaduAI/pennylane/blob/master/.github/CONTRIBUTING.md>`_
         for more details.
         
         
         Authors
         =======
         
-        Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
+        PennyLane is the work of `many contributors <https://github.com/XanaduAI/pennylane/graphs/contributors>`_.
         
         If you are doing research using PennyLane, please cite `our paper <https://arxiv.org/abs/1811.04968>`_:
         
-            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan, and Nathan Killoran.
+            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+            Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+            Zeyue Niu, Antal Száva, and Nathan Killoran.
             *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
         
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane
```

### Comparing `PennyLane-0.8.1/README.rst` & `PennyLane-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,43 +33,56 @@
 
 .. |LIC| image:: https://img.shields.io/pypi/l/PennyLane.svg?style=popout-square
     :alt: PyPI - License
     :target: https://www.apache.org/licenses/LICENSE-2.0
 
 |CI|  |COV| |PEP| |DOC| |VERS| |PY| |FORUM|
 
-`PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine learning,
-automatic differentiation, and optimization of hybrid quantum-classical computations.
+`PennyLane <https://pennylane.ai>`_ is a cross-platform Python library for `differentiable programming <https://en.wikipedia.org/wiki/Differentiable_programming>`__ of quantum computers. 
 
-Learn more about quantum machine learning with PennyLane: view and download QML examples
-and demos over at https://pennylane.ai/qml.
+PennyLane provides open-source tools for quantum machine learning, quantum computing, quantum chemistry, and hybrid quantum-classical computing. Extensive examples, tutorials, and demos are available at https://pennylane.ai/qml.
 
-Features
-========
+Key Features
+============
 
-- **Follow the gradient**. Built-in **automatic differentiation** of quantum circuits
+- *Device independent*.
+  Access quantum hardware and simulators from **Xanadu Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
+  **Microsoft QDK**.
 
-- **Best of both worlds**.
-  Support for **hybrid quantum and classical** models; connect quantum
-  hardware with PyTorch, TensorFlow, and NumPy.
+- *Best of both worlds*.
+  Build hybrid models by connecting quantum hardware to **PyTorch**, **TensorFlow**, **Keras**, and **NumPy**.
 
-- **Batteries included**. Provides **optimization and machine learning** tools
+- *Follow the gradient*. Hardware-friendly **automatic differentiation** of quantum circuits.
 
-- **Device independent**.
-  The same quantum circuit model can be **run on different backends**. Install
-  `plugins <https://pennylane.ai/plugins.html>`__ to access even more
-  devices, including **Strawberry Fields**, **IBM Q**, **Google Cirq**, **Rigetti Forest**, and
-  **Microsoft QDK**.
+- *Batteries included*. Built-in tools for **quantum machine learning**, **optimization**, and **quantum chemistry**.
+
+Getting started
+===============
+
+For an introduction to quantum machine learning, we have several guides and resources available
+on PennyLane's `quantum machine learning page <https://pennylane.ai/qml/>`_:
+
+* `What is quantum machine learning? <https://pennylane.ai/qml/whatisqml.html>`_
+* `QML tutorials and demonstrations <https://pennylane.ai/qml/demonstrations.html>`_
+* `Frequently asked questions <https://pennylane.ai/faq.html>`_
+* `Glossary of key concepts <https://pennylane.ai/qml/glossary.html>`_
+* `Curated selection of QML videos <https://pennylane.ai/qml/videos.html>`_
+
+You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
+`quickstart guides <https://pennylane.readthedocs.io/en/stable/introduction/pennylane.html>`_
+to using PennyLane, and detailed developer guides on
+`how to write your own <https://pennylane.readthedocs.io/en/stable/development/plugins.html>`_
+PennyLane-compatible quantum device.
 
 Available plugins
 =================
 
 * `PennyLane-SF <https://github.com/XanaduAI/pennylane-sf>`_: Supports integration with
   `Strawberry Fields <https://github.com/XanaduAI/strawberryfields>`__, a full-stack
-  Python library for simulating continuous variable (CV) quantum optical circuits.
+  Python library for simulating photonic quantum computing.
 
 
 * `PennyLane-qiskit <https://github.com/XanaduAI/pennylane-qiskit>`_: Supports
   integration with `Qiskit <https://qiskit.org>`__, an open-source quantum
   computation framework by IBM. Provides device support for the Qiskit Aer quantum
   simulators, and IBM Q hardware devices.
 
@@ -100,38 +113,14 @@
 PennyLane requires Python version 3.5 and above. Installation of PennyLane, as well
 as all dependencies, can be done using pip:
 
 .. code-block:: bash
 
     $ python -m pip install pennylane
 
-
-Getting started
-===============
-
-For getting started with PennyLane, check out some of the
-`key concepts <https://pennylane.ai/qml/concepts.html>`_ behind quantum machine
-learning, before moving on to some `introductory tutorials <https://pennylane.ai/qml/beginner.html>`_.
-
-Then, take a deeper dive into quantum machine learning by
-exploring cutting-edge algorithms using PennyLane and near-term quantum hardware,
-with our collection of
-`QML tutorials <https://pennylane.ai/qml/implementations.html>`_.
-
-You can also check out our `documentation <https://pennylane.readthedocs.io>`_ for
-more details on the quantum operations, and to explore the available optimization
-tools provided by PennyLane, and detailed guides on
-`how to write your own <https://pennylane.readthedocs.io/en/latest/development/plugins.html>`_
-PennyLane-compatible quantum device.
-
-Finally, play around with the numerous `devices and plugins <https://pennylane.ai/plugins.html>`_
-available for running your hybrid optimizations — these include
-IBM Q, provided by the PennyLane-Qiskit plugin, as well as the Rigetti Aspen-1 QPU.
-
-
 Contributing to PennyLane
 =========================
 
 We welcome contributions — simply fork the PennyLane repository, and then make a
 `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
 All contributers to PennyLane will be listed as authors on the releases. All users who contribute
 significantly to the code (new plugins, new functionality, etc.) will be listed on the PennyLane arXiv paper.
@@ -142,19 +131,21 @@
 See our `contributions page <https://github.com/XanaduAI/pennylane/blob/master/.github/CONTRIBUTING.md>`_
 for more details.
 
 
 Authors
 =======
 
-Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
+PennyLane is the work of `many contributors <https://github.com/XanaduAI/pennylane/graphs/contributors>`_.
 
 If you are doing research using PennyLane, please cite `our paper <https://arxiv.org/abs/1811.04968>`_:
 
-    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, Carsten Blank, Keri McKiernan, and Nathan Killoran.
+    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+    Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+    Zeyue Niu, Antal Száva, and Nathan Killoran.
     *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
 
 
 Support
 =======
 
 - **Source Code:** https://github.com/XanaduAI/pennylane
```

### Comparing `PennyLane-0.8.1/setup.py` & `PennyLane-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "semantic_version==2.6",
 ]
 
 info = {
     'name': 'PennyLane',
     'version': version,
     'maintainer': 'Xanadu Inc.',
-    'maintainer_email': 'nathan@xanadu.ai',
+    'maintainer_email': 'software@xanadu.ai',
     'url': 'https://github.com/XanaduAI/pennylane',
     'license': 'Apache License 2.0',
     'packages': find_packages(where="."),
     'entry_points': {
         'pennylane.plugins': [
             'default.qubit = pennylane.plugins:DefaultQubit',
             'default.gaussian = pennylane.plugins:DefaultGaussian',
```

### Comparing `PennyLane-0.8.1/tests/conftest.py` & `PennyLane-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/gate_data.py` & `PennyLane-0.9.0/tests/gate_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Convenience gate representations for testing"""
+import math
+import cmath
 import numpy as np
 
 # ========================================================
 #  fixed gates
 # ========================================================
 
 I = np.eye(2)
 # Pauli matrices
 X = np.array([[0, 1], [1, 0]])  #: Pauli-X matrix
 Y = np.array([[0, -1j], [1j, 0]])  #: Pauli-Y matrix
 Z = np.array([[1, 0], [0, -1]])  #: Pauli-Z matrix
 
-H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)  #: Hadamard gate
+H = np.array([[1, 1], [1, -1]]) / math.sqrt(2)  #: Hadamard gate
 # Two qubit gates
 CNOT = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])  #: CNOT gate
 SWAP = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])  #: SWAP gate
 CZ = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])  #: CZ gate
 S = np.array([[1, 0], [0, 1j]])  #: Phase Gate
-T = np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])  #: T Gate
+T = np.array([[1, 0], [0, cmath.exp(1j * np.pi / 4)]])  #: T Gate
 # Three qubit gates
 CSWAP = np.array(
     [
         [1, 0, 0, 0, 0, 0, 0, 0],
         [0, 1, 0, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 0, 0, 0, 0],
         [0, 0, 0, 1, 0, 0, 0, 0],
@@ -44,48 +46,48 @@
     r"""One-qubit phase shift.
 
     Args:
         phi (float): phase shift angle
     Returns:
         array: unitary 2x2 phase shift matrix
     """
-    return np.array([[1, 0], [0, np.exp(1j * phi)]])
+    return np.array([[1, 0], [0, cmath.exp(1j * phi)]])
 
 
 def Rotx(theta):
     r"""One-qubit rotation about the x axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_x \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * X
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * X
 
 
 def Roty(theta):
     r"""One-qubit rotation about the y axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_y \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Y
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * Y
 
 
 def Rotz(theta):
     r"""One-qubit rotation about the z axis.
 
     Args:
         theta (float): rotation angle
     Returns:
         array: unitary 2x2 rotation matrix :math:`e^{-i \sigma_z \theta/2}`
     """
-    return np.cos(theta / 2) * I + 1j * np.sin(-theta / 2) * Z
+    return math.cos(theta / 2) * I + 1j * math.sin(-theta / 2) * Z
 
 
 def Rot3(a, b, c):
     r"""Arbitrary one-qubit rotation using three Euler angles.
 
     Args:
         a,b,c (float): rotation angles
@@ -103,16 +105,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_x(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.cos(theta / 2), -1j * np.sin(theta / 2)],
-            [0, 0, -1j * np.sin(theta / 2), np.cos(theta / 2)],
+            [0, 0, math.cos(theta / 2), -1j * math.sin(theta / 2)],
+            [0, 0, -1j * math.sin(theta / 2), math.cos(theta / 2)],
         ]
     )
 
 
 def CRoty(theta):
     r"""Two-qubit controlled rotation about the y axis.
 
@@ -121,16 +123,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_y(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.cos(theta / 2), -np.sin(theta / 2)],
-            [0, 0, np.sin(theta / 2), np.cos(theta / 2)],
+            [0, 0, math.cos(theta / 2), -math.sin(theta / 2)],
+            [0, 0, math.sin(theta / 2), math.cos(theta / 2)],
         ]
     )
 
 
 def CRotz(theta):
     r"""Two-qubit controlled rotation about the z axis.
 
@@ -139,16 +141,16 @@
     Returns:
         array: unitary 4x4 rotation matrix :math:`|0\rangle\langle 0|\otimes \mathbb{I}+|1\rangle\langle 1|\otimes R_z(\theta)`
     """
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
-            [0, 0, np.exp(-1j * theta / 2), 0],
-            [0, 0, 0, np.exp(1j * theta / 2)],
+            [0, 0, cmath.exp(-1j * theta / 2), 0],
+            [0, 0, 0, cmath.exp(1j * theta / 2)],
         ]
     )
 
 
 def CRot3(a, b, c):
     r"""Arbitrary two-qubit controlled rotation using three Euler angles.
 
@@ -160,18 +162,18 @@
     return np.array(
         [
             [1, 0, 0, 0],
             [0, 1, 0, 0],
             [
                 0,
                 0,
-                np.exp(-1j * (a + c) / 2) * np.cos(b / 2),
-                -np.exp(1j * (a - c) / 2) * np.sin(b / 2),
+                cmath.exp(-1j * (a + c) / 2) * math.cos(b / 2),
+                -cmath.exp(1j * (a - c) / 2) * math.sin(b / 2),
             ],
             [
                 0,
                 0,
-                np.exp(-1j * (a - c) / 2) * np.sin(b / 2),
-                np.exp(1j * (a + c) / 2) * np.cos(b / 2),
+                cmath.exp(-1j * (a - c) / 2) * math.sin(b / 2),
+                cmath.exp(1j * (a + c) / 2) * math.cos(b / 2),
             ],
         ]
     )
```

### Comparing `PennyLane-0.8.1/tests/test_about.py` & `PennyLane-0.9.0/tests/test_about.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_classical_gradients.py` & `PennyLane-0.9.0/tests/test_classical_gradients.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_configuration.py` & `PennyLane-0.9.0/tests/test_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,66 @@
 import toml
 
 import pennylane as qml
 from pennylane import Configuration
 
 log.getLogger('defaults')
 
-config_path = 'default_config.toml'
+
+config_path = "default_config.toml"
+
+
+test_config = """\
+[main]
+shots = 1000
+
+[default.gaussian]
+hbar = 2
+
+[strawberryfields.global]
+hbar = 1
+shots = 1000
+analytic = true
+
+    [strawberryfields.fock]
+    cutoff_dim = 10
+
+    [strawberryfields.gaussian]
+    shots = 1000
+    hbar = 1
+
+[qiskit.global]
+backend = "qasm_simulator"
+
+    [qiskit.aer]
+    backend = "unitary_simulator"
+    backend_options = {"validation_threshold" = 1e-6}
+
+    [qiskit.ibmq]
+    ibmqx_token = "XXX"
+    backend = "ibmq_rome"
+    hub = "MYHUB"
+    group = "MYGROUP"
+    project = "MYPROJECT"
+"""
+
 
 @pytest.fixture(scope="function")
 def default_config():
     return Configuration(name=config_path)
 
-@pytest.fixture(scope="session")
-def default_config_toml():
+
+@pytest.fixture(scope="function")
+def default_config_toml(tmpdir):
+    with open(config_path, "w") as f:
+        f.write(test_config)
+
     return toml.load(config_path)
 
+
 class TestConfigurationFileInteraction:
     """Test the interaction with the configuration file."""
 
     def test_loading_current_directory(self, monkeypatch, default_config_toml):
         """Test that the default configuration file can be loaded
         from the current directory."""
 
@@ -110,31 +152,31 @@
         assert default_config['strawberryfields.global.hbar'] == 1
         assert default_config['strawberryfields.global']['hbar'] == 1
 
         # get nested dictionaries
         assert default_config['strawberryfields.fock'] == {'cutoff_dim': 10}
 
         # get key that doesn't exist
-        assert default_config['projectq.ibm.idonotexist'] == {}
+        assert default_config['qiskit.ibmq.idonotexist'] == {}
 
     def test_set_item(self, default_config):
         """Test setting items."""
 
         # set existing options
         default_config['main.shots'] = 10
         assert default_config['main.shots'] == 10
         assert default_config['main']['shots'] == 10
 
         default_config['strawberryfields.global']['hbar'] = 5
         assert default_config['strawberryfields.global.hbar'] == 5
         assert default_config['strawberryfields.global']['hbar'] == 5
 
         # set new options
-        default_config['projectq.ibm']['device'] = 'ibmqx4'
-        assert default_config['projectq.ibm.device'] == 'ibmqx4'
+        default_config['qiskit.ibmq']['backend'] = 'ibmq_rome'
+        assert default_config['qiskit.ibmq.backend'] == 'ibmq_rome'
 
         # set nested dictionaries
         default_config['strawberryfields.tf'] = {'batched': True, 'cutoff_dim': 6}
         assert default_config['strawberryfields.tf'] == {'batched': True, 'cutoff_dim': 6}
 
         # set nested keys that don't exist dictionaries
         default_config['strawberryfields.another.hello.world'] = 5
```

### Comparing `PennyLane-0.8.1/tests/test_default_gaussian.py` & `PennyLane-0.9.0/tests/test_default_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
                          'CubicPhase',
                          'Kerr'}
 
         assert set(qml.ops._cv__ops__) - non_supported == set(gaussian_dev._operation_map)
 
     def test_observable_map(self, gaussian_dev):
         """Test that default Gaussian device supports all PennyLane Gaussian continuous observables."""
-        assert set(qml.ops._cv__obs__)|{'Identity'}-{'Heterodyne'} == set(gaussian_dev._observable_map)
+        assert set(qml.ops._cv__obs__)-{'TensorN'}|{'Identity'}-{'Heterodyne'} == set(gaussian_dev._observable_map)
 
     def test_apply(self, gaussian_dev, tol):
         """Test the application of gates to a state"""
 
         # loop through all supported operations
         for gate_name, fn in gaussian_dev._operation_map.items():
             #log.debug("\tTesting %s gate...", gate_name)
```

### Comparing `PennyLane-0.8.1/tests/test_default_qubit.py` & `PennyLane-0.9.0/tests/test_default_qubit.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,54 +165,54 @@
     ]
 
     @pytest.mark.parametrize("operation,input,expected_output", test_data_two_wires_no_parameters)
     def test_apply_operation_two_wires_no_parameters(self, qubit_device_2_wires, tol, operation, input, expected_output):
         """Tests that applying an operation yields the expected output state for two wire
            operations that have no parameters."""
 
-        qubit_device_2_wires._state = np.array(input)
+        qubit_device_2_wires._state = np.array(input).reshape((2, 2))
         qubit_device_2_wires.apply([operation(wires=[0, 1])])
 
-        assert np.allclose(qubit_device_2_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_2_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     @pytest.mark.parametrize("operation,input,expected_output", test_data_two_wires_no_parameters)
     def test_apply_operation_two_wires_no_parameters_inverse(self, qubit_device_2_wires, tol, operation, input, expected_output):
         """Tests that applying an operation yields the expected output state for two wire
            operations that have no parameters."""
 
-        qubit_device_2_wires._state = np.array(input)
+        qubit_device_2_wires._state = np.array(input).reshape((2, 2))
         qubit_device_2_wires.apply([operation(wires=[0, 1]).inv()])
 
-        assert np.allclose(qubit_device_2_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_2_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     test_data_three_wires_no_parameters = [
         (qml.CSWAP, [1, 0, 0, 0, 0, 0, 0, 0], [1, 0, 0, 0, 0, 0, 0, 0]),
         (qml.CSWAP, [0, 0, 0, 0, 0, 1, 0, 0], [0, 0, 0, 0, 0, 0, 1, 0]),
         (qml.CSWAP, [0, 0, 0, 0, 0, 0, 1, 0], [0, 0, 0, 0, 0, 1, 0, 0]),
     ]
 
     @pytest.mark.parametrize("operation,input,expected_output", test_data_three_wires_no_parameters)
     def test_apply_operation_three_wires_no_parameters(self, qubit_device_3_wires, tol, operation, input, expected_output):
         """Tests that applying an operation yields the expected output state for three wire
            operations that have no parameters."""
 
-        qubit_device_3_wires._state = np.array(input)
+        qubit_device_3_wires._state = np.array(input).reshape((2, 2, 2))
         qubit_device_3_wires.apply([operation(wires=[0, 1, 2])])
 
-        assert np.allclose(qubit_device_3_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_3_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     @pytest.mark.parametrize("operation,input,expected_output", test_data_three_wires_no_parameters)
     def test_apply_operation_three_wires_no_parameters_inverse(self, qubit_device_3_wires, tol, operation, input, expected_output):
         """Tests that applying the inverse of an operation yields the expected output state for three wire
            operations that have no parameters."""
 
-        qubit_device_3_wires._state = np.array(input)
+        qubit_device_3_wires._state = np.array(input).reshape((2, 2, 2))
         qubit_device_3_wires.apply([operation(wires=[0, 1, 2]).inv()])
 
-        assert np.allclose(qubit_device_3_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_3_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
 
     @pytest.mark.parametrize("operation,expected_output,par", [
         (qml.BasisState, [0, 0, 1, 0], [1, 0]),
         (qml.BasisState, [0, 0, 1, 0], [1, 0]),
         (qml.BasisState, [0, 0, 0, 1], [1, 1]),
         (qml.QubitStateVector, [0, 0, 1, 0], [0, 0, 1, 0]),
@@ -225,41 +225,47 @@
         """Tests that applying an operation yields the expected output state for single wire
            operations that have no parameters."""
 
         par = np.array(par)
         qubit_device_2_wires.reset()
         qubit_device_2_wires.apply([operation(par, wires=[0, 1])])
 
-        assert np.allclose(qubit_device_2_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_2_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     test_data_single_wire_with_parameters = [
         (qml.PhaseShift, [1, 0], [1, 0], [math.pi / 2]),
         (qml.PhaseShift, [0, 1], [0, 1j], [math.pi / 2]),
         (qml.PhaseShift, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / math.sqrt(2), 1 / 2 + 1j / 2], [math.pi / 4]),
         (qml.RX, [1, 0], [1 / math.sqrt(2), -1j * 1 / math.sqrt(2)], [math.pi / 2]),
         (qml.RX, [1, 0], [0, -1j], [math.pi]),
         (qml.RX, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / 2 - 1j / 2, 1 / 2 - 1j / 2], [math.pi / 2]),
         (qml.RY, [1, 0], [1 / math.sqrt(2), 1 / math.sqrt(2)], [math.pi / 2]),
         (qml.RY, [1, 0], [0, 1], [math.pi]),
         (qml.RY, [1 / math.sqrt(2), 1 / math.sqrt(2)], [0, 1], [math.pi / 2]),
         (qml.RZ, [1, 0], [1 / math.sqrt(2) - 1j / math.sqrt(2), 0], [math.pi / 2]),
         (qml.RZ, [0, 1], [0, 1j], [math.pi]),
         (qml.RZ, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / 2 - 1j / 2, 1 / 2 + 1j / 2], [math.pi / 2]),
+        (qml.MultiRZ, [1, 0], [1 / math.sqrt(2) - 1j / math.sqrt(2), 0], [math.pi / 2]),
+        (qml.MultiRZ, [0, 1], [0, 1j], [math.pi]),
+        (qml.MultiRZ, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / 2 - 1j / 2, 1 / 2 + 1j / 2], [math.pi / 2]),
         (qml.Rot, [1, 0], [1 / math.sqrt(2) - 1j / math.sqrt(2), 0], [math.pi / 2, 0, 0]),
         (qml.Rot, [1, 0], [1 / math.sqrt(2), 1 / math.sqrt(2)], [0, math.pi / 2, 0]),
         (qml.Rot, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / 2 - 1j / 2, 1 / 2 + 1j / 2], [0, 0, math.pi / 2]),
         (qml.Rot, [1, 0], [-1j / math.sqrt(2), -1 / math.sqrt(2)], [math.pi / 2, -math.pi / 2, math.pi / 2]),
         (qml.Rot, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / 2 + 1j / 2, -1 / 2 + 1j / 2],
          [-math.pi / 2, math.pi, math.pi]),
         (qml.QubitUnitary, [1, 0], [1j / math.sqrt(2), 1j / math.sqrt(2)],
          [np.array([[1j / math.sqrt(2), 1j / math.sqrt(2)], [1j / math.sqrt(2), -1j / math.sqrt(2)]])]),
         (qml.QubitUnitary, [0, 1], [1j / math.sqrt(2), -1j / math.sqrt(2)],
          [np.array([[1j / math.sqrt(2), 1j / math.sqrt(2)], [1j / math.sqrt(2), -1j / math.sqrt(2)]])]),
         (qml.QubitUnitary, [1 / math.sqrt(2), -1 / math.sqrt(2)], [0, 1j],
          [np.array([[1j / math.sqrt(2), 1j / math.sqrt(2)], [1j / math.sqrt(2), -1j / math.sqrt(2)]])]),
+        (qml.DiagonalQubitUnitary, [1, 0], [-1, 0], [np.array([-1, 1])]),
+        (qml.DiagonalQubitUnitary, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / math.sqrt(2), 1j / math.sqrt(2)], [np.array([1, 1j])]),
+        (qml.DiagonalQubitUnitary, [1 / 2, math.sqrt(3) / 4], [cmath.exp(1j * 0.4) / 2, cmath.exp(1j * -0.4) * math.sqrt(3) / 4], [np.array([cmath.exp(1j * 0.4), cmath.exp(1j * -0.4)])]),
     ]
 
     test_data_single_wire_with_parameters_inverses = [
         (qml.PhaseShift, [1, 0], [1, 0], [math.pi / 2]),
         (qml.PhaseShift, [0, 1], [0, -1j], [math.pi / 2]),
         (qml.PhaseShift, [1 / math.sqrt(2), 1 / math.sqrt(2)],
          [1 / math.sqrt(2), 1 / 2 - 1j / 2], [math.pi / 4]),
@@ -269,14 +275,21 @@
         (qml.RY, [1, 0], [1 / math.sqrt(2), -1 / math.sqrt(2)], [math.pi / 2]),
         (qml.RY, [1, 0], [0, -1], [math.pi]),
         (qml.RY, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1, 0], [math.pi / 2]),
         (qml.RZ, [1, 0], [1 / math.sqrt(2) + 1j / math.sqrt(2), 0], [math.pi / 2]),
         (qml.RZ, [0, 1], [0, -1j], [math.pi]),
         (qml.RZ, [1 / math.sqrt(2), 1 / math.sqrt(2)],
          [1 / 2 + 1/2*1j, 1 / 2 - 1/2*1j], [math.pi / 2]),
+        (qml.MultiRZ, [1, 0], [1 / math.sqrt(2) + 1j / math.sqrt(2), 0], [math.pi / 2]),
+        (qml.MultiRZ, [0, 1], [0, -1j], [math.pi]),
+        (qml.MultiRZ, [1 / math.sqrt(2), 1 / math.sqrt(2)],
+         [1 / 2 + 1/2*1j, 1 / 2 - 1/2*1j], [math.pi / 2]),
+        (qml.DiagonalQubitUnitary, [1, 0], [-1, 0], [np.array([-1, 1])]),
+        (qml.DiagonalQubitUnitary, [1 / math.sqrt(2), 1 / math.sqrt(2)], [1 / math.sqrt(2), -1j / math.sqrt(2)], [np.array([1, 1j])]),
+        (qml.DiagonalQubitUnitary, [1 / 2, math.sqrt(3) / 4], [cmath.exp(-1j * 0.4) / 2, cmath.exp(1j * 0.4) * math.sqrt(3) / 4], [np.array([cmath.exp(1j * 0.4), cmath.exp(1j * -0.4)])]),
     ]
 
     @pytest.mark.parametrize("operation,input,expected_output,par", test_data_single_wire_with_parameters)
     def test_apply_operation_single_wire_with_parameters(self, qubit_device_1_wire, tol, operation, input, expected_output, par):
         """Tests that applying an operation yields the expected output state for single wire
            operations that have parameters."""
 
@@ -303,14 +316,17 @@
         (qml.CRX, [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0], [0, 1 / math.sqrt(2), 1 / 2, -1j / 2], [math.pi / 2]),
         (qml.CRY, [0, 0, 0, 1], [0, 0, -1 / math.sqrt(2), 1 / math.sqrt(2)], [math.pi / 2]),
         (qml.CRY, [0, 0, 0, 1], [0, 0, -1, 0], [math.pi]),
         (qml.CRY, [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [math.pi / 2]),
         (qml.CRZ, [0, 0, 0, 1], [0, 0, 0, 1 / math.sqrt(2) + 1j / math.sqrt(2)], [math.pi / 2]),
         (qml.CRZ, [0, 0, 0, 1], [0, 0, 0, 1j], [math.pi]),
         (qml.CRZ, [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [math.pi / 2]),
+        (qml.MultiRZ, [0, 0, 0, 1], [0, 0, 0, 1 / math.sqrt(2) - 1j / math.sqrt(2)], [math.pi / 2]),
+        (qml.MultiRZ, [0, 0, 1, 0], [0, 0, 1j, 0], [math.pi]),
+        (qml.MultiRZ, [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [1 / 2 - 1j / 2, 1 / 2 + 1j / 2, 0, 0], [math.pi / 2]),
         (qml.CRot, [0, 0, 0, 1], [0, 0, 0, 1 / math.sqrt(2) + 1j / math.sqrt(2)], [math.pi / 2, 0, 0]),
         (qml.CRot, [0, 0, 0, 1], [0, 0, -1 / math.sqrt(2), 1 / math.sqrt(2)], [0, math.pi / 2, 0]),
         (qml.CRot, [0, 0, 1 / math.sqrt(2), 1 / math.sqrt(2)], [0, 0, 1 / 2 - 1j / 2, 1 / 2 + 1j / 2],
          [0, 0, math.pi / 2]),
         (qml.CRot, [0, 0, 0, 1], [0, 0, 1 / math.sqrt(2), 1j / math.sqrt(2)], [math.pi / 2, -math.pi / 2, math.pi / 2]),
         (qml.CRot, [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0], [0, 1 / math.sqrt(2), 0, -1 / 2 + 1j / 2],
          [-math.pi / 2, math.pi, math.pi]),
@@ -319,42 +335,51 @@
              [0, 0, 0, 1]])]),
         (qml.QubitUnitary, [0, 1, 0, 0], [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0], [np.array(
             [[1, 0, 0, 0], [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0], [0, 1 / math.sqrt(2), -1 / math.sqrt(2), 0],
              [0, 0, 0, 1]])]),
         (qml.QubitUnitary, [1 / 2, 1 / 2, -1 / 2, 1 / 2], [1 / 2, 0, 1 / math.sqrt(2), 1 / 2], [np.array(
             [[1, 0, 0, 0], [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0], [0, 1 / math.sqrt(2), -1 / math.sqrt(2), 0],
              [0, 0, 0, 1]])]),
+        (qml.DiagonalQubitUnitary, [1, 0, 0, 0], [-1, 0, 0, 0], [np.array([-1, 1, 1, -1])]),
+        (qml.DiagonalQubitUnitary, [1/math.sqrt(2), 0, 0, 1/math.sqrt(2)], [1/math.sqrt(2), 0, 0, -1/math.sqrt(2)], [np.array([1, 1, 1, -1])]),
+        (qml.DiagonalQubitUnitary, [0, 0, 1, 0], [0, 0, 1j, 0], [np.array([-1, 1j, 1j, -1])]),
     ]
 
     test_data_two_wires_with_parameters_inverses = [
         (qml.CRX, [0, 1, 0, 0], [0, 1, 0, 0], [math.pi / 2]),
         (qml.CRX, [0, 0, 0, 1], [0, 0, 1j, 0], [math.pi]),
         (qml.CRX, [0, 1 / math.sqrt(2), 1 / math.sqrt(2), 0],
          [0, 1 / math.sqrt(2), 1 / 2, 1j / 2], [math.pi / 2]),
+        (qml.MultiRZ, [0, 0, 0, 1], [0, 0, 0, 1 / math.sqrt(2) + 1j / math.sqrt(2)], [math.pi / 2]),
+        (qml.MultiRZ, [0, 0, 1, 0], [0, 0, -1j, 0], [math.pi]),
+        (qml.MultiRZ, [1 / math.sqrt(2), 1 / math.sqrt(2), 0, 0], [1 / 2 + 1j / 2, 1 / 2 - 1j / 2, 0, 0], [math.pi / 2]),
+        (qml.DiagonalQubitUnitary, [1, 0, 0, 0], [-1, 0, 0, 0], [np.array([-1, 1, 1, -1])]),
+        (qml.DiagonalQubitUnitary, [1/math.sqrt(2), 0, 0, 1/math.sqrt(2)], [1/math.sqrt(2), 0, 0, -1/math.sqrt(2)], [np.array([1, 1, 1, -1])]),
+        (qml.DiagonalQubitUnitary, [0, 0, 1, 0], [0, 0, -1j, 0], [np.array([-1, 1j, 1j, -1])]),
     ]
 
     @pytest.mark.parametrize("operation,input,expected_output,par", test_data_two_wires_with_parameters)
     def test_apply_operation_two_wires_with_parameters(self, qubit_device_2_wires, tol, operation, input, expected_output, par):
         """Tests that applying an operation yields the expected output state for two wire
            operations that have parameters."""
 
-        qubit_device_2_wires._state = np.array(input)
+        qubit_device_2_wires._state = np.array(input).reshape((2, 2))
         qubit_device_2_wires.apply([operation(*par, wires=[0, 1])])
 
-        assert np.allclose(qubit_device_2_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_2_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     @pytest.mark.parametrize("operation,input,expected_output,par", test_data_two_wires_with_parameters_inverses)
     def test_apply_operation_two_wires_with_parameters_inverse(self, qubit_device_2_wires, tol, operation, input, expected_output, par):
         """Tests that applying the inverse of an operation yields the expected output state for two wire
            operations that have parameters."""
 
-        qubit_device_2_wires._state = np.array(input)
+        qubit_device_2_wires._state = np.array(input).reshape((2, 2))
         qubit_device_2_wires.apply([operation(*par, wires=[0, 1]).inv()])
 
-        assert np.allclose(qubit_device_2_wires._state, np.array(expected_output), atol=tol, rtol=0)
+        assert np.allclose(qubit_device_2_wires._state.flatten(), np.array(expected_output), atol=tol, rtol=0)
 
     def test_apply_errors_qubit_state_vector(self, qubit_device_2_wires):
         """Test that apply fails for incorrect state preparation, and > 2 qubit gates"""
         with pytest.raises(
             ValueError,
             match="Sum of amplitudes-squared does not equal one."
         ):
@@ -925,14 +950,16 @@
         ("PhaseShift", [-math.pi/4], 1),
         ("RX", [math.pi/2], 0),
         ("RX", [-math.pi/4], 1/math.sqrt(2)),
         ("RY", [math.pi/2], 0),
         ("RY", [-math.pi/4], 1/math.sqrt(2)),
         ("RZ", [math.pi/2], 1),
         ("RZ", [-math.pi/4], 1),
+        ("MultiRZ", [math.pi/2], 1),
+        ("MultiRZ", [-math.pi/4], 1),
         ("Rot", [math.pi/2, 0, 0], 1),
         ("Rot", [0, math.pi/2, 0], 0),
         ("Rot", [0, 0, math.pi/2], 1),
         ("Rot", [math.pi/2, -math.pi/4, -math.pi/4], 1/math.sqrt(2)),
         ("Rot", [-math.pi/4, math.pi/2, math.pi/4], 0),
         ("Rot", [-math.pi/4, math.pi/4, math.pi/2], 1/math.sqrt(2)),
         ("QubitUnitary", [np.array([[1j/math.sqrt(2), 1j/math.sqrt(2)], [1j/math.sqrt(2), -1j/math.sqrt(2)]])], 0),
@@ -959,14 +986,17 @@
         ("CRX", [math.pi/2], [-1/2, 1/4]),
         ("CRY", [0], [-1/2, -1/2]),
         ("CRY", [-math.pi], [-1/2, 1]),
         ("CRY", [math.pi/2], [-1/2, 1/4]),
         ("CRZ", [0], [-1/2, -1/2]),
         ("CRZ", [-math.pi], [-1/2, -1/2]),
         ("CRZ", [math.pi/2], [-1/2, -1/2]),
+        ("MultiRZ", [0], [-1/2, -1/2]),
+        ("MultiRZ", [-math.pi], [-1/2, -1/2]),
+        ("MultiRZ", [math.pi/2], [-1/2, -1/2]),
         ("CRot", [math.pi/2, 0, 0], [-1/2, -1/2]),
         ("CRot", [0, math.pi/2, 0], [-1/2, 1/4]),
         ("CRot", [0, 0, math.pi/2], [-1/2, -1/2]),
         ("CRot", [math.pi/2, 0, -math.pi], [-1/2, -1/2]),
         ("CRot", [0, math.pi/2, -math.pi], [-1/2, 1/4]),
         ("CRot", [-math.pi, 0, math.pi/2], [-1/2, -1/2]),
         ("QubitUnitary", [np.array([[1, 0, 0, 0], [0, 1/math.sqrt(2), 1/math.sqrt(2), 0], [0, 1/math.sqrt(2), -1/math.sqrt(2), 0], [0, 0, 0, 1]])], [-1/2, -1/2]),
@@ -1590,7 +1620,54 @@
                     - 11 * np.cos(2 * varphi)
                     + 42 * np.sin(varphi)
                     + 3 * np.sin(2 * varphi)
                 )
             )
         ) / 16
         assert np.allclose(var, expected, atol=tol, rtol=0)
+
+class TestProbabilityIntegration:
+    """Test probability method for when analytic is True/False"""
+
+    def mock_analytic_counter(self, wires=None):
+        self.analytic_counter += 1
+        return np.array([1, 0, 0, 0], dtype=float)
+
+    @pytest.mark.parametrize("x", [[0.2, 0.5], [0.4, 0.9], [0.8, 0.3]])
+    def test_probability(self, x, tol):
+        """Test that the probability function works when analytic=False"""
+        dev = qml.device("default.qubit", wires=2, analytic=False)
+        dev_analytic = qml.device("default.qubit", wires=2, analytic=True)
+
+        def circuit(x):
+            qml.RX(x[0], wires=0)
+            qml.RY(x[1], wires=0)
+            qml.CNOT(wires=[0, 1])
+            return qml.probs(wires=[0, 1])
+
+        prob = qml.QNode(circuit, dev)
+        prob_analytic = qml.QNode(circuit, dev_analytic)
+
+        assert np.isclose(prob(x).sum(), 1, atol=tol, rtol=0)
+        assert np.allclose(prob_analytic(x), prob(x), atol=0.1, rtol=0)
+        assert not np.array_equal(prob_analytic(x), prob(x))
+
+    @pytest.mark.parametrize("analytic", [True, False])
+    def test_call_generate_samples(self, analytic, monkeypatch):
+        """Test analytic_probability call when generating samples"""
+        self.analytic_counter = False
+
+        dev = qml.device("default.qubit", wires=2, analytic=analytic)
+        monkeypatch.setattr(dev, "analytic_probability", self.mock_analytic_counter)
+
+        # generate samples through `generate_samples` (using 'analytic_probability')
+        dev.generate_samples()
+
+        # should call `analytic_probability` once through `generate_samples`
+        assert self.analytic_counter == 1
+
+    def test_stateless_analytic_return(self):
+        """Test that analytic_probability returns None if device is stateless"""
+        dev = qml.device("default.qubit", wires=2)
+        dev._state = None
+
+        assert dev.analytic_probability() is None
```

### Comparing `PennyLane-0.8.1/tests/test_device.py` & `PennyLane-0.9.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_hermitian_edge_cases.py` & `PennyLane-0.9.0/tests/test_hermitian_edge_cases.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_io.py` & `PennyLane-0.9.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_observable.py` & `PennyLane-0.9.0/tests/test_observable.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_operation.py` & `PennyLane-0.9.0/tests/test_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 # pylint: disable=no-self-use, no-member, protected-access, pointless-statement
 
 # Operation subclasses to test
 op_classes = [getattr(qml.ops, cls) for cls in qml.ops.__all__]
 op_classes_cv = [getattr(qml.ops, cls) for cls in qml.ops._cv__all__]
 op_classes_gaussian = [cls for cls in op_classes_cv if cls.supports_heisenberg]
 
+op_classes_param_testable = op_classes.copy()
+op_classes_param_testable.remove(qml.ops.PauliRot)
+
 def U3(theta, phi, lam):
     return Rphi(phi) @ Rphi(lam) @ Rot3(lam, theta, -lam)
 
 
 class TestOperation:
     """Operation class tests."""
 
@@ -105,15 +108,15 @@
             op.heisenberg_expand(U_wrong_size, len(op.wires))
 
         # ensure that `heisenberg_expand` raises exception if it receives an array with order > 2
         with pytest.raises(ValueError, match='Only order-1 and order-2 arrays supported'):
             U_high_order = np.array([U] * 3)
             op.heisenberg_expand(U_high_order, len(op.wires))
 
-    @pytest.mark.parametrize("test_class", op_classes)
+    @pytest.mark.parametrize("test_class", op_classes_param_testable)
     def test_operation_init(self, test_class, monkeypatch):
         "Operation subclass initialization."
 
         n = test_class.num_params
         w = test_class.num_wires
         ww = list(range(w))
         # valid pars
@@ -150,40 +153,41 @@
                 with pytest.raises(ValueError, match='wires must be unique'):
                     test_class(*pars, wires=w*[0])
 
         if n == 0:
             return
 
         # wrong parameter types
-        if test_class.par_domain == 'A':
-            # params must be arrays
-            with pytest.raises(TypeError, match='Array parameter expected'):
-                test_class(*n*[0.0], wires=ww)
-            # params must not be Variables
-            with pytest.raises(TypeError, match='Array parameter expected'):
-                test_class(*n*[qml.variable.Variable(0)], wires=ww)
-        elif test_class.par_domain == 'N':
-            # params must be natural numbers
-            with pytest.raises(TypeError, match='Natural number'):
-                test_class(*n*[0.7], wires=ww)
-            with pytest.raises(TypeError, match='Natural number'):
-                test_class(*n*[-1], wires=ww)
-        elif test_class.par_domain == 'R':
-            # params must be real numbers
-            with pytest.raises(TypeError, match='Real scalar parameter expected'):
-                test_class(*n*[1j], wires=ww)
-
-        # if par_domain ever gets overridden to an unsupported value, should raise exception
-        monkeypatch.setattr(test_class, 'par_domain', 'junk')
-        with pytest.raises(ValueError, match='Unknown parameter domain'):
-            test_class(*pars, wires=ww)
-
-        monkeypatch.setattr(test_class, 'par_domain', 7)
-        with pytest.raises(ValueError, match='Unknown parameter domain'):
-            test_class(*pars, wires=ww)
+        if test_class.do_check_domain:
+            if test_class.par_domain == 'A':
+                # params must be arrays
+                with pytest.raises(TypeError, match='Array parameter expected'):
+                    test_class(*n*[0.0], wires=ww)
+                # params must not be Variables
+                with pytest.raises(TypeError, match='Array parameter expected'):
+                    test_class(*n*[qml.variable.Variable(0)], wires=ww)
+            elif test_class.par_domain == 'N':
+                # params must be natural numbers
+                with pytest.raises(TypeError, match='Natural number'):
+                    test_class(*n*[0.7], wires=ww)
+                with pytest.raises(TypeError, match='Natural number'):
+                    test_class(*n*[-1], wires=ww)
+            elif test_class.par_domain == 'R':
+                # params must be real numbers
+                with pytest.raises(TypeError, match='Real scalar parameter expected'):
+                    test_class(*n*[1j], wires=ww)
+
+            # if par_domain ever gets overridden to an unsupported value, should raise exception
+            monkeypatch.setattr(test_class, 'par_domain', 'junk')
+            with pytest.raises(ValueError, match='Unknown parameter domain'):
+                test_class(*pars, wires=ww)
+
+            monkeypatch.setattr(test_class, 'par_domain', 7)
+            with pytest.raises(ValueError, match='Unknown parameter domain'):
+                test_class(*pars, wires=ww)
 
     @pytest.fixture(scope="function")
     def qnode(self, mock_device):
         """Provides a QNode for the subsequent tests of do_queue"""
 
         def circuit(x):
             qml.RX(x, wires=[0])
@@ -506,27 +510,54 @@
             par_domain = 'N'
             grad_method = None
 
         assert issubclass(DummyObserv, qml.operation.Operator)
         assert issubclass(DummyObserv, qml.operation.Observable)
         assert issubclass(DummyObserv, qml.operation.Operation)
 
+    def test_tensor_n_multiple_modes(self):
+        """Checks that the TensorN operator was constructed correctly when
+        multiple modes were specified."""
+        cv_obs = qml.TensorN(wires=[0, 1])
+
+        assert isinstance(cv_obs, qml.TensorN)
+        assert cv_obs.wires == [0, 1]
+        assert cv_obs.ev_order is None
+
+    def test_tensor_n_single_mode_wires_explicit(self):
+        """Checks that instantiating a TensorN when passing a single mode as a
+        keyword argument returns a NumberOperator."""
+        cv_obs = qml.TensorN(wires=[0])
+
+        assert isinstance(cv_obs, qml.NumberOperator)
+        assert cv_obs.wires == [0]
+        assert cv_obs.ev_order == 2
+
+    def test_tensor_n_single_mode_wires_implicit(self):
+        """Checks that instantiating TensorN when passing a single mode as a
+        positional argument returns a NumberOperator."""
+        cv_obs = qml.TensorN(1)
+
+        assert isinstance(cv_obs, qml.NumberOperator)
+        assert cv_obs.wires == [1]
+        assert cv_obs.ev_order == 2
+
 
 class TestOperatorIntegration:
     """ Integration tests for the Operator class"""
 
     def test_all_wires_defined_but_init_with_one(self):
         """Test that an exception is raised if the class is defined with ALL wires,
         but then instantiated with only one"""
 
         dev1 = qml.device("default.qubit", wires=2)
 
         class DummyOp(qml.operation.Operator):
             r"""Dummy custom operator"""
-            num_wires = qml.operation.Wires.All
+            num_wires = qml.operation.ActsOn.AllWires
             num_params = 0
             par_domain = 'R'
 
         @qml.qnode(dev1)
         def circuit():
             DummyOp(wires=[0])
             return qml.expval(qml.PauliZ(0))
@@ -719,15 +750,15 @@
         """Test that the correct eigenvalues are returned for the Tensor"""
         X = qml.PauliX(0)
         Y = qml.PauliY(2)
         t = Tensor(X, Y)
         assert np.array_equal(t.eigvals, np.kron([1, -1], [1, -1]))
 
         # test that the eigvals are now cached and not recalculated
-        assert np.array_equal(t._eigvals, t.eigvals)
+        assert np.array_equal(t._eigvals_cache, t.eigvals)
 
     @pytest.mark.usefixtures("tear_down_hermitian")
     def test_eigvals_hermitian(self, tol):
         """Test that the correct eigenvalues are returned for the Tensor containing an Hermitian observable"""
         X = qml.PauliX(0)
         hamiltonian = np.array([[1,0,0,0], [0,1,0,0], [0,0,0,1], [0,0,1,0]])
         Herm = qml.Hermitian(hamiltonian, wires=[1, 2])
@@ -1027,24 +1058,24 @@
         operation_wires = [0, 1]
 
         with qml.utils.OperationRecorder() as rec:
             qml.CRY.decomposition(phi, wires=operation_wires)
 
         assert len(rec.queue) == 4
 
-        assert rec.queue[0].name == "U3"
-        assert rec.queue[0].parameters == [phi/2, 0, 0]
+        assert rec.queue[0].name == "RY"
+        assert rec.queue[0].parameters == [phi/2]
         assert rec.queue[0].wires == [1]
 
         assert rec.queue[1].name == "CNOT"
         assert rec.queue[1].parameters == []
         assert rec.queue[1].wires == operation_wires
 
-        assert rec.queue[2].name == "U3"
-        assert rec.queue[2].parameters == [-phi/2, 0, 0]
+        assert rec.queue[2].name == "RY"
+        assert rec.queue[2].parameters == [-phi/2]
         assert rec.queue[2].wires == [1]
 
         assert rec.queue[3].name == "CNOT"
         assert rec.queue[3].parameters == []
         assert rec.queue[3].wires == operation_wires
 
     @pytest.mark.parametrize("phi", [0.03236*i for i in range(5)])
```

### Comparing `PennyLane-0.8.1/tests/test_optimize.py` & `PennyLane-0.9.0/tests/test_optimize.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Unit tests for the :mod:`pennylane` :class:`GradientDescentOptimizer` subclasses.
+Unit tests for the :mod:`pennylane` optimizers.
 """
+# pylint: disable=redefined-outer-name
+import itertools as it
 import pytest
 
 import pennylane as qml
 from pennylane import numpy as np
 from pennylane.utils import _flatten
 from pennylane.optimize import (GradientDescentOptimizer,
                                 MomentumOptimizer,
                                 NesterovMomentumOptimizer,
                                 AdagradOptimizer,
                                 RMSPropOptimizer,
-                                AdamOptimizer)
+                                AdamOptimizer,
+                                RotoselectOptimizer,
+                                RotosolveOptimizer)
 
 x_vals = np.linspace(-10, 10, 16, endpoint=False)
 
 # Hyperparameters for optimizers
 stepsize = 0.1
 gamma = 0.5
 delta = 0.8
@@ -117,14 +121,16 @@
     class A:
         sgd_opt = GradientDescentOptimizer(stepsize)
         mom_opt = MomentumOptimizer(stepsize, momentum=gamma)
         nesmom_opt = NesterovMomentumOptimizer(stepsize, momentum=gamma)
         adag_opt = AdagradOptimizer(stepsize)
         rms_opt = RMSPropOptimizer(stepsize, decay=gamma)
         adam_opt = AdamOptimizer(stepsize, beta1=gamma, beta2=delta)
+        rotosolve_opt = RotosolveOptimizer()
+        rotoselect_opt = RotoselectOptimizer()
 
     return A()
 
 
 class TestOptimizer:
     """Basic optimizer tests.
     """
@@ -458,14 +464,127 @@
                 x_twosteps = bunch.adam_opt.step(f, x_onestep)
                 adapted_stepsize = stepsize * np.sqrt(1 - delta**2) / (1 - gamma**2)
                 firstmoment = (gamma * gradf(x_vec) + (1 - gamma) * gradf(x_onestep))
                 secondmoment = (delta * gradf(x_vec) * gradf(x_vec) + (1 - delta) * gradf(x_onestep) * gradf(x_onestep))
                 x_twosteps_target = x_onestep - adapted_stepsize * firstmoment / (np.sqrt(secondmoment) + 1e-8)
                 assert x_twosteps == pytest.approx(x_twosteps_target, abs=tol)
 
+    @staticmethod
+    def rotosolve_step(f, x):
+        """Helper function to test the Rotosolve and Rotoselect optimizers"""
+        # make sure that x is an array
+        if np.ndim(x) == 0:
+            x = np.array([x])
+
+        # helper function for x[d] = theta
+        def insert(xf, d, theta):
+            xf[d] = theta
+            return xf
+
+        for d, _ in enumerate(x):
+            H_0 = float(f(insert(x, d, 0)))
+            H_p = float(f(insert(x, d, np.pi / 2)))
+            H_m = float(f(insert(x, d, -np.pi / 2)))
+
+            a = np.arctan2(2 * H_0 - H_p - H_m, H_p - H_m)
+
+            x[d] = -np.pi / 2 - a
+
+            if x[d] <= -np.pi:
+                x[d] += 2 * np.pi
+        return x
+
+    @pytest.mark.parametrize('x_start', x_vals)
+    def test_rotosolve_optimizer_univar(self, x_start, bunch, tol):
+        """Tests that rotosolve optimizer takes one and two steps correctly
+        for uni-variate functions."""
+
+        for f in univariate_funcs:
+            x_onestep = bunch.rotosolve_opt.step(f, x_start)
+            x_onestep_target = self.rotosolve_step(f, x_start)
+
+            assert x_onestep == pytest.approx(x_onestep_target, abs=tol)
+
+            x_twosteps = bunch.rotosolve_opt.step(f, x_onestep)
+            x_twosteps_target = self.rotosolve_step(f, x_onestep_target)
+
+            assert x_twosteps == pytest.approx(x_twosteps_target, abs=tol)
+
+    @pytest.mark.parametrize('x_start', [[1.2, 0.2],
+                                         [-0.62, -2.1],
+                                         [0.05, 0.8],
+                                         [[0.3], [0.25]],
+                                         [[-0.6], [0.45]],
+                                         [[1.3], [-0.9]]])
+    def test_rotosolve_optimizer_multivar(self, x_start, bunch, tol):
+        """Tests that rotosolve optimizer takes one and two steps correctly
+        for multi-variate functions."""
+
+        for func in multivariate_funcs:
+            # alter multivariate_func to accept nested lists of parameters
+            f = lambda x: func(np.ravel(x))
+
+            x_onestep = bunch.rotosolve_opt.step(f, x_start)
+            x_onestep_target = self.rotosolve_step(f, x_start)
+
+            assert x_onestep == pytest.approx(x_onestep_target, abs=tol)
+
+            x_twosteps = bunch.rotosolve_opt.step(f, x_onestep)
+            x_twosteps_target = self.rotosolve_step(f, x_onestep_target)
+
+            assert x_twosteps == pytest.approx(x_twosteps_target, abs=tol)
+
+    @pytest.mark.parametrize('x_start', [[1.2, 0.2],
+                                         [-0.62, -2.1],
+                                         [0.05, 0.8]])
+    @pytest.mark.parametrize('generators', [list(tup) for tup in it.product([qml.RX, qml.RY, qml.RZ], repeat=2)])
+    def test_rotoselect_optimizer(self, x_start, generators, bunch, tol):
+        """Tests that rotoselect optimizer finds the optimal generators and parameters for the VQE circuit
+        defined in `this rotoselect tutorial <https://pennylane.ai/qml/demos/tutorial_rotoselect.html>`_."""
+
+        # the optimal generators for the 2-qubit VQE circuit
+        # H = 0.5 * Y_2 + 0.8 * Z_1 - 0.2 * X_1
+        optimal_generators = [qml.RY, qml.RX]
+        possible_generators = [qml.RX, qml.RY, qml.RZ]
+        bunch.rotoselect_opt.possible_generators = possible_generators
+
+        dev = qml.device("default.qubit", analytic=True, wires=2)
+
+        def ansatz(params, generators):
+            generators[0](params[0], wires=0)
+            generators[1](params[1], wires=1)
+            qml.CNOT(wires=[0, 1])
+
+        @qml.qnode(dev)
+        def circuit_1(params, generators=None):  # generators will be passed as a keyword arg
+            ansatz(params, generators)
+            return qml.expval(qml.PauliZ(0)), qml.expval(qml.PauliY(1))
+
+        @qml.qnode(dev)
+        def circuit_2(params, generators=None):  # generators will be passed as a keyword arg
+            ansatz(params, generators)
+            return qml.expval(qml.PauliX(0))
+
+        def cost_fn(params, generators):
+            Z_1, Y_2 = circuit_1(params, generators=generators)
+            X_1 = circuit_2(params, generators=generators)
+            return 0.5 * Y_2 + 0.8 * Z_1 - 0.2 * X_1
+
+        f_best_gen = lambda x: cost_fn(x, optimal_generators)
+        optimal_x_start = x_start.copy()
+
+        # after four steps the optimzer should find the optimal generators/x_start values
+        for _ in range(4):
+            x_start, generators = bunch.rotoselect_opt.step(cost_fn, x_start, generators)
+            optimal_x_start = self.rotosolve_step(f_best_gen, optimal_x_start)
+
+        assert x_start == pytest.approx(optimal_x_start, abs=tol)
+        assert generators == optimal_generators
+
+
     def test_update_stepsize(self):
         """Tests that the stepsize correctly updates"""
 
         eta = 0.5
         opt = AdamOptimizer(eta)
         assert opt._stepsize == eta
```

### Comparing `PennyLane-0.8.1/tests/test_prob.py` & `PennyLane-0.9.0/tests/test_prob.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,27 @@
     # expected probability, using [00, 01, 10, 11]
     # ordering, is [0.5, 0.5, 0, 0]
 
     res = circuit()
     expected = np.array([0.5, 0.5, 0, 0])
     assert np.allclose(res, expected, atol=tol, rtol=0)
 
+def test_integration_analytic_false(tol):
+    """Test the probability is correct for a known state preparation when the
+    analytic attribute is set to False."""
+    dev = qml.device('default.qubit', wires=3, analytic=False)
+
+    @qml.qnode(dev)
+    def circuit():
+        qml.PauliX(0)
+        return qml.probs(wires=[0])
+
+    res = circuit()
+    expected = np.array([0, 1])
+    assert np.allclose(res, expected, atol=tol, rtol=0)
 
 def test_numerical_analytic_diff_agree(init_state, tol):
     """Test that the finite difference and parameter shift rule
     provide the same Jacobian."""
     w = 4
     dev = qml.device("default.qubit", wires=w)
     state = init_state(w)
```

### Comparing `PennyLane-0.8.1/tests/test_quantum_gradients.py` & `PennyLane-0.9.0/tests/test_quantum_gradients.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_qubit_device.py` & `PennyLane-0.9.0/tests/test_qubit_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
         circuit_graph = CircuitGraph(queue + observables, {})
 
         call_history = []
 
         with monkeypatch.context() as m:
             m.setattr(QubitDevice, "apply", lambda self, x, **kwargs: call_history.extend(x + kwargs.get('rotations', [])))
+            m.setattr(QubitDevice, "analytic_probability", lambda *args: None)
             mock_qubit_device_with_paulis_and_methods.execute(circuit_graph)
 
         assert call_history == queue
 
         assert len(call_history) == 3
         assert isinstance(call_history[0], qml.PauliX)
         assert call_history[0].wires == [0]
@@ -332,14 +333,15 @@
 
         number_of_states = 2 ** mock_qubit_device.num_wires
 
         with monkeypatch.context() as m:
             # Mock the auxiliary methods such that they return the expected values
             m.setattr(QubitDevice, "sample_basis_states", lambda self, wires, b: wires)
             m.setattr(QubitDevice, "states_to_binary", lambda a, b: (a, b))
+            m.setattr(QubitDevice, "analytic_probability", lambda *args: None)
             mock_qubit_device._samples = mock_qubit_device.generate_samples()
 
         assert mock_qubit_device._samples == (number_of_states, mock_qubit_device.num_wires)
 
 
 class TestSampleBasisStates:
     """Test the sample_basis_states method"""
```

### Comparing `PennyLane-0.8.1/tests/test_tensor_measurements.py` & `PennyLane-0.9.0/tests/test_tensor_measurements.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_utils.py` & `PennyLane-0.9.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -203,14 +203,31 @@
         assert np.allclose(res, expected, atol=tol, rtol=0)
 
         # test applied to wire 2
         res = pu.expand(U, [2], 3)
         expected = np.kron(np.kron(I, I), U)
         assert np.allclose(res, expected, atol=tol, rtol=0)
 
+    def test_expand_one_wires_list(self, tol):
+        """Test that a 1 qubit gate correctly expands to 3 qubits."""
+        # test applied to wire 0
+        res = pu.expand(U, [0], [0, 4, 9])
+        expected = np.kron(np.kron(U, I), I)
+        assert np.allclose(res, expected, atol=tol, rtol=0)
+
+        # test applied to wire 4
+        res = pu.expand(U, [4], [0, 4, 9])
+        expected = np.kron(np.kron(I, U), I)
+        assert np.allclose(res, expected, atol=tol, rtol=0)
+
+        # test applied to wire 9
+        res = pu.expand(U, [9], [0, 4, 9])
+        expected = np.kron(np.kron(I, I), U)
+        assert np.allclose(res, expected, atol=tol, rtol=0)
+
     def test_expand_two_consecutive_wires(self, tol):
         """Test that a 2 qubit gate on consecutive wires correctly
         expands to 4 qubits."""
 
         # test applied to wire 0+1
         res = pu.expand(U2, [0, 1], 4)
         expected = np.kron(np.kron(U2, I), I)
@@ -235,15 +252,15 @@
         rows = np.array([0, 2, 1, 3])
         expected = np.kron(np.kron(CNOT[:, rows][rows], I), I)
         assert np.allclose(res, expected, atol=tol, rtol=0)
 
     def test_expand_invalid_wires(self):
         """test exception raised if unphysical subsystems provided."""
         with pytest.raises(
-            ValueError, match="Invalid target subsystems provided in 'wires' argument."
+            ValueError, match="Invalid target subsystems provided in 'original_wires' argument"
         ):
             pu.expand(U2, [-1, 5], 4)
 
     def test_expand_invalid_matrix(self):
         """test exception raised if incorrect sized matrix provided/"""
         with pytest.raises(ValueError, match="Matrix parameter must be of size"):
             pu.expand(U, [0, 1], 4)
@@ -298,135 +315,82 @@
         expected = (
             np.kron(SWAP, np.kron(I, I))
             @ np.kron(I, U_toffoli[:, rows][rows])
             @ np.kron(SWAP, np.kron(I, I))
         )
         assert np.allclose(res, expected, atol=tol, rtol=0)
 
+    VECTOR1 = np.array([1, -1])
+    ONES = np.array([1, 1])
 
-class TestRecorder:
-    """Test the Recorder QNode replacement"""
-
-    def test_append_op_calls_underlying_context(self):
-        """Test that the underlying context is called in _append_op."""
-        qnode_mock = MagicMock()
-
-        rec = pu.Recorder(qnode_mock)
-        op = qml.PauliZ(3)
-        rec._append_op(op)
-
-        assert qnode_mock._append_op.call_args[0][0] == op
-        assert rec._ops == [op]
-
-    def test_append_op_no_context(self):
-        """Test that the operation is appended when no context is supplied."""
-        rec = pu.Recorder(None)
-
-        op = qml.PauliZ(3)
-        rec._append_op(op)
-
-        assert rec._ops == [op]
-
-    def test_remove_op_calls_underlying_context(self):
-        """Test that the underlying context is called in _remove_op."""
-        qnode_mock = MagicMock()
-
-        rec = pu.Recorder(qnode_mock)
-        op = qml.PauliZ(3)
-        rec._append_op(op)
-        rec._remove_op(op)
-
-        assert qnode_mock._remove_op.call_args[0][0] == op
-        assert rec._ops == []
-
-    def test_remove_op_no_context(self):
-        """Test that the operation is removed when no context is supplied."""
-        rec = pu.Recorder(None)
-
-        op = qml.PauliZ(3)
-        rec._append_op(op)
-        assert rec._ops == [op]
-
-        rec._remove_op(op)
+    @pytest.mark.parametrize(
+        "original_wires,expanded_wires,expected",
+        [
+            ([0], 3, np.kron(np.kron(VECTOR1, ONES), ONES)),
+            ([1], 3, np.kron(np.kron(ONES, VECTOR1), ONES)),
+            ([2], 3, np.kron(np.kron(ONES, ONES), VECTOR1)),
+            ([0], [0, 4, 7], np.kron(np.kron(VECTOR1, ONES), ONES)),
+            ([4], [0, 4, 7], np.kron(np.kron(ONES, VECTOR1), ONES)),
+            ([7], [0, 4, 7], np.kron(np.kron(ONES, ONES), VECTOR1)),
+            ([0], [0, 4, 7], np.kron(np.kron(VECTOR1, ONES), ONES)),
+            ([4], [4, 0, 7], np.kron(np.kron(VECTOR1, ONES), ONES)),
+            ([7], [7, 4, 0], np.kron(np.kron(VECTOR1, ONES), ONES)),
+        ],
+    )
+    def test_expand_vector_single_wire(self, original_wires, expanded_wires, expected, tol):
+        """Test that expand_vector works with a single-wire vector."""
+
+        res = pu.expand_vector(TestExpand.VECTOR1, original_wires, expanded_wires)
 
-        assert rec._ops == []
-
-    def test_context_method_spoofing(self):
-        """Test that unknown methods are properly relayed to the underlying context."""
-
-        class MethodMock:
-            args = []
-
-            def construct(self, arg):
-                self.args.append(arg)
-
-        qnode_mock = MethodMock()
-
-        rec = pu.Recorder(qnode_mock)
-
-        rec.construct("Test")
-        assert qnode_mock.args[0] == "Test"
-
-    def test_context_attribute_spoofing(self):
-        """Test that unknown attributes are properly relayed to the underlying context."""
-
-        class AssignmentMock:
-            queue = ["A"]
-
-        qnode_mock = AssignmentMock()
-        rec = pu.Recorder(qnode_mock)
-
-        assert rec.queue == ["A"]
-        assert qnode_mock.queue == ["A"]
+        assert np.allclose(res, expected, atol=tol, rtol=0)
 
-        rec.queue.append("B")
+    VECTOR2 = np.array([1, 2, 3, 4])
+    ONES = np.array([1, 1])
+
+    @pytest.mark.parametrize(
+        "original_wires,expanded_wires,expected",
+        [
+            ([0, 1], 3, np.kron(VECTOR2, ONES)),
+            ([1, 2], 3, np.kron(ONES, VECTOR2)),
+            ([0, 2], 3, np.array([1, 2, 1, 2, 3, 4, 3, 4])),
+            ([0, 5], [0, 5, 9], np.kron(VECTOR2, ONES)),
+            ([5, 9], [0, 5, 9], np.kron(ONES, VECTOR2)),
+            ([0, 9], [0, 5, 9], np.array([1, 2, 1, 2, 3, 4, 3, 4])),
+            ([9, 0], [0, 5, 9], np.array([1, 3, 1, 3, 2, 4, 2, 4])),
+        ],
+    )
+    def test_expand_vector_two_wires(self, original_wires, expanded_wires, expected, tol):
+        """Test that expand_vector works with a single-wire vector."""
 
-        assert rec.queue == ["A", "B"]
-        assert qnode_mock.queue == ["A", "B"]
+        res = pu.expand_vector(TestExpand.VECTOR2, original_wires, expanded_wires)
 
-    def test_attribute_spoofing_error(self):
-        """Test that the proper error is raised if attribute spoofing is attemped
-        with no underlying QNode."""
-        rec = pu.Recorder(None)
+        assert np.allclose(res, expected, atol=tol, rtol=0)
 
+    def test_expand_vector_invalid_wires(self):
+        """Test exception raised if unphysical subsystems provided."""
         with pytest.raises(
-            AttributeError, match="Attribute test of Recorder mock QNode does not exist"
+            ValueError, match="Invalid target subsystems provided in 'original_wires' argument"
         ):
-            rec.test
-
-    def test_queue_no_context(self):
-        """Test that the queue property returns an empty list if there is no underlying context."""
-        qnode_mock = MagicMock()
-        qnode_mock.queue = ["A"]
-
-        rec = pu.Recorder(qnode_mock)
+            pu.expand_vector(TestExpand.VECTOR2, [-1, 5], 4)
 
-        assert rec.queue == ["A"]
-
-    def test_queue_no_context(self):
-        """Test that the queue property returns an empty list if there is no underlying context."""
-        rec = pu.Recorder(None)
-
-        assert rec.queue == []
+    def test_expand_vector_invalid_vector(self):
+        """Test exception raised if incorrect sized vector provided."""
+        with pytest.raises(ValueError, match="Vector parameter must be of length"):
+            pu.expand_vector(TestExpand.VECTOR1, [0, 1], 4)
 
 
 class TestOperationRecorder:
     """Test the OperationRecorder class."""
 
-    def test_context_switching(self, monkeypatch):
-        """Test that the current QNode context is properly switched."""
-        monkeypatch.setattr(qml, "_current_context", "Test")
-
-        assert qml._current_context == "Test"
-
+    def test_context_adding(self, monkeypatch):
+        """Test that the OperationRecorder is added to the list of contexts."""
         with pu.OperationRecorder() as recorder:
-            assert recorder.old_context == "Test"
-            assert qml._current_context == recorder.rec
+            assert recorder in qml.QueuingContext._active_contexts
 
-        assert qml._current_context == "Test"
+        assert recorder not in qml.QueuingContext._active_contexts
 
     def test_circuit_integration(self):
         """Tests that the OperationRecorder integrates well with the
         core behaviour of PennyLane."""
         expected_output = (
             "Operations\n"
             + "==========\n"
```

### Comparing `PennyLane-0.8.1/tests/test_variable.py` & `PennyLane-0.9.0/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `PennyLane-0.8.1/tests/test_vqe.py` & `PennyLane-0.9.0/tests/test_vqe.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,28 @@
     @pytest.mark.parametrize("ansatz", JUNK_INPUTS)
     def test_cost_invalid_ansatz(self, ansatz, mock_device):
         """Tests that the cost function raises an exception if the ansatz is not valid"""
         hamiltonian = qml.vqe.Hamiltonian((1.0,), [qml.PauliZ(0)])
         with pytest.raises(ValueError, match="not a callable function."):
             cost = qml.VQECost(4, hamiltonian, mock_device)
 
+    @pytest.mark.parametrize("coeffs, observables, expected", hamiltonians_with_expvals)
+    def test_passing_kwargs(self, coeffs, observables, expected):
+        """Test that the step size and order used for the finite differences
+        differentiation method were passed to the QNode instances using the
+        keyword arguments."""
+        dev = qml.device("default.qubit", wires=2)
+        hamiltonian = qml.vqe.Hamiltonian(coeffs, observables)
+        cost = qml.VQECost(lambda params, **kwargs: None, hamiltonian, dev, h=123, order=2)
+
+        # Checking that the qnodes contain the step size and order
+        for qnode in cost.qnodes:
+            assert qnode.h == 123
+            assert qnode.order == 2
+
 
 class TestAutogradInterface:
     """Tests for the Autograd interface (and the NumPy interface for backward compatibility)"""
 
     @pytest.mark.parametrize("ansatz, params", CIRCUITS)
     @pytest.mark.parametrize("observables", OBSERVABLES)
     @pytest.mark.parametrize("interface", ["autograd", "numpy"])
```

