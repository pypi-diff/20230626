# Comparing `tmp/mlpype-0.4.4.tar.gz` & `tmp/mlpype-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-0.4.4.tar", last modified: Fri Jun 23 09:47:20 2023, max compression
+gzip compressed data, was "mlpype-0.4.5.tar", last modified: Mon Jun 26 20:42:28 2023, max compression
```

## Comparing `mlpype-0.4.4.tar` & `mlpype-0.4.5.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.643888 mlpype-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 09:44:01.000000 mlpype-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 09:47:20.647888 mlpype-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-23 09:44:01.000000 mlpype-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.535887 mlpype-0.4.4/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.539888 mlpype-0.4.4/mlpype/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.547887 mlpype-0.4.4/mlpype/base/data/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/data/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/data/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/data/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.547887 mlpype-0.4.4/mlpype/base/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.555888 mlpype-0.4.4/mlpype/base/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.555888 mlpype-0.4.4/mlpype/base/deploy/wheel/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/helpers/setup_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/helpers/wheel_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/deploy/wheel/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.559888 mlpype-0.4.4/mlpype/base/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/evaluate/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/evaluate/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.559888 mlpype-0.4.4/mlpype/base/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/experiment/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.563888 mlpype-0.4.4/mlpype/base/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/logger/experiment_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/logger/local_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.567888 mlpype-0.4.4/mlpype/base/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.571888 mlpype-0.4.4/mlpype/base/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/pipeline/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/pipeline/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/pipeline/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.579888 mlpype-0.4.4/mlpype/base/serialiser/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/serialiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/serialiser/joblib_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/serialiser/serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.599888 mlpype-0.4.4/mlpype/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/base/utils/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.603888 mlpype-0.4.4/mlpype/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.603888 mlpype-0.4.4/mlpype/fastapi/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/deploy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.607888 mlpype-0.4.4/mlpype/fastapi/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/deploy/wheel/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/deploy/wheel_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/fastapi/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.607888 mlpype-0.4.4/mlpype/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/hyperopt/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/hyperopt/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.607888 mlpype-0.4.4/mlpype/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.611888 mlpype-0.4.4/mlpype/mlflow/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/deploy/load_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.611888 mlpype-0.4.4/mlpype/mlflow/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/logger/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/mlflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.615888 mlpype-0.4.4/mlpype/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.615888 mlpype-0.4.4/mlpype/sklearn/data/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/data/data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/data/sklearn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/data/sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.619888 mlpype-0.4.4/mlpype/sklearn/model/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/model/linear_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/model/logistic_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/model/sklearn_base_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/model/sklearn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.623888 mlpype-0.4.4/mlpype/sklearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/pipeline/numpy_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/pipeline/pandas_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/sklearn/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.623888 mlpype-0.4.4/mlpype/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.627888 mlpype-0.4.4/mlpype/spark/data/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/data/spark_data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/data/spark_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/data/spark_sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.627888 mlpype-0.4.4/mlpype/spark/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/evaluate/spark_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.631888 mlpype-0.4.4/mlpype/spark/model/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/model/linear_spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/model/spark_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.635888 mlpype-0.4.4/mlpype/spark/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/pipeline/spark_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/pipeline/spark_type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.635888 mlpype-0.4.4/mlpype/spark/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/serialisation/spark_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/spark/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.635888 mlpype-0.4.4/mlpype/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.639888 mlpype-0.4.4/mlpype/tensorflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/data/tensor_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.643888 mlpype-0.4.4/mlpype/tensorflow/model/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/model/keras_pype_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/model/mlp_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/model/mlp_pype_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.643888 mlpype-0.4.4/mlpype/tensorflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/pipeline/tensor_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/tensorflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.643888 mlpype-0.4.4/mlpype/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/xgboost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.643888 mlpype-0.4.4/mlpype/xgboost/model/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/xgboost/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/xgboost/model/xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/xgboost/model/xgboost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 09:44:01.000000 mlpype-0.4.4/mlpype/xgboost/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:20.539888 mlpype-0.4.4/mlpype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 09:47:20.000000 mlpype-0.4.4/mlpype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-23 09:47:20.000000 mlpype-0.4.4/mlpype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:20.000000 mlpype-0.4.4/mlpype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 09:47:20.000000 mlpype-0.4.4/mlpype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-23 09:44:01.000000 mlpype-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 09:47:20.647888 mlpype-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 09:44:01.000000 mlpype-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.833034 mlpype-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 20:39:45.000000 mlpype-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-26 20:42:28.833034 mlpype-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-26 20:39:45.000000 mlpype-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.793034 mlpype-0.4.5/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.793034 mlpype-0.4.5/mlpype/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.797034 mlpype-0.4.5/mlpype/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/data/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/data/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/data/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.797034 mlpype-0.4.5/mlpype/base/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.797034 mlpype-0.4.5/mlpype/base/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.797034 mlpype-0.4.5/mlpype/base/deploy/wheel/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/helpers/setup_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/helpers/wheel_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/deploy/wheel/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.801034 mlpype-0.4.5/mlpype/base/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/evaluate/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/evaluate/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.801034 mlpype-0.4.5/mlpype/base/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/experiment/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.801034 mlpype-0.4.5/mlpype/base/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/logger/experiment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/logger/local_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.801034 mlpype-0.4.5/mlpype/base/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.805034 mlpype-0.4.5/mlpype/base/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/pipeline/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/pipeline/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/pipeline/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.805034 mlpype-0.4.5/mlpype/base/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/serialiser/joblib_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/serialiser/serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.805034 mlpype-0.4.5/mlpype/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/base/utils/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/fastapi/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/deploy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/fastapi/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/deploy/wheel/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/deploy/wheel_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/fastapi/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/hyperopt/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/hyperopt/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/mlflow/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/deploy/load_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.809034 mlpype-0.4.5/mlpype/mlflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/logger/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/mlflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.813034 mlpype-0.4.5/mlpype/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.813034 mlpype-0.4.5/mlpype/sklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/data/data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/data/sklearn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/data/sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.817034 mlpype-0.4.5/mlpype/sklearn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/model/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/model/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/model/sklearn_base_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/model/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.817034 mlpype-0.4.5/mlpype/sklearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/pipeline/numpy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/pipeline/pandas_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/sklearn/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.817034 mlpype-0.4.5/mlpype/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.821034 mlpype-0.4.5/mlpype/spark/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/data/spark_data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/data/spark_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/data/spark_sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.821034 mlpype-0.4.5/mlpype/spark/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/evaluate/spark_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.821034 mlpype-0.4.5/mlpype/spark/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/model/linear_spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/model/spark_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.825034 mlpype-0.4.5/mlpype/spark/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/pipeline/spark_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/pipeline/spark_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.825034 mlpype-0.4.5/mlpype/spark/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/serialisation/spark_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/spark/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.825034 mlpype-0.4.5/mlpype/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.825034 mlpype-0.4.5/mlpype/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/data/tensor_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.829034 mlpype-0.4.5/mlpype/tensorflow/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/model/keras_pype_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/model/mlp_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/model/mlp_pype_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.829034 mlpype-0.4.5/mlpype/tensorflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/pipeline/tensor_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/tensorflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.829034 mlpype-0.4.5/mlpype/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.833034 mlpype-0.4.5/mlpype/xgboost/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/xgboost/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/xgboost/model/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/xgboost/model/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 20:39:45.000000 mlpype-0.4.5/mlpype/xgboost/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:28.793034 mlpype-0.4.5/mlpype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-26 20:42:28.000000 mlpype-0.4.5/mlpype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-26 20:42:28.000000 mlpype-0.4.5/mlpype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:42:28.000000 mlpype-0.4.5/mlpype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 20:42:28.000000 mlpype-0.4.5/mlpype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-26 20:39:45.000000 mlpype-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 20:42:28.833034 mlpype-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 20:39:45.000000 mlpype-0.4.5/setup.py
```

### Comparing `mlpype-0.4.4/LICENSE.txt` & `mlpype-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/PKG-INFO` & `mlpype-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.4
+Version: 0.4.5
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.4/README.md` & `mlpype-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/data/data_catalog.py` & `mlpype-0.4.5/mlpype/base/data/data_catalog.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/data/dataset.py` & `mlpype-0.4.5/mlpype/base/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/deploy/inference.py` & `mlpype-0.4.5/mlpype/base/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/deploy/wheel/builder.py` & `mlpype-0.4.5/mlpype/base/deploy/wheel/builder.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/deploy/wheel/extensions.py` & `mlpype-0.4.5/mlpype/base/deploy/wheel/extensions.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/deploy/wheel/helpers/setup_template.py` & `mlpype-0.4.5/mlpype/base/deploy/wheel/helpers/setup_template.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/deploy/wheel/wheel.py` & `mlpype-0.4.5/mlpype/base/deploy/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/evaluate/base_evaluator.py` & `mlpype-0.4.5/mlpype/base/evaluate/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/evaluate/evaluator.py` & `mlpype-0.4.5/mlpype/base/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/experiment/argument_parsing.py` & `mlpype-0.4.5/mlpype/base/experiment/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/experiment/experiment.py` & `mlpype-0.4.5/mlpype/base/experiment/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     def run(self) -> Dict[str, Dict[str, Union[str, float, int, bool]]]:
         """Execute the experiment.
 
         Returns:
             Dict[str, Union[str, float, int, bool]]: The performance metrics of this run.
         """
         with self.experiment_logger:
+            self.logger.info("Log parameters")
+            self.experiment_logger.log_parameters(self.parameters)
+
             self.logger.info("Load data")
             datasets = {
                 name: data_source_set.read() if isinstance(data_source_set, DataCatalog) else data_source_set
                 for name, data_source_set in self.data_sources.items()
             }
 
             self.logger.info("Create input type checker")
@@ -127,18 +130,17 @@
             self.logger.info("Evaluate model")
             metrics = {name: self.evaluator.evaluate(self.model, data) for name, data in transformed.items()}
 
             self.logger.info("Create output type checker")
             predicted_train = self.model.transform(transformed["train"])
             self.output_type_checker.fit(predicted_train)
 
-            self.logger.info("Log results: metrics, parameters")
+            self.logger.info("Log results: metrics")
             for dataset_name, metric_set in metrics.items():
                 self.experiment_logger.log_metrics(dataset_name, metric_set)
-            self.experiment_logger.log_parameters(self.parameters)
 
             self.logger.info("Log results: pipeline, model, serialiser")
             self._log_run()
         return metrics
 
     def _log_run(self) -> None:
         self._create_output_folders()
```

### Comparing `mlpype-0.4.4/mlpype/base/logger/experiment_logger.py` & `mlpype-0.4.5/mlpype/base/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/logger/local_logger.py` & `mlpype-0.4.5/mlpype/base/logger/local_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/model/model.py` & `mlpype-0.4.5/mlpype/base/model/model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/pipeline/operator.py` & `mlpype-0.4.5/mlpype/base/pipeline/operator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/pipeline/pipe.py` & `mlpype-0.4.5/mlpype/base/pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/pipeline/pipeline.py` & `mlpype-0.4.5/mlpype/base/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/pipeline/type_checker.py` & `mlpype-0.4.5/mlpype/base/pipeline/type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/serialiser/joblib_serialiser.py` & `mlpype-0.4.5/mlpype/base/serialiser/joblib_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/serialiser/serialiser.py` & `mlpype-0.4.5/mlpype/base/serialiser/serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/setup.py` & `mlpype-0.4.5/mlpype/base/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
+    version = "0.4.5"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```

### Comparing `mlpype-0.4.4/mlpype/base/utils/parsing.py` & `mlpype-0.4.5/mlpype/base/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/base/utils/workspace.py` & `mlpype-0.4.5/mlpype/base/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/fastapi/deploy/app.py` & `mlpype-0.4.5/mlpype/fastapi/deploy/app.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/fastapi/deploy/wheel/helpers.py` & `mlpype-0.4.5/mlpype/fastapi/deploy/wheel/helpers.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/fastapi/setup.py` & `mlpype-0.4.5/mlpype/tensorflow/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from typing import List
-
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
-    deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
-    dev_deps = ["uvicorn==0.18.2"]
+    version = "0.4.5"
+
+    deps = [
+        f"mlpype-base=={version}",
+        # on mac, it is recommended to use conda/mamba or source to install tensorflow
+        "tensorflow>=2.12",
+        "numpy>=1.23.0",
+        "protobuf>=3.20.3",
+    ]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
-        name="mlpype-fastapi",
+        name="mlpype-tensorflow",
         install_requires=deps,
-        extras_require={"dev": strict_deps + dev_deps, "strict": strict_deps},
+        extras_require={"dev": strict_deps, "strict": strict_deps},
         packages=find_namespace_packages(include=["mlpype.*"]),
         version=version,
     )
```

### Comparing `mlpype-0.4.4/mlpype/hyperopt/optimise.py` & `mlpype-0.4.5/mlpype/hyperopt/optimise.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/mlflow/deploy/load_experiment.py` & `mlpype-0.4.5/mlpype/mlflow/deploy/load_experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/mlflow/logger/mlflow_logger.py` & `mlpype-0.4.5/mlpype/mlflow/logger/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/mlflow/setup.py` & `mlpype-0.4.5/mlpype/mlflow/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
+    version = "0.4.5"
 
     deps = [
         f"mlpype-base=={version}",
         "mlflow>=1.28.0, <2.0",
         "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
```

### Comparing `mlpype-0.4.4/mlpype/sklearn/data/data_frame_source.py` & `mlpype-0.4.5/mlpype/sklearn/data/data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/sklearn/data/sql_source.py` & `mlpype-0.4.5/mlpype/sklearn/data/sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/sklearn/model/sklearn_model.py` & `mlpype-0.4.5/mlpype/sklearn/model/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/sklearn/pipeline/numpy_type_checker.py` & `mlpype-0.4.5/mlpype/sklearn/pipeline/numpy_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/sklearn/pipeline/pandas_type_checker.py` & `mlpype-0.4.5/mlpype/sklearn/pipeline/pandas_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/sklearn/setup.py` & `mlpype-0.4.5/mlpype/sklearn/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
+    version = "0.4.5"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

### Comparing `mlpype-0.4.4/mlpype/spark/data/spark_data_frame_source.py` & `mlpype-0.4.5/mlpype/spark/data/spark_data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/data/spark_read.py` & `mlpype-0.4.5/mlpype/spark/data/spark_read.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/data/spark_sql_source.py` & `mlpype-0.4.5/mlpype/spark/data/spark_sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/evaluate/spark_evaluator.py` & `mlpype-0.4.5/mlpype/spark/evaluate/spark_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/model/spark_model.py` & `mlpype-0.4.5/mlpype/spark/model/spark_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/pipeline/spark_pipe.py` & `mlpype-0.4.5/mlpype/spark/pipeline/spark_pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/pipeline/spark_type_checker.py` & `mlpype-0.4.5/mlpype/spark/pipeline/spark_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/serialisation/spark_serialiser.py` & `mlpype-0.4.5/mlpype/spark/serialisation/spark_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/spark/setup.py` & `mlpype-0.4.5/mlpype/spark/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.4"
+    version = "0.4.5"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

### Comparing `mlpype-0.4.4/mlpype/tensorflow/data/tensor_source.py` & `mlpype-0.4.5/mlpype/tensorflow/data/tensor_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/tensorflow/model/keras_pype_model.py` & `mlpype-0.4.5/mlpype/tensorflow/model/keras_pype_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/tensorflow/model/mlp_keras.py` & `mlpype-0.4.5/mlpype/tensorflow/model/mlp_keras.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/tensorflow/pipeline/tensor_checker.py` & `mlpype-0.4.5/mlpype/tensorflow/pipeline/tensor_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/xgboost/model/xgboost_classifier.py` & `mlpype-0.4.5/mlpype/xgboost/model/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype/xgboost/model/xgboost_regressor.py` & `mlpype-0.4.5/mlpype/xgboost/model/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/mlpype.egg-info/PKG-INFO` & `mlpype-0.4.5/mlpype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.4
+Version: 0.4.5
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.4/mlpype.egg-info/SOURCES.txt` & `mlpype-0.4.5/mlpype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.4/pyproject.toml` & `mlpype-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mlpype"
 authors = [
     {name = "Jeroen van den Hoven"},
 ]
 description = "Standardise model training across libraries"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.4"
+version = "0.4.5"
 dynamic = ["license"]
 
 [tool.kedro]
 package_name = "data_cube_pipeline"
 project_name = "Data Cube Pipeline"
 project_version = "0.17.0"
```

