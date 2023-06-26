# Comparing `tmp/datarobot_early_access-3.2.0.2023.6.26.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.6.26.tar", last modified: Mon Jun 26 16:46:36 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.6.5.tar", last modified: Mon Jun  5 16:46:57 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.6.26.tar` & `datarobot_early_access-3.2.0.2023.6.5.tar`

### file list

```diff
@@ -1,173 +1,169 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   177966 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5712 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2309 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      927 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4428 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21331 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25820 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4121 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19691 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    66977 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13004 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33089 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59836 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5605 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18064 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    58746 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    96313 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18187 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21166 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5106 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   267372 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215251 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5049 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7236 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4554 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24079 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12298 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-06-26 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5805 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1154 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-06-26 16:46:13.000000 datarobot_early_access-3.2.0.2023.6.26/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-06-26 16:46:36.000000 datarobot_early_access-3.2.0.2023.6.26/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-06-26 16:46:13.000000 datarobot_early_access-3.2.0.2023.6.26/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-06-26 16:46:13.000000 datarobot_early_access-3.2.0.2023.6.26/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   173551 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5678 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2257 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      927 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18879 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3126 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25285 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8680 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4012 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23047 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    32642 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59153 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    58123 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93319 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256455 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215251 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6340 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24565 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8680 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17330 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-06-05 16:46:11.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5684 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1108 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-06-05 16:46:56.000000 datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-06-05 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.5/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-06-05 16:46:57.000000 datarobot_early_access-3.2.0.2023.6.5/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-06-05 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.5/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-06-05 16:46:12.000000 datarobot_early_access-3.2.0.2023.6.5/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.6.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,14 @@
 Changelog
 #########
 3.2.0b0
 ========
 
 New Features
 ************
-- Added new methods to trigger batch monitoring jobs without providing a job definition.
-  :meth:`BatchMonitoringJob.run <datarobot.models.BatchMonitoringJob.run>`
-  :meth:`BatchMonitoringJob.get_status <datarobot.models.BatchMonitoringJob.get_status>`
-  :meth:`BatchMonitoringJob.cancel <datarobot.models.BatchMonitoringJob.cancel>`
-  :meth:`BatchMonitoringJob.download <datarobot.models.BatchMonitoringJob.download>`
-
-- Added :meth:`Deployment.submit_actuals_from_catalog_async<datarobot.models.Deployment.submit_actuals_from_catalog_async>` to submit actuals from the AI Catalog.
-- Added a new class :class:`StatusCheckJob <datarobot.models.StatusCheckJob>` which represents a job for a status check of submitted async jobs.
-- Added a new class :class:`JobStatusResult <datarobot.models.JobStatusResult>` represents the result for a status check job of a submitted async task.
 - Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
 - Added method :meth:`DatetimePartitioning.datetime_partitioning_log_list <datarobot.DatetimePartitioning.datetime_partitioning_log_list>` to list the datetime partitioning log.
 - Added :meth:`DatetimePartitioning.get_input_data <datarobot.DatetimePartitioning.get_input_data>` to retrieve the input data used to create an optimized datetime partitioning.
 - Added :class:`DatetimePartitioningId <datarobot.helpers.partitioning_methods.DatetimePartitioningId>`, which can be passed as a `partitioning_method` to :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>`.
 - Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
 
 - Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings.
@@ -57,52 +48,25 @@
   :meth:`Project.start <datarobot.models.Project.start>`
 - Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set in several ways.
 
   - If the user configures the client via `Client(...)`, then invoke `Client(..., default_use_case = <id>)`.
   - If the user configures the client via dr.config.yaml, then add the property `default_use_case: <id>`.
   - If the user configures the client via env vars, then set the env var ``DATAROBOT_DEFAULT_USE_CASE``.
   - The default use case can also be set programmatically as a context manager via `with UseCase.get(<id>):`.
-- Added the ability to configure sending package usage metrics to DataRobot with the following configuration setting:
-
-  - If the user configures the client via `Client(...)`, then invoke `Client(..., enable_api_consumer_tracking = <True/False>)`.
-  - If the user configures the client via dr.config.yaml, then add the property `enable_api_consumer_tracking: <True/False>`.
-  - If the user configures the client via env vars, then set the env var ``DATAROBOT_API_CONSUMER_TRACKING_ENABLED``.
-
-  Currently the default value for ``enable_api_consumer_tracking`` is ``True``.
 
 - Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
 - Added a new class :class:`FairnessScoresOverTime <datarobot.models.deployment.bias_and_fairness.FairnessScoresOverTime>` to retrieve fairness over time information.
 - Added a new method :meth:`Deployment.get_fairness_scores_over_time <datarobot.models.Deployment.get_fairness_scores_over_time>` to retrieve fairness scores over time of a deployment.
 - Added a new `use_gpu` parameter to the method :meth:`Project.analyze_and_model<datarobot.models.Project.analyze_and_model>` to set whether the project should allow usage of GPU
 - Added a new `use_gpu` parameter to the class :class:`Project <datarobot.models.Project>` with information whether project allows usage of GPU
 - Added a new class :class:`TrainingData <datarobot.models.custom_model_version.TrainingData>` for retrieving TrainingData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
 - Added a new class :class:`HoldoutData <datarobot.models.custom_model_version.HoldoutData>` for retrieving HoldoutData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
 - Added the ability to retrieve the model and blueprint json using the following methods:
   :meth:`Model.get_model_blueprint_json <datarobot.models.Model.get_model_blueprint_json>`
   :meth:`Blueprint.get_json <datarobot.models.Blueprint.get_json>`
-- Added :meth:`Credential.update <datarobot.models.Credential.update>` which allows you to update existing credential resources.
-- Added a new optional parameter `trace_context` to `datarobot.Client` to provide additional information on the DataRobot code being run. This parameter defaults to `None`.
-- Updated methods in :class:`Model <datarobot.models.model.Model>` to support use of Sliced Insights:
-  :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>`
-  :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>`
-  :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>`
-  :meth:`Model.get_lift_chart <datarobot.models.Model.get_lift_chart>`
-  :meth:`Model.get_all_lift_charts <datarobot.models.Model.get_all_lift_charts>`
-  :meth:`Model.get_residuals_chart <datarobot.models.Model.get_residuals_chart>`
-  :meth:`Model.get_all_residuals_charts <datarobot.models.Model.get_all_residuals_charts>`
-  :meth:`Model.request_lift_chart <datarobot.models.Model.request_lift_chart>`
-  :meth:`Model.request_residuals_chart <datarobot.models.Model.request_residuals_chart>`
-- Added support for :class:`SharingRole <datarobot.models.sharing.SharingRole>` to the following methods:
-  - :meth:`DataStore.share <datarobot.DataStore.share>`
-- Added new methods for retrieving :class:`SharingRole <datarobot.models.sharing.SharingRole>` information for the following classes:
-  - :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>`
-- Added new method for calculating sliced roc curve :meth: `Model.request_roc_curve <datarobot.models.Model.request_roc_curve>`
-- Added new :class: `DataSlice <datarobot.models.data_slice.DataSlice>` to support the following slices methods:
-  :meth: `DataSlice.list <datarobot.models.data_slice.DataSlice.list>` to retrieve all data slices in a project
-  :meth: `DataSlice.create <datarobot.models.data_slice.DataSlice.create>` to create a new data slice
 
 
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
@@ -126,17 +90,14 @@
         - `holdout_dataset_id`
         - `keep_training_holdout_data`
         - `max_wait`
 
 - Extended :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.create>` and :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.update>`
   with `is_training_data_for_versions_permanently_enabled` parameter.
 
-- Added value `DR_API_ACCESS` to the `NETWORK_EGRESS_POLICY` enum.
-
-- Added new parameter `low_memory` to :meth:`Dataset.get_as_dataframe <datarobot.models.Dataset.get_as_dataframe>` to allow a low memory mode for larger datasets
 
 Bugfixes
 ********
 - Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
 - Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 - Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
 
@@ -158,27 +119,19 @@
   Use :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>` instead.
 - ``DatetimeModel.get_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` instead.
 - ``Model.get_or_request_feature_fit`` has been removed.
   Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
 - ``DatetimeModel.get_or_request_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
-- Deprecated the use of :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` in favor of :class:`SharingRole <datarobot.models.sharing.SharingRole>` for sharing in the following classes:
-  - :meth:`DataStore.share <datarobot.DataStore.share>`
-- Deprecated the following methods for retrieving :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` information.
-  - :meth:`DataStore.get_access_list <datarobot.DataStore.get_access_list>`. Please use :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>` instead.
 
 Configuration Changes
 *********************
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
-Deprecation Summary
-*******************
-- Deprecated parameter `user_agent_suffix` in `datarobot.Client`. `user_agent_suffix` will be removed in v3.4. Please use `trace_context` instead.
-
 Documentation Changes
 *********************
 - Fixed in-line documentation of `DataRobotClientConfig`.
 - Fixed documentation around client configuration from environment variables or config file.
 
 Experimental changes
 *********************
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/PKG-INFO` & `datarobot_early_access-3.2.0.2023.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.6.26
+Version: 3.2.0.2023.6.5
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/README.md` & `datarobot_early_access-3.2.0.2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/common_setup.py` & `datarobot_early_access-3.2.0.2023.6.5/common_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 ]
 
 images_require = ["Pillow==9.2.0"]
 
 lint_require = (
     [
         "black==22.8.0",
-        "black[jupyter]==22.8.0",
         "isort==5.10.1",
         "flake8==5.0.4",
         "pylint==2.15.0",
     ]
     + _mypy_require
     + images_require
 )
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # flake8: noqa
+
 from ._version import __version__
 from .client import Client
 from .context import Context
 from .enums import (
     AUTOPILOT_MODE,
     NETWORK_EGRESS_POLICY,
     QUEUE_STATUS,
@@ -41,15 +42,14 @@
     DataDriver,
     DataEngineQueryGenerator,
     Dataset,
     DatasetDetails,
     DatasetFeature,
     DatasetFeatureHistogram,
     DatasetFeaturelist,
-    DataSlice,
     DataSource,
     DataSourceParameters,
     DataStore,
     DatetimeModel,
     Deployment,
     ExecutionEnvironment,
     ExecutionEnvironmentVersion,
@@ -94,15 +94,12 @@
     SecondaryDatasetConfigurations,
     SegmentationTask,
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
     ShapMatrixJob,
     SharingAccess,
-    SharingRole,
     TrainingPredictions,
     TrainingPredictionsJob,
     UseCase,
     UserBlueprint,
 )
-
-DR_TRACKABLE = True
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from datarobot.models import DatetimeModel as datarobot_datetime_model
 from datarobot.models import FeatureEffects
 from datarobot.models import Model as datarobot_model
 
 
 class Model(datarobot_model):  # pylint: disable=missing-class-docstring
-    # pylint: disable-next=arguments-renamed
     def get_feature_effect(self, source, include_ice_plots=False):
         """
         Retrieve Feature Effects for the model.
 
         Feature Effects provides partial dependence and predicted vs actual values for top-500
         features ordered by feature impact score.
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional, Tuple, TYPE_CHECKING, Union
 import warnings
 
 from urllib3 import Retry
 import yaml
 
 from ._version import __expected_server_version__, __version__
-from .context import Context, DefaultUseCase, ENABLE_API_CONSUMER_TRACKING_DEFAULT, env_to_bool
+from .context import Context, DefaultUseCase
 from .errors import ClientError
 from .rest import DataRobotClientConfig, RESTClientObject
 
 if TYPE_CHECKING:
     from requests import Response
 
 logger = logging.getLogger(__package__)
@@ -45,17 +45,15 @@
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
     default_use_case: Optional[str] = None,
-    enable_api_consumer_tracking: Optional[bool] = None,
-    trace_context: Optional[str] = None,
-) -> Tuple[RESTClientObject, Optional[str], Optional[bool], Optional[str]]:
+) -> Tuple[RESTClientObject, Optional[str]]:
     """Return a new `RESTClientObject` and default_use_case id with optional configuration.
     The client will be configured in one of the following ways, in order of priority.
 
       1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
       2. From a YAML file at the path specified in the ``config_path`` kwarg;
       3. From a YAML file at the path specified in the env var ``DATAROBOT_CONFIG_FILE``;
       4. From env vars, iff ``DATAROBOT_ENDPOINT`` and ``DATAROBOT_API_TOKEN`` are specified;
@@ -89,40 +87,26 @@
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools
     default_use_case: str, optional
         The entity ID of the default Use Case to use with any requests made by this Client instance.
-    enable_api_consumer_tracking: bool, optional
-        Enable and disable user metrics tracking within the datarobot module. Default: False.
-    trace_context: str, optional
-        An ID or other string for identifying which code template or AI Accelerator was used to make
-        a request.
-
     """
     env_config = _get_config_file_from_env()
-    if enable_api_consumer_tracking is None:
-        enable_api_consumer_tracking = env_to_bool(
-            os.environ.get(
-                "DATAROBOT_API_CONSUMER_TRACKING_ENABLED", ENABLE_API_CONSUMER_TRACKING_DEFAULT
-            )
-        )
     if token and endpoint:
         drconfig = DataRobotClientConfig(
             endpoint=endpoint,
             token=token,
             connect_timeout=connect_timeout,
             user_agent_suffix=user_agent_suffix,
             ssl_verify=ssl_verify,
             max_retries=max_retries,
             token_type=token_type,
             default_use_case=default_use_case,
-            enable_api_consumer_tracking=enable_api_consumer_tracking,
-            trace_context=trace_context,
         )
     elif config_path:
         if not _file_exists(config_path):
             raise ValueError(f"Invalid config path - no file at {config_path}")
         drconfig = _config_from_file(config_path)
     elif env_config:
         if not _file_exists(env_config):
@@ -141,29 +125,27 @@
     if not drconfig.max_retries:
         drconfig.max_retries = Retry(backoff_factor=0.1, respect_retry_after_header=True)
 
     client = RESTClientObject.from_config(drconfig)
     if not _is_compatible_client(client):
         raise ValueError("The client is not compatible with the server version")
 
-    return client, drconfig.default_use_case, drconfig.enable_api_consumer_tracking, trace_context
+    return client, drconfig.default_use_case
 
 
 def Client(
     token: Optional[str] = None,
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
     default_use_case: Optional[str] = None,
-    enable_api_consumer_tracking: Optional[bool] = None,
-    trace_context: Optional[str] = None,
 ) -> RESTClientObject:
     """
     Configures the global API client for the Python SDK. The client will be configured in one of
     the following ways, in order of priority.
 
       1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
       2. From a YAML file at the path specified in the ``config_path`` kwarg;
@@ -200,41 +182,32 @@
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools.
     default_use_case: str, optional
         The entity ID of the default Use Case to use with any requests made by the client.
-    enable_api_consumer_tracking: bool, optional
-        Enable and disable user metrics tracking within the datarobot module. Default: False.
-    trace_context: str, optional
-        An ID or other string for identifying which code template or AI Accelerator was used to make
-        a request.
     Returns
     -------
         The ``RESTClientObject`` instance created.
     """
-    new_client, default_use_case, enable_api_consumer_tracking, trace_context = _create_client(
+    new_client, default_use_case = _create_client(
         token,
         endpoint,
         config_path,
         connect_timeout,
         user_agent_suffix,
         ssl_verify,
         max_retries,
         token_type,
         default_use_case,
-        enable_api_consumer_tracking,
-        trace_context,
     )
 
     set_client(new_client)
     Context.use_case = default_use_case
-    Context.trace_context = trace_context
-    Context.enable_api_consumer_tracking = enable_api_consumer_tracking
 
     return new_client
 
 
 def _is_compatible_client(client: RESTClientObject) -> bool:
     """
     Check that this client version is not ahead of the DataRobot version that
@@ -456,39 +429,31 @@
         variable
     IOError
         If the config file that DATAROBOT_CONFIG_FILE points to does not exist
     """
     endpoint: Optional[str] = os.environ.get("DATAROBOT_ENDPOINT")
     token: Optional[str] = os.environ.get("DATAROBOT_API_TOKEN")
     user_agent_suffix: Optional[str] = os.environ.get("DATAROBOT_USER_AGENT_SUFFIX")
-    trace_context: Optional[str] = os.environ.get("DATAROBOT_TRACE_CONTEXT")
     max_retries: Optional[Union[str, int]] = os.environ.get("DATAROBOT_MAX_RETRIES")
     if max_retries is not None:
         max_retries = int(max_retries)
     use_case_id: Optional[str] = os.environ.get("DATAROBOT_DEFAULT_USE_CASE")
-    enable_api_consumer_tracking: bool = env_to_bool(
-        os.environ.get(
-            "DATAROBOT_API_CONSUMER_TRACKING_ENABLED", ENABLE_API_CONSUMER_TRACKING_DEFAULT
-        )
-    )
 
     if endpoint is None or token is None:
         e_msg = (
             "Incomplete DataRobot configuration specified in environment variables; both "
             "DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN must be specified"
         )
         raise ValueError(e_msg)
     return DataRobotClientConfig(
         endpoint=endpoint,
         token=token,
         user_agent_suffix=user_agent_suffix,
         max_retries=max_retries,
         default_use_case=use_case_id,
-        enable_api_consumer_tracking=enable_api_consumer_tracking,
-        trace_context=trace_context,
     )
 
 
 def _config_from_file(config_path: str) -> DataRobotClientConfig:
     """
     Create and return a DataRobotClientConfig from a config path. The file must be
     a yaml formatted file
@@ -544,27 +509,17 @@
         with client_configuration(config_path="/path/to/a/drconfig.yaml"):
             # Interact with DataRobot using a different configuration.
             Project.list()
     """
 
     contextvars_token: contextvars.Token[RESTClientObject] = None
     previous_use_case: DefaultUseCase = None
-    previous_enable_api_consumer_tracking: Optional[bool] = None
-    previous_trace_context: Optional[str] = None
     try:
-        client, default_use_case, enable_api_consumer_tracking, trace_context = _create_client(
-            *args, **kwargs
-        )
+        client, default_use_case = _create_client(*args, **kwargs)
         contextvars_token = _context_client.set(client)
         previous_use_case = Context.get_use_case(raw=True)
-        previous_enable_api_consumer_tracking = Context.enable_api_consumer_tracking
-        previous_trace_context = Context.trace_context
         Context.use_case = default_use_case
-        Context.enable_api_consumer_tracking = enable_api_consumer_tracking
-        Context.trace_context = trace_context
         yield
     finally:
         if contextvars_token is not None:
             _context_client.reset(contextvars_token)
         Context.use_case = previous_use_case
-        Context.enable_api_consumer_tracking = previous_enable_api_consumer_tracking
-        Context.trace_context = previous_trace_context
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -551,18 +551,17 @@
     ALL = _SHARED_TARGET_TYPE.ALL + [TRANSFORM]
 
 
 class NETWORK_EGRESS_POLICY:
     """Enum of valid network egress policy"""
 
     NONE = "NONE"
-    DR_API_ACCESS = "DR_API_ACCESS"
     PUBLIC = "PUBLIC"
 
-    ALL = [NONE, DR_API_ACCESS, PUBLIC]
+    ALL = [NONE, PUBLIC]
 
 
 @use_all
 class SOURCE_TYPE(str, Enum):
     """Enum of backtest source types"""
 
     TRAINING = "training"
@@ -932,30 +931,7 @@
     CAN_VIEW = "CAN_VIEW"
 
 
 class CredentialTypes(str, Enum):
     BASIC = "basic"
     OAUTH = "oauth"
     S3 = "s3"
-
-
-class IntakeAdapters(str, Enum, metaclass=StrEnum):
-    LOCAL_FILE = "localFile"
-    AZURE = "azure"
-    GCP = "gcp"
-    S3 = "s3"
-    JDBC = "jdbc"
-    DATASET = "dataset"
-    SNOWFLAKE = "snowflake"
-    SYNAPSE = "synapse"
-    BIG_QUERY = "bigquery"
-
-
-class OutputAdapters(str, Enum, metaclass=StrEnum):
-    LOCAL_FILE = "localFile"
-    AZURE = "azure"
-    GCP = "gcp"
-    S3 = "s3"
-    JDBC = "jdbc"
-    SNOWFLAKE = "snowflake"
-    SYNAPSE = "synapse"
-    BIG_QUERY = "bigquery"
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,20 +276,11 @@
 
     See Also
     --------
     DataRobotDeprecationWarning
     """
 
 
-class MultipleUseCasesNotAllowed(UserWarning):
-    """
-    Raised when a method decorated with add_to_use_case(allow_multiple=True) calls a method
-    decorated with add_to_use_case(allow_multiple=False) with multiple UseCases passed
-    """
-
-    message = "Entity can't be added to multiple UseCases"
-
-
 warnings.filterwarnings("default", category=DataRobotDeprecationWarning)
 warnings.filterwarnings("always", category=PlatformDeprecationWarning)
 warnings.filterwarnings("always", category=InvalidRatingTableWarning)
 warnings.filterwarnings("always", category=ParentModelInsightFallbackWarning)
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     CustomModelVersion,
     CustomModelVersionConversion,
     CustomModelVersionDependencyBuild,
 )
 from .custom_task import CustomTask
 from .custom_task_version import CustomTaskVersion
 from .data_engine_query_generator import DataEngineQueryGenerator
-from .data_slice import DataSlice
 from .data_source import DataSource, DataSourceParameters
 from .data_store import DataStore
 from .dataset import Dataset, DatasetDetails
 from .deployment import Deployment
 from .driver import DataDriver
 from .execution_environment import ExecutionEnvironment
 from .execution_environment_version import ExecutionEnvironmentVersion
@@ -100,16 +99,15 @@
 from .relationships_configuration import RelationshipsConfiguration
 from .ruleset import Ruleset
 from .secondary_dataset import SecondaryDatasetConfigurations
 from .segmentation import SegmentationTask, SegmentInfo
 from .shap_impact import ShapImpact
 from .shap_matrix import ShapMatrix
 from .shap_matrix_job import ShapMatrixJob
-from .sharing import SharingAccess, SharingRole
-from .status_check_job import JobStatusResult, StatusCheckJob
+from .sharing import SharingAccess
 from .training_predictions import TrainingPredictions
 from .types import (
     AnomalyAssessmentDataPoint,
     AnomalyAssessmentPreviewBin,
     AnomalyAssessmentRecordMetadata,
     RegionExplanationsData,
     RocCurveEstimatedMetric,
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/application.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/batch_prediction_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,63 +11,123 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import csv
 import datetime
 import io
-from typing import cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+import os
+import threading
+import time
+from typing import Any, cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import pandas as pd
+import requests
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import Int, String
-from datarobot.models.batch_job import (
-    AbstractBatchJob,
-    CsvSettings,
-    IntakeSettings,
-    OutputSettings,
-    recognize_sourcedata,
-    Schedule,
-)
 from datarobot.models.credential import Credential
 from datarobot.models.dataset import Dataset
+from datarobot.models.job import AbstractSpecificJob
 from datarobot.models.prediction_explanations import PredictionExplanationsMode
 from datarobot.models.project import Project
-from datarobot.utils import get_id_from_response, pagination, to_api
+from datarobot.utils import get_id_from_response, pagination
+from datarobot.utils import recognize_sourcedata as orig_recognize_sourcedata
+from datarobot.utils import to_api
 
-from ..enums import DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
+from ..enums import AVAILABLE_STATEMENT_TYPES, DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
 from ..utils import logger, parse_time
 from .api_object import APIObject
 
 LOG = logger.get_logger(__name__)
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.deployment import Deployment
 
     DeploymentType = Union[str, Deployment]
 
+    class IntakeSettings(TypedDict, total=False):
+        """Intake settings typed dict"""
+
+        type: str
+        file: Optional[Union[str, pd.DataFrame, io.IOBase]]
+        url: Optional[str]
+        credential_id: Optional[str]
+        data_store_id: Optional[str]
+        query: Optional[str]
+        table: Optional[str]
+        schema: Optional[str]
+        catalog: Optional[str]
+        fetch_size: Optional[int]
+        format: Optional[str]
+        endpoint_url: Optional[str]
+
+    class OutputSettings(TypedDict, total=False):
+        """Output settings typed dict"""
+
+        type: str
+        path: Optional[str]
+        url: Optional[str]
+        credential_id: Optional[str]
+        data_store_id: Optional[str]
+        table: Optional[str]
+        schema: Optional[str]
+        catalog: Optional[str]
+        statement_type: Optional[str]
+        update_columns: Optional[List[str]]
+        where_columns: Optional[List[str]]
+        create_table_if_not_exists: Optional[bool]
+
+    class CsvSettings(TypedDict):
+        delimiter: Optional[str]
+        quotechar: Optional[str]
+        encoding: Optional[str]
+
     class TimeSeriesSettings(TypedDict, total=False):
         type: str
         forecast_point: Optional[datetime.datetime]
         predictions_start_date: Optional[datetime.datetime]
         predictions_end_date: Optional[datetime.datetime]
         relax_known_in_advance_features_check: bool
 
     class PredictionInstance(TypedDict):
         hostName: str
         sslEnabled: Optional[bool]
         datarobotKey: Optional[str]
         apiKey: Optional[str]
 
+    class Schedule(TypedDict):
+        day_of_week: List[Union[int, str]]
+        month: List[Union[int, str]]
+        hour: List[Union[int, str]]
+        minute: List[Union[int, str]]
+        day_of_month: List[Union[int, str]]
+
+
+def recognize_sourcedata(sourcedata: Any, default_fname: str) -> Dict[str, Any]:
+    """Override the default recognize_sourcedata with one that converts
+    DataFrame to io.BytesIO"""
+    if not isinstance(sourcedata, pd.DataFrame):
+        return orig_recognize_sourcedata(sourcedata, default_fname)
+    # The original recognize_sourcedata will encode dataframes into StringIO
+    # To pass this to requests.put, we need BytesIO - otherwise, requests will
+    # try to encode it using latin-1 encoding (the default HTTP encoding),
+    # which will crash when a charater not contained in latin-1 is used
+    #
+    # https://github.com/python/cpython/blob/b9797417315cc2d1700cb2d427685016d3380711/Lib/http/client.py#L1046
+    buf = io.BytesIO()
+    sourcedata.to_csv(buf, encoding="utf-8", index=False, quoting=csv.QUOTE_ALL)
+    buf.seek(0)
+    return {"filelike": buf, "fname": default_fname}
+
 
-class BatchPredictionJob(AbstractBatchJob):
+class BatchPredictionJob(AbstractSpecificJob):
     """
     A Batch Prediction Job is used to score large data sets on
     prediction servers using the Batch Prediction API.
 
     Attributes
     ----------
     id : str
@@ -116,14 +176,74 @@
                 "FAILED",
             ),
             t.Key("project_id", optional=True): String,
             t.Key("is_blocked", optional=True): t.Bool,
         }
     )
 
+    _s3_settings = t.Dict(
+        {
+            t.Key("url"): String(),
+            t.Key("credential_id", optional=True): String(),
+            t.Key("endpoint_url", optional=True): String(),
+            t.Key("format", optional=True): String(),
+        }
+    )
+
+    _gcp_settings = t.Dict(
+        {
+            t.Key("url"): String(),
+            t.Key("credential_id", optional=True): String(),
+            t.Key("format", optional=True): String(),
+        }
+    )
+
+    _azure_settings = t.Dict(
+        {
+            t.Key("url"): String(),
+            t.Key("credential_id", optional=True): String(),
+            t.Key("format", optional=True): String(),
+        }
+    )
+
+    _dataset_intake_settings = t.Dict(
+        {t.Key("dataset"): t.Type(Dataset), t.Key("dataset_version_id", optional=True): String()}
+    )
+
+    _jdbc_intake_settings = t.Dict(
+        {
+            t.Key("data_store_id"): String(),
+            t.Key("query", optional=True): String(),
+            t.Key("table", optional=True): String(),
+            t.Key("schema", optional=True): String(),
+            t.Key("catalog", optional=True): String(),
+            t.Key("fetch_size", optional=True): Int(),
+            t.Key("credential_id", optional=True): String(),
+        }
+    )
+
+    _jdbc_output_settings = t.Dict(
+        {
+            t.Key("data_store_id"): String(),
+            t.Key("table"): String(),
+            t.Key("schema", optional=True): String(),
+            t.Key("catalog", optional=True): String(),
+            t.Key("statement_type"): t.Enum(
+                AVAILABLE_STATEMENT_TYPES.INSERT,
+                AVAILABLE_STATEMENT_TYPES.UPDATE,
+                AVAILABLE_STATEMENT_TYPES.INSERT_UPDATE,
+                AVAILABLE_STATEMENT_TYPES.CREATE_TABLE,
+            ),
+            t.Key("update_columns", optional=True): t.List(String),
+            t.Key("where_columns", optional=True): t.List(String),
+            t.Key("credential_id", optional=True): String(),
+            t.Key("create_table_if_not_exists", optional=True): t.Bool(),
+        }
+    )
+
     _timeseries_settings = t.Dict(
         {
             t.Key("type"): t.Atom("forecast"),
             t.Key("forecast_point", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
         }
     ) | t.Dict(
@@ -131,14 +251,22 @@
             t.Key("type"): t.Atom("historical"),
             t.Key("predictions_start_date", optional=True): parse_time,
             t.Key("predictions_end_date", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
         }
     )
 
+    _csv_settings = t.Dict(
+        {
+            t.Key("delimiter", optional=True): t.Atom("tab") | String(min_length=1, max_length=1),
+            t.Key("quotechar", optional=True): String(),
+            t.Key("encoding", optional=True): String(),
+        }
+    )
+
     _prediction_instance = t.Dict(
         {
             t.Key("hostName"): String(),
             t.Key("sslEnabled", optional=True): t.Bool(),
             t.Key("datarobotKey", optional=True): String(),
             t.Key("apiKey", optional=True): String(),
         }
@@ -154,17 +282,17 @@
     def _jobs_path(cls) -> str:
         return "batchPredictions/"
 
     @classmethod
     def _job_path(  # pylint: disable=arguments-renamed
         cls,
         project_id: str,
-        job_id: str,
+        batch_prediction_job_id: str,
     ) -> str:
-        return f"batchPredictions/{job_id}/"
+        return f"batchPredictions/{batch_prediction_job_id}/"
 
     @classmethod
     def _from_existing_path(cls) -> str:
         return "batchPredictions/fromExisting/"
 
     @classmethod
     def score(
@@ -549,48 +677,298 @@
                 if forecast_point and not isinstance(forecast_point, datetime.datetime):
                     raise ValueError(
                         "The value provided for forecast_point was not a valid format."
                     )
 
             job_data["timeseriesSettings"] = to_api(timeseries_settings)
 
-        # validate input settings, return a copy not original
-        intake_settings = cls.validate_intake_settings(intake_settings)
+        if intake_settings is None:
+            intake_settings = {"type": "localFile"}
+        else:
+            # avoid mutating the input argument
+            intake_settings = dict(intake_settings)
+
         intake_file = None
-        if intake_settings["type"] == "localFile":
+
+        # Validate the intake settings
+
+        if intake_settings.get("type") not in (
+            "localFile",
+            "azure",
+            "gcp",
+            "s3",
+            "jdbc",
+            "dataset",
+            "snowflake",
+            "synapse",
+            "bigquery",
+        ):
+            raise ValueError(
+                "Unsupported type parameter for intake_settings: {}".format(
+                    intake_settings.get("type")
+                )
+            )
+
+        elif intake_settings["type"] == "localFile":
+
+            # This intake option requires us to upload the source
+            # data ourselves
+
+            if intake_settings.get("file") is None:
+                raise ValueError(
+                    "Missing source data. Either supply the `file` "
+                    "parameter or switch to an intake option that does not "
+                    "require it."
+                )
+
             intake_file = recognize_sourcedata(intake_settings.pop("file"), "prediction.csv")
+
+        elif intake_settings["type"] == "s3":
+
+            del intake_settings["type"]
+            intake_settings = cls._s3_settings.check(intake_settings)
+            intake_settings["type"] = "s3"
+
+        elif intake_settings["type"] == "gcp":
+
+            del intake_settings["type"]
+            intake_settings = cls._gcp_settings.check(intake_settings)
+            intake_settings["type"] = "gcp"
+
+        elif intake_settings["type"] == "azure":
+
+            del intake_settings["type"]
+            intake_settings = cls._azure_settings.check(intake_settings)
+            intake_settings["type"] = "azure"
+
+        elif intake_settings["type"] == "jdbc":
+
+            del intake_settings["type"]
+            intake_settings = cls._jdbc_intake_settings.check(intake_settings)
+            intake_settings["type"] = "jdbc"
+
+        elif intake_settings["type"] == "dataset":
+
+            del intake_settings["type"]
+            intake_settings = cls._dataset_intake_settings.check(intake_settings)
+            intake_settings["type"] = "dataset"
+
+            dataset = intake_settings["dataset"]
+            intake_settings["dataset_id"] = dataset.id
+            if "dataset_version_id" not in intake_settings:
+                intake_settings["dataset_version_id"] = dataset.version_id
+
+            del intake_settings["dataset"]
+
         job_data["intakeSettings"] = to_api(intake_settings)
 
+        if output_settings is None:
+            output_settings = {"type": "localFile"}
+        else:
+            output_settings = dict(output_settings)
+
         output_file = None
 
         # Validate the output settings
 
-        output_settings = cls.validate_output_settings(output_settings)
-        if output_settings["type"] == "localFile":
+        if output_settings.get("type") not in (
+            "localFile",
+            "azure",
+            "gcp",
+            "s3",
+            "jdbc",
+            "snowflake",
+            "synapse",
+            "bigquery",
+        ):
+            raise ValueError(
+                "Unsupported type parameter for output_settings: {}".format(
+                    output_settings.get("type")
+                )
+            )
+
+        elif output_settings["type"] == "localFile":
+
             if output_settings.get("path") is not None:
                 output_file = open(  # pylint: disable=consider-using-with
                     output_settings.pop("path"), "wb"
                 )
+
+        elif output_settings["type"] == "s3":
+
+            del output_settings["type"]
+            output_settings = cls._s3_settings.check(output_settings)
+            output_settings["type"] = "s3"
+
+        elif output_settings["type"] == "gcp":
+
+            del output_settings["type"]
+            output_settings = cls._gcp_settings.check(output_settings)
+            output_settings["type"] = "gcp"
+
+        elif output_settings["type"] == "azure":
+
+            del output_settings["type"]
+            output_settings = cls._azure_settings.check(output_settings)
+            output_settings["type"] = "azure"
+
+        elif output_settings["type"] == "jdbc":
+
+            del output_settings["type"]
+            output_settings = cls._jdbc_output_settings.check(output_settings)
+            output_settings["type"] = "jdbc"
+
         job_data["outputSettings"] = to_api(output_settings)
 
         if csv_settings is not None:
             cls._csv_settings.check(csv_settings)
             job_data["csvSettings"] = to_api(csv_settings)
 
         response = cls._client.post(url=cls._jobs_path(), json=job_data)
 
         job_response = response.json()
         job_id = get_id_from_response(response)
 
         upload_thread = None
 
         if intake_file is not None:
-            upload_thread = cls._upload_intake_file(
-                intake_file, intake_settings, job_response, upload_read_timeout, output_file
-            )
+
+            # There is source data to upload, so spin up a thread to handle
+            # the upload concurrently and for thread safety issues, make
+            # a copy of the REST client object
+
+            _upload_client = cls._client.copy()
+            job_csv_settings = job_response.get("jobSpec", {}).get("csvSettings", {})
+
+            def _get_file_size(fileobj):
+                # To cover both files and filelike obj utilize .tell
+                cur = fileobj.tell()
+                fileobj.seek(0, os.SEEK_END)
+                file_size = fileobj.tell()
+                fileobj.seek(cur)
+
+                return file_size
+
+            # pylint: disable-next=unused-argument
+            def _create_csv_chunk(header, reader, max_size, delimiter, encoding, quotechar):
+                chunk = io.StringIO()
+                bytes_written = 0
+                writer = csv.writer(chunk, delimiter=delimiter, quotechar=quotechar)
+                writer.writerow(header)
+                while bytes_written < max_size:
+                    try:
+                        csv_chunk_content = next(reader)
+                        written = writer.writerow(csv_chunk_content)
+                        bytes_written += written
+                    except (StopIteration):
+                        break
+
+                return chunk, bytes_written
+
+            def _fileobj_to_csv_stream(fileobj, encoding):
+                stream = io.TextIOWrapper(fileobj, encoding=encoding)
+
+                yield from csv.reader(stream)
+
+                stream.close()
+
+            def _upload_multipart(fileobj, base_upload_url):
+                is_async = intake_settings.get("async", True)
+                MAX_RETRY = 1 if is_async else 3
+                MB_PER_CHUNK = 5
+                CHUNK_MAX_SIZE = MB_PER_CHUNK * 1024 * 1024
+
+                delimiter = job_csv_settings.get("delimiter", ",")
+                encoding = job_csv_settings.get("encoding", "utf-8")
+                quotechar = job_csv_settings.get("quotechar", '"')
+
+                file_size = _get_file_size(fileobj)
+                csv_stream = _fileobj_to_csv_stream(fileobj, encoding)
+
+                # grab the header so it can be added on all parts
+                header = next(csv_stream)
+
+                part_number = 0
+                bytes_written = 0
+                while bytes_written <= file_size:
+                    part_upload_url = f"{base_upload_url}part/{part_number}"
+
+                    # Read the inputfile in chunks of CHUNK_MAX_SIZE
+                    # Then call put multiple times increasing the part_number each time
+                    chunk, chunk_bytes = _create_csv_chunk(
+                        header, csv_stream, CHUNK_MAX_SIZE, delimiter, encoding, quotechar
+                    )
+                    bytes_written += chunk_bytes
+                    if chunk_bytes == 0:
+                        break
+
+                    for attempts in range(MAX_RETRY):
+                        try:
+                            chunk.seek(0)
+                            response = _upload_client.put(
+                                url=part_upload_url,
+                                data=chunk,
+                                headers={"content-type": "text/csv"},
+                                timeout=(_upload_client.connect_timeout, upload_read_timeout),
+                            )
+
+                            # Success! don't retry
+                            if response.status_code == 202:
+                                chunk.close()
+                                break
+                        except (requests.exceptions.ConnectionError, requests.exceptions.Timeout):
+                            attempts += 1
+                            if attempts == MAX_RETRY:
+                                raise
+
+                    part_number += 1
+
+                # finalize the upload to indicate no more data is arriving
+                _upload_client.post(url=f"{base_upload_url}finalizeMultipart")
+
+            def _uploader() -> None:
+                upload_url = job_response["links"]["csvUpload"]
+
+                if "file_path" in intake_file:
+                    fileobj = open(  # pylint: disable=consider-using-with
+                        intake_file["file_path"], "rb"
+                    )
+                else:
+                    fileobj = intake_file["filelike"]
+                    fileobj.seek(0)
+
+                try:
+                    if intake_settings.get("multipart"):
+                        _upload_multipart(fileobj, upload_url)
+
+                    else:
+                        _upload_client.put(
+                            url=upload_url,
+                            data=fileobj,
+                            headers={"content-type": "text/csv"},
+                            timeout=(_upload_client.connect_timeout, upload_read_timeout),
+                        )
+                finally:
+                    if hasattr(fileobj, "close"):
+                        fileobj.close()
+
+            if output_file is not None:
+
+                # If output_file is specified, we upload and download
+                # concurrently
+
+                upload_thread = threading.Thread(target=_uploader)
+                upload_thread.setDaemon(True)
+                upload_thread.start()
+
+            else:
+
+                # Otherwise, upload is synchronous
+
+                _uploader()
 
         job = BatchPredictionJob.get(job_id)
 
         if output_file is not None:
 
             # We must download the result to `output_file`
             # And clean up any thread we spawned during uploading
@@ -1228,32 +1606,99 @@
             Set to -1 to wait infinitely.
 
         read_timeout : int (optional, default 660)
             .. versionadded:: 2.22
 
             Seconds to wait for the server to respond between chunks.
         """
-        self._download(fileobj, timeout, read_timeout)
+        status = self._wait_for_download(timeout=timeout)
+        download_iter = self._client.get(
+            status["links"]["download"],
+            stream=True,
+            timeout=read_timeout,
+        ).iter_content(chunk_size=8192)
+
+        for chunk in download_iter:
+            if chunk:
+                fileobj.write(chunk)
+
+        # Check if job was aborted during download (and the download is incomplete)
+        status = self.get_status()
+        if status["status"] in ("ABORTED", "FAILED"):
+            raise RuntimeError("Job {} was aborted: {}".format(self.id, status["status_details"]))
+
+    def _wait_for_download(self, timeout: int = 120):
+        """Waits for download to become available"""
+        start = time.time()
+        status = None
+        while True:
+            status = self.get_status()
+
+            output_adapter_type = status["job_spec"].get("output_settings", {}).get("type")
+            if output_adapter_type and not output_adapter_type == "localFile":
+                raise RuntimeError(
+                    (
+                        "You cannot download predictions from jobs that did not use local_file as "
+                        "the output adapter. Job with ID {} had the output adapter defined as {}."
+                    ).format(self.id, output_adapter_type)
+                )
+
+            if status["status"] in ("ABORTED", "FAILED"):
+                raise RuntimeError(
+                    "Job {} was aborted: {}".format(self.id, status["status_details"])
+                )
+
+            if "download" in status["links"]:
+                break
+
+            if timeout >= 0 and time.time() - start > timeout:  # pylint: disable=chained-comparison
+                break
+
+            time.sleep(1)
+
+        if "download" not in status["links"]:
+            # Ignore 404 errors here if the job never started - then we can't abort it
+            self.delete(ignore_404_errors=True)
+            raise RuntimeError(
+                (
+                    "Timed out waiting for download to become available for job ID {}. "
+                    "Other jobs may be occupying the queue. Consider raising the timeout."
+                ).format(self.id)
+            )
+
+        return status
 
     def delete(self, ignore_404_errors: bool = False) -> None:
         """
         Cancel this job. If this job has not finished running, it will be
         removed and canceled.
         """
-        self._delete(ignore_404_errors)
+        status = self.get_status()
+
+        prediction_job_id = status["links"]["self"].split("/")[-2]
+        try:
+            self._client.delete(self._job_path(None, prediction_job_id))
+        except errors.ClientError as exc:
+            if exc.status_code == 404 and ignore_404_errors:
+                return
+            raise
 
     def get_status(self):
         """Get status of batch prediction job
 
         Returns
         -------
         BatchPredictionJob status data
             Dict with job status
         """
-        return self._get_status()
+
+        batch_job = super().get(None, self.id)
+        batch_job.id = self.id
+
+        return batch_job._safe_data
 
     @classmethod
     def list_by_status(cls, statuses: Optional[List[str]] = None) -> List[BatchPredictionJob]:
         """Get jobs collection for specific set of statuses
 
         Attributes
         ----------
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/credential.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
 import json
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import trafaret as t
 from trafaret.contrib.rfc_3339 import DateTime
 
 from datarobot._compat import String
 from datarobot.models.api_object import APIObject
 from datarobot.utils import pagination, rawdict
@@ -377,42 +377,14 @@
             "name": name,
             "credentialType": "gcp",
             "gcpKey": rawdict(gcp_key),  # type: ignore[arg-type]
             "description": description,
         }
         return cls.from_server_data(cls._client.post(cls._path, data=payload).json())
 
-    def update(
-        self, name: Optional[str] = None, description: Optional[str] = None, **kwargs: Any
-    ) -> None:
-        """Update the credential values of an existing credential. Updates this object in place.
-
-        .. versionadded:: v3.2
-
-        Parameters
-        ----------
-        name : str
-            The name to use for this set of credentials.
-        description : str, optional
-            The description to use for this set of credentials; if omitted, and name is not
-            omitted, then it clears any previous description for that name.
-        kwargs : Keyword arguments specific to the given credential_type that should be updated.
-        """
-        if name is not None:
-            kwargs["name"] = name
-        if description is not None:
-            kwargs["description"] = description
-
-        self._client.patch(f"{self._path}{self.credential_id}/", data=kwargs)
-
-        if name is not None:
-            self.name = name
-        if description is not None:
-            self.description = description
-
 
 BasicCredentialsSchema = t.Dict(
     {
         t.Key("credentialType"): t.Atom("basic"),
         t.Key("user"): String(),
         t.Key("password"): String(),
     }
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,25 +411,22 @@
     training_dataset_version_id: str, optional
         The ID of a dataset version assigned to the custom model.
     training_data_file_name: str, optional
         The name of assigned training data file.
     training_data_partition_column: str, optional
         The name of a partition column in a training dataset assigned to the custom model.
     created_by: str
-        The username of a user who created the custom model.
+        The username of a user who user who created the custom model.
     updated_at: str
         ISO-8601 formatted timestamp of when the custom model was updated
     created_at: str
         ISO-8601 formatted timestamp of when the custom model was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
-        is only supported by the SaaS (cloud) environment.
+        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     is_training_data_for_versions_permanently_enabled: bool, optional
         Whether training data assignment on the version level is permanently enabled for the model.
@@ -635,18 +632,15 @@
             Custom inference model class labels for multiclass classification.
             Cannot be used with class_labels_file.
         class_labels_file: str, optional
             Path to file containing newline separated class labels for multiclass classification.
             Cannot be used with class_labels.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`]
-            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
-            is only supported by the SaaS (cloud) environment.
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         is_training_data_for_versions_permanently_enabled: bool, optional
             Permanently enable training data assignment on the version level for the current model,
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,17 +58,15 @@
         id of a dataset version used for testing
     completed_at: str, optional
         ISO-8601 formatted timestamp of when the test has completed
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
+        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     """
 
@@ -165,18 +163,15 @@
             The id of the testing dataset for non-unstructured custom models.
             Ignored and not required for unstructured models.
         max_wait: int, optional
             max time to wait for a test completion.
             If set to None - method will return without waiting.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
-            is only supported by the SaaS (cloud) environment.
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
 
         Returns
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,17 +523,15 @@
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created.
     dependencies: List[CustomDependency]
         The parsed dependencies of the custom model version if the
         version has a valid requirements.txt file.
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
+        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster.
     required_metadata_values: List[RequiredMetadataValue]
         Additional parameters required by the execution environment. The required keys are
@@ -688,18 +686,15 @@
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
-            is only supported by the SaaS (cloud) environment.
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
@@ -858,18 +853,15 @@
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         files_to_delete: list, optional
             The list of a file items ids to be deleted.
             Example: ["5ea95f7a4024030aba48e4f9", "5ea6b5da402403181895cc51"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
-            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
-            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
-            is only supported by the SaaS (cloud) environment.
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/data_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Dict, List, Optional, TYPE_CHECKING, Union
+from typing import Dict, List, Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
 from datarobot.enums import DATA_STORE_TABLE_TYPE
 from datarobot.models.api_object import APIObject, ServerDataType
-from datarobot.models.credential import CredentialDataSchema
-from datarobot.models.sharing import SharingAccess, SharingRole
-from datarobot.utils import deprecated, deprecation_warning, from_api, parse_time, to_api
+from datarobot.models.sharing import SharingAccess
+from datarobot.utils import from_api, parse_time
 from datarobot.utils.pagination import unpaginate
 
 _data_store_params_converter = t.Dict(
     {t.Key("driver_id"): String(), t.Key("jdbc_url", optional=True): t.Or(String(), t.Null())}
 ).ignore_extra("*")
 
 if TYPE_CHECKING:
@@ -246,43 +245,25 @@
         self.canonical_name = r_data["canonicalName"]
         self.params = DataStoreParameters(r_data["params"]["driverId"], r_data["params"]["jdbcUrl"])
 
     def delete(self) -> None:
         """Removes the DataStore"""
         self._client.delete(f"{self._path}{self.id}/")
 
-    def test(
-        self,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        credential_id: Optional[str] = None,
-        use_kerberos: Optional[bool] = None,
-        credential_data: Optional[Dict[str, str]] = None,
-    ) -> TestResponse:
+    def test(self, username: str, password: str) -> TestResponse:
         """
         Tests database connection.
 
-        .. versionchanged:: v3.2
-           Added `credential_id`, `use_kerberos` and `credential_data` optional params and made
-           `username` and `password` optional.
-
         Parameters
         ----------
         username : str
-            optional, the username for database authentication.
+            the username for database authentication.
         password : str
-            optional, the password for database authentication. The password is encrypted
+            the password for database authentication. The password is encrypted
             at server side and never saved / stored
-        credential_id : str
-            optional, id of the set of credentials to use instead of username and password
-        use_kerberos : bool
-            optional, whether to use Kerberos for data store authentication
-        credential_data : dict
-            optional, the credentials to authenticate with the database, to use instead of
-            user/password or credential ID
 
         Returns
         -------
         message : dict
             message with status.
 
         Examples
@@ -290,23 +271,16 @@
         .. code-block:: python
 
             >>> import datarobot as dr
             >>> data_store = dr.DataStore.get('5ad5d2afef5cd700014d3cae')
             >>> data_store.test(username='db_username', password='db_password')
             {'message': 'Connection successful'}
         """
-        payload = {
-            "user": username,
-            "password": password,
-            "credential_id": credential_id,
-            "use_kerberos": use_kerberos,
-        }
-        if credential_data:
-            payload["credential_data"] = CredentialDataSchema(credential_data)
-        return self._client.post(f"{self._path}{self.id}/test/", data=to_api(payload)).json()  # type: ignore[no-any-return] # noqa: E501
+        payload = {"user": username, "password": password}
+        return self._client.post(f"{self._path}{self.id}/test/", data=payload).json()  # type: ignore[no-any-return]
 
     def schemas(self, username: str, password: str) -> SchemasResponse:
         """
         Returns list of available schemas.
 
         Parameters
         ----------
@@ -391,117 +365,56 @@
     def type(self) -> Optional[str]:
         return self._type
 
     @property
     def updated(self) -> Optional[datetime]:
         return self._updated
 
-    @deprecated(
-        deprecated_since_version="v3.2",
-        will_remove_version="v3.4",
-        message="Please use get_shared_roles instead.",
-    )
     def get_access_list(self) -> List[SharingAccess]:
         """Retrieve what users have access to this data store
 
         .. versionadded:: v2.14
 
         Returns
         -------
         list of :class:`SharingAccess <datarobot.SharingAccess>`
         """
         url = f"{self._path}{self.id}/accessControl/"
         return [
             SharingAccess.from_server_data(datum) for datum in unpaginate(url, {}, self._client)
         ]
 
-    def get_shared_roles(self) -> List[SharingRole]:
-        """Retrieve what users have access to this data store
-
-        .. versionadded:: v3.2
-
-        Returns
-        -------
-        list of :class:`SharingRole <datarobot.models.sharing.SharingRole>`
-        """
-        url = f"{self._path}{self.id}/sharedRoles/"
-        return [SharingRole.from_server_data(datum) for datum in unpaginate(url, {}, self._client)]
-
-    def share(self, access_list: Union[List[SharingAccess], List[SharingRole]]) -> None:
+    def share(self, access_list: List[SharingAccess]) -> None:
         """Modify the ability of users to access this data store
 
         .. versionadded:: v2.14
 
         Parameters
         ----------
-        access_list : list of :class:`SharingRole <datarobot.models.sharing.SharingRole>`
+        access_list : list of :class:`SharingAccess <datarobot.SharingAccess>`
             the modifications to make.
 
         Raises
         ------
         datarobot.ClientError :
             if you do not have permission to share this data store, if the user you're sharing with
             doesn't exist, if the same user appears multiple times in the access_list, or if these
             changes would leave the data store without an owner.
 
         Examples
         --------
-        The :class:`SharingRole <datarobot.models.sharing.SharingRole>` class is needed in order to
-        share a Data Store with one or more users.
-
-        For example, suppose you had a list of user IDs you wanted to share this DataStore with. You could use
-        a loop to generate a list of :class:`SharingRole <datarobot.models.sharing.SharingRole>` objects for them,
-        and bulk share this Data Store.
+        Transfer access to the data store from old_user@datarobot.com to new_user@datarobot.com
 
         .. code-block:: python
 
-            >>> import datarobot as dr
-            >>> from datarobot.models.sharing import SharingRole
-            >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
-            >>>
-            >>> user_ids = ["60912e09fd1f04e832a575c1", "639ce542862e9b1b1bfa8f1b", "63e185e7cd3a5f8e190c6393"]
-            >>> sharing_roles = []
-            >>> for user_id in user_ids:
-            ...     new_sharing_role = SharingRole(
-            ...         role=SHARING_ROLE.CONSUMER,
-            ...         share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
-            ...         id=user_id,
-            ...         can_share=True,
-            ...     )
-            ...     sharing_roles.append(new_sharing_role)
-            >>> dr.DataStore.get('my-data-store-id').share(access_list)
-
-        Similarly, a :class:`SharingRole <datarobot.models.sharing.SharingRole>` instance can be used to
-        remove a user's access if the ``role`` is set to ``SHARING_ROLE.NO_ROLE``, like in this example:
-
-        .. code-block:: python
+            import datarobot as dr
 
-            >>> import datarobot as dr
-            >>> from datarobot.models.sharing import SharingRole
-            >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
-            >>>
-            >>> user_to_remove = "foo.bar@datarobot.com"
-            ... remove_sharing_role = SharingRole(
-            ...     role=SHARING_ROLE.NO_ROLE,
-            ...     share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
-            ...     username=user_to_remove,
-            ...     can_share=False,
-            ... )
-            >>> dr.DataStore.get('my-data-store-id').share(roles=[remove_sharing_role])
-        """
-        if any(isinstance(access, SharingAccess) for access in access_list):
-            if not (all(isinstance(access, SharingAccess) for access in access_list)):
-                raise ValueError("Please use either all SharingRole or all SharingAccess objects.")
-            deprecation_warning(
-                subject="SharingAccess",
-                deprecated_since_version="v3.2",
-                will_remove_version="v3.4",
-                message="Please use SharingRole objects instead of SharingAccess objects.",
-            )
-            payload = {"data": [access.collect_payload() for access in access_list]}
-            self._client.patch(
-                f"{self._path}{self.id}/accessControl/", data=payload, keep_attrs={"role"}
-            )
-        else:
-            formatted_roles = [access.collect_payload() for access in access_list]
-            payload = {"roles": formatted_roles, "operation": "updateRoles"}  # type: ignore[dict-item]
-            self._client.patch(f"{self._path}{self.id}/sharedRoles/", data=payload)
+            new_access = dr.SharingAccess(new_user@datarobot.com,
+                                          dr.enums.SHARING_ROLE.OWNER, can_share=True)
+            access_list = [dr.SharingAccess(old_user@datarobot.com, None), new_access]
+
+            dr.DataStore.get('my-data-store-id').share(access_list)
+        """
+        payload = {"data": [access.collect_payload() for access in access_list]}
+        self._client.patch(
+            f"{self._path}{self.id}/accessControl/", data=payload, keep_attrs={"role"}
+        )
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from collections import namedtuple
 from io import BytesIO, IOBase, StringIO
 import os
-import tempfile
 from typing import Any, cast, Dict, Generator, List, Optional, Set, Type, TypeVar, Union
 
 import dateutil
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
@@ -968,41 +967,28 @@
         response = self._client.get(f"{self._path}{self.id}/file/")
         if file_path:
             with open(file_path, "wb") as f:
                 f.write(response.content)
         if filelike:
             filelike.write(response.content)
 
-    def get_as_dataframe(self, low_memory: Optional[bool] = False) -> pd.DataFrame:
+    def get_as_dataframe(self) -> pd.DataFrame:
         """
         Retrieves all the originally uploaded data in a pandas DataFrame.
 
         .. versionadded:: v3.0
 
-        Parameters
-        ----------
-        low_memory: bool, optional
-            If True, use local files to reduce memory usage which will be slower.
-
         Returns
         -------
         pd.DataFrame
         """
-        if low_memory:
-            with tempfile.NamedTemporaryFile(suffix=".csv") as csv_file:
-                iter = self._client.get(f"{self._path}{self.id}/file/", stream=True)
-                with open(csv_file.name, "wb") as out:
-                    for chunk in iter.iter_content(1000):
-                        out.write(chunk)
-                return pd.read_csv(csv_file.name)
-        else:
-            raw_bytes = BytesIO()
-            self.get_file(filelike=raw_bytes)
-            data = StringIO(raw_bytes.getvalue().decode())
-            return pd.read_csv(data)
+        raw_bytes = BytesIO()
+        self.get_file(filelike=raw_bytes)
+        data = StringIO(raw_bytes.getvalue().decode())
+        return pd.read_csv(data)
 
     def get_projects(self) -> List[ProjectLocation]:
         """
         Retrieves the Dataset's projects as ProjectLocation named tuples.
 
         Returns
         -------
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
-from datarobot.models.status_check_job import StatusCheckJob
 from datarobot.utils import deprecated, from_api, get_id_from_location
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
@@ -995,91 +994,14 @@
                         timestamp = timestamp.isoformat()
                     actual["timestamp"] = timestamp
 
                 payload.append(actual)
             response = self._client.post(url, data={"data": payload})
             wait_for_async_resolution(self._client, response.headers["Location"])
 
-    def submit_actuals_from_catalog_async(
-        self,
-        dataset_id: str,
-        actual_value_column: str,
-        association_id_column: str,
-        dataset_version_id: Optional[str] = None,
-        timestamp_column: Optional[str] = None,
-        was_acted_on_column: Optional[str] = None,
-    ) -> StatusCheckJob:
-        """Submit actuals from AI Catalog for processing.
-        The actuals submitted will be used to calculate accuracy metrics.
-
-        Parameters
-        ----------
-        dataset_id: str,
-            The ID of the source dataset.
-        dataset_version_id: str, optional
-            The ID of the dataset version to apply the query to. If not specified, the
-            latest version associated with dataset_id is used.
-        association_id_column: str,
-            The name of the column that contains a unique identifier used with a prediction.
-        actual_value_column: str,
-            The name of the column that contains the actual value of a prediction.
-        was_acted_on_column: str, optional,
-            The name of the column that indicates if the prediction was acted on in a way that
-            could have affected the actual outcome.
-        timestamp_column: str, optional,
-            The name of the column that contains datetime or string in RFC3339 format.
-
-        Returns
-        -------
-        status_check_job : StatusCheckJob
-            Object contains all needed logic for a periodical status check of an async job.
-
-        Raises
-        ------
-        ValueError
-            if dataset_id not provided
-            if actual_value_column not provided
-            if association_id_column not provided
-
-        Examples
-        --------
-        .. code-block:: python
-
-            from datarobot import Deployment
-            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
-            status_check_job = deployment.submit_actuals_from_catalog_async(data)
-        """
-        if not dataset_id:
-            raise ValueError("Catalog Dataset ID is required to submit actuals.")
-
-        if not actual_value_column:
-            raise ValueError("Actual value column is required to submit actuals.")
-
-        if not association_id_column:
-            raise ValueError("Association id column is required to submit actuals.")
-
-        actuals_config = {
-            "actualValueColumn": actual_value_column,
-            "associationIdColumn": association_id_column,
-            "datasetId": dataset_id,
-            "datasetVersionId": dataset_version_id,
-        }
-
-        if timestamp_column:
-            actuals_config["timestampColumn"] = timestamp_column
-
-        if was_acted_on_column:
-            actuals_config["wasActedOnColumn"] = was_acted_on_column
-
-        url = f"{self._path}{self.id}/actuals/fromDataset/"
-
-        response = self._client.post(url, data=actuals_config)
-
-        return StatusCheckJob.from_response(response)
-
     def get_predictions_by_forecast_date_settings(self) -> ForecastDateSettings:
         """Retrieve predictions by forecast date settings of this deployment.
 
         .. versionadded:: v2.27
 
         Returns
         -------
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/feature_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,16 +135,14 @@
     ----------
     project_id: string
         The project that contains requested model
     model_id: string
         The model to retrieve Feature Effects for
     source: string
         The source to retrieve Feature Effects for
-    data_slice_id: string or None
-        The slice to retrieve Feature Effects for; if None, retrieve unsliced data
     feature_effects: list
         Feature Effects for every feature
     backtest_index: string, required only for DatetimeModels,
         The backtest index to retrieve Feature Effects for.
 
     Notes
     -----
@@ -243,57 +241,52 @@
     ).ignore_extra("*")
 
     _converter = t.Dict(
         {
             t.Key("project_id"): String,
             t.Key("model_id"): String,
             t.Key("source"): String,
-            t.Key("data_slice_id", optional=True): t.Or(String, t.Null),
             t.Key("backtest_index", optional=True): String,
             t.Key("feature_effects"): t.List(_FeatureEffect),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         project_id,
         model_id,
         source,
         feature_effects,
-        data_slice_id=None,
         backtest_index=None,
     ):
         self.project_id = project_id
         self.model_id = model_id
         self.source = source
-        self.data_slice_id = data_slice_id
         self.backtest_index = backtest_index
         self.feature_effects = feature_effects
 
     def __repr__(self):
         return (
             "{}(project_id={},"
-            "model_id={}, source={}, data_slice_id={},backtest_index={}, feature_effects={}".format(
+            "model_id={}, source={}, backtest_index={}, feature_effects={}".format(
                 self.__class__.__name__,
                 self.project_id,
                 self.model_id,
                 self.source,
-                self.data_slice_id,
                 self.backtest_index,
                 self.feature_effects,
             )
         )
 
     def __eq__(self, other):
         return all(
             [
                 self.project_id == other.project_id,
                 self.model_id == other.model_id,
                 self.source == other.source,
-                self.data_slice_id == other.data_slice_id,
                 self.backtest_index == other.backtest_index,
                 (
                     sorted(self.feature_effects, key=lambda k: k["feature_name"])
                     == sorted(other.feature_effects, key=lambda k: k["feature_name"])
                 ),
             ]
         )
@@ -301,63 +294,33 @@
     def __hash__(self):
         return hash(
             (
                 self.__class__.__name__,
                 self.project_id,
                 self.model_id,
                 self.source,
-                self.data_slice_id,
                 self.backtest_index,
             )
         )
 
     def __iter__(self):
         return iter(self.feature_effects)
 
-    @staticmethod
-    def _repack_insights_response(server_data, insight_name):
-        """Repack the JSON sent by the GET /insights/ endpoint to match the format expected by the
-        insight APIObject class.
-
-        Parameters
-        ----------
-        raw_server_data : dict
-        insight_name : str
-
-        Returns
-        -------
-        server_data : dict
-        """
-        this_item = server_data["data"][0]
-        repacked_server_data = {
-            "projectId": this_item["projectId"],
-            "modelId": this_item["entityId"],
-            "source": this_item["source"],
-            insight_name: this_item["data"][insight_name],
-            "dataSliceId": this_item["dataSliceId"],
-        }
-        return repacked_server_data
-
     @classmethod
-    def from_server_data(cls, data, *args, use_insights_format=False, **kwargs):
+    def from_server_data(cls, data, *args, **kwargs):
         """
         Instantiate an object of this class using the data directly from the server,
         meaning that the keys may have the wrong camel casing.
 
         Parameters
         ----------
         data : dict
             The directly translated dict of JSON from the server. No casing fixes have
             taken place
-        use_insights_format : bool, optional
-            Whether to repack the data from the format used in the GET /insights/featureEffects/ URL
-            to the format used in the legacy URL.
         """
-        if use_insights_format:
-            data = cls._repack_insights_response(data, insight_name="featureEffects")
         # keep_null_keys is required for predicted/actual
         case_converted = from_api(data, keep_null_keys=True)
         return cls.from_data(case_converted)
 
 
 class FeatureEffectsMulticlass(APIObject):
     """
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,15 @@
             return Model.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PREDICT:
             return raw_prediction_response_to_dataframe(server_data, PREDICTION_PREFIX.DEFAULT)
         elif self.job_type == JOB_TYPE.FEATURE_IMPACT:
             # Note: a custom FeatureImpactJob class is used for high level API now.
             return server_data["featureImpacts"]
         elif self.job_type == JOB_TYPE.FEATURE_EFFECTS:
-            use_insights_format = "count" in server_data
-            return FeatureEffects.from_server_data(
-                server_data, use_insights_format=use_insights_format
-            )
+            return FeatureEffects.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_RULESETS:
             return [Ruleset.from_server_data(ruleset_data) for ruleset_data in server_data]
         elif self.job_type == JOB_TYPE.PRIME_MODEL:
             return PrimeModel.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_VALIDATION:
             return PrimeFile.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PREDICTION_EXPLANATIONS_INITIALIZATION:
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,14 @@
         were used to train the model and evaluate backtest scores.
     supports_composable_ml : bool or None
         (New in version v2.26)
         whether this model is supported in the Composable ML.
     """
 
     _base_model_path_template = "projects/{}/models/"
-    _base_insights_template = "insights/{}/"
 
     _converter = t.Dict(
         {
             t.Key("id", optional=True): String,
             t.Key("processes", optional=True): t.List(String),
             t.Key("featurelist_name", optional=True): String,
             t.Key("featurelist_id", optional=True): String,
@@ -986,46 +985,14 @@
         from .predict_job import PredictJob  # pylint: disable=import-outside-toplevel,cyclic-import
 
         url = f"projects/{self.project_id}/predictions/"
         response = self._client.post(url, data=data)
         job_id = get_id_from_response(response)
         return PredictJob.from_id(self.project_id, job_id)
 
-    def _raise_if_not_slice_forbidden_error(self, e: Exception) -> None:
-        """If the user does not have the SLICED_INSIGHTS feature flag enabled, then all requests to
-        the /insights/ endpoints will be rejected with 403 FORBIDDEN. Also, some project types
-        are currently not supported by the /insights/ endpoint. Use this method to check the
-        error for that case. For any other error, reraise.
-        """
-        if e.status_code not in [403, 422]:
-            raise e
-
-    def _post_insights_url(self, insight_name: str) -> str:
-        """Build URL for requests to POST /insights/.../ endpoints, used with sliced insights."""
-        return self._base_insights_template.format(insight_name)
-
-    def _get_insights_url(self, insight_name: str) -> str:
-        """Build URL for requests to GET /insights/.../ endpoints, used with sliced insights."""
-        if self.id is None:
-            # This check is why this is a method instead of an attribute. Once we stop creating
-            # models without model id's in the tests, we can make this an attribute we set in the
-            # constructor.
-            raise ValueError("Sorry, id attribute is None so I can't make the url to this model.")
-        return f"insights/{insight_name}/models/{self.id}"
-
-    def _get_data_slice_params(self, data_slice_id: str, unsliced_only: bool) -> Dict[str, str]:
-        """Validate user input, raise an exception or return a valid data slice params dict"""
-
-        if data_slice_id:
-            if unsliced_only:
-                raise ValueError("Do not specify unsliced_only=true and data_slice_id together")
-
-            return {"dataSliceId": data_slice_id}
-        return {"unslicedOnly": "true"} if unsliced_only else {}
-
     def _get_feature_impact_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureImpact/"
 
     def get_feature_impact(self, with_metadata: bool = False):
         """
         Retrieve the computed Feature Impact results, a measure of the relevance of each
@@ -1244,57 +1211,43 @@
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadata.from_server_data(server_data)
 
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffects/"
 
-    def request_feature_effect(
-        self, row_count: Optional[int] = None, data_slice_id: Optional[str] = None
-    ):
+    def request_feature_effect(self, row_count: Optional[int] = None):
         """
-        Submit request to compute Feature Effects for the model.
+        Request feature effects to be computed for the model.
 
         See :meth:`get_feature_effect <datarobot.models.Model.get_feature_effect>` for more
         information on the result of the job.
 
         Parameters
         ----------
         row_count : int
             (New in version v2.21) The sample size to use for Feature Impact computation.
             Minimum is 10 rows. Maximum is 100000 rows or the training sample size of the model,
             whichever is less.
-        data_slice_id : str, optional
-            ID for the data slice used in the request. If None, request unsliced insight data.
 
         Returns
         -------
          job : Job
             A Job representing the feature effect computation. To get the completed feature effect
             data, use `job.get_result` or `job.get_result_when_complete`.
 
         Raises
         ------
         JobAlreadyRequested (422)
             If the feature effect have already been requested.
         """
         from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
-        if data_slice_id:
-            route = self._post_insights_url("featureEffects")
-            payload = {
-                "subset": "training",
-                "dataSliceId": data_slice_id,
-                "entityType": "datarobotModel",
-                "entityId": self.id,
-            }
-        else:
-            route = self._get_feature_effect_url()
-            payload = {"row_count": row_count}
-        response = self._client.post(route, data=payload)
+        route = self._get_feature_effect_url()
+        response = self._client.post(route, data={"row_count": row_count})
         job_id = get_id_from_response(response)
         return Job.get(self.project_id, job_id)
 
     def request_feature_effects_multiclass(
         self,
         row_count: Optional[int] = None,
         top_n_features: Optional[int] = None,
@@ -1325,15 +1278,15 @@
             project_id=self.project_id,
             model_id=self.id,
             row_count=row_count,
             top_n_features=top_n_features,
             features=features,
         )
 
-    def get_feature_effect(self, source: str, data_slice_id: Optional[str] = None):
+    def get_feature_effect(self, source: str):
         """
         Retrieve Feature Effects for the model.
 
         Feature Effects provides partial dependence and predicted vs actual values for top-500
         features ordered by feature impact score.
 
         The partial dependence shows marginal effect of a feature on the target variable after
@@ -1347,41 +1300,29 @@
         See :meth:`get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>`
         for retrieving information the available sources.
 
         Parameters
         ----------
         source : string
             The source Feature Effects are retrieved for.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, retrieve unsliced insight data.
 
         Returns
         -------
         feature_effects : FeatureEffects
            The feature effects data.
 
         Raises
         ------
         ClientError (404)
             If the feature effects have not been computed or source is not valid value.
         """
-        insight_name = "featureEffects"
         params = {"source": source}
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-        try:
-            insights_fe_url = self._get_insights_url(insight_name)
-            server_data = self._client.get(insights_fe_url, params=params).json()
-            use_insights_format = True
-        except ClientError as e:
-            self._raise_if_not_slice_forbidden_error(e)
-            fe_url = self._get_feature_effect_url()
-            server_data = self._client.get(fe_url, params=params).json()
-            use_insights_format = False
-        return FeatureEffects.from_server_data(server_data, use_insights_format=use_insights_format)
+        fe_url = self._get_feature_effect_url()
+        server_data = self._client.get(fe_url, params=params).json()
+        return FeatureEffects.from_server_data(server_data)
 
     def get_feature_effects_multiclass(
         self, source: str = "training", class_: Optional[str] = None
     ):
         """
         Retrieve Feature Effects for the multiclass model.
 
@@ -1471,56 +1412,49 @@
                 )
             else:
                 raise e
 
         return feature_effects
 
     def get_or_request_feature_effect(
-        self,
-        source: str,
-        max_wait: int = DEFAULT_MAX_WAIT,
-        row_count: Optional[int] = None,
-        data_slice_id: Optional[str] = None,
+        self, source: str, max_wait: int = DEFAULT_MAX_WAIT, row_count: Optional[int] = None
     ):
         """
-        Retrieve Feature Effects for the model, requesting a new job if it hasn't been run previously.
+        Retrieve feature effect for the model, requesting a job if it hasn't been run previously
 
         See :meth:`get_feature_effect_metadata \
         <datarobot.models.Model.get_feature_effect_metadata>`
         for retrieving information of source.
 
         Parameters
         ----------
-        source : string
-            The source Feature Effects are retrieved for.
         max_wait : int, optional
-            The maximum time to wait for a requested Feature Effect job to complete before erroring.
+            The maximum time to wait for a requested feature effect job to complete before erroring
         row_count : int, optional
             (New in version v2.21) The sample size to use for Feature Impact computation.
             Minimum is 10 rows. Maximum is 100000 rows or the training sample size of the model,
             whichever is less.
-        data_slice_id : str, optional
-            ID for the data slice used in the request. If None, request unsliced insight data.
+
+        source : string
+            The source Feature Effects are retrieved for.
 
         Returns
         -------
         feature_effects : FeatureEffects
-           The Feature Effects data.
+           The feature effects data.
         """
         try:
-            feature_effect_job = self.request_feature_effect(
-                row_count=row_count, data_slice_id=data_slice_id
-            )
+            feature_effect_job = self.request_feature_effect(row_count=row_count)
         except JobAlreadyRequested as e:
             # if already requested it may be still running
             # check and get the jobid in that case
             qid = e.json["jobId"]
             from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
-            feature_effect_job = Job.get(self.project_id, qid)  # fixme need custom job here too
+            feature_effect_job = Job.get(self.project_id, qid)
 
         params = {"source": source}
         return feature_effect_job.get_result_when_complete(max_wait=max_wait, params=params)
 
     def get_prime_eligibility(self):
         """Check if this model can be approximated with DataRobot Prime
 
@@ -1906,197 +1840,74 @@
         }
         if list(response_data) == ["residuals"]:
             response_data = response_data["residuals"]
         for data_source, data in response_data.items():
             reformatted["charts"].append(dict(source=data_source, **data))
         return reformatted
 
-    def request_lift_chart(
-        self, source: CHART_DATA_SOURCE, data_slice_id: Optional[str] = None
-    ) -> str:
-        """
-        Request the model Lift Chart for the specified source.
-
-        Parameters
-        ----------
-        source : str
-            Lift chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, request unsliced insight data.
-
-        Returns
-        -------
-        status_id : str
-            A statusId of computation request.
-        """
-
-        route = self._post_insights_url("liftChart")
-        params = {"entityId": self.id, "source": source}
-
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-
-        response = self._client.post(route, data=params)
-        status_id = get_id_from_response(response)
-
-        return status_id
-
-    def get_lift_chart(
-        self,
-        source: str,
-        fallback_to_parent_insights: Optional[bool] = False,
-        data_slice_id: Optional[str] = None,
-    ):
+    def get_lift_chart(self, source, fallback_to_parent_insights=False):
         """Retrieve the model Lift chart for the specified source.
 
         Parameters
         ----------
         source : str
             Lift chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
             (New in version v2.23) For time series and OTV models, also accepts values `backtest_2`,
             `backtest_3`, ..., up to the number of backtests in the model.
         fallback_to_parent_insights : bool
             (New in version v2.14) Optional, if True, this will return lift chart data for this
             model's parent if the lift chart is not available for this model and the model has a
             defined parent model. If omitted or False, or there is no parent model, will not
             attempt to return insight data from this model's parent.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, retrieve unsliced insight data.
 
         Returns
         -------
         LiftChart
             Model lift chart data
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
         """
-        insight_name = "liftChart"
-        params = {"source": source}
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-        else:
-            params["unslicedOnly"] = "true"
-        try:
-            insights_lift_url = self._get_insights_url(insight_name)
-            paginated_response = self._client.get(insights_lift_url, params=params).json()
-            response_data = paginated_response["data"][0]
-            use_insights_format = True
-        except ClientError as e:
-            self._raise_if_not_slice_forbidden_error(e)
-            url_template = "projects/{}/models/{}/liftChart/{}/"
-            response_data = self._get_insight(
-                url_template,
-                source,
-                "Lift Chart",
-                fallback_to_parent_insights=fallback_to_parent_insights,
-            )
-            use_insights_format = False
-        return LiftChart.from_server_data(
-            data=response_data, use_insights_format=use_insights_format
+        url_template = "projects/{}/models/{}/liftChart/{}/"
+        response_data = self._get_insight(
+            url_template,
+            source,
+            "Lift Chart",
+            fallback_to_parent_insights=fallback_to_parent_insights,
         )
+        return LiftChart.from_server_data(response_data)
 
-    def request_roc_curve(
-        self, source: CHART_DATA_SOURCE, data_slice_id: Optional[str] = None
-    ) -> str:
-        """
-        Request the model Roc Curve for the specified source.
-
-        Parameters
-        ----------
-        source : str
-            Roc Curve data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, request unsliced insight data.
-
-        Returns
-        -------
-        status_id : str
-            A statusId of computation request.
-        """
-
-        route = self._post_insights_url("rocCurve")
-        params = {"entityId": self.id, "source": source}
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-
-        response = self._client.post(route, data=params)
-        status_id = get_id_from_response(response)
-
-        return status_id
-
-    def get_all_lift_charts(
-        self,
-        fallback_to_parent_insights: Optional[bool] = False,
-        data_slice_id: Optional[str] = None,
-        unsliced_only: Optional[bool] = False,
-    ):
+    def get_all_lift_charts(self, fallback_to_parent_insights=False):
         """Retrieve a list of all Lift charts available for the model.
 
         Parameters
         ----------
-        fallback_to_parent_insights : bool, optional
+        fallback_to_parent_insights : bool
             (New in version v2.14) Optional, if True, this will return lift chart data for this
             model's parent for any source that is not available for this model and if this model
             has a defined parent model. If omitted or False, or this model has no parent,
             this will not attempt to retrieve any data from this model's parent.
-        data_slice_id : string, optional
-            ID for the data slice used in the request.
-        unsliced_only: bool
-            Optional, defaults to False.
-            If True return unsliced insight data.
 
         Returns
         -------
         list of LiftChart
             Data for all available model lift charts.
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
-
-        Examples
-        --------
-        .. code-block:: python
-
-            model = datarobot.Model.get('project-id', 'model-id')
-
-            # Get lift chart insights for sliced data
-            sliced_lift_charts = model.get_all_lift_charts(data_slice_id='data-slice-id')
-
-            # Get lift chart insights for unsliced data
-            unsliced_lift_charts = model.get_all_lift_charts(unsliced_only=True)
-
-            # Get all lift chart insights
-            all_lift_charts = model.get_all_lift_charts()
-
         """
-        insight_name = "liftChart"
-        params = self._get_data_slice_params(data_slice_id, unsliced_only)
-
-        try:
-            insights_lift_url = self._get_insights_url(insight_name)
-            paginated_response = self._client.get(insights_lift_url, params=params).json()
-            response_data = paginated_response["data"]
-            use_insights_format = True
-        except ClientError as e:
-            self._raise_if_not_slice_forbidden_error(e)
-            url_template = "projects/{}/models/{}/liftChart/"
-            data = self._get_all_source_insight(
-                url_template, "Lift Chart", fallback_to_parent_insights=fallback_to_parent_insights
-            )
-            response_data = data["charts"]
-            use_insights_format = False
-        return [
-            LiftChart.from_server_data(data=lc_data, use_insights_format=use_insights_format)
-            for lc_data in response_data
-        ]
+        url_template = "projects/{}/models/{}/liftChart/"
+        response_data = self._get_all_source_insight(
+            url_template, "Lift Chart", fallback_to_parent_insights=fallback_to_parent_insights
+        )
+        return [LiftChart.from_server_data(lc_data) for lc_data in response_data["charts"]]
 
     def get_multiclass_lift_chart(self, source, fallback_to_parent_insights=False):
         """Retrieve model Lift chart for the specified source.
 
         Parameters
         ----------
         source : str
@@ -2217,164 +2028,70 @@
                     target_class=bin["label"],
                     bins=bin["bins"],
                 )
             )
             lift_charts.append(lift_chart)
         return lift_charts
 
-    def get_residuals_chart(
-        self, source, fallback_to_parent_insights=False, data_slice_id: Optional[str] = None
-    ):
+    def get_residuals_chart(self, source, fallback_to_parent_insights=False):
         """Retrieve model residuals chart for the specified source.
 
         Parameters
         ----------
         source : str
             Residuals chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible
             values.
         fallback_to_parent_insights : bool
             Optional, if True, this will return residuals chart data for this model's parent if
             the residuals chart is not available for this model and the model has a defined parent
             model. If omitted or False, or there is no parent model, will not attempt to return
             residuals data from this model's parent.
-        data_slice_id: string
-            Optional, defaults to None.
-            ID for the data slice used in the request. If None, retrieve unsliced insight data.
 
         Returns
         -------
         ResidualsChart
             Model residuals chart data
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
         """
-
-        insight_name = "residuals"
-        params = {"source": source}
-
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-        else:
-            params["unslicedOnly"] = "true"
-
-        try:
-            insights_url = self._get_insights_url(insight_name)
-            response = self._client.get(insights_url, params=params).json()
-            response_data = response["data"][0]
-            use_insights_format = True
-        except ClientError as e:
-            self._raise_if_not_slice_forbidden_error(e)
-            url_template = "projects/{}/models/{}/residuals/{}/"
-            response_data = self._get_insight(
-                url_template,
-                source,
-                "Residuals Chart",
-                fallback_to_parent_insights=fallback_to_parent_insights,
-            )
-            use_insights_format = False
-
-        return ResidualsChart.from_server_data(
-            response_data, use_insights_format=use_insights_format
+        url_template = "projects/{}/models/{}/residuals/{}/"
+        response_data = self._get_insight(
+            url_template,
+            source,
+            "Residuals Chart",
+            fallback_to_parent_insights=fallback_to_parent_insights,
         )
+        return ResidualsChart.from_server_data(response_data)
 
-    def get_all_residuals_charts(
-        self,
-        fallback_to_parent_insights=False,
-        data_slice_id: Optional[str] = None,
-        unsliced_only: Optional[bool] = False,
-    ):
-        """Retrieve a list of all residuals charts available for the model.
+    def get_all_residuals_charts(self, fallback_to_parent_insights=False):
+        """Retrieve a list of all Lift charts available for the model.
 
         Parameters
         ----------
         fallback_to_parent_insights : bool
             Optional, if True, this will return residuals chart data for this model's parent
             for any source that is not available for this model and if this model has a
             defined parent model. If omitted or False, or this model has no parent, this will
             not attempt to retrieve any data from this model's parent.
-        data_slice_id: string
-            Optional, defaults to None.
-            ID for the data slice used in the request.
-        unsliced_only: bool
-            Optional, defaults to False.
-            If True return unsliced insight data.
 
         Returns
         -------
         list of ResidualsChart
             Data for all available model residuals charts.
-
-        Examples
-        --------
-        .. code-block:: python
-
-            model = datarobot.Model.get('project-id', 'model-id')
-
-            # Get residuals chart insights for sliced data
-            sliced_residuals_charts = model.get_all_residuals_charts(data_slice_id='data-slice-id')
-
-            # Get residuals chart insights for unsliced data
-            unsliced_residuals_charts = model.get_all_residuals_charts(unsliced_only=True)
-
-            # Get all residuals chart insights
-            all_residuals_charts = model.get_all_residuals_charts()
-
         """
-
-        insight_name = "residuals"
-        params = self._get_data_slice_params(data_slice_id, unsliced_only)
-
-        try:
-            insights_url = self._get_insights_url(insight_name)
-            data = self._client.get(insights_url, params=params).json()
-            response_data = data["data"]
-            use_insights_format = True
-        except ClientError as e:
-            self._raise_if_not_slice_forbidden_error(e)
-            url_template = "projects/{}/models/{}/residuals/"
-            data = self._get_all_source_insight(
-                url_template,
-                "Residuals Chart",
-                fallback_to_parent_insights=fallback_to_parent_insights,
-            )
-            response_data = data["charts"]
-            use_insights_format = False
-
-        return [
-            ResidualsChart.from_server_data(lc_data, use_insights_format=use_insights_format)
-            for lc_data in response_data
-        ]
-
-    def request_residuals_chart(
-        self, source: CHART_DATA_SOURCE, data_slice_id: Optional[str] = None
-    ) -> str:
-        """Request the model residuals chart for the specified source.
-
-        Parameters
-        ----------
-        source : str
-            Residuals chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, request unsliced insight data.
-
-        Returns
-        -------
-        status_id : str
-            The status ID of the computation request.
-        """
-
-        payload = {"entityId": self.id, "source": source}
-        if data_slice_id:
-            payload["dataSliceId"] = data_slice_id
-        route = self._post_insights_url("residuals")
-        response = self._client.post(route, data=payload)
-        return get_id_from_response(response)
+        url_template = "projects/{}/models/{}/residuals/"
+        response_data = self._get_all_source_insight(
+            url_template,
+            "Residuals Chart",
+            fallback_to_parent_insights=fallback_to_parent_insights,
+        )
+        return [ResidualsChart.from_server_data(lc_data) for lc_data in response_data["charts"]]
 
     def get_pareto_front(self):
         """Retrieve the Pareto Front for a Eureqa model.
 
         This method is only supported for Eureqa models.
 
         Returns
@@ -4494,15 +4211,15 @@
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadataDatetime.from_server_data(server_data)
 
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_datetime_model_url() + "featureEffects/"
 
-    # pylint: disable-next=arguments-differ
+    # pylint: disable-next=arguments-renamed
     def request_feature_effect(self, backtest_index):
         """
         Request feature effects to be computed for the model.
 
         See :meth:`get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` for more
         information on the result of the job.
 
@@ -4530,15 +4247,15 @@
 
         payload = {"backtestIndex": backtest_index}
         route = self._get_feature_effect_url()
         response = self._client.post(route, data=payload)
         job_id = get_id_from_response(response)
         return Job.get(self.project_id, job_id)
 
-    # pylint: disable-next=arguments-renamed
+    # pylint: disable-next=arguments-differ
     def get_feature_effect(self, source, backtest_index):
         """
         Retrieve Feature Effects for the model.
 
         Feature Effects provides partial dependence and predicted vs actual values for top-500
         features ordered by feature impact score.
 
@@ -4578,18 +4295,18 @@
             "source": source,
             "backtestIndex": backtest_index,
         }
         fe_url = self._get_feature_effect_url()
         server_data = self._client.get(fe_url, params=params).json()
         return FeatureEffects.from_server_data(server_data)
 
-    # pylint: disable-next=arguments-differ
+    # pylint: disable-next=arguments-renamed
     def get_or_request_feature_effect(self, source, backtest_index, max_wait=DEFAULT_MAX_WAIT):
         """
-        Retrieve Feature Effects computations for the model, requesting a new job if it hasn't been run previously.
+        Retrieve feature effect for the model, requesting a job if it hasn't been run previously
 
         See :meth:`get_feature_effect_metadata \
         <datarobot.models.DatetimeModel.get_feature_effect_metadata>`
         for retrieving information of source, backtest_index.
 
         Parameters
         ----------
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/sharing.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,21 +25,14 @@
 
     class SharingAccessPayload(TypedDict, total=False):
         username: str
         role: str
         can_share: bool
         can_use_data: bool
 
-    class SharingRolePayload(TypedDict, total=False):
-        id: Optional[str]
-        role: SHARING_ROLE
-        share_recipient_type: SHARING_RECIPIENT_TYPE
-        username: Optional[str]
-        can_share: bool
-
 
 class SharingAccess(APIObject):
     """Represents metadata about whom a entity (e.g. a data store) has been shared with
 
     .. versionadded:: v2.14
 
     Currently :py:class:`DataStores <datarobot.DataStore>`,
@@ -175,27 +168,7 @@
             raise InvalidUsageError("Please include either a username or an ID of a user.")
         self.id = id
         self.user_full_name = user_full_name
         self.role = SHARING_ROLE[role]
         self.share_recipient_type = share_recipient_type
         self.username = username
         self.can_share = can_share
-
-    def collect_payload(self) -> SharingRolePayload:
-        """
-        Generate a dictionary representation of this SharingRole.
-
-        Returns
-        -------
-        formatted_role : SharingRolePayload
-            A dictionary representation of this SharingRole ready for sending to DataRobot.
-        """
-        formatted_role: SharingRolePayload = {
-            "role": self.role,
-            "share_recipient_type": self.share_recipient_type,
-            "can_share": self.can_share,
-        }
-        if self.id:
-            formatted_role["id"] = self.id
-        if self.username:
-            formatted_role["username"] = self.username
-        return formatted_role
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/types.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/use_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,60 +118,14 @@
         self.entity_id = entity_id
         self.use_case_id = use_case_id
         self.created_at = created_at
         self.created = UseCaseUser(**created)
         self.is_deleted = is_deleted
 
 
-def get_reference_entity_info(
-    entity: Union[UseCaseReferenceEntity, T]
-) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
-    """
-    Get the entity type and entity id for a reference entity instance
-    Parameters
-    ----------
-    entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
-        The entity instance to add to a Use Case.
-    Returns
-    -------
-    entity_info : Tuple[UseCaseEntityType, str]
-        The entity type and entity id
-    """
-    from ..application import Application
-    from ..dataset import Dataset
-    from ..prediction_dataset import PredictionDataset
-    from ..project import Project
-
-    if isinstance(entity, Project):
-        return UseCaseAPIPathEntityType.PROJECT, entity.id
-    elif isinstance(entity, Dataset):
-        return UseCaseAPIPathEntityType.DATASET, entity.id
-    elif isinstance(entity, Application):
-        return UseCaseAPIPathEntityType.APPLICATION, entity.id
-    elif isinstance(entity, UseCaseReferenceEntity):
-        entity_type = UseCaseReferenceEntityMap.get(entity.entity_type)
-        if entity_type:
-            return entity_type, entity.entity_id
-    error_message = (
-        f"Entity must be Project, Dataset, Application, "
-        f"or UseCaseReferenceEntity. Invalid type: {type(entity).__name__}."
-    )
-    if isinstance(entity, UseCaseReferenceEntity):
-        # If we're failing here, it's because the UseCaseReferenceEntity is a notebook or other unsupported type
-        error_message = error_message + f" Unsupported Entity Type: {entity.entity_type}."
-    if isinstance(entity, PredictionDataset):
-        # Adding a specific error for PredictionDataset since the name would indicate it could
-        # be treated as a Dataset, when in fact it's a separate entity and not a subclass.
-        error_message = (
-            error_message + " PredictionDataset is not a subclass of Dataset and "
-            "cannot be added to a UseCase at this time."
-        )
-    raise TypeError(error_message)
-
-
 class UseCase(APIObject):
     """Representation of a Use Case.
 
     Attributes
     ----------
     id : str
         The ID of the Use Case.
@@ -437,14 +391,59 @@
             The updated Use Case.
         """
         payload = {"name": name, "description": description}
         path = f"{self._path}{self.id}/"
         r_data = self._client.patch(path, data=payload).json()
         return self.from_server_data(r_data)
 
+    def _get_reference_entity_info(
+        self, entity: Union[UseCaseReferenceEntity, T]
+    ) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
+        """
+        Get the entity type and entity id for a reference entity instance
+        Parameters
+        ----------
+        entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
+            The entity instance to add to a Use Case.
+        Returns
+        -------
+        entity_info : Tuple[UseCaseEntityType, str]
+            The entity type and entity id
+        """
+        from ..application import Application
+        from ..dataset import Dataset
+        from ..prediction_dataset import PredictionDataset
+        from ..project import Project
+
+        if isinstance(entity, Project):
+            return UseCaseAPIPathEntityType.PROJECT, entity.id
+        elif isinstance(entity, Dataset):
+            return UseCaseAPIPathEntityType.DATASET, entity.id
+        elif isinstance(entity, Application):
+            return UseCaseAPIPathEntityType.APPLICATION, entity.id
+        elif isinstance(entity, UseCaseReferenceEntity):
+            entity_type = UseCaseReferenceEntityMap.get(entity.entity_type)
+            if entity_type:
+                return entity_type, entity.entity_id
+        error_message = (
+            f"Entity must be Project, Dataset, Application, "
+            f"or UseCaseReferenceEntity. Invalid type: {type(entity).__name__}."
+        )
+        if isinstance(entity, UseCaseReferenceEntity):
+            # If we're failing here, it's because the UseCaseReferenceEntity is a notebook or other unsupported type
+            error_message = error_message + f" Unsupported Entity Type: {entity.entity_type}."
+        if isinstance(entity, PredictionDataset):
+            # Adding a specific error for PredictionDataset since the name would indicate it could
+            # be treated as a Dataset, when in fact it's a separate entity and not a subclass.
+            error_message = (
+                error_message + " PredictionDataset is not a subclass of Dataset and "
+                "cannot be added to a UseCase at this time."
+            )
+        raise TypeError(error_message)
+
     def add(
         self,
         entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
         entity_type: Optional[UseCaseEntityType] = None,
         entity_id: Optional[str] = None,
     ) -> UseCaseReferenceEntity:
         """
@@ -476,15 +475,15 @@
         if entity and (e_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not e_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
-            e_type, e_id = get_reference_entity_info(entity)
+            e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         r_data = self._client.post(path)
         return UseCaseReferenceEntity.from_server_data(r_data.json())
 
     def remove(
         self,
         entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
@@ -510,15 +509,15 @@
         if entity and (entity_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not entity_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
         if entity:
-            e_type, e_id = get_reference_entity_info(entity)
+            e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         self._client.delete(path)
         return None
 
     def share(
         self,
         roles: List[SharingRole],
@@ -597,15 +596,22 @@
             raise InvalidUsageError(
                 "Only NO_ROLE, OWNER, EDITOR, and CONSUMER roles are supported by Use Cases"
             )
         if any(role.share_recipient_type != SHARING_RECIPIENT_TYPE.USER for role in roles):
             raise InvalidUsageError(
                 "Use Cases currently only support sharing with users, not organizations."
             )
-        formatted_roles = [role.collect_payload() for role in roles]
+        formatted_roles = []
+        for role in roles:
+            formatted_role = {"role": role.role, "shareRecipientType": role.share_recipient_type}
+            if role.id:
+                formatted_role["id"] = role.id
+            if role.username:
+                formatted_role["username"] = role.username
+            formatted_roles.append(formatted_role)
         payload = {"roles": formatted_roles, "operation": "updateRoles"}
         path = f"{self._path}{self.id}/sharedRoles/"
         self._client.patch(path, data=payload)
         return None
 
     def get_shared_roles(
         self,
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/use_cases/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,48 +6,31 @@
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=cyclic-import
-import contextvars
 import functools
 from inspect import Parameter, signature
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, TypeVar, Union
-import warnings
+from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
 
 from typing_extensions import ParamSpec
 
 from datarobot.enums import UseCaseReferenceEntityMap
-from datarobot.errors import InvalidUsageError, MultipleUseCasesNotAllowed
-from datarobot.models.use_cases.use_case import (
-    get_reference_entity_info,
-    UseCase,
-    UseCaseReferenceEntity,
-)
+from datarobot.errors import InvalidUsageError
+from datarobot.models.use_cases.use_case import UseCase
 
 from ...context import Context
-from ...utils.logger import get_logger
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 UseCaseLike = Union[List[UseCase], UseCase, List[str], str]
 
-_use_case_linked: contextvars.ContextVar[Optional[Set[Tuple[str, str]]]] = contextvars.ContextVar(
-    "use_case_linked", default=None
-)
-_decorator_use_cases: contextvars.ContextVar[Optional[UseCaseLike]] = contextvars.ContextVar(
-    "decorator_use_cases", default=None
-)
-
-
-logger = get_logger(__name__)
-
 
 def resolve_use_cases(
     params: Dict[str, Any],
     use_cases: Optional[UseCaseLike] = None,
     use_case_key: str = "experiment_container_ids",
 ) -> Dict[str, Any]:
     """
@@ -98,23 +81,14 @@
         ]
     if isinstance(use_cases, UseCase):
         return [use_cases.id]
     else:
         return [use_cases]
 
 
-def _add_to_use_case(use_case_id: str, entity: Union[UseCaseReferenceEntity, T]) -> None:
-    _, entity_id = get_reference_entity_info(entity)
-    linked = _use_case_linked.get()
-    if entity_id is not None and linked is not None and (use_case_id, entity_id) not in linked:
-        use_case = UseCase.get(use_case_id=use_case_id)
-        use_case.add(entity=entity)
-        linked.add((use_case_id, entity_id))
-
-
 def add_to_use_case(
     allow_multiple: bool,
 ) -> Callable[[Callable[P, T]], Callable[..., T]]:
     """
     A decorator to mark functions as adding the return value to a given Use Case. When implemented,
     the decorator will add a `use_cases` keyword-only argument to the decorated function or method that
     will automatically add the returned object to a Use Case.
@@ -214,47 +188,23 @@
                 """
                 Parameters
                 ----------
                 use_cases: list[UseCase] | UseCase | list[string] | string, optional
                     A list of UseCase objects, UseCase object,
                     list of Use Case IDs or a single Use Case ID to add this new entity to. Must be a kwarg.
                 """
-                use_case_ids = None
-                context_use_case_token = None
-                linked_use_cases_token = None
+                ret = func(*args, **kwargs)
 
-                # take care of use_case param
                 if use_cases is None:
-                    # check contextvar that could be set by outer iterations first then Context
-                    use_cases = _decorator_use_cases.get(Context.use_case)
-                else:
-                    # if use_case passed, set it to be used by inner calls instead of Context
-                    context_use_case_token = _decorator_use_cases.set(use_cases)
-
-                try:
-                    if use_cases is not None:
-                        # Should only ever resolve to a single use case
-                        use_case_ids = resolve_use_case_ids(use_cases=use_cases)
-
-                    # _use_case_linked never created? must be top level call, initialize set
-                    # to track entities added to UseCase before we call the wrapped function
-                    # as it can also call decorated method inside
-                    if _use_case_linked.get() is None:
-                        linked_use_cases_token = _use_case_linked.set(set())
-                    ret = func(*args, **kwargs)
-
-                    if use_case_ids:
-                        for use_case_id in use_case_ids:
-                            _add_to_use_case(use_case_id, ret)
-                finally:
-                    if context_use_case_token:
-                        _decorator_use_cases.reset(context_use_case_token)
-                    if linked_use_cases_token:
-                        _use_case_linked.reset(linked_use_cases_token)
-
+                    use_cases = Context.use_case
+                if use_cases is not None:
+                    use_case_ids = resolve_use_case_ids(use_cases=use_cases)
+                    for use_case_id in use_case_ids:
+                        use_case = UseCase.get(use_case_id=use_case_id)
+                        use_case.add(entity=ret)
                 return ret
 
             return add_to_multiple
         else:
 
             @functools.wraps(func)
             def add_to_one(
@@ -264,49 +214,21 @@
             ) -> T:
                 """
                 Parameters
                 ----------
                 use_case: UseCase | string, optional
                     A single UseCase object or ID to add this new <return_object_type> to. Must be a kwarg.
                 """
-                use_case_id: Optional[str] = None
-                context_use_case_token: Optional[contextvars.Token[Union[UseCaseLike, None]]] = None
-                linked_use_cases_token = None
+                ret = func(*args, **kwargs)
 
-                # take care of use_case param
                 if use_case is None:
-                    # check contextvar that could be set by outer iterations first then Context
-                    use_cases = _decorator_use_cases.get(Context.use_case)
-                    # but it may have been set to a list
-                    if isinstance(use_cases, list):
-                        warnings.warn(MultipleUseCasesNotAllowed())
-                    else:
-                        use_case = use_cases
-                else:
-                    # if use_case passed, set it to be used by inner calls instead of Context
-                    context_use_case_token = _decorator_use_cases.set(use_case)
-
-                try:
-                    if use_case is not None:
-                        # Should only ever resolve to a single use case
-                        use_case_id = resolve_use_case_ids(use_cases=use_case)[0]
-
-                    # _use_case_linked never created? must be top level call, initialize set
-                    # to track entities added to UseCase before we call the wrapped function
-                    # as it can also call decorated method inside
-                    if _use_case_linked.get() is None:
-                        linked_use_cases_token = _use_case_linked.set(set())
-                    ret = func(*args, **kwargs)
-
-                    if use_case_id:
-                        _add_to_use_case(use_case_id, ret)
-                finally:
-                    if context_use_case_token:
-                        _decorator_use_cases.reset(context_use_case_token)
-                    if linked_use_cases_token:
-                        _use_case_linked.reset(linked_use_cases_token)
-
+                    use_case = Context.use_case
+                if use_case is not None:
+                    # Should only ever resolve to a single use case
+                    use_case_id = resolve_use_case_ids(use_cases=use_case)[0]
+                    use_case = UseCase.get(use_case_id=use_case_id)
+                    use_case.add(entity=ret)
                 return ret
 
             return add_to_one
 
     return wrapper
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,19 @@
 from requests.adapters import HTTPAdapter
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 import trafaret as t
 from urllib3 import Retry
 
 from datarobot.mixins.browser_mixin import BrowserMixin
 
-from . import analytics
 from ._compat import Int, String
 from ._version import __version__
-from .context import Context
 from .enums import DEFAULT_TIMEOUT
 from .errors import ClientError, JobAlreadyRequested, PlatformDeprecationWarning, ServerError
 from .utils import to_api
-from .utils.deprecation import deprecation_warning
 
 if TYPE_CHECKING:
     from io import BufferedReader, IOBase
 
     from requests import Response
 
 
@@ -177,19 +174,14 @@
             raise ValueError(f"unexpected url format: {url} does not start with {expected}")
         return url.split(expected)[1]
 
     # pylint: disable-next=arguments-differ
     def request(  # type: ignore[override]
         self, method: str, url: str, join_endpoint: bool = False, **kwargs: Any
     ) -> Response:
-        if "headers" not in kwargs:
-            kwargs["headers"] = {}
-        if Context.enable_api_consumer_tracking:
-            stack_trace = analytics.get_stack_trace()
-            kwargs["headers"][analytics.STACK_TRACE_HEADER] = stack_trace
         kwargs.setdefault("timeout", (self.connect_timeout, DEFAULT_TIMEOUT.READ))
         if not url.startswith("http") or join_endpoint:
             url = self._join_endpoint(url)
         response = super().request(method, url, **kwargs)
         handle_deprecation_header(response, **kwargs)
         if not response:
             handle_http_error(response, **kwargs)
@@ -419,48 +411,35 @@
             t.Key("token"): String(),
             t.Key("connect_timeout", optional=True): Int(),
             t.Key("ssl_verify", optional=True): t.Or(t.Bool(), String()),
             t.Key("user_agent_suffix", optional=True): String(),
             t.Key("max_retries", optional=True): Int(),
             t.Key("token_type", optional=True): String(),
             t.Key("default_use_case", optional=True): String(),
-            t.Key("enable_api_consumer_tracking", optional=True): t.Bool(),
-            t.Key("trace_context", optional=True): String(),
         }
     ).allow_extra("*")
     _fields = {k.to_name or k.name for k in _converter.keys}
 
     def __init__(
         self,
         endpoint: str,
         token: str,
         connect_timeout: Optional[int] = None,
         ssl_verify: bool = True,
         user_agent_suffix: Optional[str] = None,
         max_retries: Optional[Union[int, Retry]] = None,
         token_type: Optional[str] = None,
         default_use_case: Optional[str] = None,
-        enable_api_consumer_tracking: Optional[bool] = None,
-        trace_context: Optional[str] = None,
     ) -> None:
         self.endpoint = endpoint
         self.token = token
         self.connect_timeout = connect_timeout
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
         self.default_use_case = default_use_case
-        self.enable_api_consumer_tracking = enable_api_consumer_tracking
-        self.trace_context = trace_context
-        if self.user_agent_suffix:
-            deprecation_warning(
-                subject="Parameter `user_agent_suffix` is deprecated.",
-                deprecated_since_version="3.2",
-                will_remove_version="3.4",
-                message="The parameter `user_agent_suffix` has been deprecated. Please use `trace_context` instead.",
-            )
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.6.5/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.6.26
+Version: 3.2.0.2023.6.5
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 setup_weekly.py
 datarobot/__init__.py
 datarobot/_compat.py
 datarobot/_version.py
-datarobot/analytics.py
 datarobot/client.py
 datarobot/context.py
 datarobot/enums.py
 datarobot/errors.py
 datarobot/py.typed
 datarobot/rest.py
 datarobot/_experimental/__init__.py
@@ -41,15 +40,14 @@
 datarobot/mixins/update_attributes_mixin.py
 datarobot/models/__init__.py
 datarobot/models/advanced_tuning.py
 datarobot/models/anomaly_assessment.py
 datarobot/models/api_object.py
 datarobot/models/application.py
 datarobot/models/automated_documentation.py
-datarobot/models/batch_job.py
 datarobot/models/batch_monitoring_job.py
 datarobot/models/batch_prediction_job.py
 datarobot/models/blueprint.py
 datarobot/models/calendar_file.py
 datarobot/models/change_request.py
 datarobot/models/cluster.py
 datarobot/models/cluster_insight.py
@@ -60,15 +58,14 @@
 datarobot/models/custom_model.py
 datarobot/models/custom_model_test.py
 datarobot/models/custom_model_version.py
 datarobot/models/custom_task.py
 datarobot/models/custom_task_version.py
 datarobot/models/custom_task_version_dependency_build.py
 datarobot/models/data_engine_query_generator.py
-datarobot/models/data_slice.py
 datarobot/models/data_source.py
 datarobot/models/data_store.py
 datarobot/models/dataset.py
 datarobot/models/datetime_trend_plots.py
 datarobot/models/driver.py
 datarobot/models/execution_environment.py
 datarobot/models/execution_environment_version.py
@@ -102,15 +99,14 @@
 datarobot/models/ruleset.py
 datarobot/models/secondary_dataset.py
 datarobot/models/segmentation.py
 datarobot/models/shap_impact.py
 datarobot/models/shap_matrix.py
 datarobot/models/shap_matrix_job.py
 datarobot/models/sharing.py
-datarobot/models/status_check_job.py
 datarobot/models/trafarets.py
 datarobot/models/training_predictions.py
 datarobot/models/types.py
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.6.5/datarobot_early_access.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio
 Pillow==9.2.0
 black==22.8.0
-black[jupyter]==22.8.0
 isort==5.10.1
 flake8==5.0.4
 pylint==2.15.0
 mypy==1.0.0
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
@@ -45,15 +44,14 @@
 colour<=0.1.4
 
 [images]
 Pillow==9.2.0
 
 [lint]
 black==22.8.0
-black[jupyter]==22.8.0
 isort==5.10.1
 flake8==5.0.4
 pylint==2.15.0
 mypy==1.0.0
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
```

### Comparing `datarobot_early_access-3.2.0.2023.6.26/pyproject.toml` & `datarobot_early_access-3.2.0.2023.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/setup.py` & `datarobot_early_access-3.2.0.2023.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.6.26/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.6.5/setup_weekly.py`

 * *Files identical despite different names*

