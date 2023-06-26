# Comparing `tmp/azureml_train_core-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_train_core-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,71 @@
-Zip file size: 8636949 bytes, number of entries: 69
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/__init__.py
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/__init__.py
--rw-rw-rw-  2.0 fat     5115 b- defN 20-Jun-22 17:21 azureml/train/_distributed_training.py
--rw-rw-rw-  2.0 fat    24425 b- defN 20-Jun-22 17:21 azureml/train/_estimator_helper.py
--rw-rw-rw-  2.0 fat    16238 b- defN 20-Jun-22 17:21 azureml/train/_script_validation.py
--rw-rw-rw-  2.0 fat     3120 b- defN 20-Jun-22 17:21 azureml/train/_telemetry_logger.py
--rw-rw-rw-  2.0 fat    18289 b- defN 20-Jun-22 17:22 azureml/train/sklearn.py
--rw-rw-rw-  2.0 fat      628 b- defN 20-Jun-22 17:21 azureml/train/dnn/__init__.py
--rw-rw-rw-  2.0 fat    23488 b- defN 20-Jun-22 17:22 azureml/train/dnn/_chainer.py
--rw-rw-rw-  2.0 fat    25235 b- defN 20-Jun-22 17:22 azureml/train/dnn/_pytorch.py
--rw-rw-rw-  2.0 fat    29640 b- defN 20-Jun-22 17:22 azureml/train/dnn/_tensorflow.py
--rw-rw-rw-  2.0 fat      791 b- defN 20-Jun-22 17:21 azureml/train/estimator/__init__.py
--rw-rw-rw-  2.0 fat    25524 b- defN 20-Jun-22 17:22 azureml/train/estimator/_estimator.py
--rw-rw-rw-  2.0 fat    17883 b- defN 20-Jun-22 17:21 azureml/train/estimator/_framework_base_estimator.py
--rw-rw-rw-  2.0 fat    20623 b- defN 20-Jun-22 17:21 azureml/train/estimator/_mml_base_estimator.py
--rw-rw-rw-  2.0 fat      206 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/chainer-5.1.0-cpu.yml
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/chainer-5.1.0-gpu.yml
--rw-rw-rw-  2.0 fat      206 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/chainer-7.0.0-cpu.yml
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/chainer-7.0.0-gpu.yml
--rw-rw-rw-  2.0 fat       68 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/lightgbm-2.2.3-cpu.yml
--rw-rw-rw-  2.0 fat      184 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/mockframework-1.0-cpu.yml
--rw-rw-rw-  2.0 fat      202 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/mockframework-1.0-gpu.yml
--rw-rw-rw-  2.0 fat      184 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/mockframework-1.1-cpu.yml
--rw-rw-rw-  2.0 fat      202 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/mockframework-1.1-gpu.yml
--rw-rw-rw-  2.0 fat      230 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.0-cpu.yml
--rw-rw-rw-  2.0 fat      248 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.0-gpu.yml
--rw-rw-rw-  2.0 fat      279 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.1-cpu.yml
--rw-rw-rw-  2.0 fat      297 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.1-gpu.yml
--rw-rw-rw-  2.0 fat      279 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.2-cpu.yml
--rw-rw-rw-  2.0 fat      297 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.2-gpu.yml
--rw-rw-rw-  2.0 fat      281 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.3-cpu.yml
--rw-rw-rw-  2.0 fat      299 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.3-gpu.yml
--rw-rw-rw-  2.0 fat      279 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.4-cpu.yml
--rw-rw-rw-  2.0 fat      299 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.4-gpu.yml
--rw-rw-rw-  2.0 fat      279 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.5-cpu.yml
--rw-rw-rw-  2.0 fat      299 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/pytorch-1.5-gpu.yml
--rw-rw-rw-  2.0 fat      240 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/sklearn-0.20.3-cpu.yml
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.10-cpu.yml
--rw-rw-rw-  2.0 fat      274 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.10-gpu.yml
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.12-cpu.yml
--rw-rw-rw-  2.0 fat      274 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.12-gpu.yml
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.13-cpu.yml
--rw-rw-rw-  2.0 fat      275 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-1.13-gpu.yml
--rw-rw-rw-  2.0 fat      248 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-2.0-cpu.yml
--rw-rw-rw-  2.0 fat      272 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-2.0-gpu.yml
--rw-rw-rw-  2.0 fat      218 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-2.1-cpu.yml
--rw-rw-rw-  2.0 fat      238 b- defN 20-Jun-22 17:21 azureml/train/estimator/scenarios/tensorflow-2.1-gpu.yml
--rw-rw-rw-  2.0 fat     2314 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/__init__.py
--rw-rw-rw-  2.0 fat    11345 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/_search.py
--rw-rw-rw-  2.0 fat     3647 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/exceptions.py
--rw-rw-rw-  2.0 fat     8548 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/parameter_expressions.py
--rw-rw-rw-  2.0 fat    21063 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/policy.py
--rw-rw-rw-  2.0 fat    21078 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/run.py
--rw-rw-rw-  2.0 fat    47707 b- defN 20-Jun-22 17:22 azureml/train/hyperdrive/runconfig.py
--rw-rw-rw-  2.0 fat    15763 b- defN 20-Jun-22 17:21 azureml/train/hyperdrive/sampling.py
--rw-rw-rw-  2.0 fat  2630689 b- defN 20-Jun-22 17:21 azureml/train/metadata/a-i.zip
--rw-rw-rw-  2.0 fat   569801 b- defN 20-Jun-22 17:21 azureml/train/metadata/conda-mapping.zip
--rw-rw-rw-  2.0 fat   961731 b- defN 20-Jun-22 17:21 azureml/train/metadata/dependencies.zip
--rw-rw-rw-  2.0 fat  2645746 b- defN 20-Jun-22 17:21 azureml/train/metadata/j-r.zip
--rw-rw-rw-  2.0 fat  1734403 b- defN 20-Jun-22 17:21 azureml/train/metadata/s-z.zip
--rw-rw-rw-  2.0 fat    13280 b- defN 20-Jun-22 17:21 azureml/train/metadata/stdlib
--rw-rw-rw-  2.0 fat       84 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat       96 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat     1252 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1019 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat     7058 b- defN 20-Jun-22 17:22 azureml_train_core-1.8.0.dist-info/RECORD
-69 files, 8917001 bytes uncompressed, 8625425 bytes compressed:  3.3%
+Zip file size: 8636968 bytes, number of entries: 69
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/__init__.py
+-rw-rw-rw-  2.0 fat     5115 b- defN 20-Jul-06 20:24 azureml/train/_distributed_training.py
+-rw-rw-rw-  2.0 fat    24425 b- defN 20-Jul-06 20:24 azureml/train/_estimator_helper.py
+-rw-rw-rw-  2.0 fat    16238 b- defN 20-Jul-06 20:24 azureml/train/_script_validation.py
+-rw-rw-rw-  2.0 fat     3120 b- defN 20-Jul-06 20:24 azureml/train/_telemetry_logger.py
+-rw-rw-rw-  2.0 fat    18289 b- defN 20-Jul-06 20:26 azureml/train/sklearn.py
+-rw-rw-rw-  2.0 fat      628 b- defN 20-Jul-06 20:24 azureml/train/dnn/__init__.py
+-rw-rw-rw-  2.0 fat    23488 b- defN 20-Jul-06 20:26 azureml/train/dnn/_chainer.py
+-rw-rw-rw-  2.0 fat    25235 b- defN 20-Jul-06 20:26 azureml/train/dnn/_pytorch.py
+-rw-rw-rw-  2.0 fat    29640 b- defN 20-Jul-06 20:26 azureml/train/dnn/_tensorflow.py
+-rw-rw-rw-  2.0 fat      791 b- defN 20-Jul-06 20:24 azureml/train/estimator/__init__.py
+-rw-rw-rw-  2.0 fat    25524 b- defN 20-Jul-06 20:26 azureml/train/estimator/_estimator.py
+-rw-rw-rw-  2.0 fat    17883 b- defN 20-Jul-06 20:24 azureml/train/estimator/_framework_base_estimator.py
+-rw-rw-rw-  2.0 fat    20623 b- defN 20-Jul-06 20:24 azureml/train/estimator/_mml_base_estimator.py
+-rw-rw-rw-  2.0 fat      206 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/chainer-5.1.0-cpu.yml
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/chainer-5.1.0-gpu.yml
+-rw-rw-rw-  2.0 fat      206 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/chainer-7.0.0-cpu.yml
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/chainer-7.0.0-gpu.yml
+-rw-rw-rw-  2.0 fat       68 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/lightgbm-2.2.3-cpu.yml
+-rw-rw-rw-  2.0 fat      184 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/mockframework-1.0-cpu.yml
+-rw-rw-rw-  2.0 fat      202 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/mockframework-1.0-gpu.yml
+-rw-rw-rw-  2.0 fat      184 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/mockframework-1.1-cpu.yml
+-rw-rw-rw-  2.0 fat      202 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/mockframework-1.1-gpu.yml
+-rw-rw-rw-  2.0 fat      230 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.0-cpu.yml
+-rw-rw-rw-  2.0 fat      248 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.0-gpu.yml
+-rw-rw-rw-  2.0 fat      279 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.1-cpu.yml
+-rw-rw-rw-  2.0 fat      297 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.1-gpu.yml
+-rw-rw-rw-  2.0 fat      279 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.2-cpu.yml
+-rw-rw-rw-  2.0 fat      297 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.2-gpu.yml
+-rw-rw-rw-  2.0 fat      281 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.3-cpu.yml
+-rw-rw-rw-  2.0 fat      299 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.3-gpu.yml
+-rw-rw-rw-  2.0 fat      279 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.4-cpu.yml
+-rw-rw-rw-  2.0 fat      299 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.4-gpu.yml
+-rw-rw-rw-  2.0 fat      279 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.5-cpu.yml
+-rw-rw-rw-  2.0 fat      299 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/pytorch-1.5-gpu.yml
+-rw-rw-rw-  2.0 fat      240 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/sklearn-0.20.3-cpu.yml
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.10-cpu.yml
+-rw-rw-rw-  2.0 fat      274 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.10-gpu.yml
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.12-cpu.yml
+-rw-rw-rw-  2.0 fat      274 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.12-gpu.yml
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.13-cpu.yml
+-rw-rw-rw-  2.0 fat      275 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-1.13-gpu.yml
+-rw-rw-rw-  2.0 fat      248 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-2.0-cpu.yml
+-rw-rw-rw-  2.0 fat      272 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-2.0-gpu.yml
+-rw-rw-rw-  2.0 fat      218 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-2.1-cpu.yml
+-rw-rw-rw-  2.0 fat      238 b- defN 20-Jul-06 20:24 azureml/train/estimator/scenarios/tensorflow-2.1-gpu.yml
+-rw-rw-rw-  2.0 fat     2314 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/__init__.py
+-rw-rw-rw-  2.0 fat    11345 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/_search.py
+-rw-rw-rw-  2.0 fat     3647 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/exceptions.py
+-rw-rw-rw-  2.0 fat     8548 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/parameter_expressions.py
+-rw-rw-rw-  2.0 fat    21063 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/policy.py
+-rw-rw-rw-  2.0 fat    21078 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/run.py
+-rw-rw-rw-  2.0 fat    47707 b- defN 20-Jul-06 20:26 azureml/train/hyperdrive/runconfig.py
+-rw-rw-rw-  2.0 fat    15914 b- defN 20-Jul-06 20:24 azureml/train/hyperdrive/sampling.py
+-rw-rw-rw-  2.0 fat  2630689 b- defN 20-Jul-06 20:24 azureml/train/metadata/a-i.zip
+-rw-rw-rw-  2.0 fat   569801 b- defN 20-Jul-06 20:24 azureml/train/metadata/conda-mapping.zip
+-rw-rw-rw-  2.0 fat   961731 b- defN 20-Jul-06 20:24 azureml/train/metadata/dependencies.zip
+-rw-rw-rw-  2.0 fat  2645746 b- defN 20-Jul-06 20:24 azureml/train/metadata/j-r.zip
+-rw-rw-rw-  2.0 fat  1734403 b- defN 20-Jul-06 20:24 azureml/train/metadata/s-z.zip
+-rw-rw-rw-  2.0 fat    13280 b- defN 20-Jul-06 20:24 azureml/train/metadata/stdlib
+-rw-rw-rw-  2.0 fat       84 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat       96 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat     1252 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1019 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     7058 b- defN 20-Jul-06 20:26 azureml_train_core-1.9.0.dist-info/RECORD
+69 files, 8917152 bytes uncompressed, 8625444 bytes compressed:  3.3%
```

## zipnote {}

```diff
@@ -177,32 +177,32 @@
 
 Filename: azureml/train/metadata/s-z.zip
 Comment: 
 
 Filename: azureml/train/metadata/stdlib
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_train_core-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_train_core-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/entry_points.txt
+Filename: azureml_train_core-1.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/metadata.json
+Filename: azureml_train_core-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/top_level.txt
+Filename: azureml_train_core-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/WHEEL
+Filename: azureml_train_core-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/METADATA
+Filename: azureml_train_core-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_train_core-1.8.0.dist-info/RECORD
+Filename: azureml_train_core-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/train/hyperdrive/sampling.py

```diff
@@ -104,17 +104,15 @@
                     msg = "Unsupported distribution. Only [{}] are supported for \
                           this sampling method.".format(", ".join(self._supported_distributions))
                     raise HyperDriveConfigException(msg)
                 if self._distributions_validators is not None and \
                         distribution[0] in self._distributions_validators:
                     validation_result = self._distributions_validators[distribution[0]](distribution)
                     if not validation_result[0]:
-                        # TODO I do not know if the validation_result would have any CMK. Therefore, scrubbing.
-                        # raise AzureMLException(validation_result[1])
-                        raise HyperDriveConfigException("Validation exception")
+                        raise HyperDriveConfigException(validation_result[1])
 
     def __eq__(self, other):
         """Define equality in terms of the equality of the properties."""
         return self.__dict__ == other.__dict__
 
     @staticmethod
     def _validate_dict_sampling(dict_sampling, name):
@@ -130,17 +128,24 @@
     def _choice_validator(choice_definition):
         """Validate the choice distribution arguments.
 
         :param choice_definition: Distribution to validate.
         :return: a tuple <True, None> if the choice distribution is correctly defined, or <False, Message> if not.
         """
         choice_values = choice_definition[1][0]
-        for value in choice_values:
-            if not type(value) in (int, str, float):
-                return False, "'choice' values should be 'int', 'string' or 'float'."
+        if choice_values:
+            for value in choice_values:
+                if not type(value) in (int, str, float):
+                    return False, "'choice' values should be 'int', 'string' or 'float'."
+
+            choice_types = [type(c) for c in choice_values]
+            if not all(t == choice_types[0] for t in choice_types):
+                return False, "All 'choice' values should be of same types"
+        else:
+            return False, "At least one 'choice' value is required."
 
         return True, None
 
 
 class RandomParameterSampling(HyperParameterSampling):
     """Defines random sampling over a hyperparameter search space.
 
@@ -246,29 +251,29 @@
         HyperParameterSampling._validate_dict_sampling(dict_sampling,
                                                        GridParameterSampling.SAMPLING_NAME)
 
         return GridParameterSampling(parameter_space=dict_sampling["parameter_space"])
 
 
 class BayesianParameterSampling(HyperParameterSampling):
-    """Defines Bayesian sampling over a hyperparameter search space.
+    r"""Defines Bayesian sampling over a hyperparameter search space.
 
     Bayesian sampling tries to intelligently pick the next sample of hyperparameters,
     based on how the previous samples performed, such that the new sample improves
     the reported primary metric.
 
     .. remarks::
         Note that when using Bayesian sampling, the number of concurrent runs has an impact
         on the effectiveness of the tuning process. Typically, a smaller number of concurrent
         runs leads to better sampling convergence. That is because some runs start without
         fully benefiting from runs that are still running.
 
-        .. note:: Bayesian sampling does not support early termination policies. When using Bayesian parameter
-            sampling, use :class:`azureml.train.hyperdrive.NoTerminationPolicy`, set early termination policy to None,
-            or leave off the ``early_termination_policy`` parameter.
+        .. note:: Bayesian sampling does not support early termination policies. When using Bayesian parameter \
+            sampling, use :class:`azureml.train.hyperdrive.NoTerminationPolicy`, set early termination policy to \
+            None, or leave off the ``early_termination_policy`` parameter.
 
         For more information about using BayesianParameter sampling, see the tutorial
         `Tune hyperparameters for your model
         <https://docs.microsoft.com/azure/machine-learning/how-to-tune-hyperparameters#define-search-space>`__.
 
     :param parameter_space: A dictionary containing each parameter and its distribution.
                             The dictionary key is the name of the parameter. Note that only
```

## Comparing `azureml_train_core-1.8.0.dist-info/LICENSE.txt` & `azureml_train_core-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_train_core-1.8.0.dist-info/metadata.json` & `azureml_train_core-1.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9479166666666666%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-core (~=1.9.0)', 'azureml-telemetry (~=1.9.0)', "*

 * *                   "'azureml-train-restclients-hyperdrive (~=1.9.0)']}}",*

 * * "'version'": "'1.9.0'"}*

```diff
@@ -38,22 +38,22 @@
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-train-core",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-core (~=1.8.0)",
-                "azureml-telemetry (~=1.8.0)",
-                "azureml-train-restclients-hyperdrive (~=1.8.0)"
+                "azureml-core (~=1.9.0)",
+                "azureml-telemetry (~=1.9.0)",
+                "azureml-train-restclients-hyperdrive (~=1.9.0)"
             ]
         },
         {
             "environment": "python_version >= \"3.6\"",
             "requires": [
                 "flake8 (<=3.7.9,>=3.1.0)"
             ]
         }
     ],
     "summary": "azureml train core",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_train_core-1.8.0.dist-info/METADATA` & `azureml_train_core-1.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-train-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: azureml train core
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
@@ -13,16 +13,16 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/x-rst
-Requires-Dist: azureml-train-restclients-hyperdrive (~=1.8.0)
-Requires-Dist: azureml-core (~=1.8.0)
-Requires-Dist: azureml-telemetry (~=1.8.0)
+Requires-Dist: azureml-train-restclients-hyperdrive (~=1.9.0)
+Requires-Dist: azureml-core (~=1.9.0)
+Requires-Dist: azureml-telemetry (~=1.9.0)
 Requires-Dist: flake8 (<=3.7.9,>=3.1.0); python_version >= "3.6"
 
 The azureml-train-core contains functionality used by azureml-train metapackage.
```

## Comparing `azureml_train_core-1.8.0.dist-info/RECORD` & `azureml_train_core-1.9.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 azureml/train/hyperdrive/__init__.py,sha256=-LbL_C7T3JvQ62w40QaydpsR0r2aVVqC_zd1R3tv1Mg,2314
 azureml/train/hyperdrive/_search.py,sha256=JmqquyxHUiB-yNAyoOmBIH6-cNKlQ5cPqLxjGnZThx4,11345
 azureml/train/hyperdrive/exceptions.py,sha256=wma0M2Q8LoRVjhduAi-AxxLQlI1WQeqIRiJoBIvzwhM,3647
 azureml/train/hyperdrive/parameter_expressions.py,sha256=XzSbyyhcI9ypNQ8Sjv_-95SnZwGpSXouC_FJSoOCZHY,8548
 azureml/train/hyperdrive/policy.py,sha256=5031ay62ZP748VvZU7877O_glJMjyJQ1ojKjCJSpdYA,21063
 azureml/train/hyperdrive/run.py,sha256=kAxfEcbxkmSvWp4_UX3l3SA4aH2HzGEYLYpxHeaUv38,21078
 azureml/train/hyperdrive/runconfig.py,sha256=mRrrC6s-2QfCX1bL29l9Aj2ZIR4SGiV0NixyLvGeUs0,47707
-azureml/train/hyperdrive/sampling.py,sha256=3DHaL_5gJ7DULJhs8_fSxnE-Sv25Ke5uAcBizLRX0i4,15763
+azureml/train/hyperdrive/sampling.py,sha256=PbpsPZyhnDaY_wFCwI6VilWk1GYwJcAIAOzlxopq150,15914
 azureml/train/metadata/a-i.zip,sha256=I5Eb5zJV9kR4rboP__lICRr_9KqKtfUz0ePgt6PF-6w,2630689
 azureml/train/metadata/conda-mapping.zip,sha256=Z-7Z31h2AXAxj2jPbsYYfc6lHmITiwCvkWYeBkLJqeo,569801
 azureml/train/metadata/dependencies.zip,sha256=jgkCcD_qz-7o3tXlfKG48WspjpFw05zhTx9utNdGSD0,961731
 azureml/train/metadata/j-r.zip,sha256=eNBE02VAifhy3NmllpQR3OF-pvpF1t359SX-8T7mHb0,2645746
 azureml/train/metadata/s-z.zip,sha256=83PiPpLotVohTLfXH5ANFJiyPaRlFvGkMQdNbmwfzpw,1734403
 azureml/train/metadata/stdlib,sha256=cHgSU3tVfLOdD131Vx3j6baU2Uqg9I95_ntcieQ-Qp0,13280
-azureml_train_core-1.8.0.dist-info/DESCRIPTION.rst,sha256=szqPYQZE1wnj_mLzYbvUAu8UMD3dGE-iV1fBI3LvyZw,84
-azureml_train_core-1.8.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_train_core-1.8.0.dist-info/METADATA,sha256=TWy-QkwoMn7Km5uE7Qf179n8EwE_J_4QaOECO7vBM8k,1019
-azureml_train_core-1.8.0.dist-info/RECORD,,
-azureml_train_core-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_train_core-1.8.0.dist-info/entry_points.txt,sha256=lPc7gYAvvPeYAYzJ6iXOCULTmrdGteJS1UhWIcqTLNY,96
-azureml_train_core-1.8.0.dist-info/metadata.json,sha256=P9rS2-3-SIjKbOnFaC2zKVcXPZBKIA-IvhKt7i1XHsU,1252
-azureml_train_core-1.8.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_train_core-1.9.0.dist-info/DESCRIPTION.rst,sha256=szqPYQZE1wnj_mLzYbvUAu8UMD3dGE-iV1fBI3LvyZw,84
+azureml_train_core-1.9.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_train_core-1.9.0.dist-info/METADATA,sha256=eyTJf0CKVJZZhb1RESJ8WwEO4ndeobLcm2p0E05F8B8,1019
+azureml_train_core-1.9.0.dist-info/RECORD,,
+azureml_train_core-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_train_core-1.9.0.dist-info/entry_points.txt,sha256=lPc7gYAvvPeYAYzJ6iXOCULTmrdGteJS1UhWIcqTLNY,96
+azureml_train_core-1.9.0.dist-info/metadata.json,sha256=ryvZrpjGrI5LzfQ7X1M8PRIXE8li4I25jh0wtt03U_M,1252
+azureml_train_core-1.9.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
```

